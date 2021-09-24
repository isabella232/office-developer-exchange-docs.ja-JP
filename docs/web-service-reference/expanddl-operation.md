---
title: ExpandDL 操作
manager: sethgros
ms.date: 07/27/2018
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ExpandDL
api_type:
- schema
ms.assetid: 1f7837e7-9eff-4e10-9577-c40f7ed6af94
description: ExpandDL 操作は、配布リストの完全なメンバーシップを公開します。
ms.openlocfilehash: 9878ecff0eeee1ef386c7bb26a092eec47f471de
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513781"
---
# <a name="expanddl-operation"></a>ExpandDL 操作

ExpandDL 操作は、配布リストの完全なメンバーシップを公開します。
  
## <a name="using-the-expanddl-web-method"></a>ExpandDL Web メソッドの使用

ExpandDL 操作は、Exchange.asmx にある Web サービスを使用します。 この Web サービス メソッド[](mailbox.md)は、パブリック配布リストを展開する[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md)子要素、またはプライベート配布リストの展開用の[ItemId](itemid.md)子要素のいずれかを含むメールボックス要素を受け入れる。 
  
パブリック配布リストは、次のいずれかを使用して展開できます。
  
1. 配布リストのエイリアス
    
2. 簡易メール転送プロトコル (SMTP) アドレス
    
3. X400
    
4. X500
    
5. Exchangeレガシ アドレス
    
6. 配布リスト名
    
7. 表示名
    
> [!IMPORTANT]
> 表示名は一意ではありません。 複数のアカウントで同じ表示名を共有できます。 
  
## <a name="remarks"></a>注釈

再帰的拡張はサポートされていません。 1 回の呼び出しで展開できる配布リストは 1 つのみです。 複数の配布リストが条件に一致する場合、Web サービスはエラーを報告します。 クライアント アプリケーションは、あいまいな名前解決 (ANR) を使用してあいまいな配布リストを検索し [、ExpandDL](expanddl-operation.md)操作のパラメーターとして必要な配布リストの正しい電子メール アドレスを選択できます。 詳細については [、「ResolveNames 操作」を参照してください](resolvenames-operation.md)。
  
パブリック配布リストは Active Directory にあります。 メールが有効な配布グループまたは動的配布グループを指定できます。 グループをアドレス一覧から非表示にし、各メンバーに空でない電子メール アドレスを設定する必要があります。 配布リストのメンバーには、メールが有効なユーザーと連絡先、パブリック フォルダー、メールが有効な配布リストと動的グループを指定できます。
  
プライベート配布リストは、ユーザーのメールボックスの連絡先フォルダーにあります。 プライベート配布リストには電子メール アドレスが含めないので、ストア アイテム識別子は ExpandDL 要求で使用されます。 プライベート配布リストのメンバーには、Active Directory のメールが有効なユーザー、連絡先または配布リスト、ユーザーの連絡先フォルダーの連絡先またはプライベート配布リストを指定できます。
  
連絡先またはプライベート配布リストの場合、アイテム識別子は応答で返されます。 これは、オブジェクトに関する情報を取得したり、プライベート配布リストのメンバーシップを拡張したりするために使用できます。
  
## <a name="expanddl-private-distribution-list-request-example"></a>ExpandDL プライベート配布リスト要求の例

### <a name="description"></a>説明

ExpandDL 要求の次の例は、プライベート配布リストを展開する要求を形成する方法を示しています。
  
### <a name="code"></a>コード

```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013_SP1" />
  </soap:Header>
  <soap:Body>
    <m:ExpandDL>
      <m:Mailbox>
       <t:EmailAddress>test</t:EmailAddress>
      </m:Mailbox>
    </m:ExpandDL>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>コメント

プライベート配布リストを展開するには [、Mailbox](mailbox.md) 要素に、ユーザーのメールボックス内のプライベート配布リストを識別する [ItemId](itemid.md) 要素が含まれる。 
  
## <a name="expanddl-public-distribution-list-request-example"></a>ExpandDL パブリック配布リスト要求の例

### <a name="description"></a>説明

ExpandDL 要求の次の例は、パブリック配布リストを展開する要求を形成する方法を示しています。 この例では、表示名を使用して配布リストを展開します。
  
### <a name="code"></a>コード

```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ExpandDL xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
              xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
        <t:Mailbox>
          <t:EmailAddress>TheDistributionList</t:EmailAddress>
        </t:Mailbox>
    </ExpandDL>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>コメント

この要求に対する応答には、 **配布** リスト内の各メールボックスを識別する Mailbox 要素が含まれます。 配布リストが配布リスト内に含まれている場合は、埋め込み配布リストで別の配布リストの展開を実行する必要があります。 配布リストにメンバーがない場合、または要求された配布リストが存在しない場合 **、ResponseClass** 属性には Success と等しい値が含まれる。 
  
### <a name="request-elements"></a>要求要素

要求では、次の要素が使用されます。
  
- [ExpandDL](expanddl.md)
    
- [メールボックス](mailbox.md)
    
- [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) は、パブリック配布リストを識別するために使用されます。 [ItemId 要素は](itemid.md)、プライベート配布リストを識別するために使用されます。 
    
> [!NOTE]
> これらの要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。 
  
## <a name="successful-expanddl-response-example"></a>ExpandDL 応答の成功例

### <a name="description"></a>説明

ExpandDL 応答の次の例は、上記の要求に対する応答を示しています。 配布リストの展開では、次の項目について説明します。 
  
- 応答で返される配布リストのメンバーの数。
    
- 応答に配布リストのすべてのメンバーが含まれているかどうか。
    
- メールボックスの名前。
    
- メールボックスの電子メール アドレス。
    
- メールボックスのルーティングの種類。
    
- メールボックスの種類。
    
> [!NOTE]
> 配布リスト名は応答に含まれません。したがって、要求から名前を追跡する必要があります。 
  
### <a name="code"></a>コード

```xml
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" 
                         MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ExpandDLResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:ExpandDLResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:DLExpansion TotalItemsInView="3" IncludesLastItemInRange="true">
            <t:Mailbox>
              <t:Name>Dan Park</t:Name>
              <t:EmailAddress>dpark@exampledomain.com</t:EmailAddress>
              <t:RoutingType>SMTP</t:RoutingType>
              <t:MailboxType>Mailbox</t:MailboxType>
            </t:Mailbox>
            <t:Mailbox>
              <t:Name>Jeff Price</t:Name>
              <t:EmailAddress>jprice@exampledomain.com</t:EmailAddress>
              <t:RoutingType>SMTP</t:RoutingType>
              <t:MailboxType>Mailbox</t:MailboxType>
            </t:Mailbox>
            <t:Mailbox>
              <t:Name>Tanja Plate</t:Name>
              <t:EmailAddress>tplate@exampledomain.com</t:EmailAddress>
              <t:RoutingType>SMTP</t:RoutingType>
              <t:MailboxType>Mailbox</t:MailboxType>
            </t:Mailbox>
          </m:DLExpansion>
        </m:ExpandDLResponseMessage>
      </m:ResponseMessages>
    </ExpandDLResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a>成功した応答要素

応答では、次の要素が使用されます。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [ExpandDLResponse](expanddlresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [ExpandDLResponseMessage](expanddlresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [DLExpansion](dlexpansion.md)
    
- [メールボックス](mailbox.md)
    
- [Name (EmailAddressType)](name-emailaddresstype.md)
    
- [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md)
    
- [RoutingType (EmailAddressType)](routingtype-emailaddresstype.md)
    
- [MailboxType](mailboxtype.md)
    
ExpandDL 操作の応答メッセージのその他のオプションを見つけるには、スキーマ階層を確認します。 [ExpandDLResponse 要素から開始](expanddlresponse.md)します。 
  
## <a name="expanddl-error-response"></a>ExpandDL エラー応答

### <a name="description"></a>説明

次の例は、ExpandDL 要求に対するエラー応答を示しています。
  
### <a name="code"></a>コード

```xml
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" 
                         MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ExpandDLResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:ExpandDLResponseMessage ResponseClass="Error">
          <m:MessageText>No results are found.</m:MessageText>
          <m:ResponseCode>ErrorNameResolutionNoResults</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:ExpandDLResponseMessage>
      </m:ResponseMessages>
    </ExpandDLResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a>エラー応答要素

エラー応答では、次の要素が使用されます。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [ExpandDLResponse](expanddlresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [ExpandDLResponseMessage](expanddlresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
ExpandDL 操作の応答メッセージのその他のオプションを見つけるには、スキーマ階層を確認します。 [ExpandDLResponse 要素から開始](expanddlresponse.md)します。 
  
## <a name="see-also"></a>関連項目

- [ResolveNames 操作](resolvenames-operation.md)
- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

