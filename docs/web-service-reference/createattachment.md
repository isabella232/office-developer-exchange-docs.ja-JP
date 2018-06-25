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
description: CreateAttachment 要素は、Exchange ストア内のアイテムに添付ファイルを作成する要求を定義します。
ms.openlocfilehash: d403eb5ca15623d3a973f7b224dbcde5529cf1bc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759799"
---
# <a name="createattachment"></a>CreateAttachment

**CreateAttachment**要素は、Exchange ストア内のアイテムに添付ファイルを作成する要求を定義します。 
  
```xml
<CreateAttachment>
   <ParentItemId/>
   <Attachments/>
</CreateAttachment>
```

 **CreateAttachmentType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[ParentItemId](parentitemid.md) <br/> |作成された添付ファイルを含む親の Exchange ストアの項目を識別します。 [ParentItemId](parentitemid.md)要素は、実際の Exchange の ID の項目を格納する必要があります。 [GetItem 操作](getitem-operation.md)を使用して、実際のオンライン ストアのアイテムを取得することができます。[GetAttachment 操作](getattachment-operation.md)を使用して添付ファイルが取得されます。 [ParentItemId](parentitemid.md)の添付ファイルの ID が渡された場合、エラーが発生します。 [ParentItemId](parentitemid.md)は、既存のアイテムの添付ファイルの ID を表している場合、 [CreateAttachment 操作](createattachment-operation.md)は、既存の添付ファイルに新しい添付ファイルを追加します。  <br/> この要素は、 [CreateAttachment 操作](createattachment-operation.md)に必要です。  <br/> |
|[添付ファイル](attachments-ex15websvcsotherref.md) <br/> |アイテムまたは Exchange ストア内のアイテムに添付するファイルが含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>備考

アイテムの添付ファイルは、ストアのアイテムとしては存在しません。 アイテムの添付ファイルまたは別の添付ファイルとしてのみ存在します。 [GetAttachment](getattachment.md)要求を使用して項目の添付ファイルを取得することができますのみです。 
  
次の項目の添付ファイルを作成することができます。
  
- Item
    
- Message
    
- カレンダー項目
    
- 連絡先
    
- タスク
    
- MeetingMessage
    
- MeetingRequest
    
MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="example"></a>例

次の例では、作成し、Exchange ストア内の別のアイテムにアイテムを添付する方法を示します。
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateAttachment xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" 
                  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[CreateAttachment 操作](createattachment-operation.md)
  
[DeleteAttachment 操作](deleteattachment-operation.md)
  
[GetAttachment 操作](getattachment-operation.md)

