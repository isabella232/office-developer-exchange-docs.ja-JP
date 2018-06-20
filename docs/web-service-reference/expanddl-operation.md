---
title: ExpandDL 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExpandDL
api_type:
- schema
ms.assetid: 1f7837e7-9eff-4e10-9577-c40f7ed6af94
description: ExpandDL 操作では、配布リストの完全なメンバーシップを公開します。
ms.openlocfilehash: e4654120881f81a79358e0e7c0ab016f94db3288
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760379"
---
# <a name="expanddl-operation"></a>ExpandDL 操作

ExpandDL 操作では、配布リストの完全なメンバーシップを公開します。
  
## <a name="using-the-expanddl-web-method"></a>ExpandDL Web メソッドを使用します。

ExpandDL 操作では、Exchange.asmx に配置されている Web サービスを使用します。 この Web サービス メソッドは、パブリックな配布リストの拡張の[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md)の子要素またはプライベートの拡張のため、[アイテム Id](itemid.md)の子要素のいずれかを含むことができる[メールボックス](mailbox.md)の要素を受け入れる配布リストです。 
  
パブリックな配布リストを展開するには、次のいずれかを使用します。
  
1. 配布リストのエイリアス
    
2. 簡易メール転送プロトコル (SMTP) アドレス
    
3. X400
    
4. X500
    
5. Exchange の従来のアドレス
    
6. 配布リストの名前
    
7. 表示名
    
> [!IMPORTANT]
> 表示名が一意ではありません。 複数のアカウントは、同じ表示名を共有できます。 
  
## <a name="remarks"></a>備考

再帰的な拡張はサポートされていません。 1 回の呼び出しでは、1 つの配布リストを拡張できます。 1 つ以上の配布リストには、条件が一致すると、Web サービスはエラーを報告します。 クライアント アプリケーションでは、あいまいな配布リストと、 [ExpandDL 操作](expanddl-operation.md)のパラメーターとして必要な配布リストの正しい電子メール アドレスを選択し、あいまいな名前解決 (ANR) を使用できます。 詳細については、 [ResolveNames の操作](resolvenames-operation.md)を参照してください。
  
パブリックな配布リストは、Active Directory に配置されます。 メールが有効なまたは動的配布グループすることができます。 アドレス] ボックスの一覧からグループを表示する必要があり、各メンバーには空でない電子メール アドレスが必要があります。 配布リストのメンバーには、メールが有効なユーザーと連絡先、パブリック フォルダー、およびメールが有効な配布リストおよび動的グループを指定できます。
  
個人用配布リストは、ユーザーのメールボックスの [連絡先] フォルダーに配置されます。 個人用配布リストは、ExpandDL 要求でそのストアの項目の識別子を使用するための電子メール アドレスがありません。 個人用配布リストのメンバーは、メールが有効なユーザー、連絡先または配布リストを Active Directory から、またはユーザーの連絡先フォルダーから連絡先または非公開の配布が一覧表示します。
  
連絡先または個人用配布リストは、項目の識別子が応答で返されます。 これは、オブジェクトに関する情報を取得または個人用配布リストのメンバーシップを展開に使用できます。
  
## <a name="expanddl-private-distribution-list-request-example"></a>ExpandDL プライベート同報リストの要求の例

### <a name="description"></a>説明

ExpandDL 要求の次の例では、個人用配布リストを展開するための要求を作成する方法を示します。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ExpandDL xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
              xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
        <t:Mailbox>
          <t:ItemId Id="xASUAd==" ChangeKey="AAts0Q=="/>
        </t:Mailbox>
    </ExpandDL>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>コメント

個人用配布リストを展開するには、[メールボックス](mailbox.md)の要素にユーザーのメールボックス内の個人用配布リストを識別する[ItemId](itemid.md)の要素が含まれます。 
  
## <a name="expanddl-public-distribution-list-request-example"></a>ExpandDL パブリック同報リストの要求の例

### <a name="description"></a>説明

ExpandDL 要求の次の例では、パブリックな配布リストを展開するための要求を作成する方法を示します。 例では、配布リストを展開するのには表示名の使用を示します。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ExpandDL xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
              xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
        <t:Mailbox>
          <t:EmailAddress>TheDistributionList</t:EmailAddress>
        </t:Mailbox>
    </ExpandDL>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>コメント

この要求に対する応答を配布リストには、各メールボックスを識別する**メールボックス**の要素が含まれます。 配布リストに含まれる配布リストが含まれる場合は、埋め込みの配布リストに別の配布リストの展開を実行しなければなりません。 配布リストにメンバーが存在しないか、要求された配布リストが存在しない場合、 **ResponseClass**属性には成功した場合に相当する値が含まれます。 
  
### <a name="request-elements"></a>要素を要求します。

次の要素は、要求で使用されます。
  
- [ExpandDL](expanddl.md)
    
- [メールボックス](mailbox.md)
    
- [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md)を使用して、パブリックな配布リストを識別します。 [アイテム Id](itemid.md)要素を使用して、個人用配布リストを識別します。 
    
> [!NOTE]
> MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、これらの要素を記述するスキーマがあります。 
  
## <a name="successful-expanddl-response-example"></a>成功した ExpandDL の応答の例

### <a name="description"></a>説明

ExpandDL 応答の次の使用例は、上記の要求への応答を示しています。 配布リストの展開では、次の項目について説明します。 
  
- 応答で返される配布リストのメンバーの数です。
    
- かどうか、応答には、配布リストのすべてのメンバーが含まれています。
    
- メールボックスの名前です。
    
- メールボックスの電子メール アドレスです。
    
- メールボックスのルーティングの種類です。
    
- メールボックスの種類です。
    
> [!NOTE]
> 配布リストの名前が応答に含まれていません。したがって、する必要がありますの追跡の要求からの名前。 
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" 
                         MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ExpandDLResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="successful-response-elements"></a>正常な応答の要素

次の要素は、応答で使用されます。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [ExpandDLResponse](expanddlresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [ExpandDLResponseMessage](expanddlresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [DLExpansion](dlexpansion.md)
    
- [メールボックス](mailbox.md)
    
- [名 (EmailAddressType)](name-emailaddresstype.md)
    
- [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md)
    
- [RoutingType (EmailAddressType)](routingtype-emailaddresstype.md)
    
- [MailboxType](mailboxtype.md)
    
ExpandDL 操作の応答メッセージには、他のオプションを検索するには、スキーマの階層構造を表示します。 [ExpandDLResponse](expanddlresponse.md)要素から開始します。 
  
## <a name="expanddl-error-response"></a>ExpandDL エラー応答

### <a name="description"></a>説明

ExpandDL 要求に対するエラー応答の例を次に示します。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" 
                         MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ExpandDLResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="error-response-elements"></a>エラー応答の要素

エラー応答では、次の要素が使用されます。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [ExpandDLResponse](expanddlresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [ExpandDLResponseMessage](expanddlresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
ExpandDL 操作の応答メッセージには、他のオプションを検索するには、スキーマの階層構造を表示します。 [ExpandDLResponse](expanddlresponse.md)要素から開始します。 
  
## <a name="see-also"></a>関連項目

- [ResolveNames 操作](resolvenames-operation.md)
- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

