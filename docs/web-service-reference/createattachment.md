---
title: CreateAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateAttachment
api_type:
- schema
ms.assetid: e33b403a-b7d3-48ee-8d24-6b7abf0d70bc
description: CreateAttachment 要素は、Exchange ストア内のアイテムに添付ファイルを作成するための要求を定義します。
ms.openlocfilehash: 4cba1b8865dae5da58b9617b249a29314c67331a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466438"
---
# <a name="createattachment"></a>CreateAttachment

**Createattachment**要素は、Exchange ストア内のアイテムに添付ファイルを作成するための要求を定義します。 
  
```xml
<CreateAttachment>
   <ParentItemId/>
   <Attachments/>
</CreateAttachment>
```

 **CreateAttachmentType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[ParentItemId](parentitemid.md) <br/> |作成された添付ファイルを含む親 Exchange ストアアイテムを識別します。 [Parentitemid](parentitemid.md)要素は、実際の Exchange ストアアイテムの ID を提供する必要があります。 実際のストアアイテムは、 [GetItem 操作](getitem-operation.md)を使用して取得できます。添付ファイルは、 [Getattachment 操作](getattachment-operation.md)を使用して取得されます。 [Parentitemid](parentitemid.md)に添付ファイルの id が渡されると、エラーが発生します。 [Parentitemid](parentitemid.md)が既存のアイテムの添付ファイルの id を表す場合、 [createattachment 操作](createattachment-operation.md)は既存の添付ファイルに新しい添付ファイルを追加します。  <br/> この要素は、 [Createattachment 操作](createattachment-operation.md)に必要です。  <br/> |
|[Attachments](attachments-ex15websvcsotherref.md) <br/> |Exchange ストア内のアイテムに添付するアイテムまたはファイルが保存されています。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>注釈

アイテムの添付ファイルは、ストアアイテムとして存在しません。 アイテムまたは他の添付ファイルの添付ファイルとしてのみ存在します。 アイテムの添付ファイルは、 [Getattachment](getattachment.md)要求を使用してのみ取得できます。 
  
次のアイテムの添付ファイルを作成できます。
  
- 項目
    
- メッセージ
    
- CalendarItem
    
- Contact
    
- タスク
    
- MeetingMessage
    
- MeetingRequest
    
この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="example"></a>例

次の例は、Exchange ストア内の別のアイテムにアイテムを作成して接続する方法を示しています。
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateAttachment xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" 
                  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <ParentItemId Id="ASkAS"/>
      <Attachments>
        <t:ItemAttachment>
          <t:Name>MyAttachment</t:Name>
          <t:Message>
            <t:ItemClass>IPM>Note</t:ItemClass>
            <t:Subject>My attachment subject</t:Subject>
            <t:Body BodyType="Text">My attachment body</t:Body>
          </t:Message>
        </t:ItemAttachment>
      </Attachments>
    </CreateAttachment>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[CreateAttachment 操作](createattachment-operation.md)
  
[DeleteAttachment 操作](deleteattachment-operation.md)
  
[GetAttachment 操作](getattachment-operation.md)

