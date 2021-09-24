---
title: RelativeFolderPath
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 54e3ba52-08a6-4d48-8a44-6fd5fdbffb25
description: RelativeFolderPath 要素には、作成するフォルダー パスの相対フォルダー パスを示すフォルダーの配列が含まれています。
ms.openlocfilehash: f9a1f193678e9dbd7686376c630ab2fbd0eaf1bd
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513459"
---
# <a name="relativefolderpath"></a>RelativeFolderPath

**RelativeFolderPath** 要素には、作成するフォルダー パスの相対フォルダー パスを示すフォルダーの配列が含まれています。 
  
```XML
<RelativeFolderPath>
   <Folder/>
   <CalendarFolder/>
   <ContactsFolder/>
   <SearchFolder/>
   <TasksFolder/>
</RelativeFolderPath>
```

 **NonEmptyArrayOfFoldersType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[フォルダー](folder.md)  | [CalendarFolder](calendarfolder.md)  | [ContactsFolder](contactsfolder.md)  | [SearchFolder](searchfolder.md)  | [TasksFolder](tasksfolder.md)
  
### <a name="parent-elements"></a>親要素

[CreateFolderPath](createfolderpath.md)
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空の場合  <br/> ||
   

