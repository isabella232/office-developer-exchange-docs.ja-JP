---
title: GetAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GetAttachment
api_type:
- schema
ms.assetid: 9443cf96-b451-4530-b868-490dff798673
description: GetAttachment 要素は、アプリケーション ストアから添付ファイルを取得する要求のルートExchangeです。
ms.openlocfilehash: 057b42e78845f583cf1e52804e0108f335ef951c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546372"
---
# <a name="getattachment"></a>GetAttachment

**GetAttachment 要素** は、ファイル ストアから添付ファイルを取得する要求のルートExchangeです。 
  
```xml
<GetAttachment>
   <AttachmentShape/>
   <AttachmentIds/>
</GetAttachment>
```

 **GetAttachmentType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[AttachmentShape](attachmentshape.md) <br/> |[GetAttachment](getattachment.md)要求への応答で返す追加の拡張アイテム プロパティを識別します。 この要素は省略できます。  <br/> |
|[AttachmentIds](attachmentids.md) <br/> |添付ファイル識別子の配列を含む。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>注釈

[AttachmentShape](attachmentshape.md)要素は、応答で返されるプロパティを識別する必要はありません。 [GetAttachment 操作は、](getattachment-operation.md)添付ファイルの Name、ContentType、ContentId、ContentLocation、および Content プロパティを返します。 アイテムの添付ファイルの場合、返されるプロパティは Name、ContentType、ContentId、ContentLocation、および添付されたアイテムのすべてのプロパティです。 これは、GetItem 要求で AllProperties 基本図形を使用 [する場合と同](getitem.md) じです。 
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[GetAttachment 操作](getattachment-operation.md)
  
[GetAttachmentResponse](getattachmentresponse.md)

