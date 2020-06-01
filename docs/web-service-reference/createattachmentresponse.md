---
title: CreateAttachmentResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateAttachmentResponse
api_type:
- schema
ms.assetid: cf6bd8bb-5317-4a03-bd75-297dd359b5da
description: CreateAttachmentResponse 要素は、CreateAttachment 要求に対する応答を定義します。
ms.openlocfilehash: df2b0e37adaeaef32f845e5a28615ce874cb3447
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466417"
---
# <a name="createattachmentresponse"></a>CreateAttachmentResponse

**Createattachmentresponse**要素は、createattachment 要求に対する応答を定義します。 
  
```xml
<CreateAttachmentResponse>
   <ResponseMessages/>
</CreateAttachmentResponse>
```

 **CreateAttachmentResponseType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Exchange Web サービス要求に対する応答メッセージを含みます。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空にすることができます。  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[CreateAttachment 操作](createattachment-operation.md)
  
[CreateAttachment](createattachment.md)


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

