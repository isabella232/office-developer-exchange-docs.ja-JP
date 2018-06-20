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
# <a name="identify-the-account-to-impersonate"></a>偽装するアカウントを識別します。

サービス アプリケーションが EWS を使用して偽装するユーザーを識別する方法について説明します。
  
サービス アプリケーションは、次の 3 つの識別子のいずれかを使用して偽装するユーザー アカウントを識別します。
  
- プライマリ SMTP アドレス。
    
- ユーザー プリンシパル名 (UPN)。
    
- セキュリティ識別子 (SID)。
    
もちろん、使用する識別子は、アプリケーションが使用可能な情報によって異なります。
  
## <a name="identifying-the-user-account-to-impersonate"></a>偽装するユーザー アカウントを識別する

アプリケーションは、それが偽装しているユーザー アカウントを識別するのに、EWS のマネージ API または EWS の SOAP 要求を使用できます。 EWS のマネージ API では、 [ExchangeService.ImpersonatedUserId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.impersonateduserid.aspx)プロパティを使用して、偽装されたユーザーを識別します。 EWS は、次の XML フラグメントに示すように、 [ExchangeImpersonation](http://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx)要素を使用します。 
  
```XML
<soap:Header>
    <t:ExchangeImpersonation>
        <t:ConnectingSID>
            Identifier
        </t:ConnectingSID>
    </t:ExchangeImpersonation>
</soap:Header>
```

次のセクションは、識別子のいずれかを使用する方法を示します。 アクションで偽装 id を表示する例では、 [Exchange の偽装を使用して予定を追加](how-to-add-appointments-by-using-exchange-impersonation.md)を参照してください。
  
### <a name="use-the-smtp-email-address-to-identify-the-user-account"></a>SMTP 電子メール アドレスを使用してユーザー アカウントを識別する

SMTP 電子メール アドレスは、ユーザー アカウントに関連付けられているプライマリ電子メール アドレスです。
  
EWS のマネージ API アプリケーションでは、 [ConnectingIdType.SMTP](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.connectingidtype.aspx)列挙型の値と SMTP の電子メール アドレスを指定します。 
  
```cs
exchangeServiceInstance.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.SMTP, "alisa@contoso.com");
```

EWS の SOAP の要求では、 [PrimarySmtpAddress](http://msdn.microsoft.com/library/eee79904-9412-4e61-b9b8-aff0ce25fade%28Office.15%29.aspx)要素には、ユーザー アカウントの電子メール アドレスが含まれています。 
  
```XML
<soap:Header>
  <t:ExchangeImpersonation>
    <t:ConnectingSID>
      <t:PrimarySmtpAddress>alisa@contoso.com</t: PrimarySmtpAddress>
    </t:ConnectingSID>
  </t:ExchangeImpersonation>
</soap:Header>
```

### <a name="use-the-upn-to-identify-the-user-account"></a>UPN を使用してユーザー アカウントを識別する

UPN には、ユーザー アカウントの場所の完全修飾ドメイン名 (FQDN) が含まれています。 これは必ずしもユーザーのメールボックスのドメインではありません。 **UserPrincipleName**属性する必要があります正しく設定されて Active Directory ドメイン サービス (AD DS) 内のユーザー アカウントのユーザー検索を成功させるため。 
  
EWS のマネージ API アプリケーションでは、 [ConnectingIdType.PrincipleName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.connectingidtype.aspx)列挙値の UPN を指定します。 
  
```cs
exchangeServiceInstance.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.PrincipleName, "alias@billing.contoso.com");
```

EWS の SOAP の要求で、 [PrincipalName 要素 (ConnectingSIDType の複合型) (EWS)](http://msdn.microsoft.com/library/6aac5388-c971-817b-b0bb-095a2639c6de%28Office.15%29.aspx)要素には、ユーザー アカウントの UPN が含まれています。 
  
```XML
<soap:Header>
  <t:ExchangeImpersonation>
    <t:ConnectingSID>
      <t:PrincipalName>alisa@billing.contoso.com</t:PrincipalName>
    </t:ConnectingSID>
  </t:ExchangeImpersonation>
</soap:Header>
```

### <a name="use-the-sid-to-identify-the-user-account"></a>SID を使用してユーザー アカウントを識別する

SID は、セキュリティ記述子定義言語 (SDDL) フォームで偽装するアカウントの識別子です。
  
EWS のマネージ API アプリケーションでは、 [ConnectingIdType.SID](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.connectingidtype.aspx)列挙型の値と SID を指定します。 
  
```cs
exchangeServiceInstance.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.SID, "S-1-5-21-1493619105-1843311271-3936346804-1118");
```

EWS の SOAP の要求では、 [SID](http://msdn.microsoft.com/library/2f33b29b-163b-4106-a74d-6fb76ec38951%28Office.15%29.aspx)の要素には、ユーザー アカウントの SID が含まれています。 
  
```XML
<soap:Header>
  <t:ExchangeImpersonation>
    <t:ConnectingSID>
      <t:SID>S-1-5-21-1493619105-1843311271-3936346804-1118</t:SID>
    </t:ConnectingSID>
  </t:ExchangeImpersonation>
</soap:Header>
```

## <a name="see-also"></a>関連項目


- [Exchange の偽装と EWS](impersonation-and-ews-in-exchange.md)
    
- [Exchange の偽装を使用して予定を追加します。](how-to-add-appointments-by-using-exchange-impersonation.md)
    
- [ExchangeService クラス](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.aspx)
    
- [ExchangeImpersonation](http://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx)
    

