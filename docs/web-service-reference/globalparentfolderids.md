---
title: GlobalParentFolderIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 8f5fcbcb-05ed-462a-99cf-a6b112a4aef6
description: GlobalParentFolderIds 要素は、グローバル親フォルダーの識別子を指定します。
ms.openlocfilehash: 7ab3d1ba627c5568b2c1f4579689c43c96624558
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516826"
---
# <a name="globalparentfolderids"></a>GlobalParentFolderIds

**GlobalParentFolderIds 要素は**、グローバル親フォルダーの識別子を指定します。 
  
```XML
<GlobalParentFolderIds>
    <FolderId/>
    <DistinguishedFolderId/>
</GlobalParentFolderIds>
```

 **NonEmptyArrayOfBaseFolderIdsType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |フォルダーの識別子と変更キーを格納します。  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |名前で参照できるフォルダーを識別します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Conversation (ConversationType)](conversation-conversationtype.md) <br/> |1 つの会話を表します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |types.xsd  <br/> |
|空にできる  <br/> ||
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

