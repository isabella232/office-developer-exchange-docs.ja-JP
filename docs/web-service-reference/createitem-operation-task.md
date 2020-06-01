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
description: CreateItem 操作は、Exchange ストアにタスクアイテムを作成します。
ms.openlocfilehash: 502108843193e7ed8377b0fade9e106ef3d1976c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457103"
---
# <a name="createitem-operation-task"></a>CreateItem 操作 (タスク)

CreateItem 操作は、Exchange ストアにタスクアイテムを作成します。
  
## <a name="task-createitem-request"></a>Task CreateItem 要求

### <a name="description"></a>説明

次の CreateItem 要求の例は、メールボックス内のタスクアイテムを作成する方法を示しています。
  
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

定期的なタスクに対する要求は、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターが受信したときに変更されます。 次の変更が行われます。
  
- タスクの定期的なアイテムの期間の開始日[(定期的なアイテム)](startdate-recurrence.md)のプロパティには、日付のみが保存されます。 時刻部分は切り捨てられます。 
    
- [StartDate (定期的なアイテム)](startdate-recurrence.md)プロパティは、定期的なパターンに応じて調整できます。 たとえば、定期パターンが毎週月曜日として指定されていて、StartDate が2006年10月26日に設定されている場合、StartDate は次の月曜日である2006年10月30日に調整されます。 
    
- タスクの[startdate](startdate.md)プロパティが設定されている場合は、定期的なアイテムの範囲の[startdate (繰り返し)](startdate-recurrence.md)に合わせて更新されます。 タスクの[DueDate](duedate.md)プロパティも、新しい[StartDate](startdate.md)に基づいて更新されます。
    
- [Startdate](startdate.md)が設定されていない場合は、 [DueDate](duedate.md)プロパティのみが更新され、定期的なアイテムの範囲の[startdate (繰り返し)](startdate-recurrence.md)に一致します。 
    
次の表に、クライアントアクセスサーバーが、毎週月曜日の定期タスクに対して行う変更を示します。
  
**定期的なタスクに対する変更**

|**Property**|**元の値**|**更新された値**|
|:-----|:-----|:-----|
|タスクの開始日  <br/> |2006年1月1日  <br/> |2006年10月30日  <br/> |
|DueDate  <br/> |2006年1月3日  <br/> |2006年11月1日  <br/> |
|タスクの定期的なアイテムの指定。  <br/> |2006年10月26日  <br/> |2006年10月30日  <br/> |
   
既定では、宛先フォルダーが指定されていない場合、タスクアイテムは [タスク] フォルダーに作成されます。
  
### <a name="request-elements"></a>Request 要素

要求では、次の要素が使用されます。
  
- [CreateItem](createitem.md)
    
- [アイテム (非 Emptyarrayofallitemstype)](items-nonemptyarrayofallitemstype.md)
    
- [Task](task.md)
    
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

応答には、次の要素が含まれています。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [CreateItemResponse](createitemresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [CreateItemResponseMessage](createitemresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [アイテム (非 Emptyarrayofallitemstype)](items-nonemptyarrayofallitemstype.md)
    
- [Task](task.md)
    
- [ItemId](itemid.md)
    
## <a name="see-also"></a>関連項目




  [CreateItem 操作](createitem-operation.md)


[タスクの作成](https://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[タスクの更新](https://msdn.microsoft.com/library/0a1bf360-d40c-4a99-929b-4c73a14394d5%28Office.15%29.aspx)
  
[タスクの削除](https://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

