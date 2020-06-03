---
title: UpdateItem 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateItem
api_type:
- schema
ms.assetid: 5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4
description: UpdateItem 操作は、Exchange ストア内の既存のアイテムのプロパティを変更するために使用されます。
ms.openlocfilehash: c001b7656862144023e9704cb04e6b4c0030f9df
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459392"
---
# <a name="updateitem-operation"></a>UpdateItem 操作

**Updateitem**操作は、Exchange ストア内の既存のアイテムのプロパティを変更するために使用されます。 
  
## <a name="remarks"></a>注釈

アイテムに対して3つの基本的な更新操作を実行できます。 次の表に、実行できるアクションを示します。
  
|**操作**|**説明**|
|:-----|:-----|
|追加  <br/> |既存のプロパティにデータを追加します。 この操作を行うと、現在のデータが保持されます。 Append は、すべてのプロパティに適用されません。  <br/> |
|Set  <br/> |プロパティのデータが含まれている場合は、プロパティのデータを置換します。プロパティが存在しない場合は、プロパティを作成し、その値を設定します。 Set アクションは、書き込み可能なプロパティにのみ適用されます。  <br/> |
|削除  <br/> |アイテムからプロパティを削除します。 これは、プロパティを空の値に設定することとは異なります。 この操作が完了すると、アイテムのプロパティが存在しなくなります。 Delete は、書き込み可能なプロパティにのみ適用されます。  <br/> |
   
**Updateitem**呼び出しを使用すると、1つ以上のアイテム、および各アイテムの1つ以上のプロパティを変更できます。 [Itemchanges](itemchanges.md)要素には、この呼び出しの一部として実行されるすべての変更が含まれています。 [Itemchange](itemchange.md)要素 ( [itemchange](itemchanges.md)要素の子) は、1つのアイテムに対して実行される変更を表します。 [Itemchange](itemchange.md)要素には、1つのアイテムに対して実行できる更新アクションのセットが含まれています。 これらの変更は、 [Updates (Item)](updates-item.md)要素に含まれています。 [ItemId](itemid.md)要素は、更新するアイテムを識別します。 アイテムで複数のプロパティを更新するには、更新が必要な各プロパティに対して[SetItemField](setitemfield.md)、 [appendtoitemfield](appendtoitemfield.md)、または[deleteitemfield](deleteitemfield.md)を指定する必要があります。 
  
> [!NOTE]
> 更新操作は、指定された順序で適用されます。 
  
変更ごとに、変更するプロパティのパスと、そのアイテムの新しい値を表す表現を指定する必要があります。 Delete アクションは、削除する必要のあるプロパティのパスのみが必要になるということとは少し異なります。 Set および append アクションの場合、指定されたパスは、アイテム表現で設定されているのと同じプロパティを参照する必要があります。 これらが異なる場合は、エラーが返されます。
  
**Updateitem**操作は、Exchange ストアアイテムの[開始](start.md)時刻と[終了](end-ex15websvcsotherref.md)時刻を設定できます。 **Updateitem**要求では、[終了](end-ex15websvcsotherref.md)時刻を設定することなく、[開始](start.md)時刻を設定することもできます。 これにより、[開始](start.md)時刻が[終了](end-ex15websvcsotherref.md)時刻よりも後の場合にエラーが発生することがあります。 期間を保持するために[開始](start.md)時刻が変更された場合、クライアントアプリケーションは[終了](end-ex15websvcsotherref.md)時刻を調整する必要があることに注意してください。 
  
1つの予定表アイテムを定期的マスターの予定表アイテムに更新する場合は、予定表アイテムの元のタイムゾーンを保持するために、 **updateitem**操作によって、[会議 timezone](meetingtimezone.md)プロパティを設定する必要があります。 
  
## <a name="setitemfield-request-example"></a>SetItemField 要求の例

### <a name="description"></a>Description

次の**updateitem**要求の例は、アイテムに対して [秘密度] プロパティを設定する方法を示しています。 
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateItem MessageDisposition="SaveOnly" ConflictResolution="AutoResolve" 
                xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="AAAtAEFkb..." ChangeKey="CQAAABYAAAB..."/>
          <t:Updates>
            <t:SetItemField>
              <t:FieldURI FieldURI="item:Sensitivity"/>
              <t:Message>
                <t:Sensitivity>Normal</t:Sensitivity>
              </t:Message>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
      </ItemChanges>
    </UpdateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>コメント

読みやすくするために、アイテム識別子と変更キーが短縮されています。
  
### <a name="setitemfield-request-elements"></a>SetItemField Request 要素

要求では、次の要素が使用されます。
  
- [UpdateItem](updateitem.md)
    
- [ItemChanges](itemchanges.md)
    
- [ItemChange](itemchange.md)
    
- [ItemId](itemid.md)
    
- [Updates (Item)](updates-item.md)
    
- [SetItemField](setitemfield.md)
    
- [FieldURI](fielduri.md)
    
- [Message](message-ex15websvcsotherref.md)
    
- [Sensitivity](sensitivity.md)
    
## <a name="appendtoitemfield-request-example"></a>AppendToItemField 要求の例

### <a name="description"></a>Description

次の**updateitem**要求の例は、アイテムの body プロパティにテキストを追加する方法を示しています。 
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
  xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateItem MessageDisposition="SaveOnly" ConflictResolution="AutoResolve" 
                xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="AAAtAEFkbW..." ChangeKey="CQAAABYA..."/>
          <t:Updates>
            <t:AppendToItemField>
              <t:FieldURI FieldURI="item:Body"/>
              <t:Message>
                <t:Body BodyType="Text">Some additional text to append</t:Body>
              </t:Message>
            </t:AppendToItemField>
          </t:Updates>
        </t:ItemChange>
      </ItemChanges>
    </UpdateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>コメント

次のプロパティは、append アクションをサポートします。
  
- **メッセージ: ReplyTo**
    
- **アイテム: 本文**
    
- すべての受信者と出席者のコレクションのプロパティ
    
読みやすくするために、アイテム識別子と変更キーが短縮されています。
  
### <a name="appendtoitemfield-request-elements"></a>AppendToItemField Request 要素

要求では、次の要素が使用されます。
  
- [UpdateItem](updateitem.md)
    
- [ItemChanges](itemchanges.md)
    
- [ItemChange](itemchange.md)
    
- [ItemId](itemid.md)
    
- [Updates (Item)](updates-item.md)
    
- [AppendToItemField](appendtoitemfield.md)
    
- [FieldURI](fielduri.md)
    
- [Message](message-ex15websvcsotherref.md)
    
- [Body](body.md)
    
## <a name="deleteitemfield-request-example"></a>DeleteItemField 要求の例

### <a name="description"></a>Description

次の**updateitem**要求の例は、アイテムのプロパティを削除する方法を示しています。 
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
  xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateItem MessageDisposition="SaveOnly" ConflictResolution="AutoResolve" 
                xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="AAAtAEFkbWluaXN0cm..." ChangeKey="CQAAABYAA..."/>
          <t:Updates>
            <t:DeleteItemField>
              <t:FieldURI FieldURI="item:Body"/>
            </t:DeleteItemField>
          </t:Updates>
        </t:ItemChange>
      </ItemChanges>
    </UpdateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>コメント

読みやすくするために、アイテム識別子と変更キーが短縮されています。
  
### <a name="deleteitemfield-request-elements"></a>DeleteItemField 要求要素

要求では、次の要素が使用されます。
  
- [UpdateItem](updateitem.md)
    
- [ItemChanges](itemchanges.md)
    
- [ItemChange](itemchange.md)
    
- [ItemId](itemid.md)
    
- [Updates (Item)](updates-item.md)
    
- [DeleteItemField](deleteitemfield.md)
    
- [FieldURI](fielduri.md)
    
## <a name="successful-response-example"></a>成功した応答の例

### <a name="description"></a>Description

次の例は、 **Updateitem**要求に対する正常な応答を示しています。 
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
  xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="664" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <UpdateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:UpdateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Message>
              <t:ItemId Id="AAAtAEFkbW..." ChangeKey="CQAAABYAAA..."/>
            </t:Message>
          </m:Items>
        </m:UpdateItemResponseMessage>
      </m:ResponseMessages>
    </UpdateItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>コメント

読みやすくするために、アイテム識別子と変更キーが短縮されています。
  
### <a name="successful-response-elements"></a>成功した応答要素

応答では、次の要素が使用されます。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [UpdateItemResponse](updateitemresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [UpdateItemResponseMessage](updateitemresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [Items](items.md)
    
- [Message](message-ex15websvcsotherref.md)
    
- [ItemId](itemid.md)
    
## <a name="see-also"></a>関連項目



[UpdateItem 操作 (タスク)](updateitem-operation-task.md)
  
[UpdateItem 操作 (連絡先)](updateitem-operation-contact.md)


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)


[連絡先の更新](https://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
  
[タスクの更新](https://msdn.microsoft.com/library/0a1bf360-d40c-4a99-929b-4c73a14394d5%28Office.15%29.aspx)

