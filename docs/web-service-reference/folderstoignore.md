---
title: FoldersToIgnore
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: b5d18516-a617-4daf-8baf-c7ce29c76f6b
description: FoldersToIgnore 要素は、スレッド内のアイテムを取得するときに無視されるフォルダーの一覧を識別します。 無視されたフォルダー内のすべての会話アイテムは、GetConversationItems 応答では返されません。
ms.openlocfilehash: c0102d12b24df2cadd5e307e80c5acda9a3c0589
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59528661"
---
# <a name="folderstoignore"></a>FoldersToIgnore

**FoldersToIgnore** 要素は、スレッド内のアイテムを取得するときに無視されるフォルダーの一覧を識別します。 無視されたフォルダー内のすべての会話アイテムは **、GetConversationItems 応答では返** されません。 
  
```XML
<FoldersToIgnore>
   <FolderId/>
   <DistinguishedFolderId/>
</FoldersToIgnore>
```

 **NonEmptyArrayOfBaseFolderIdsType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[FolderId](folderid.md)  | [DistinguishedFolderId](distinguishedfolderid.md)
  
### <a name="parent-elements"></a>親要素

[GetConversationItems](getconversationitems.md)
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空の場合  <br/> |false  <br/> |
   

