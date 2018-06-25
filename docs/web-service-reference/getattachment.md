---
title: GetAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetAttachment
api_type:
- schema
ms.assetid: 9443cf96-b451-4530-b868-490dff798673
description: GetAttachment 要素は、Exchange ストアからの添付ファイルを取得する要求のルート要素です。
ms.openlocfilehash: fb639c86a0654e8f9e9601310f7c2f5b0fc7d729
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760640"
---
# <a name="getattachment"></a>GetAttachment

**GetAttachment**要素は、Exchange ストアからの添付ファイルを取得する要求のルート要素です。 
  
```xml
<GetAttachment>
   <AttachmentShape/>
   <AttachmentIds/>
</GetAttachment>
```

 **GetAttachmentType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[AttachmentShape](attachmentshape.md) <br/> |[GetAttachment](getattachment.md)要求への応答で返されるその他の拡張アイテム プロパティを識別します。 この要素はオプションです。  <br/> |
|[AttachmentIds](attachmentids.md) <br/> |添付ファイル識別子の配列が含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>備考

[AttachmentShape](attachmentshape.md)要素は、応答で返されるプロパティを識別するために必要ではありません。 [GetAttachment 操作](getattachment-operation.md)には、名前、コンテンツ タイプ、ContentId、ContentLocation、および添付ファイルのコンテンツのプロパティが返されます。 項目の添付ファイルは、返されるプロパティは、名前、コンテンツ タイプ、ContentId、ContentLocation、およびすべての接続されているアイテムのプロパティです。 これは、 [GetItem](getitem.md)要求で AllProperties の基本図形を使用するのと同じです。 
  
MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[GetAttachment 操作](getattachment-operation.md)
  
[GetAttachmentResponse](getattachmentresponse.md)

