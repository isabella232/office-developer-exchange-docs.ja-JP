---
title: CreateItem 操作 (タスク)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateItem
api_type:
- schema
ms.assetid: 12c5da4d-290c-4a8a-a965-0bf5d55c7978
description: CreateItem 操作は、Exchange ストア内の作業項目を作成します。
ms.openlocfilehash: 5a5203202071ae9391faa9348902424317ee96d1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759838"
---
# <a name="createitem-operation-task"></a>CreateItem 操作 (タスク)

CreateItem 操作は、Exchange ストア内の作業項目を作成します。
  
## <a name="task-createitem-request"></a>CreateItem 要求のタスク

### <a name="description"></a>説明

CreateItem 要求の次の例では、メールボックス内のタスク項目を作成する方法を示します。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
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

定期タスクの要求は、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターで受信したときに変更されます。 次の変更が発生します。
  
- タスクの期間の[開始日 (反復)](startdate-recurrence.md)プロパティの値は、日付のみが保存されます。 時刻の部分が切り捨てられます。 
    
- 定期的なパターンによって、[開始日 (繰り返し)](startdate-recurrence.md)のプロパティを調整することがあります。 開始日の調整など、定期的なパターンが、毎週月曜日を指定し、開始日が 2006 年 10 月 26 日に設定されている場合は木曜日で、2006 年 10 月 30 日には次の月曜日です。 
    
- タスクの[開始日](startdate.md)のプロパティが設定されている場合は、定期的なアイテムの範囲の[開始日 (反復)](startdate-recurrence.md)を一致するように更新されます。 タスクの[DueDate](duedate.md)プロパティに新しい[開始日](startdate.md)に基づいて更新されます。
    
- [開始日](startdate.md)が設定されていない場合は、定期的なアイテムの範囲の[開始日 (反復)](startdate-recurrence.md)を一致するように[DueDate](duedate.md)プロパティのみが更新されます。 
    
次の表は、定期的なタスクを毎週月曜日の Task.Recurrence.Pattern を持つクライアント アクセス サーバーが行った変更を示しています。
  
**定期的なタスクへの変更**

|**プロパティ**|**元の値**|**更新された値**|
|:-----|:-----|:-----|
|Task.StartDate  <br/> |2006 年 1 月 1 日  <br/> |2006 年 10 月 30 日  <br/> |
|Task.DueDate  <br/> |2006 年 1 月 3 日  <br/> |2006 年 11 月 1 日  <br/> |
|Task.Recurrence.Range.StartDate  <br/> |2006 年 10 月 26 日  <br/> |2006 年 10 月 30 日  <br/> |
   
既定では、インストール先のフォルダーが指定されていない場合タスク項目は、[タスク] フォルダーに作成されます。
  
### <a name="request-elements"></a>要素を要求します。

次の要素は、要求で使用されます。
  
- [CreateItem](createitem.md)
    
- [アイテム (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md)
    
- [タスク](task.md)
    
- [Subject](subject.md)
    
- [DueDate](duedate.md)
    
- [Status](status.md)
    
## <a name="successful-task-createitem-response"></a>Createitem メソッドの応答を正常終了したタスク

### <a name="description"></a>説明

次の使用例は、CreateItem 要求に正常な応答を示しています。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="653" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="successful-response-elements"></a>正常な応答の要素

応答では、次の要素が含まれています。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [CreateItemResponse](createitemresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [CreateItemResponseMessage](createitemresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [アイテム (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md)
    
- [タスク](task.md)
    
- [ItemId](itemid.md)
    
## <a name="see-also"></a>関連項目




  [CreateItem 操作](createitem-operation.md)


[タスクを作成します。](http://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[タスクの更新](http://msdn.microsoft.com/library/0a1bf360-d40c-4a99-929b-4c73a14394d5%28Office.15%29.aspx)
  
[タスクを削除します。](http://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

