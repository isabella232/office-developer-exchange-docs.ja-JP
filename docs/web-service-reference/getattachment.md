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
description: GetAttachment 要素は、Exchange ストアから添付ファイルを取得する要求のルート要素です。
ms.openlocfilehash: d03d086ff443db87b0104a2ec83599eb9eaea6b9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463980"
---
# <a name="getattachment"></a>GetAttachment

**Getattachment**要素は、Exchange ストアから添付ファイルを取得する要求のルート要素です。 
  
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
|[AttachmentShape](attachmentshape.md) <br/> |[Getattachment](getattachment.md)要求に対する応答で返される追加の拡張アイテムプロパティを識別します。 この要素は省略できます。  <br/> |
|[AttachmentIds](attachmentids.md) <br/> |添付ファイル識別子の配列を格納します。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>注釈

[Attachmentshape](attachmentshape.md)要素は、応答で返されるプロパティを識別するために必須ではありません。 [Getattachment 操作](getattachment-operation.md)は、Name、ContentType、ContentId、contentlocation、および添付ファイルのコンテンツプロパティを返します。 アイテムの添付ファイルの場合、返されるプロパティは、Name、ContentType、ContentId、ContentLocation、および添付されているすべてのアイテムのプロパティです。 これは、 [GetItem](getitem.md)要求で allproperties 基本図形を使用するのと同じです。 
  
この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[GetAttachment 操作](getattachment-operation.md)
  
[GetAttachmentResponse](getattachmentresponse.md)

