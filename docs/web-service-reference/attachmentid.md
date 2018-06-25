---
title: AttachmentId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AttachmentId
api_type:
- schema
ms.assetid: 55a5fd77-60d1-40fa-8144-770600cedc6a
description: AttachmentId 要素は、アイテムまたはファイルの添付ファイルを識別します。 CreateAttachment の応答は、この要素を使用します。
ms.openlocfilehash: 2910503d1661ca3aaeeb4e319deb39f6b57c5c0a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759451"
---
# <a name="attachmentid"></a>AttachmentId

**AttachmentId**要素は、アイテムまたはファイルの添付ファイルを識別します。 CreateAttachment の応答は、この要素を使用します。 
  
```xml
<AttachmentId Id="" RootItemId="" RootItemChangeKey="" />
```

 **AttachmentIdType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**Id** <br/> |添付ファイルの一意の識別子を指定します。  <br/> |
|**RootItemId** <br/> |添付ファイルが関連付けられているルート ストア アイテムの一意の識別子を指定します。  <br/> |
|**RootItemChangeKey** <br/> |添付ファイルが関連付けられているルート ストアの項目のキーの変更を識別します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ItemAttachment](itemattachment.md) <br/> |Exchange の他のアイテムに関連付けられている Exchange アイテムを表します。  <br/> |
|[FileAttachment](fileattachment.md) <br/> |Exchange ストア内のアイテムに関連付けられているファイルを表します。  <br/> |
   
## <a name="remarks"></a>備考

添付ファイルが作成されると、ルート アイテムの変更キーが変更されることに注意する必要があります。
  
DeleteAttachment および GetAttachment 要求は、 [AttachmentId](attachmentid-getattachment-and-deleteattachment.md)要素を使用します。 
  
MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空にすることができます。  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

