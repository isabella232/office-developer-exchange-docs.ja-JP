---
title: ResolveNames 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResolveNames
api_type:
- schema
ms.assetid: 6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb
description: ResolveNames 操作は、あいまいな電子メールアドレスと表示名を解決します。
ms.openlocfilehash: 51728addddd2bfb9d35b874ae8c11e83a4c8629b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468279"
---
# <a name="resolvenames-operation"></a>ResolveNames 操作

**ResolveNames**操作は、あいまいな電子メールアドレスと表示名を解決します。 
  
## <a name="using-the-resolvenames-operation"></a>ResolveNames 操作の使用

この操作は、エイリアスを確認し、表示名を適切なメールボックスユーザーに解決するために使用できます。 あいまいな名前が存在する場合、 **ResolveNames**操作の応答は、クライアントアプリケーションが名前を解決できるように、各メールボックスユーザーに関する情報を提供します。 
  
## <a name="remarks"></a>注釈

ResolveNames 応答は、最大100の候補を返します。 返される100候補は、参照操作で検出された最初の100です。
  
Smtp、sip などのプレフィックス付きルーティングタイプを持つ電子メールアドレスは、複数値配列に保存されます。 **ResolveNames**操作は、未解決の名前の先頭 ("sip:User1@Contoso.com" など) にルーティングの種類を追加するときに、その配列の各値に対して部分一致を実行します。 ルーティングの種類を指定しない場合、 **ResolveNames**は smtp のルーティングの種類を既定で設定し、それをプライマリ smtp アドレスプロパティに一致させ、複数値配列は検索しません。 
  
1つの要求で指定できるあいまいな名前は1つだけです。 Active Directory が最初に検索されてから、ユーザーの連絡先フォルダーが検索されます。 解決されたユーザーの連絡先フォルダーのエントリには、非 null の**ItemId**プロパティがあります。このプロパティは、GetItem 要求で使用できます。 プライベート配布リストの ID である場合は、 [Expanddl 操作](expanddl-operation.md)で使用できます。 **Returnfullcontactdata**属性が**true**に設定されている場合、 **ResolveNames**操作で見つかった Active Directory エントリは、[連絡先](contact.md)を記述する追加のプロパティを返します。 **Returnfullcontactdata**属性は、ユーザーの連絡先フォルダーから連絡先およびプライベート配布リストに対して返されるデータには影響しません。 
  
## <a name="resolvenames-request-example"></a>ResolveNames 要求の例

### <a name="description"></a>説明

次の**ResolveNames**要求の例は、ユーザーのエントリを解決する方法を示しています。
  
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

この要求への応答では、"Jo" または "Mi" で始まるすべてのエントリが返されます。 返されるアイテムは、パブリックメールボックス、パブリックおよびプライベート配布リスト、および連絡先です。
  
> [!NOTE]
> 既定の個人用連絡先フォルダー内の連絡先のみが検索されます。 
  
**ResolveNames**要求に対して考えられる結果は次のとおりです。 
  
- 解決されたエンティティを含まない応答は、**エラー**と等しい**ResponseClass**属性値を返します。 **Messagetext**要素には、"**結果が見つかりません**" が含まれています。
    
- 1つの解決されたエンティティを含む応答は、**成功**と等しい**ResponseClass**属性値を返します。
    
- 複数の可能なエンティティが含まれる応答は、**警告**と同じ**ResponseClass**属性値を返します。 この場合、エンティティを一意の id に解決できませんでした。 **Messagetext**要素には、"複数の結果が見つかりました" という文字列が含まれています。 
    
### <a name="request-elements"></a>Request 要素

要求では、次の要素が使用されます。
  
- [ResolveNames](resolvenames.md)
    
- [UnresolvedEntry](unresolvedentry.md)
    
## <a name="successful-resolvenames-operation-response-example"></a>成功した ResolveNames 操作の応答の例

### <a name="description"></a>説明

次の例は、 **ResolveNames**要求に対する正常な応答を示しています。 
  
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

### <a name="successful-resolvenames-response-elements"></a>Successful ResolveNames response 要素

応答では、次の要素が使用されます。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [ResolveNamesResponse](resolvenamesresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [ResolveNamesResponseMessage](resolvenamesresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [解像度セット](resolutionset.md)
    
- [Resolution](resolution.md)
    
- [メールボックス](mailbox.md)
    
- [Name (EmailAddressType)](name-emailaddresstype.md)
    
- [EmailAddress (非 Emptystringtype)](emailaddress-nonemptystringtype.md)
    
- [RoutingType (EmailAddressType)](routingtype-emailaddresstype.md)
    
- [MailboxType](mailboxtype.md)
    
- [連絡先](contact.md)
    
- [DisplayName (文字列)](displayname-string.md)
    
- [EmailAddresses](emailaddresses.md)
    
- [Entry (EmailAddress)](entry-emailaddress.md)
    
- [ContactSource](contactsource.md)
    
## <a name="resolvenames-operation-error-response"></a>ResolveNames 操作エラー応答

### <a name="description"></a>説明

次の例は、 **ResolveNames**要求に対するエラー応答を示しています。 解決できない名前を解決しようとすると、エラーが発生します。 
  
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

