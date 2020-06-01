---
title: ArchiveTag
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c4cb0718-37cd-41aa-86e7-b492c4bb86aa
description: アーカイブタグ要素は、アイテムまたはフォルダーに設定されているアーカイブタグセットの保持識別子を指定します。
ms.openlocfilehash: 23167f3c96a6756fe4c6d915a4de91e815e620d9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464764"
---
# <a name="archivetag"></a>ArchiveTag

アーカイブ**タグ要素は、アイテム**またはフォルダーに設定されているアーカイブタグセットの保持識別子を指定します。 
  
```XML
<ArchiveTag IsExplicit=""></ArchiveTag>
```

 **RetentionTagType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**IsExplicit** <br/> |アイテムまたはフォルダーにアイテム保持ポリシーを明示的に設定するかどうか、または親フォルダーから継承するかどうかを指定します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CalendarFolder](calendarfolder.md) <br/> |主に予定表アイテムを含むフォルダーを表します。  <br/> |
|[CalendarItem](calendaritem.md) <br/> |Exchange の予定表アイテムを表します。  <br/> |
|[連絡先](contact.md) <br/> |Exchange ストア内の連絡先アイテムを表します。  <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |メールボックスに含まれている連絡先フォルダーを表します。  <br/> |
|[DistributionList](distributionlist.md) <br/> |配布リストを表します。  <br/> |
|[Folder](folder.md) <br/> |作成、取得、検索、同期、更新を行うフォルダーを定義します。  <br/> |
|[アイテム](item.md) <br/> |Exchange ストア内の汎用アイテムを表します。  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Microsoft Exchange の電子メールメッセージを表します。  <br/> |
|[PostItem](postitem.md) <br/> |Exchange ストア内の投稿アイテムを表します。  <br/> |
|[SearchFolder](searchfolder.md) <br/> |メールボックスに含まれている検索フォルダーを表します。  <br/> |
|[Task](task.md) <br/> |Exchange ストア内のタスクを表します。  <br/> |
|[TasksFolder](tasksfolder.md) <br/> |メールボックスに含まれる tasks フォルダーを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

**アーカイブタグ**要素のテキスト値は、アイテム保持ポリシーを識別する GUID です。 
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> ||
   
## <a name="see-also"></a>関連項目

- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

