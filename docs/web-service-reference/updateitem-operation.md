---
title: UpdateItem 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- UpdateItem
api_type:
- schema
ms.assetid: 5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4
description: UpdateItem 操作は、アイテム ストア内の既存のアイテムのプロパティを変更Exchangeされます。
ms.openlocfilehash: 6ac09c24c13efff8053fc605ec2c0e6cf2957429
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514061"
---
# <a name="updateitem-operation"></a>UpdateItem 操作

**UpdateItem 操作は**、アイテム ストア内の既存のアイテムのプロパティを変更Exchangeされます。 
  
## <a name="remarks"></a>注釈

アイテムに対して 3 つの基本的な更新アクションを実行できます。 次の表に、実行できるアクションの一覧を示します。
  
|**操作**|**説明**|
|:-----|:-----|
|追加  <br/> |既存のプロパティにデータを追加します。 このアクションでは、現在のデータが保持されます。 Append は、すべてのプロパティには適用されません。  <br/> |
|Set  <br/> |プロパティにデータが含まれている場合はプロパティのデータを置き換えるか、プロパティを作成し、プロパティが存在しない場合は値を設定します。 set アクションは、書き込み可能なプロパティにのみ適用されます。  <br/> |
|削除  <br/> |アイテムからプロパティを削除します。 これは、プロパティを空の値に設定する場合とは異なります。 このアクションが完了すると、アイテムのプロパティは存在しません。 Delete は書き込み可能なプロパティにのみ適用されます。  <br/> |
   
**UpdateItem 呼び出** しを使用して、1 つ以上のアイテム、および各アイテムの 1 つ以上のプロパティを変更できます。 [ItemChanges 要素](itemchanges.md)には、この呼び出しの一部として実行されるすべての変更が含まれる。 [ItemChange](itemchange.md)要素の子である[ItemChange](itemchanges.md)要素は、1 つのアイテムに対して実行する変更を表します。 [ItemChange 要素には](itemchange.md)、1 つのアイテムに対して実行できる一連の更新アクションが含まれる。 これらの変更は、Updates [(Item) 要素に含](updates-item.md) まれています。 [ItemId 要素は](itemid.md)、更新するアイテムを識別します。 アイテムの複数のプロパティを更新するには、更新が必要なプロパティごとに SetItemField、AppendToItemField、[または DeleteItemField](deleteitemfield.md)を指定する必要があります。 [](setitemfield.md) [](appendtoitemfield.md) 
  
> [!NOTE]
> 更新アクションは、指定された順序で適用されます。 
  
変更ごとに、変更するプロパティのパスと、新しい値を持つそのアイテムの表現を指定する必要があります。 削除アクションは、削除する必要があるプロパティのパスだけが必要になるという理由で少し異なります。 set アクションと append アクションの場合、指定するパスは、アイテム表現で設定されているのと同じプロパティを参照する必要があります。 これらが異なる場合は、エラーが返されます。
  
**UpdateItem 操作では**、ストア アイテム [](end-ex15websvcsotherref.md)の [開始](start.md)時刻と終了時刻Exchange設定できます。 **UpdateItem 要求では**、終了 [](start.md)時刻も設定せずに開始時刻を [設定](end-ex15websvcsotherref.md)できます。 開始時刻が終了時刻より後[](start.md)の場合、エラーが[発生する可能性](end-ex15websvcsotherref.md)があります。 クライアント アプリケーションは、期間を維持するために[](end-ex15websvcsotherref.md)開始時刻が変更[](start.md)された場合に終了時刻を調整する必要があります。 
  
1 つの予定表アイテムが定期的なマスター 予定表アイテムに更新される場合、予定表アイテムの元のタイム ゾーンを保持するには [、MeetingTimeZone](meetingtimezone.md) プロパティを **UpdateItem** 操作で設定する必要があります。 
  
## <a name="setitemfield-request-example"></a>SetItemField 要求の例

### <a name="description"></a>説明

UpdateItem 要求の次 **の例** は、アイテムの感度プロパティを設定する方法を示しています。 
  
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

アイテム識別子と変更キーは、読みやすさを維持するために短縮されました。
  
### <a name="setitemfield-request-elements"></a>SetItemField 要求要素

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

### <a name="description"></a>説明

**UpdateItem** 要求の次の例は、アイテムの body プロパティにテキストを追加する方法を示しています。 
  
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

次のプロパティは、追加アクションをサポートします。
  
- **message:ReplyTo**
    
- **item:Body**
    
- すべての受信者および出席者コレクションのプロパティ
    
アイテム識別子と変更キーは、読みやすさを維持するために短縮されました。
  
### <a name="appendtoitemfield-request-elements"></a>AppendToItemField 要求要素

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

### <a name="description"></a>説明

**UpdateItem** 要求の次の例は、アイテムのプロパティを削除する方法を示しています。 
  
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

アイテム識別子と変更キーは、読みやすさを維持するために短縮されました。
  
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

### <a name="description"></a>説明

次の例は、UpdateItem 要求に対する正常な **応答を示** しています。 
  
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

アイテム識別子と変更キーは、読みやすさを維持するために短縮されました。
  
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


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)


[連絡先の更新](https://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
  
[タスクの更新](https://msdn.microsoft.com/library/0a1bf360-d40c-4a99-929b-4c73a14394d5%28Office.15%29.aspx)

