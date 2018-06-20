---
title: ArchiveTag
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c4cb0718-37cd-41aa-86e7-b492c4bb86aa
description: ArchiveTag 要素は、アイテムまたはフォルダーの [アーカイブのタグの保存期間の識別子を指定します。
ms.openlocfilehash: ae9c7d512981af3bf564bcb73a9a27c5c78217fc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759435"
---
# <a name="archivetag"></a>ArchiveTag

**ArchiveTag**要素は、アイテムまたはフォルダーの [アーカイブのタグの保存期間の識別子を指定します。 
  
```XML
<ArchiveTag IsExplicit=""></ArchiveTag>
```

 **RetentionTagType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**IsExplicit** <br/> |アイテムまたはフォルダーにアイテム保持ポリシーを明示的に設定するかどうか、または親フォルダーから継承されているかどうかを指定します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CalendarFolder](calendarfolder.md) <br/> |主に予定表のアイテムを含むフォルダーを表します。  <br/> |
|[カレンダー項目](calendaritem.md) <br/> |Exchange 予定表アイテムを表します。  <br/> |
|[Contact](contact.md) <br/> |Exchange ストア内の連絡先アイテムを表します。  <br/> |
|[メッセージ](contactsfolder.md) <br/> |メールボックスに格納されている連絡先フォルダーを表します。  <br/> |
|[DistributionList](distributionlist.md) <br/> |配布リストを表します。  <br/> |
|[Folder](folder.md) <br/> |作成、取得、検索、同期、または更新するフォルダーを定義します。  <br/> |
|[アイテム](item.md) <br/> |Exchange ストア内の一般的な項目を表します。  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Microsoft Exchange の電子メール メッセージを表します。  <br/> |
|[PostItem](postitem.md) <br/> |Exchange ストア内の投稿アイテムを表します。  <br/> |
|[SearchFolder](searchfolder.md) <br/> |メールボックスに格納されている検索フォルダーを表します。  <br/> |
|[タスク](task.md) <br/> |Exchange ストア内のタスクを表します。  <br/> |
|[TasksFolder](tasksfolder.md) <br/> |メールボックスに含まれるタスク フォルダーを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

**ArchiveTag**要素のテキスト値は、保持ポリシーを識別する GUID です。 
  
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型のスキーマ  <br/> |
|検証ファイル  <br/> |types.xsd  <br/> |
|空にすることができます。  <br/> ||
   
## <a name="see-also"></a>関連項目

- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

