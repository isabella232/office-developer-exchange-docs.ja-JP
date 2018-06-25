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
description: ResolveNames 操作解決あいまいな電子メール アドレスと表示名です。
ms.openlocfilehash: 8443cf834dfdf104daeaaa92fdee3742c3fa3719
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833162"
---
# <a name="resolvenames-operation"></a>ResolveNames 操作

**ResolveNames**操作解決あいまいな電子メール アドレスと表示名です。 
  
## <a name="using-the-resolvenames-operation"></a>ResolveNames 操作を使用します。

エイリアスを確認し、適切なメールボックスのユーザーに表示名を解決するのには、この操作を使用できます。 あいまいな名前が存在する場合、 **ResolveNames**操作の応答は、クライアント アプリケーションは、名前を解決できるよう、各メールボックスのユーザーに関する情報を提供します。 
  
## <a name="remarks"></a>備考

ResolveNames 応答では、最大 100 の候補を返します。 返される 100 の候補は、検索操作で発生した最初の 100 人です。
  
プレフィックスが付けられたルーティングなど、smtp または sip、電子メール アドレスは、複数値配列に保存されます。 **ResolveNames**操作は、ルーティングの種類を「sip:User1@Contoso.com」など、未解決の名前の先頭に追加するときに、その配列の各値に対して部分的一致を実行します。 ルーティングの種類を指定しない場合**ResolveNames**が既定の smtp ルーティングの種類に、照合するプライマリ smtp アドレスのプロパティでは、および複数値の配列を検索します。 
  
1 つの要求では、1 つだけのあいまいな名前を指定できます。 最初に active Directory を検索し、ユーザーの連絡先フォルダーを検索し、します。 GetItem 要求で使用できる null 以外の**ItemId**プロパティがあるユーザーの連絡先フォルダーからエントリを解決します。 個人用配布リストの ID である場合は、 [ExpandDL の操作](expanddl-operation.md)で使用できます。 **ReturnFullContactData**属性は、 **true**に設定されている場合**ResolveNames**操作で Active Directory エントリの間で[連絡先](contact.md)を記述する追加のプロパティが返されます。 **ReturnFullContactData**属性は、メンバーとプライベートで返されるデータには影響は、ユーザーの連絡先フォルダーから配布リストを使用します。 
  
## <a name="resolvenames-request-example"></a>ResolveNames 要求の例

### <a name="description"></a>説明

**ResolveNames**要求の次の例では、ユーザーのエントリを解決する方法を示します。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ResolveNames xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                  ReturnFullContactData="true">
      <UnresolvedEntry>User2</UnresolvedEntry>
    </ResolveNames>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>コメント

この要求への応答は"Jo"または「マイル」で始まるすべてのエントリを返す 返されたアイテムは、パブリックのメールボックス、パブリックとプライベートの配布リスト、および連絡先です。
  
> [!NOTE]
> 既定の個人用連絡先フォルダー内の連絡先だけが検索されます。 
  
**ResolveNames**要求の可能な結果は、次のように。 
  
- 解決されたエンティティが含まれていない応答を返します**ResponseClass**属性値**エラー**と同じです。 **メッセージ テキスト**要素には「が**ない結果があります**。
    
- 1 つの解決されたエンティティを含む応答を返します**ResponseClass**属性値**成功した場合**と同じです。
    
- 複数の可能なエンティティを含む応答を返します**ResponseClass**属性の値**の警告**と同じ。 この例では、エンティティは、一意の id を解決できませんでした。 [複数の結果が見つかりました"**メッセージ テキスト**要素が含まれます 
    
### <a name="request-elements"></a>要素を要求します。

次の要素は、要求で使用されます。
  
- [ResolveNames](resolvenames.md)
    
- [UnresolvedEntry](unresolvedentry.md)
    
## <a name="successful-resolvenames-operation-response-example"></a>ResolveNames 操作の正常な応答例

### <a name="description"></a>説明

**ResolveNames**要求に正常な応答の例を次に示します。 
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ResolveNamesResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="successful-resolvenames-response-elements"></a>ResolveNames 応答の成功の要素

次の要素は、応答で使用されます。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [ResolveNamesResponse](resolvenamesresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [ResolveNamesResponseMessage](resolvenamesresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [ResolutionSet](resolutionset.md)
    
- [解決策](resolution.md)
    
- [メールボックス](mailbox.md)
    
- [名 (EmailAddressType)](name-emailaddresstype.md)
    
- [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md)
    
- [RoutingType (EmailAddressType)](routingtype-emailaddresstype.md)
    
- [MailboxType](mailboxtype.md)
    
- [Contact](contact.md)
    
- [表示名 (文字列)](displayname-string.md)
    
- [EmailAddresses](emailaddresses.md)
    
- [エントリ (EmailAddress)](entry-emailaddress.md)
    
- [ContactSource](contactsource.md)
    
## <a name="resolvenames-operation-error-response"></a>ResolveNames 操作のエラー応答

### <a name="description"></a>説明

**ResolveNames**要求に対してエラー応答の例を次に示します。 解決できない名前を解決しようとしてエラーが発生します。 
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ResolveNamesResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="error-response-elements"></a>エラー応答の要素

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


[名前解決の使用](http://msdn.microsoft.com/library/9257fb07-89d2-46eb-b885-e2173fe6fbc1%28Office.15%29.aspx)

