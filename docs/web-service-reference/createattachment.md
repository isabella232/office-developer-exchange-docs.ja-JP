---
title: CreateAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CreateAttachment
api_type:
- schema
ms.assetid: e33b403a-b7d3-48ee-8d24-6b7abf0d70bc
description: CreateAttachment 要素は、カスタム ストア内のアイテムへの添付ファイルを作成する要求をExchangeします。
ms.openlocfilehash: 6716a83b0d1ba9d7f39351da60f7009df04a3fa0
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515874"
---
# <a name="createattachment"></a>CreateAttachment

**CreateAttachment 要素** は、カスタム ストア内のアイテムへの添付ファイルを作成する要求をExchangeします。 
  
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
|[ParentItemId](parentitemid.md) <br/> |作成された添付ファイルExchange含むストア アイテムの親オブジェクトを識別します。 [ParentItemId 要素は](parentitemid.md)、実際のストア アイテムの ID をExchange必要があります。 GetItem 操作を使用して、実際のストア アイテム [を取得できます](getitem-operation.md)。添付ファイルは [GetAttachment 操作を使用して取得されます](getattachment-operation.md)。 [ParentItemId](parentitemid.md)に添付ファイルの ID が渡された場合、エラーが発生します。 [ParentItemId が既存](parentitemid.md)のアイテム添付ファイルの ID を表す場合[、CreateAttachment](createattachment-operation.md)操作は新しい添付ファイルを既存の添付ファイルに追加します。  <br/> この要素は [、CreateAttachment 操作に必要です](createattachment-operation.md)。  <br/> |
|[添付ファイル](attachments-ex15websvcsotherref.md) <br/> |アイテム ストア内のアイテムに添付するアイテムまたはファイルExchangeします。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>注釈

アイテムの添付ファイルは、ストア アイテムとして存在しません。 アイテムまたは別の添付ファイルへの添付ファイルとしてのみ存在します。 アイテムの添付ファイルは [、GetAttachment](getattachment.md) 要求を使用してのみ取得できます。 
  
次のアイテムの添付ファイルを作成できます。
  
- アイテム
    
- メッセージ
    
- CalendarItem
    
- Contact
    
- タスク
    
- MeetingMessage
    
- MeetingRequest
    
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="example"></a>例

次の使用例は、アイテムを作成し、アイテムストア内の別のアイテムにExchangeします。
  
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
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[CreateAttachment 操作](createattachment-operation.md)
  
[DeleteAttachment 操作](deleteattachment-operation.md)
  
[GetAttachment 操作](getattachment-operation.md)

