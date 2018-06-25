---
title: FindItem 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindItem
api_type:
- schema
ms.assetid: ebad6aae-16e7-44de-ae63-a95b24539729
description: FindItem EWS に関する情報の検索操作です。
ms.openlocfilehash: b033ac2930981819a20f1336d40058a5f7c03b89
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760521"
---
# <a name="finditem-operation"></a>FindItem 操作

**FindItem** EWS の操作に関する情報を検索します。 
  
**FindItem**操作は、ユーザーのメールボックス内にある項目を検索します。 この操作は、多くのフィルタ リングする方法と検索結果がどのように呼び出し元に返される形式を提供します。 
  
## <a name="using-the-finditem-operation"></a>FindItem 操作を使用します。

**FindItem**操作の要求は、メールボックスとデータがどのように応答で返される形式を検索するためのさまざまな方法を提供します。 **FindItem**要求では、以下を指定できます。 
  
- かどうか検索では、浅いまたはソフト削除走査の実行がされます。 これを指定することが必要です。 検索の制限と組み合わせて、ソフト削除走査が返される項目の数を 0 にすると、でもある場合に一致するアイテムの検索条件を注意してください。
    
- アイテムの応答の図形です。 応答で返されるプロパティを識別します。 これを指定することが必要です。
    
- 検索を実行するフォルダーです。 これを指定することが必要です。
    
- ページング機構とビューの種類を返すためでは、ページのデータを表示します。 この指定は省略可能です。
    
- グループ化して、返されるアイテムの並べ替えのオプションです。 この指定は省略可能です。
    
- 制限または返される項目をフィルター処理するための高度なクエリ構文 (AQS) 文字列を検索します。 AQS を使用して、コンテンツのインデックス検索の詳細については、[クエリ文字列 (文字列)](querystring-string.md)を参照してください。 この指定は省略可能です。
    
- 応答で返されたアイテムの並べ替え順序です。 この指定は省略可能です。
    
**FindItem**操作では、ストリーム再生可能なプロパティの最初の 512 バイトのみを返します。 Unicode では、null で終わる Unicode 文字列を使用して、最初の 255 文字を返します。 メッセージ本文の形式または受信者の一覧は返されません。 **FindItem**受信者はサマリー返されます。 [GetItem 操作](getitem-operation.md)を使用すると、アイテムの詳細を取得します。 
  
 **FindItem**は[名 (EmailAddressType)](name-emailaddresstype.md)の要素のみを返し、[メールボックス](mailbox.md)の要素に次のフィールド[(NonEmptyStringType) の EmailAddress](emailaddress-nonemptystringtype.md)要素を返しません。 
  
- メッセージの [[差出人](from.md)] フィールド 
    
- メッセージの[[送信者](sender.md)] フィールド 
    
- 予定表アイテムの[開催者](organizer.md)フィールド 
    
> [!NOTE]
> **FindItem**操作では、[予定表ビュー](calendarview.md)の要素の結果を返すことができます。 **予定表ビュー**の要素は、1 つの予定表アイテムと定期的な会議のすべての出現回数を返します。 **予定表ビュー**の要素を使用しない場合は、1 つの予定表アイテムと定期的なマスターの予定表アイテムが返されます。 **予定表ビュー**の要素を使用しない場合は、定期的なマスターから出現するを展開する必要があります。 
  
**FindItem**操作では、次の表に記載されている SOAP ヘッダーを使用できます。 
  
**表 1 です。FindItem 操作の SOAP ヘッダー**

|**Header**|**要素**|**説明**|
|:-----|:-----|:-----|
|**DateTimePrecision** <br/> |[DateTimePrecision](datetimeprecision.md) <br/> |秒またはミリ秒単位のいずれか、サーバーからの応答では、日付/時刻値の解像度を指定します。 これは、要求に適用されます。  <br/> |
|**偽装** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |クライアント アプリケーションが偽装するユーザーを識別します。 これは、要求に適用されます。  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |RFC3066 カルチャを使用してメールボックスへのアクセスを識別します。 これは、要求に適用されます。  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |操作要求のスキーマのバージョンを識別します。 これは、要求に適用されます。  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |要求に応答するサーバーのバージョンを識別します。 これは、応答に適用されます。  <br/> |
|**TimeZoneContext** <br/> |[TimeZoneContext](timezonecontext.md) <br/> |サーバーからのすべての応答に使用するタイム ゾーンを識別します。 これは、要求に適用されます。  <br/> |
   
## <a name="finditem-operation-request-example"></a>FindItem 操作要求の例

**FindItem**要求の次の例では、削除済みアイテム フォルダーにあるアイテムの[BaseShape](baseshape.md)の要素の**IdOnly**列挙で定義されている項目の識別子を取得する方法を示します。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
              Traversal="Shallow">
      <ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
      </ItemShape>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="deleteditems"/>
      </ParentFolderIds>
    </FindItem>
  </soap:Body>
</soap:Envelope>
```

次の要素は、要求で使用されます。 
  
- [FindItem](finditem.md)
    
- [ItemShape](itemshape.md)
    
- [BaseShape](baseshape.md)
    
- [ParentFolderIds](parentfolderids.md)
    
- [DistinguishedFolderId](distinguishedfolderid.md)
    
**FindItem**要求メッセージの詳細については、スキーマの階層構造を表示します。 [FindItem](finditem.md)要素から開始します。 
  
## <a name="successful-finditem-operation-response"></a>FindItem 操作の成功の応答

**FindItem**要求に正常な応答の例を次に示します。 
  
[メッセージ](message-ex15websvcsotherref.md)要素は、電子メール メッセージおよび EWS スキーマが厳密に型指定されない他のすべての項目を表します。 IPM などの項目です。共有し、IPM.InfoPath は、[メッセージ](message-ex15websvcsotherref.md)の要素として返されます。 Exchange では、応答の基本要素の[項目](item.md)が返されません。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder TotalItemsInView="10" IncludesLastItemInRange="true">
            <t:Items>
              <t:Message>
                <t:ItemId Id="AS4AUn=" ChangeKey="fsVU4==" />
              </t:Message>
              <t:Message>
                <t:ItemId Id="AS4AUM=" ChangeKey="fsVUA==" />
              </t:Message>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </FindItemResponse>
  </soap:Body>
</soap:Envelope>
```

次の要素は、応答で使用されます。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [FindItemResponse](finditemresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [FindItemResponseMessage](finditemresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [RootFolder (FindItemResponseMessage)](rootfolder-finditemresponsemessage.md)
    
- [Items](items.md)
    
- [Message](message-ex15websvcsotherref.md)
    
- [ItemId](itemid.md)
    
**FindItem**応答メッセージの詳細については、スキーマの階層構造を表示します。 [FindItemResponse](finditemresponse.md)要素から開始します。 
  
## <a name="finditem-operation-error-response"></a>FindItem 操作のエラー応答

**FindItem**要求に対してエラー応答の例を次に示します。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Error">
          <m:MessageText>Id is malformed.</m:MessageText>
          <m:ResponseCode>ErrorInvalidIdMalformed</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </FindItemResponse>
  </soap:Body>
</soap:Envelope>
```

エラー応答では、次の要素が使用されます。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [FindItemResponse](finditemresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [FindItemResponseMessage](finditemresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
**FindItem**エラーの応答メッセージの詳細については、スキーマの階層構造を表示します。 [FindItemResponse](finditemresponse.md)要素から開始します。 
  
## <a name="version-differences"></a>バージョンの相違点

バージョンの Exchange でメジャー バージョン 15 で開始および終了は、 **FindItem**操作を使用して、アーカイブ メールボックスに複数のフォルダーを検索する場合に、15.0.898.11 の戻り値の[ResponseCode](responsecode.md)要素内の ErrorInvalidOperation 値を構築します。 
  
## <a name="see-also"></a>関連項目

- [項目を検索します。](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)
    
- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)
    
- **FindItemType**
    

