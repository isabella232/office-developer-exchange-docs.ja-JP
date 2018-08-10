---
title: 偽装するアカウントを識別する
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: c7749f12-b97f-48d9-88e5-a545e108efb0
description: サービス アプリケーションが EWS を使用して偽装するユーザーを識別する方法について説明します。
ms.openlocfilehash: 01c6ee797359c38c8539257003a2f110fdf253cf
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354296"
---
# <a name="identify-the-account-to-impersonate"></a>偽装するアカウントを識別する

サービス アプリケーションが EWS を使用して偽装するユーザーを識別する方法について説明します。
  
サービス アプリケーションは、次の 3 つの識別子のいずれかを使用して偽装するユーザー アカウントを識別します。
  
- プライマリ SMTP アドレス。
    
- ユーザー プリンシパル名 (UPN)。
    
- セキュリティ識別子 (SID)。
    
もちろん、使用する識別子は、アプリケーションが使用可能な情報によって異なります。
  
## <a name="identifying-the-user-account-to-impersonate"></a>偽装するユーザー アカウントを識別する

アプリケーションは、EWS マネージ API または EWS SOAP 要求を使用して、偽装するユーザー アカウントを識別できます。 EWS マネージ API は、[ExchangeService.ImpersonatedUserId](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.impersonateduserid.aspx) プロパティを使用して、偽装されたユーザーを識別します。 次の XML フラグメントに示すように、EWS は [ExchangeImpersonation](http://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx) 要素を使用します。 
  
```XML
<soap:Header>
    <t:ExchangeImpersonation>
        <t:ConnectingSID>
            Identifier
        </t:ConnectingSID>
    </t:ExchangeImpersonation>
</soap:Header>
```

次の各セクションは、識別子のいずれかを使用する方法を示します。 偽装識別子の動作を示す例については、「[Exchange の偽装を使用して予定を追加する](how-to-add-appointments-by-using-exchange-impersonation.md)」を参照してください。
  
### <a name="use-the-smtp-email-address-to-identify-the-user-account"></a>SMTP 電子メール アドレスを使用してユーザー アカウントを識別する

SMTP 電子メール アドレスは、ユーザー アカウントに関連付けられているプライマリ電子メール アドレスです。
  
EWS マネージ API アプリケーションで、SMTP 電子メール アドレスを [ConnectingIdType.SMTP](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.connectingidtype.aspx) 列挙値と共に指定します。 
  
```cs
exchangeServiceInstance.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.SMTP, "alisa@contoso.com");
```

EWS SOAP 要求で、[PrimarySmtpAddress ](http://msdn.microsoft.com/library/eee79904-9412-4e61-b9b8-aff0ce25fade%28Office.15%29.aspx) 要素にはユーザー アカウントの電子メール アドレスが含まれています。 
  
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

UPN には、ユーザー アカウントの場所を示す完全修飾ドメイン名 (FQDN) が含まれています。 これは必ずしもユーザーのメールボックス ドメインではありません。 ユーザー検索を正常に行うには、Active Directory ドメイン サービス (AD DS) 内のユーザー アカウントで **UserPrincipleName** 属性を正しく設定する必要があります。 
  
EWS マネージ API アプリケーションで、UPN を [ConnectingIdType.PrincipleName](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.connectingidtype.aspx) 列挙値と共に指定します。 
  
```cs
exchangeServiceInstance.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.PrincipleName, "alias@billing.contoso.com");
```

EWS SOAP 要求で、[PrincipalName 要素 (ConnectingSIDType complexType) (EWS)](../web-service-reference/principalname.md) 要素にはユーザー アカウントの UPN が含まれています。 
  
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
  
EWS マネージ API アプリケーションで、SID を [ConnectingIdType.SID](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.connectingidtype.aspx) 列挙値と共に指定します。 
  
```cs
exchangeServiceInstance.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.SID, "S-1-5-21-1493619105-1843311271-3936346804-1118");
```

EWS SOAP 要求で、[SID](http://msdn.microsoft.com/library/2f33b29b-163b-4106-a74d-6fb76ec38951%28Office.15%29.aspx) 要素には、ユーザー アカウントの SID が含まれています。 
  
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
    
- [Exchange の偽装を使用して予定を追加する](how-to-add-appointments-by-using-exchange-impersonation.md)
    
- [ExchangeService クラス](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.aspx)
    
- [ExchangeImpersonation](http://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx)
    

