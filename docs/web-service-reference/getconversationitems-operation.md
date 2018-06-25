---
title: GetConversationItems の操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8ae00a99-b37b-4194-829c-fe300db6ab99
description: GetConversationItems の操作に関する情報を検索します。
ms.openlocfilehash: 9d9fb9cc04bcbb5846162c77c852defa51dff98b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760672"
---
# <a name="getconversationitems-operation"></a>GetConversationItems の操作

**GetConversationItems**の操作に関する情報を検索します。 
  
**GetConversationItems**操作では、会話内のノードで構成されたアイテムの 1 つまたは複数のセットを取得します。 
  
この操作は Exchange Server 2013 で導入されました。
  
## <a name="using-the-getconversationitems-operation"></a>GetConversationItems 操作を使用します。

**GetConversationItems**操作を使用すると、原色の両方の会話とアーカイブ メールボックス内のアイテムを取得します。 
  
### <a name="getconversationitems-operation-soap-headers"></a>GetConversationItems 操作の SOAP ヘッダー

**GetConversationItems**操作は、次の表に記載されている SOAP ヘッダーを使用できます。 
  
|**ヘッダー名**|**要素**|**説明**|
|:-----|:-----|:-----|
|**偽装** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |クライアント アプリケーションが偽装するユーザーを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |操作要求のスキーマのバージョンを識別します。 この要素の最小値は、 **Exchange2013**です。 このヘッダーは、要求に適用されます。  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |要求に応答するサーバーのバージョンを識別します。 このヘッダーは、応答に適用されます。  <br/> |
   
## <a name="getconversationitems-operation-request-example-get-items-in-a-single-conversation"></a>GetConversationItems 操作の要求の例: 1 つの会話でアイテムを取得

**GetConversationItems**操作要求の次の例では、削除済みアイテムおよび [下書き] フォルダー内にある項目を除いて、1 つのテーマでの会話のすべての項目を取得する方法を示します。 応答で返される各項目は、項目 id、件名、およびアイテムをメールボックスで受信した時間に含まれます。 
  
> [!NOTE]
> すべての項目の識別子と変更キーをこの資料では、読みやすさを保持するために短縮されています。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body>
      <m:GetConversationItems>
         <m:ItemShape>
            <t:BaseShape>IdOnly</t:BaseShape>
            <t:AdditionalProperties>
               <t:FieldURI FieldURI="item:Subject" />
               <t:FieldURI FieldURI="item:DateTimeReceived" />
            </t:AdditionalProperties>
         </m:ItemShape>
         <m:FoldersToIgnore>
            <t:DistinguishedFolderId Id="deleteditems" />
            <t:DistinguishedFolderId Id="drafts" />
         </m:FoldersToIgnore>
         <m:SortOrder>TreeOrderDescending</m:SortOrder>
         <m:Conversations>
            <t:Conversation>
               <t:ConversationId Id="AAQkADEzOTExYjJkakJCs=" />
            </t:Conversation>
         </m:Conversations>
      </m:GetConversationItems>
   </soap:Body>
</soap:Envelope>
```

**GetConversationItems**要求の次の使用例では、次のオプションは含まれません。 
  
- [MaxItemsToReturn](maxitemstoreturn.md)要素の応答を取得するアイテムの最大数を設定します。 
    
- [MailboxScope](mailboxscope.md)要素、 **GetConversationItems**操作は、プライマリ メールボックス、アーカイブ先のメールボックス、または両方のメールボックスに対して実行するかどうかを示すことによってメールボックスのスコープを設定します。 
    
- [同期状態 (base64Binary)](syncstate-base64binary.md)要素、だけは、スレッドの会話の項目を取得するのには同期の状態を設定します。 この要素は、会話ごとに設定されています。 
    
要求 SOAP 本体にはには、次の要素が含まれています。
  
- [GetConversationItems](getconversationitems.md)
    
- [ItemShape](itemshape.md)
    
- [BaseShape](baseshape.md)
    
- [AdditionalProperties](additionalproperties.md)
    
- [FieldURI](fielduri.md)
    
- [FoldersToIgnore](folderstoignore.md)
    
- [DistinguishedFolderId](distinguishedfolderid.md)
    
- [並べ替え順序 (ConversationNodeSortOrder)](sortorder-conversationnodesortorder.md)
    
- [スレッド](conversations-ex15websvcsotherref.md)
    
- [会話 (ConversationRequestType)](conversation-conversationrequesttype.md)
    
- [ConversationId](conversationid.md)
    
## <a name="successful-getconversationitems-operation-response"></a>GetConversationItems 操作の成功の応答

次の例では、1 つの会話でアイテムを取得する**GetConversationItems**操作要求に正常な応答を示します。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15"
                           MinorVersion="0"
                           MajorBuildNumber="545"
                           MinorBuildNumber="11"
                           Version="Exchange2013"
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:GetConversationItemsResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:GetConversationItemsResponseMessage ResponseClass="Success">
               <m:ResponseCode>NoError</m:ResponseCode>
               <m:Conversation>
                  <t:ConversationId Id="AAQkADEzOTExYjJkakJCs=" />
                  <t:SyncState>AQIAAABNVkUwAgIAAABhHqHUAwIAAABNVkUxBAIAAABhHqHfBAIAAABhHqHV</t:SyncState>
                  <t:ConversationNodes>
                     <t:ConversationNode>
                        <t:InternetMessageId>6a4838fa804045e09d40c1a39b9ea916@contoso.com</t:InternetMessageId>
                        <t:ParentInternetMessageId>15a56698d503438fbdaa18186d5b81b7@contoso.com</t:ParentInternetMessageId>
                        <t:Items>
                           <t:Message>
                              <t:ItemId Id="AAMkADEzOTQrAABhHqHfAAA=" ChangeKey="CQAAABYAAACYAABhPpaq" />
                              <t:Subject>RE: Daily issue scrub</t:Subject>
                              <t:DateTimeReceived>2012-10-30T18:42:27Z</t:DateTimeReceived>
                           </t:Message>
                        </t:Items>
                     </t:ConversationNode>
                     <t:ConversationNode>
                        <t:InternetMessageId>2695d2b837954d68846b0c30491f5af1@contoso.com</t:InternetMessageId>
                        <t:ParentInternetMessageId>15a56698d503438fbdaa18186d5b81b7@contoso.com</t:ParentInternetMessageId>
                        <t:Items>
                           <t:Message>
                              <t:ItemId Id="AAMkADEzOTExYjJkLTYxZDAt" ChangeKey="CQAAABQrAABhPpaP" />
                              <t:Subject>RE: Daily issue scrub</t:Subject>
                              <t:DateTimeReceived>2012-10-30T17:38:26Z</t:DateTimeReceived>
                           </t:Message>
                        </t:Items>
                     </t:ConversationNode>
                     <t:ConversationNode>
                        <t:InternetMessageId>15a56698d503438fbdaa18186d5b81b7@contoso.com</t:InternetMessageId>
                        <t:ParentInternetMessageId>d3113e59c89c4288ae13100d033f8dbc@contoso.com</t:ParentInternetMessageId>
                        <t:Items>
                           <t:Message>
                              <t:ItemId Id="AAMkADEzOTFNVkUxAAA=" ChangeKey="CQAAABY4QrAABhPvYK" />
                              <t:Subject>RE: Daily issue scrub</t:Subject>
                              <t:DateTimeReceived>2012-10-30T17:37:00Z</t:DateTimeReceived>
                           </t:Message>
                        </t:Items>
                     </t:ConversationNode>
                     <t:ConversationNode>
                        <t:InternetMessageId>d3113e59c89c4288ae13100d033f8dbc@contoso.com</t:InternetMessageId>
                        <t:ParentInternetMessageId>189b712056c2430dbce334b40496ad00@contoso.com</t:ParentInternetMessageId>
                        <t:Items>
                           <t:Message>
                              <t:ItemId Id="AAMkm4QrAABhHqHUAAA=" ChangeKey="CQAAABQrAABhPpaN" />
                              <t:Subject>RE: Daily issue scrub</t:Subject>
                              <t:DateTimeReceived>2012-10-30T17:37:05Z</t:DateTimeReceived>
                           </t:Message>
                        </t:Items>
                     </t:ConversationNode>
                     <t:ConversationNode>
                        <t:InternetMessageId>189b712056c2430dbce334b40496ad00@contoso.com</t:InternetMessageId>
                        <t:Items>
                           <t:Message>
                              <t:ItemId Id="AAMkArAABNVkUwAAA=" ChangeKey="CQAAABm4QrAABhPvYJ" />
                              <t:Subject>Daily issue scrub</t:Subject>
                              <t:DateTimeReceived>2012-10-30T17:36:00Z</t:DateTimeReceived>
                           </t:Message>
                        </t:Items>
                     </t:ConversationNode>
                  </t:ConversationNodes>
               </m:Conversation>
            </m:GetConversationItemsResponseMessage>
         </m:ResponseMessages>
      </m:GetConversationItemsResponse>
   </s:Body>
</s:Envelope>
```

**GetConversationItems**の後続の操作要求の同期状態を保存することをお勧めします。 
  
応答 SOAP 本文には、次の要素が含まれています。
  
- [GetConversationItemsResponse](getconversationitemsresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [GetConversationItemsResponseMessage](getconversationitemsresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [会話 (ConversationResponseType)](conversation-conversationresponsetype.md)
    
- [ConversationId](conversationid.md)
    
- [同期状態 (base64Binary)](syncstate-base64binary.md)
    
- [ConversationNodes](conversationnodes.md)
    
- [ConversationNode](conversationnode.md)
    
- [InternetMessageId](internetmessageid.md)
    
- [アイテム (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md)
    
- [Message](message-ex15websvcsotherref.md)
    
- [ItemId](itemid.md)
    
- [Subject](subject.md)
    
- [DateTimeReceived](datetimereceived.md)
    
## <a name="getconversationitems-operation-error-response"></a>GetConversationItems 操作のエラー応答

次の使用例は、メールボックス、または、会話のすべての項目内にあるフォルダーは無視されるは、存在しないのいずれかの会話で項目を取得する**GetConversationItems**の操作要求に対するエラー応答を示しています。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="556" MinorBuildNumber="8" Version="Exchange2013" xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" xmlns="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetConversationItemsResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetConversationItemsResponseMessage ResponseClass="Error">
          <m:MessageText>The specified object was not found in the store.</m:MessageText>
          <m:ResponseCode>ErrorItemNotFound</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:GetConversationItemsResponseMessage>
      </m:ResponseMessages>
    </m:GetConversationItemsResponse>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a>関連項目

- [Exchange での EWS の操作](ews-operations-in-exchange.md)
    
- [ApplyConversationAction 操作](applyconversationaction-operation.md)
    
- 
  [FindConversation 操作](findconversation-operation.md)
    

