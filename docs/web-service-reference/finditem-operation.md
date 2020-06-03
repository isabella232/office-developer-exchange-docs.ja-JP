---
title: FindItem 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
api_name:
- FindItem
api_type:
- schema
ms.assetid: ebad6aae-16e7-44de-ae63-a95b24539729
description: FindItem EWS 操作についての情報を検索します。
localization_priority: Priority
ms.openlocfilehash: 499d1ee80ef323c883fa86eb125d8c037fb37d4e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462557"
---
# <a name="finditem-operation"></a>FindItem 操作

**FindItem** EWS 操作についての情報を検索します。 
  
**FindItem**操作は、ユーザーのメールボックスにあるアイテムを検索します。 この操作では、検索結果が発信者に返される方法をフィルター処理し、書式設定するためのさまざまな方法を提供します。 
  
## <a name="using-the-finditem-operation"></a>FindItem 操作の使用

**FindItem**操作要求では、メールボックスを検索して、そのデータが応答で返される方法を書式設定するさまざまな方法を使用できます。 **FindItem**要求では、次のものを指定できます。 
  
- 検索が浅い、または削除済みの走査であるかどうか。 これを指定する必要があります。 検索条件に一致するアイテムが存在する場合でも、削除済み検査と検索制限を組み合わせると、返されるアイテムが0になることに注意してください。
    
- アイテムの応答の形状。 これは、応答で返されるプロパティを識別します。 これを指定する必要があります。
    
- 検索を実行するフォルダー。 これを指定する必要があります。
    
- ページ内のビューデータを返すページングメカニズムとビューの種類。 この指定は省略可能です。
    
- 返されるアイテムをグループ化および並べ替えするためのオプション。 この指定は省略可能です。
    
- 返されるアイテムをフィルター処理するための検索制限または高度なクエリ構文 (AQS) 文字列。 コンテンツインデックス検索での AQS の使用の詳細については、「 [QueryString (String)](querystring-string.md)」を参照してください。 この指定は省略可能です。
    
- 応答で返されるアイテムの並べ替え順序を示します。 この指定は省略可能です。
    
**FindItem**操作は、任意の streamable プロパティの最初の512バイトのみを返します。 Unicode の場合は、Null 終了の Unicode 文字列を使用して最初の 255 文字を返します。 メッセージ本文の形式や受信者リストは返されません。 **FindItem**は受信者の概要を返します。 [GetItem 操作](getitem-operation.md)を使用して、アイテムの詳細を取得できます。 
  
 **FindItem**は、 [Name (emailaddresstype)](name-emailaddresstype.md)要素のみを返します。次のフィールドの[Mailbox](mailbox.md)要素には、 [EmailAddress (nonemptystringtype)](emailaddress-nonemptystringtype.md)要素は返されません。 
  
- メッセージの [[差出人](from.md)] フィールド 
    
- メッセージの[Sender](sender.md)フィールド 
    
- 予定表アイテムの[開催者](organizer.md)フィールド 
    
> [!NOTE]
> **FindItem**操作は、 [CalendarView](calendarview.md)要素で結果を返すことができます。 **CalendarView**要素は、1つの予定表アイテムと定期的な会議のすべてのオカレンスを返します。 **CalendarView**要素を使用しない場合は、1つの予定表アイテムと定期的な予定表アイテムが返されます。 **CalendarView**要素が使用されていない場合は、定期的なマスターからオカレンスを展開する必要があります。 
  
**FindItem**操作では、次の表に示す SOAP ヘッダーを使用できます。 
  
**表1FindItem 操作の SOAP ヘッダー**

|**Header**|**要素**|**説明**|
|:-----|:-----|:-----|
|**DateTimePrecision** <br/> |[DateTimePrecision](datetimeprecision.md) <br/> |サーバーからの応答におけるデータ/時刻値の解決方法を秒単位で指定します。またはミリ秒単位で指定します。 これは要求に適用されます。  <br/> |
|**偽装** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |クライアントアプリケーションが偽装しているユーザーを識別します。 これは要求に適用されます。  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |メールボックスへのアクセスに使用する RFC3066 カルチャを指定します。 これは要求に適用されます。  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |操作要求のスキーマバージョンを識別します。 これは要求に適用されます。  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |要求に応答したサーバーのバージョンを識別します。 これは応答に適用されます。  <br/> |
|**TimeZoneContext** <br/> |[TimeZoneContext](timezonecontext.md) <br/> |サーバーからのすべての応答に使用するタイムゾーンを指定します。 これは要求に適用されます。  <br/> |
   
## <a name="finditem-operation-request-example"></a>FindItem 操作要求の例

次の**FindItem**要求の例は、[削除済みアイテム] フォルダーにあるアイテムの[Baseshape](baseshape.md)要素の**idonly**列挙で定義されているアイテム識別子を取得する方法を示しています。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
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

要求では、次の要素が使用されます。 
  
- [FindItem](finditem.md)
    
- [ItemShape](itemshape.md)
    
- [BaseShape](baseshape.md)
    
- [ParentFolderIds](parentfolderids.md)
    
- [DistinguishedFolderId](distinguishedfolderid.md)
    
**FindItem**要求メッセージのその他のオプションについては、スキーマ階層を参照してください。 [FindItem](finditem.md)要素から開始します。 
  
## <a name="successful-finditem-operation-response"></a>成功した FindItem 操作応答

次の例は、 **FindItem**要求に対する正常な応答を示しています。 
  
[Message](message-ex15websvcsotherref.md)要素は、電子メールメッセージと、EWS スキーマで厳密に型指定されていないその他すべてのアイテムを表します。 IPM などのアイテム。共有と IPM. InfoPath は、[メッセージ](message-ex15websvcsotherref.md)要素として返されます。 Exchange は、応答で基本[Item](item.md)要素を返しません。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

応答では、次の要素が使用されます。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [FindItemResponse](finditemresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [FindItemResponseMessage](finditemresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [RootFolder (FindItemResponseMessage)](rootfolder-finditemresponsemessage.md)
    
- [Items](items.md)
    
- [Message](message-ex15websvcsotherref.md)
    
- [ItemId](itemid.md)
    
**FindItem**応答メッセージのその他のオプションについては、スキーマ階層を参照してください。 [Finditemresponse](finditemresponse.md)要素から開始します。 
  
## <a name="finditem-operation-error-response"></a>FindItem 操作エラー応答

次の例は、 **FindItem**要求に対するエラー応答を示しています。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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
    
**FindItem**エラー応答メッセージのその他のオプションについては、スキーマ階層を参照してください。 [Finditemresponse](finditemresponse.md)要素から開始します。 
  
## <a name="version-differences"></a>バージョンの相違点

メジャーバージョン15以降のバージョンの Exchange は、アーカイブメールボックス内の複数のフォルダーを検索するために**FindItem**操作を使用し[て、15.0.898.11](responsecode.md)の ErrorInvalidOperation 値を返します。 
  
## <a name="see-also"></a>関連項目

- [アイテムの検索](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)
    
- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)
    
- **FindItemType**
    

