---
title: FoldersToIgnore
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b5d18516-a617-4daf-8baf-c7ce29c76f6b
description: FoldersToIgnore 要素は、会話内のアイテムを取得するときに無視されるフォルダーのリストを識別します。 無視されたフォルダー内のすべての会話アイテムは、GetConversationItems 応答で返されません。
ms.openlocfilehash: 07813a54a9a3afa3de23ae94f1c9b191d1cb6fac
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44453358"
---
# <a name="folderstoignore"></a>FoldersToIgnore

**Folderstoignore**要素は、会話内のアイテムを取得するときに無視されるフォルダーのリストを識別します。 無視されたフォルダー内のすべての会話アイテムは、 **GetConversationItems**応答で返されません。 
  
```XML
<FoldersToIgnore>
   <FolderId/>
   <DistinguishedFolderId/>
</FoldersToIgnore>
```

 **非 Emptyarrayofbasefolderidstype**
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
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> |false  <br/> |
   

