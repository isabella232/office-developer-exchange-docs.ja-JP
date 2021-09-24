---
title: CreateItem 操作 (タスク)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CreateItem
api_type:
- schema
ms.assetid: 12c5da4d-290c-4a8a-a965-0bf5d55c7978
description: CreateItem 操作では、タスク アイテムが作成され、Exchangeされます。
ms.openlocfilehash: 814a32e82cd5c1c95be252d1b53387741898dd40
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510259"
---
# <a name="createitem-operation-task"></a>CreateItem 操作 (タスク)

CreateItem 操作では、タスク アイテムが作成され、Exchangeされます。
  
## <a name="task-createitem-request"></a>タスクの CreateItem 要求

### <a name="description"></a>説明

CreateItem 要求の次の例は、メールボックスにタスク アイテムを作成する方法を示しています。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                MessageDisposition="SaveOnly">
      <Items>
        <t:Task>
          <t:Subject>My task</t:Subject>
          <t:DueDate>2006-10-26T21:32:52</t:DueDate>
          <t:Status>NotStarted</t:Status>
        </t:Task>
      </Items>
    </CreateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>コメント

定期的なタスクの要求は、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターによって受信された場合に変更されます。 次の変更が行われます。
  
- タスクの定期的な範囲の [StartDate (Recurrence)](startdate-recurrence.md) プロパティの日付だけが保存されます。 タイム パーツは切り捨てられて表示されます。 
    
- StartDate [(Recurrence)](startdate-recurrence.md) プロパティは、定期的なパターンに応じて調整できます。 たとえば、定期的なパターンが毎週月曜日として指定され、StartDate が 2006 年 10 月 26 日 (木曜日) に設定されている場合、StartDate は次の月曜日である 2006 年 10 月 30 日に調整されます。 
    
- タスクの [StartDate](startdate.md) プロパティが設定されている場合は、定期的な範囲の [StartDate (Recurrence)](startdate-recurrence.md) に一致する更新されます。 タスク [の DueDate](duedate.md) プロパティも、新しい StartDate に基づいて [更新されます](startdate.md)。
    
- [StartDate が設定されていない](startdate.md)場合、定期的な範囲の[StartDate (Recurrence)](startdate-recurrence.md)に一致する[DueDate](duedate.md)プロパティだけが更新されます。 
    
次の表は、毎週月曜日の Task.Recurrence.Pattern を持つ定期的なタスクに対してクライアント アクセス サーバーが行った変更を示しています。
  
**定期的なタスクへの変更**

|**プロパティ**|**元の値**|**更新された値**|
|:-----|:-----|:-----|
|Task.StartDate  <br/> |2006 年 1 月 1 日  <br/> |2006 年 10 月 30 日  <br/> |
|Task.DueDate  <br/> |2006 年 1 月 3 日  <br/> |2006 年 11 月 1 日  <br/> |
|Task.Recurrence.Range.StartDate  <br/> |2006 年 10 月 26 日  <br/> |2006 年 10 月 30 日  <br/> |
   
既定では、移動先フォルダーを指定しない場合、タスク アイテムは Tasks フォルダーに作成されます。
  
### <a name="request-elements"></a>要求要素

要求では、次の要素が使用されます。
  
- [CreateItem](createitem.md)
    
- [Items (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md)
    
- [タスク](task.md)
    
- [[件名]](subject.md)
    
- [DueDate](duedate.md)
    
- [状態](status.md)
    
## <a name="successful-task-createitem-response"></a>成功したタスクの CreateItem 応答

### <a name="description"></a>説明

次の例は、CreateItem 要求に対する正常な応答を示しています。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="653" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Task>
              <t:ItemId Id="AAAtAE=" ChangeKey="EwAAABYA"/>
            </t:Task>
          </m:Items>
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </CreateItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a>成功した応答要素

応答には、次の要素が含まれます。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [CreateItemResponse](createitemresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [CreateItemResponseMessage](createitemresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [Items (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md)
    
- [タスク](task.md)
    
- [ItemId](itemid.md)
    
## <a name="see-also"></a>関連項目



[CreateItem 操作](createitem-operation.md)


[タスクの作成](https://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[タスクの更新](https://msdn.microsoft.com/library/0a1bf360-d40c-4a99-929b-4c73a14394d5%28Office.15%29.aspx)
  
[タスクの削除](https://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

