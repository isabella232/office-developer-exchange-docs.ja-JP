---
title: RootItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RootItemId
api_type:
- schema
ms.assetid: f613c705-17ce-48ce-aa64-4dc2cea25e31
description: RootItemId 要素は、削除された添付ファイルのルート アイテムを識別します。
ms.openlocfilehash: 484b185db63c9692eaca7e43c49d6e95375a1a98
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833251"
---
# <a name="rootitemid"></a>RootItemId

**RootItemId**要素は、削除された添付ファイルのルート アイテムを識別します。 
  
[DeleteAttachmentResponse](deleteattachmentresponse.md)
  
[ResponseMessages](responsemessages.md)
  
[DeleteAttachmentResponseMessage](deleteattachmentresponsemessage.md)
  
[RootItemId](rootitemid.md)
  
```xml
<RootItemId RootItemId="" RootItemChangeKey="" />
```

 **RootItemIdType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**RootItemId** <br/> |削除された添付ファイルのルート アイテムを識別します。  <br/> |
|**RootItemChangeKey** <br/> |削除された添付ファイルのルート アイテムの新しいキーの変更を識別します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[DeleteAttachmentResponseMessage](deleteattachmentresponsemessage.md) <br/> |DeleteAttachment 要求の結果ステータスを格納します。  <br/> |
   
## <a name="remarks"></a>備考

**RootItemId**要素は、DeleteAttachment 応答にのみ使用されます。 ルート項目 id、およびより重要なは、親アイテムに新しいキーの変更を識別します。 
  
MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空にすることができます。  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[DeleteAttachment](deleteattachment.md)
  
[DeleteAttachment 操作](deleteattachment-operation.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

