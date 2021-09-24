---
title: ResolveNames 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ResolveNames
api_type:
- schema
ms.assetid: 6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb
description: ResolveNames 操作は、あいまいなメール アドレスと表示名を解決します。
ms.openlocfilehash: f5ab0e3ee23cc085d8aa425c6eeb0ac7c392b9bb
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59509449"
---
# <a name="resolvenames-operation"></a>ResolveNames 操作

**ResolveNames 操作は**、あいまいなメール アドレスと表示名を解決します。 
  
## <a name="using-the-resolvenames-operation"></a>ResolveNames 操作の使用

この操作を使用すると、エイリアスを確認し、表示名を適切なメールボックス ユーザーに解決できます。 あいまいな名前が存在する場合 **、ResolveNames** 操作応答は、クライアント アプリケーションが名前を解決できるよう、各メールボックス ユーザーに関する情報を提供します。 
  
## <a name="remarks"></a>注釈

ResolveNames 応答は、最大 100 の候補を返します。 返される 100 の候補は、ルックアップ操作で検出された最初の 100 です。
  
smtp や sip などのプレフィックス付きルーティングの種類を持つ電子メール アドレスは、複数値配列に保存されます。 **ResolveNames** 操作は、"sip:User1@Contoso.com" などの未解決の名前の先頭にルーティングの種類を追加すると、その配列の各値に対して部分的に一致します。 ルーティングの種類を指定しない場合 **、ResolveNames** は既定で smtp のルーティングの種類に設定され、プライマリ smtp アドレス プロパティに一致し、複数値配列を検索しません。 
  
1 つの要求で指定できるあいまいな名前は 1 つのみです。 Active Directory が最初に検索され、次にユーザーの連絡先フォルダーが検索されます。 ユーザーの連絡先フォルダーから解決されたエントリには、Null 以外の **ItemId** プロパティが設定され、GetItem 要求で使用できます。 プライベート配布リストの ID である場合は [、ExpandDL 操作で使用できます](expanddl-operation.md)。 **ReturnFullContactData** 属性が **true** に設定されている場合 **、ResolveNames** 操作で見つかった Active Directory エントリは、Contact を表す追加のプロパティを返 [します](contact.md)。 **ReturnFullContactData** 属性は、ユーザーの連絡先フォルダーから連絡先とプライベート配布リストに返されるデータには影響しません。 
  
## <a name="resolvenames-request-example"></a>ResolveNames 要求の例

### <a name="description"></a>説明

**ResolveNames 要求の次の例は、User** のエントリを解決する方法を示しています。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ResolveNames xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                  ReturnFullContactData="true">
      <UnresolvedEntry>User2</UnresolvedEntry>
    </ResolveNames>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>コメント

この要求に対する応答は、"Jo" または "Mi" で始まるすべてのエントリを返します。 返されるアイテムは、パブリック メールボックス、パブリックおよびプライベート配布リスト、および連絡先です。
  
> [!NOTE]
> 既定の個人用連絡先フォルダー内の連絡先だけが検索されます。 
  
**ResolveNames** 要求の結果を次に示します。 
  
- 解決済みエンティティを含む応答は、Error に等しい **ResponseClass** 属性値を **返します**。 **MessageText 要素には**"結果が **見つかりません." が含まれる。**
    
- 1 つの解決済みエンティティを含む応答は、Success に等しい **ResponseClass** 属性値を **返します**。
    
- 複数のエンティティを含む応答は、Warning に等しい **ResponseClass** 属性値を **返します**。 この場合、エンティティを一意の ID に解決する必要があります。 **MessageText 要素には**"複数の結果が見つかりました" が含まれる。 
    
### <a name="request-elements"></a>要求要素

要求では、次の要素が使用されます。
  
- [ResolveNames](resolvenames.md)
    
- [UnresolvedEntry](unresolvedentry.md)
    
## <a name="successful-resolvenames-operation-response-example"></a>ResolveNames 操作応答の成功例

### <a name="description"></a>説明

次の例は **、ResolveNames** 要求に対する正常な応答を示しています。 
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ResolveNamesResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:ResolveNamesResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:ResolutionSet TotalItemsInView="1" IncludesLastItemInRange="true">
            <t:Resolution>
              <t:Mailbox>
                <t:Name>User2</t:Name>
                <t:EmailAddress>User2@example.com</t:EmailAddress>
                <t:RoutingType>SMTP</t:RoutingType>
                <t:MailboxType>Mailbox</t:MailboxType>
              </t:Mailbox>
              <t:Contact>
                <t:DisplayName>User2</t:DisplayName>
                <t:EmailAddresses>
                  <t:Entry Key="EmailAddress1">SMTP:User2@example.com</t:Entry>
                </t:EmailAddresses>
                <t:ContactSource>ActiveDirectory</t:ContactSource>
              </t:Contact>
            </t:Resolution>
          </m:ResolutionSet>
        </m:ResolveNamesResponseMessage>
      </m:ResponseMessages>
    </ResolveNamesResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-resolvenames-response-elements"></a>ResolveNames 応答要素の成功

応答では、次の要素が使用されます。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [ResolveNamesResponse](resolvenamesresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [ResolveNamesResponseMessage](resolvenamesresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [ResolutionSet](resolutionset.md)
    
- [解決策](resolution.md)
    
- [メールボックス](mailbox.md)
    
- [Name (EmailAddressType)](name-emailaddresstype.md)
    
- [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md)
    
- [RoutingType (EmailAddressType)](routingtype-emailaddresstype.md)
    
- [MailboxType](mailboxtype.md)
    
- [Contact](contact.md)
    
- [DisplayName (string)](displayname-string.md)
    
- [EmailAddresses](emailaddresses.md)
    
- [Entry (EmailAddress)](entry-emailaddress.md)
    
- [ContactSource](contactsource.md)
    
## <a name="resolvenames-operation-error-response"></a>ResolveNames 操作エラー応答

### <a name="description"></a>説明

次の例は、ResolveNames 要求に対する **エラー応答を示** しています。 このエラーは、解決できない名前を解決しようとして発生します。 
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ResolveNamesResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:ResolveNamesResponseMessage ResponseClass="Error">
          <m:MessageText>No results were found.</m:MessageText>
          <m:ResponseCode>ErrorNameResolutionNoResults</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:ResolveNamesResponseMessage>
      </m:ResponseMessages>
    </ResolveNamesResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a>エラー応答要素

エラー応答では、次の要素が使用されます。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [ResolveNamesResponse](resolvenamesresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [ResolveNamesResponseMessage](resolvenamesresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
## <a name="see-also"></a>関連項目



[ExpandDL 操作](expanddl-operation.md)


[名前解決の使用](https://msdn.microsoft.com/library/9257fb07-89d2-46eb-b885-e2173fe6fbc1%28Office.15%29.aspx)

