---
title: ExpandDL 操作
manager: sethgros
ms.date: 07/27/2018
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExpandDL
api_type:
- schema
ms.assetid: 1f7837e7-9eff-4e10-9577-c40f7ed6af94
description: ExpandDL 操作は、配布リストの完全なメンバーシップを公開します。
ms.openlocfilehash: 8edaf057538e2c1136465f0ff7937c14477b2c47
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44454051"
---
# <a name="expanddl-operation"></a>ExpandDL 操作

ExpandDL 操作は、配布リストの完全なメンバーシップを公開します。
  
## <a name="using-the-expanddl-web-method"></a>ExpandDL Web メソッドの使用

ExpandDL 操作では、Exchange .asmx に配置されている Web サービスを使用します。 この Web サービスメソッドは、パブリック配布リストの拡張用の[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md)子要素、またはプライベート配布リストの展開用の[ItemId](itemid.md)子要素のいずれかを含むことができる[Mailbox](mailbox.md)要素を受け入れます。 
  
パブリック配布リストは、次のいずれかを使用して展開できます。
  
1. 配布リストのエイリアス
    
2. 簡易メール転送プロトコル (SMTP) アドレス
    
3. X400
    
4. X500
    
5. Exchange 従来のアドレス
    
6. 配布リストの名前
    
7. 表示名
    
> [!IMPORTANT]
> 表示名が一意ではありません。 複数のアカウントで同じ表示名を共有できます。 
  
## <a name="remarks"></a>注釈

再帰的な展開はサポートされていません。 1回の呼び出しで展開できる配布リストは1つだけです。 複数の配布リストが条件に一致する場合、Web サービスはエラーを報告します。 クライアントアプリケーションはあいまいな名前解決 (ANR) を使用してあいまいな配布リストを見つけ、必要な配布リストの正しい電子メールアドレスを[Expanddl 操作](expanddl-operation.md)のパラメーターとして選択することができます。 詳細については、「 [ResolveNames operation](resolvenames-operation.md)」を参照してください。
  
パブリック配布リストは、Active Directory にあります。 任意のメールが有効な配布グループまたは動的配布グループを指定できます。 このグループは、アドレス一覧から非表示にしないでください。また、各メンバーには空ではない電子メールアドレスを設定する必要があります。 配布リストのメンバーには、メールが有効なユーザーと連絡先、パブリックフォルダー、およびメールが有効な配布リストと動的グループを使用できます。
  
プライベート配布リストは、ユーザーのメールボックスの [連絡先] フォルダーにあります。 プライベート配布リストに電子メールアドレスが含まれていないため、ストアのアイテム識別子が ExpandDL 要求で使用されます。 プライベート配布リストのメンバーは、メールが有効なユーザー、Active Directory からの連絡先または配布リスト、またはユーザーの連絡先フォルダーの連絡先またはプライベート配布リストを使用できます。
  
連絡先またはプライベート配布リストの場合は、アイテムの識別子が応答で返されます。 これは、オブジェクトに関する情報を取得したり、プライベート配布リストのメンバーシップを拡張したりするために使用できます。
  
## <a name="expanddl-private-distribution-list-request-example"></a>ExpandDL プライベート配布リスト要求の例

### <a name="description"></a>説明

次の ExpandDL 要求の例は、プライベート配布リストを展開するための要求を形成する方法を示しています。
  
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

プライベート配布リストを展開する場合、 [mailbox](mailbox.md)要素には、ユーザーのメールボックス内のプライベート配布リストを識別する[ItemId](itemid.md)要素が含まれます。 
  
## <a name="expanddl-public-distribution-list-request-example"></a>ExpandDL パブリック配布リスト要求の例

### <a name="description"></a>説明

次の ExpandDL 要求の例は、パブリック配布リストを展開するための要求を形成する方法を示しています。 この例では、表示名を使用して配布リストを展開する方法を示します。
  
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

この要求への応答には、配布リスト内の各メールボックスを識別する**メールボックス**要素が含まれます。 配布リストが配布リスト内に含まれている場合は、埋め込まれた配布リストに対して別の配布リストの展開を実行する必要があります。 配布リストにメンバーが含まれていない場合、または要求された配布リストが存在しない場合、 **ResponseClass**属性の値は Success と等しくなります。 
  
### <a name="request-elements"></a>Request 要素

要求では、次の要素が使用されます。
  
- [ExpandDL](expanddl.md)
    
- [メールボックス](mailbox.md)
    
- [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md)は、パブリック配布リストを識別するために使用されます。 [ItemId](itemid.md)要素は、プライベート配布リストを識別するために使用されます。 
    
> [!NOTE]
> これらの要素を説明するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。 
  
## <a name="successful-expanddl-response-example"></a>Successful ExpandDL 応答の例

### <a name="description"></a>説明

次に示す ExpandDL 応答の例は、上記の要求に対する応答を示しています。 配布リストの展開では、以下について説明します。 
  
- 応答で返される配布リストのメンバー数。
    
- 応答に配布リストのすべてのメンバーが含まれているかどうか。
    
- メールボックスの名前。
    
- メールボックスの電子メールアドレス。
    
- メールボックスのルーティングの種類。
    
- メールボックスの種類。
    
> [!NOTE]
> 配布リストの名前は、応答に含まれていません。そのため、要求からの名前を記録しておく必要があります。 
  
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
    
- [DLExpansion 展開](dlexpansion.md)
    
- [メールボックス](mailbox.md)
    
- [Name (EmailAddressType)](name-emailaddresstype.md)
    
- [EmailAddress (非 Emptystringtype)](emailaddress-nonemptystringtype.md)
    
- [RoutingType (EmailAddressType)](routingtype-emailaddresstype.md)
    
- [MailboxType](mailboxtype.md)
    
ExpandDL 操作の応答メッセージに関するその他のオプションについては、スキーマ階層を参照してください。 [Expanddlresponse](expanddlresponse.md)要素から開始します。 
  
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
    
ExpandDL 操作の応答メッセージに関するその他のオプションについては、スキーマ階層を参照してください。 [Expanddlresponse](expanddlresponse.md)要素から開始します。 
  
## <a name="see-also"></a>関連項目

- [ResolveNames 操作](resolvenames-operation.md)
- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

