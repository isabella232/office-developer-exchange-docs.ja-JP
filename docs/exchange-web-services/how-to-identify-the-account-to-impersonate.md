---
title: 偽装するアカウントを識別します。
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: c7749f12-b97f-48d9-88e5-a545e108efb0
description: サービス アプリケーションが EWS を使用して偽装するユーザーを識別する方法について説明します。
ms.openlocfilehash: 78df4b511a9947d4d815b2802a53ab178b14622b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19758957"
---
# <a name="identify-the-account-to-impersonate"></a><span data-ttu-id="f3f2b-103">偽装するアカウントを識別します。</span><span class="sxs-lookup"><span data-stu-id="f3f2b-103">Identify the account to impersonate</span></span>

<span data-ttu-id="f3f2b-104">サービス アプリケーションが EWS を使用して偽装するユーザーを識別する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="f3f2b-104">Learn how your service application uses EWS to identify the user to impersonate.</span></span>
  
<span data-ttu-id="f3f2b-105">サービス アプリケーションは、次の 3 つの識別子のいずれかを使用して偽装するユーザー アカウントを識別します。</span><span class="sxs-lookup"><span data-stu-id="f3f2b-105">Your service application identifies the user account to impersonate by using one of the following three identifiers:</span></span>
  
- <span data-ttu-id="f3f2b-106">プライマリ SMTP アドレス。</span><span class="sxs-lookup"><span data-stu-id="f3f2b-106">The primary SMTP address.</span></span>
    
- <span data-ttu-id="f3f2b-107">ユーザー プリンシパル名 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="f3f2b-107">The user principle name (UPN).</span></span>
    
- <span data-ttu-id="f3f2b-108">セキュリティ識別子 (SID)。</span><span class="sxs-lookup"><span data-stu-id="f3f2b-108">The security identifier (SID).</span></span>
    
<span data-ttu-id="f3f2b-109">もちろん、使用する識別子は、アプリケーションが使用可能な情報によって異なります。</span><span class="sxs-lookup"><span data-stu-id="f3f2b-109">The identifier that you use depends, of course, on the information that your application has available.</span></span>
  
## <a name="identifying-the-user-account-to-impersonate"></a><span data-ttu-id="f3f2b-110">偽装するユーザー アカウントを識別する</span><span class="sxs-lookup"><span data-stu-id="f3f2b-110">Identifying the user account to impersonate</span></span>

<span data-ttu-id="f3f2b-111">アプリケーションは、それが偽装しているユーザー アカウントを識別するのに、EWS のマネージ API または EWS の SOAP 要求を使用できます。</span><span class="sxs-lookup"><span data-stu-id="f3f2b-111">Your application can use either the EWS Managed API or EWS SOAP requests to identify the user account that it is impersonating.</span></span> <span data-ttu-id="f3f2b-112">EWS のマネージ API では、 [ExchangeService.ImpersonatedUserId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.impersonateduserid.aspx)プロパティを使用して、偽装されたユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="f3f2b-112">The EWS Managed API uses the [ExchangeService.ImpersonatedUserId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.impersonateduserid.aspx) property to identify the impersonated user.</span></span> <span data-ttu-id="f3f2b-113">EWS は、次の XML フラグメントに示すように、 [ExchangeImpersonation](http://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx)要素を使用します。</span><span class="sxs-lookup"><span data-stu-id="f3f2b-113">EWS uses the [ExchangeImpersonation](http://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx) element, as shown in the following XML fragment.</span></span> 
  
```XML
<soap:Header>
    <t:ExchangeImpersonation>
        <t:ConnectingSID>
            Identifier
        </t:ConnectingSID>
    </t:ExchangeImpersonation>
</soap:Header>
```

<span data-ttu-id="f3f2b-114">次のセクションは、識別子のいずれかを使用する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="f3f2b-114">Each of the following sections shows how to use one of the identifiers.</span></span> <span data-ttu-id="f3f2b-115">アクションで偽装 id を表示する例では、 [Exchange の偽装を使用して予定を追加](how-to-add-appointments-by-using-exchange-impersonation.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f3f2b-115">For an example that shows the impersonation identifier in action, see [Add appointments by using Exchange impersonation](how-to-add-appointments-by-using-exchange-impersonation.md).</span></span>
  
### <a name="use-the-smtp-email-address-to-identify-the-user-account"></a><span data-ttu-id="f3f2b-116">SMTP 電子メール アドレスを使用してユーザー アカウントを識別する</span><span class="sxs-lookup"><span data-stu-id="f3f2b-116">Use the SMTP email address to identify the user account</span></span>

<span data-ttu-id="f3f2b-117">SMTP 電子メール アドレスは、ユーザー アカウントに関連付けられているプライマリ電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="f3f2b-117">The SMTP email address is the primary email address that is associated with a user account.</span></span>
  
<span data-ttu-id="f3f2b-118">EWS のマネージ API アプリケーションでは、 [ConnectingIdType.SMTP](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.connectingidtype.aspx)列挙型の値と SMTP の電子メール アドレスを指定します。</span><span class="sxs-lookup"><span data-stu-id="f3f2b-118">In an EWS Managed API application, you specify the SMTP email address along with the [ConnectingIdType.SMTP](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.connectingidtype.aspx) enumeration value.</span></span> 
  
```cs
exchangeServiceInstance.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.SMTP, "alisa@contoso.com");
```

<span data-ttu-id="f3f2b-119">EWS の SOAP の要求では、 [PrimarySmtpAddress](http://msdn.microsoft.com/library/eee79904-9412-4e61-b9b8-aff0ce25fade%28Office.15%29.aspx)要素には、ユーザー アカウントの電子メール アドレスが含まれています。</span><span class="sxs-lookup"><span data-stu-id="f3f2b-119">In an EWS SOAP request, the [PrimarySmtpAddress](http://msdn.microsoft.com/library/eee79904-9412-4e61-b9b8-aff0ce25fade%28Office.15%29.aspx) element contains the email address for the user account.</span></span> 
  
```XML
<soap:Header>
  <t:ExchangeImpersonation>
    <t:ConnectingSID>
      <t:PrimarySmtpAddress>alisa@contoso.com</t: PrimarySmtpAddress>
    </t:ConnectingSID>
  </t:ExchangeImpersonation>
</soap:Header>
```

### <a name="use-the-upn-to-identify-the-user-account"></a><span data-ttu-id="f3f2b-120">UPN を使用してユーザー アカウントを識別する</span><span class="sxs-lookup"><span data-stu-id="f3f2b-120">Use the UPN to identify the user account</span></span>

<span data-ttu-id="f3f2b-121">UPN には、ユーザー アカウントの場所の完全修飾ドメイン名 (FQDN) が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f3f2b-121">The UPN contains the fully qualified domain name (FQDN) for the location of the user account.</span></span> <span data-ttu-id="f3f2b-122">これは必ずしもユーザーのメールボックスのドメインではありません。</span><span class="sxs-lookup"><span data-stu-id="f3f2b-122">This is not necessarily the user's mailbox domain.</span></span> <span data-ttu-id="f3f2b-123">**UserPrincipleName**属性する必要があります正しく設定されて Active Directory ドメイン サービス (AD DS) 内のユーザー アカウントのユーザー検索を成功させるため。</span><span class="sxs-lookup"><span data-stu-id="f3f2b-123">The **UserPrincipleName** attribute must be set correctly on the user account in Active Directory Domain Services (AD DS) for the user lookup to succeed.</span></span> 
  
<span data-ttu-id="f3f2b-124">EWS のマネージ API アプリケーションでは、 [ConnectingIdType.PrincipleName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.connectingidtype.aspx)列挙値の UPN を指定します。</span><span class="sxs-lookup"><span data-stu-id="f3f2b-124">In an EWS Managed API application, you specify the UPN along with the [ConnectingIdType.PrincipleName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.connectingidtype.aspx) enumeration value.</span></span> 
  
```cs
exchangeServiceInstance.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.PrincipleName, "alias@billing.contoso.com");
```

<span data-ttu-id="f3f2b-125">EWS の SOAP の要求で、 [PrincipalName 要素 (ConnectingSIDType の複合型) (EWS)](http://msdn.microsoft.com/library/6aac5388-c971-817b-b0bb-095a2639c6de%28Office.15%29.aspx)要素には、ユーザー アカウントの UPN が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f3f2b-125">In an EWS SOAP request, the [PrincipalName element (ConnectingSIDType complexType) (EWS)](http://msdn.microsoft.com/library/6aac5388-c971-817b-b0bb-095a2639c6de%28Office.15%29.aspx) element contains the UPN for the user account.</span></span> 
  
```XML
<soap:Header>
  <t:ExchangeImpersonation>
    <t:ConnectingSID>
      <t:PrincipalName>alisa@billing.contoso.com</t:PrincipalName>
    </t:ConnectingSID>
  </t:ExchangeImpersonation>
</soap:Header>
```

### <a name="use-the-sid-to-identify-the-user-account"></a><span data-ttu-id="f3f2b-126">SID を使用してユーザー アカウントを識別する</span><span class="sxs-lookup"><span data-stu-id="f3f2b-126">Use the SID to identify the user account</span></span>

<span data-ttu-id="f3f2b-127">SID は、セキュリティ記述子定義言語 (SDDL) フォームで偽装するアカウントの識別子です。</span><span class="sxs-lookup"><span data-stu-id="f3f2b-127">The SID is the identifier of the account to be impersonated in security descriptor definition language (SDDL) form.</span></span>
  
<span data-ttu-id="f3f2b-128">EWS のマネージ API アプリケーションでは、 [ConnectingIdType.SID](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.connectingidtype.aspx)列挙型の値と SID を指定します。</span><span class="sxs-lookup"><span data-stu-id="f3f2b-128">In an EWS Managed API application, you specify the SID along with the [ConnectingIdType.SID](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.connectingidtype.aspx) enumeration value.</span></span> 
  
```cs
exchangeServiceInstance.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.SID, "S-1-5-21-1493619105-1843311271-3936346804-1118");
```

<span data-ttu-id="f3f2b-129">EWS の SOAP の要求では、 [SID](http://msdn.microsoft.com/library/2f33b29b-163b-4106-a74d-6fb76ec38951%28Office.15%29.aspx)の要素には、ユーザー アカウントの SID が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f3f2b-129">In an EWS SOAP request, the [SID](http://msdn.microsoft.com/library/2f33b29b-163b-4106-a74d-6fb76ec38951%28Office.15%29.aspx) element contains the SID for the user account.</span></span> 
  
```XML
<soap:Header>
  <t:ExchangeImpersonation>
    <t:ConnectingSID>
      <t:SID>S-1-5-21-1493619105-1843311271-3936346804-1118</t:SID>
    </t:ConnectingSID>
  </t:ExchangeImpersonation>
</soap:Header>
```

## <a name="see-also"></a><span data-ttu-id="f3f2b-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="f3f2b-130">See also</span></span>


- [<span data-ttu-id="f3f2b-131">Exchange の偽装と EWS</span><span class="sxs-lookup"><span data-stu-id="f3f2b-131">Impersonation and EWS in Exchange</span></span>](impersonation-and-ews-in-exchange.md)
    
- [<span data-ttu-id="f3f2b-132">Exchange の偽装を使用して予定を追加します。</span><span class="sxs-lookup"><span data-stu-id="f3f2b-132">Add appointments by using Exchange impersonation</span></span>](how-to-add-appointments-by-using-exchange-impersonation.md)
    
- [<span data-ttu-id="f3f2b-133">ExchangeService クラス</span><span class="sxs-lookup"><span data-stu-id="f3f2b-133">ExchangeService class</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.aspx)
    
- [<span data-ttu-id="f3f2b-134">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="f3f2b-134">ExchangeImpersonation</span></span>](http://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx)
    

