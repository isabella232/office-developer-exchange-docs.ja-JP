---
title: 偽装するアカウントを識別する
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.assetid: c7749f12-b97f-48d9-88e5-a545e108efb0
description: サービス アプリケーションが EWS を使用して偽装するユーザーを識別する方法について説明します。
localization_priority: Priority
ms.openlocfilehash: 7159707abe96632aba2ed70dc0057417e087349f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527993"
---
# <a name="identify-the-account-to-impersonate"></a><span data-ttu-id="68d2d-103">偽装するアカウントを識別する</span><span class="sxs-lookup"><span data-stu-id="68d2d-103">Identify the account to impersonate</span></span>

<span data-ttu-id="68d2d-104">サービス アプリケーションが EWS を使用して偽装するユーザーを識別する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="68d2d-104">Learn how your service application uses EWS to identify the user to impersonate.</span></span>
  
<span data-ttu-id="68d2d-105">サービス アプリケーションは、次の 3 つの識別子のいずれかを使用して偽装するユーザー アカウントを識別します。</span><span class="sxs-lookup"><span data-stu-id="68d2d-105">Your service application identifies the user account to impersonate by using one of the following three identifiers:</span></span>
  
- <span data-ttu-id="68d2d-106">プライマリ SMTP アドレス。</span><span class="sxs-lookup"><span data-stu-id="68d2d-106">The primary SMTP address.</span></span>
    
- <span data-ttu-id="68d2d-107">ユーザープリンシパル名 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="68d2d-107">The user principal name (UPN).</span></span>
    
- <span data-ttu-id="68d2d-108">セキュリティ識別子 (SID)。</span><span class="sxs-lookup"><span data-stu-id="68d2d-108">The security identifier (SID).</span></span>
    
<span data-ttu-id="68d2d-109">もちろん、使用する識別子は、アプリケーションが使用可能な情報によって異なります。</span><span class="sxs-lookup"><span data-stu-id="68d2d-109">The identifier that you use depends, of course, on the information that your application has available.</span></span>
  
## <a name="identifying-the-user-account-to-impersonate"></a><span data-ttu-id="68d2d-110">偽装するユーザー アカウントを識別する</span><span class="sxs-lookup"><span data-stu-id="68d2d-110">Identifying the user account to impersonate</span></span>

<span data-ttu-id="68d2d-111">アプリケーションは、EWS マネージ API または EWS SOAP 要求を使用して、偽装するユーザー アカウントを識別できます。</span><span class="sxs-lookup"><span data-stu-id="68d2d-111">Your application can use either the EWS Managed API or EWS SOAP requests to identify the user account that it is impersonating.</span></span> <span data-ttu-id="68d2d-112">EWS マネージ API は、[ExchangeService.ImpersonatedUserId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.impersonateduserid.aspx) プロパティを使用して、偽装されたユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="68d2d-112">The EWS Managed API uses the [ExchangeService.ImpersonatedUserId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.impersonateduserid.aspx) property to identify the impersonated user.</span></span> <span data-ttu-id="68d2d-113">次の XML フラグメントに示すように、EWS は [ExchangeImpersonation](https://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx) 要素を使用します。</span><span class="sxs-lookup"><span data-stu-id="68d2d-113">EWS uses the [ExchangeImpersonation](https://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx) element, as shown in the following XML fragment.</span></span> 
  
```XML
<soap:Header>
    <t:ExchangeImpersonation>
        <t:ConnectingSID>
            Identifier
        </t:ConnectingSID>
    </t:ExchangeImpersonation>
</soap:Header>
```

<span data-ttu-id="68d2d-114">次の各セクションは、識別子のいずれかを使用する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="68d2d-114">Each of the following sections shows how to use one of the identifiers.</span></span> <span data-ttu-id="68d2d-115">偽装識別子の動作を示す例については、「[Exchange の偽装を使用して予定を追加する](how-to-add-appointments-by-using-exchange-impersonation.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="68d2d-115">For an example that shows the impersonation identifier in action, see [Add appointments by using Exchange impersonation](how-to-add-appointments-by-using-exchange-impersonation.md).</span></span>
  
### <a name="use-the-smtp-email-address-to-identify-the-user-account"></a><span data-ttu-id="68d2d-116">SMTP 電子メール アドレスを使用してユーザー アカウントを識別する</span><span class="sxs-lookup"><span data-stu-id="68d2d-116">Use the SMTP email address to identify the user account</span></span>

<span data-ttu-id="68d2d-117">SMTP 電子メール アドレスは、ユーザー アカウントに関連付けられているプライマリ電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="68d2d-117">The SMTP email address is the primary email address that is associated with a user account.</span></span>
  
<span data-ttu-id="68d2d-118">EWS マネージ API アプリケーションで、SMTP 電子メール アドレスを [ConnectingIdType.SMTP](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.connectingidtype.aspx) 列挙値と共に指定します。</span><span class="sxs-lookup"><span data-stu-id="68d2d-118">In an EWS Managed API application, you specify the SMTP email address along with the [ConnectingIdType.SMTP](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.connectingidtype.aspx) enumeration value.</span></span> 
  
```cs
exchangeServiceInstance.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.SMTP, "alisa@contoso.com");
```

<span data-ttu-id="68d2d-119">EWS SOAP 要求で、[PrimarySmtpAddress ](https://msdn.microsoft.com/library/eee79904-9412-4e61-b9b8-aff0ce25fade%28Office.15%29.aspx) 要素にはユーザー アカウントの電子メール アドレスが含まれています。</span><span class="sxs-lookup"><span data-stu-id="68d2d-119">In an EWS SOAP request, the [PrimarySmtpAddress](https://msdn.microsoft.com/library/eee79904-9412-4e61-b9b8-aff0ce25fade%28Office.15%29.aspx) element contains the email address for the user account.</span></span> 
  
```XML
<soap:Header>
  <t:ExchangeImpersonation>
    <t:ConnectingSID>
      <t:PrimarySmtpAddress>alisa@contoso.com</t: PrimarySmtpAddress>
    </t:ConnectingSID>
  </t:ExchangeImpersonation>
</soap:Header>
```

### <a name="use-the-upn-to-identify-the-user-account"></a><span data-ttu-id="68d2d-120">UPN を使用してユーザー アカウントを識別する</span><span class="sxs-lookup"><span data-stu-id="68d2d-120">Use the UPN to identify the user account</span></span>

<span data-ttu-id="68d2d-121">UPN には、ユーザー アカウントの場所を示す完全修飾ドメイン名 (FQDN) が含まれています。</span><span class="sxs-lookup"><span data-stu-id="68d2d-121">The UPN contains the fully qualified domain name (FQDN) for the location of the user account.</span></span> <span data-ttu-id="68d2d-122">これは必ずしもユーザーのメールボックス ドメインではありません。</span><span class="sxs-lookup"><span data-stu-id="68d2d-122">This is not necessarily the user's mailbox domain.</span></span> <span data-ttu-id="68d2d-123">ユーザー参照が成功するには、Active Directory ドメインサービス (AD DS) のユーザーアカウントで**UserPrincipalName**属性が正しく設定されている必要があります。</span><span class="sxs-lookup"><span data-stu-id="68d2d-123">The **UserPrincipalName** attribute must be set correctly on the user account in Active Directory Domain Services (AD DS) for the user lookup to succeed.</span></span> 
  
<span data-ttu-id="68d2d-124">EWS マネージ API アプリケーションで、UPN を[ConnectingIdType](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.connectingidtype.aspx)列挙値と共に指定します。</span><span class="sxs-lookup"><span data-stu-id="68d2d-124">In an EWS Managed API application, you specify the UPN along with the [ConnectingIdType.PrincipalName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.connectingidtype.aspx) enumeration value.</span></span> 
  
```cs
exchangeServiceInstance.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.PrincipalName, "alias@billing.contoso.com");
```

<span data-ttu-id="68d2d-125">EWS SOAP 要求で、[PrincipalName 要素 (ConnectingSIDType complexType) (EWS)](../web-service-reference/principalname.md) 要素にはユーザー アカウントの UPN が含まれています。</span><span class="sxs-lookup"><span data-stu-id="68d2d-125">In an EWS SOAP request, the [PrincipalName element (ConnectingSIDType complexType) (EWS)](../web-service-reference/principalname.md) element contains the UPN for the user account.</span></span> 
  
```XML
<soap:Header>
  <t:ExchangeImpersonation>
    <t:ConnectingSID>
      <t:PrincipalName>alisa@billing.contoso.com</t:PrincipalName>
    </t:ConnectingSID>
  </t:ExchangeImpersonation>
</soap:Header>
```

### <a name="use-the-sid-to-identify-the-user-account"></a><span data-ttu-id="68d2d-126">SID を使用してユーザー アカウントを識別する</span><span class="sxs-lookup"><span data-stu-id="68d2d-126">Use the SID to identify the user account</span></span>

<span data-ttu-id="68d2d-127">SID は、セキュリティ記述子定義言語 (SDDL) フォームで偽装するアカウントの識別子です。</span><span class="sxs-lookup"><span data-stu-id="68d2d-127">The SID is the identifier of the account to be impersonated in security descriptor definition language (SDDL) form.</span></span>
  
<span data-ttu-id="68d2d-128">EWS マネージ API アプリケーションで、SID を [ConnectingIdType.SID](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.connectingidtype.aspx) 列挙値と共に指定します。</span><span class="sxs-lookup"><span data-stu-id="68d2d-128">In an EWS Managed API application, you specify the SID along with the [ConnectingIdType.SID](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.connectingidtype.aspx) enumeration value.</span></span> 
  
```cs
exchangeServiceInstance.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.SID, "S-1-5-21-1493619105-1843311271-3936346804-1118");
```

<span data-ttu-id="68d2d-129">EWS SOAP 要求で、[SID](https://msdn.microsoft.com/library/2f33b29b-163b-4106-a74d-6fb76ec38951%28Office.15%29.aspx) 要素には、ユーザー アカウントの SID が含まれています。</span><span class="sxs-lookup"><span data-stu-id="68d2d-129">In an EWS SOAP request, the [SID](https://msdn.microsoft.com/library/2f33b29b-163b-4106-a74d-6fb76ec38951%28Office.15%29.aspx) element contains the SID for the user account.</span></span> 
  
```XML
<soap:Header>
  <t:ExchangeImpersonation>
    <t:ConnectingSID>
      <t:SID>S-1-5-21-1493619105-1843311271-3936346804-1118</t:SID>
    </t:ConnectingSID>
  </t:ExchangeImpersonation>
</soap:Header>
```

## <a name="see-also"></a><span data-ttu-id="68d2d-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="68d2d-130">See also</span></span>


- [<span data-ttu-id="68d2d-131">Exchange の偽装と EWS</span><span class="sxs-lookup"><span data-stu-id="68d2d-131">Impersonation and EWS in Exchange</span></span>](impersonation-and-ews-in-exchange.md)
    
- [<span data-ttu-id="68d2d-132">Exchange の偽装を使用して予定を追加する</span><span class="sxs-lookup"><span data-stu-id="68d2d-132">Add appointments by using Exchange impersonation</span></span>](how-to-add-appointments-by-using-exchange-impersonation.md)
    
- [<span data-ttu-id="68d2d-133">ExchangeService クラス</span><span class="sxs-lookup"><span data-stu-id="68d2d-133">ExchangeService class</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.aspx)
    
- [<span data-ttu-id="68d2d-134">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="68d2d-134">ExchangeImpersonation</span></span>](https://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx)
    

