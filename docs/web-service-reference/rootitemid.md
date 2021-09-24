---
title: RootItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- RootItemId
api_type:
- schema
ms.assetid: f613c705-17ce-48ce-aa64-4dc2cea25e31
description: RootItemId 要素は、削除された添付ファイルのルート アイテムを識別します。
ms.openlocfilehash: eab3cc30c2e3f2b6cdc443ba8eb7ae4bfa38d257
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59509371"
---
# <a name="rootitemid"></a>RootItemId

**RootItemId 要素は**、削除された添付ファイルのルート アイテムを識別します。 
  
[DeleteAttachmentResponse](deleteattachmentresponse.md)
  
[ResponseMessages](responsemessages.md)
  
[DeleteAttachmentResponseMessage](deleteattachmentresponsemessage.md)
  
[RootItemId](rootitemid.md)
  
```xml
<RootItemId RootItemId="" RootItemChangeKey="" />
```

 **RootItemIdType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**RootItemId** <br/> |削除された添付ファイルのルート アイテムを識別します。  <br/> |
|**RootItemChangeKey** <br/> |削除された添付ファイルのルート アイテムの新しい変更キーを識別します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[DeleteAttachmentResponseMessage](deleteattachmentresponsemessage.md) <br/> |DeleteAttachment 要求の状態と結果を格納します。  <br/> |
   
## <a name="remarks"></a>注釈

**RootItemId 要素** は、DeleteAttachment 応答でのみ使用されます。 これにより、ルート アイテム識別子が識別され、さらに重要なのは、親アイテムへの新しい変更キーです。 
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空の場合  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[DeleteAttachment](deleteattachment.md)
  
[DeleteAttachment 操作](deleteattachment-operation.md)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

