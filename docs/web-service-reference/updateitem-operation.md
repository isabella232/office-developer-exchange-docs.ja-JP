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
description: UpdateItem 操作を使用して、Exchange ストア内の既存のアイテムのプロパティを変更します。
ms.openlocfilehash: 009ba16315017c4418fbd71d49744015c4d6d1b1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839865"
---
# <a name="updateitem-operation"></a>UpdateItem 操作

**UpdateItem**操作を使用して、Exchange ストア内の既存のアイテムのプロパティを変更します。 
  
## <a name="remarks"></a>備考

項目を次の 3 つの基本的な更新操作を行うことができます。 次の表は、実行できるアクションを示します。
  
|**アクション**|**説明**|
|:-----|:-----|
|追加  <br/> |データを既存のプロパティに追加します。 このアクションは、現在のデータを保持します。 追加のすべてのプロパティには適用されません。  <br/> |
|設定  <br/> |プロパティは、データ、または、プロパティを作成し、プロパティが存在しない場合、その値を設定する場合は、プロパティのデータを置き換えます。 アクションのセットは、書き込み可能なプロパティに適用できるのみです。  <br/> |
|削除  <br/> |アイテムからプロパティを削除します。 これは、空の値をプロパティの設定によって異なります。 この操作が完了したら、プロパティは項目には存在しません。 削除は、書き込み可能なプロパティに該当する場合のみです。  <br/> |
   
**UpdateItem**呼び出しは、1 つまたは複数の項目と各項目の 1 つまたは複数のプロパティを変更するのには使用できます。 [ItemChanges](itemchanges.md)要素には、この呼び出しの一部として実行されるすべての変更が含まれています。 [ItemChange](itemchange.md)の要素、 [ItemChanges](itemchanges.md)の要素の子では、1 つのアイテムに対して実行できる変更を表します。 [ItemChange](itemchange.md)要素には、1 つのアイテムに対して実行できる更新操作のセットが含まれています。 [(項目) の更新プログラム](updates-item.md)の要素では、これらの変更が含まれています。 [アイテム Id](itemid.md)要素は、更新する項目を識別します。 アイテムの 1 つ以上のプロパティを更新するには、 [SetItemField](setitemfield.md)、 [AppendToItemField](appendtoitemfield.md)、または[DeleteItemField](deleteitemfield.md)を更新プログラムを必要とするプロパティごとに指定してください。 
  
> [!NOTE]
> 更新アクションは、指定されている順序で適用されます。 
  
それぞれの変更の新しい値で変更するプロパティのパスと、その項目の表現を指定する必要です。 削除アクションは、削除するプロパティのパスのみが必要な点で多少異なります。 一連のアクションを追加しは、指定されているパスは、品目の表示に設定されている同じプロパティを参照する必要があります。 これらが異なる場合、エラーが戻されます。
  
**UpdateItem**操作は、Exchange ストアの項目の[開始](start.md)と[終了](end-ex15websvcsotherref.md)時間を設定できます。 **UpdateItem**要求では、[[終了](end-ex15websvcsotherref.md)時刻を設定せず、[開始](start.md)時刻を設定できます。 [開始](start.md)時刻は[終了](end-ex15websvcsotherref.md)時刻より後の場合は、エラーが発生することができます。 クライアント アプリケーションが、期間を保持するために[開始](start.md)時刻が変更されたときの[終了](end-ex15websvcsotherref.md)時刻を調整する必要があります。 
  
マスターの予定表の定期的なアイテムを 1 つの予定表アイテムが更新されると、予定表アイテムの元のタイム ゾーンを保持するために**UpdateItem**操作で[MeetingTimeZone](meetingtimezone.md)プロパティを設定しなければなりません。 
  
## <a name="setitemfield-request-example"></a>SetItemField 要求の例

### <a name="description"></a>説明

**UpdateItem**要求の次の使用例は、アイテムの秘密度のプロパティを設定する方法を示しています。 
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateItem MessageDisposition="SaveOnly" ConflictResolution="AutoResolve" 
                xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

項目の識別子と変更キーは、読みやすさを保持するために短縮されています。
  
### <a name="setitemfield-request-elements"></a>SetItemField 要求の要素

次の要素は、要求で使用されます。
  
- [UpdateItem](updateitem.md)
    
- [ItemChanges](itemchanges.md)
    
- [ItemChange](itemchange.md)
    
- [ItemId](itemid.md)
    
- [更新 (アイテム)](updates-item.md)
    
- [SetItemField](setitemfield.md)
    
- [FieldURI](fielduri.md)
    
- [Message](message-ex15websvcsotherref.md)
    
- [Sensitivity](sensitivity.md)
    
## <a name="appendtoitemfield-request-example"></a>AppendToItemField 要求の例

### <a name="description"></a>説明

**UpdateItem**要求の次の例では、アイテムの body プロパティにテキストを追加する方法を示します。 
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
  xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateItem MessageDisposition="SaveOnly" ConflictResolution="AutoResolve" 
                xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

次のプロパティは、追加操作をサポートします。
  
- **メッセージ: ReplyTo**
    
- **アイテムの本文:**
    
- すべての出席者と受信者コレクションのプロパティ
    
項目の識別子と変更キーは、読みやすさを保持するために短縮されています。
  
### <a name="appendtoitemfield-request-elements"></a>AppendToItemField 要求の要素

次の要素は、要求で使用されます。
  
- [UpdateItem](updateitem.md)
    
- [ItemChanges](itemchanges.md)
    
- [ItemChange](itemchange.md)
    
- [ItemId](itemid.md)
    
- [更新 (アイテム)](updates-item.md)
    
- [AppendToItemField](appendtoitemfield.md)
    
- [FieldURI](fielduri.md)
    
- [Message](message-ex15websvcsotherref.md)
    
- [Body/本文](body.md)
    
## <a name="deleteitemfield-request-example"></a>DeleteItemField 要求の例

### <a name="description"></a>説明

**UpdateItem**要求の次の例では、アイテムのプロパティを削除する方法を示します。 
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
  xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateItem MessageDisposition="SaveOnly" ConflictResolution="AutoResolve" 
                xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

項目の識別子と変更キーは、読みやすさを保持するために短縮されています。
  
### <a name="deleteitemfield-request-elements"></a>DeleteItemField 要求の要素

次の要素は、要求で使用されます。
  
- [UpdateItem](updateitem.md)
    
- [ItemChanges](itemchanges.md)
    
- [ItemChange](itemchange.md)
    
- [ItemId](itemid.md)
    
- [更新 (アイテム)](updates-item.md)
    
- [DeleteItemField](deleteitemfield.md)
    
- [FieldURI](fielduri.md)
    
## <a name="successful-response-example"></a>正常な応答の例

### <a name="description"></a>説明

**UpdateItem**要求に正常な応答の例を次に示します。 
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
  xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="664" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <UpdateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

項目の識別子と変更キーは、読みやすさを保持するために短縮されています。
  
### <a name="successful-response-elements"></a>正常な応答の要素

次の要素は、応答で使用されます。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [UpdateItemResponse](updateitemresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [UpdateItemResponseMessage](updateitemresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [Items](items.md)
    
- [Message](message-ex15websvcsotherref.md)
    
- [ItemId](itemid.md)
    
## <a name="see-also"></a>関連項目



[UpdateItem 処理 (タスク)](updateitem-operation-task.md)
  
[UpdateItem 操作 (連絡先)](updateitem-operation-contact.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)


[連絡先を更新](http://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
  
[タスクの更新](http://msdn.microsoft.com/library/0a1bf360-d40c-4a99-929b-4c73a14394d5%28Office.15%29.aspx)

