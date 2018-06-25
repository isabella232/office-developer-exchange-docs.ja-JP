---
title: ManagedFolderInformation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ManagedFolderInformation
api_type:
- schema
ms.assetid: dea980eb-8303-47fe-a380-20a8efc9ead6
description: ManagedFolderInformation 要素には、管理されたカスタム フォルダーに関する情報が含まれています。
ms.openlocfilehash: ef46e2e0db440de2a8acae8316ce98d11bd6710e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832341"
---
# <a name="managedfolderinformation"></a>ManagedFolderInformation

**ManagedFolderInformation**要素には、管理されたカスタム フォルダーに関する情報が含まれています。 
  
```xml
<ManagedFolderInformation>
   <CanDelete/>
   <CanRenameOrMove/>
   <MustDisplayComment/>
   <HasQuota/>
   <IsManagedFoldersRoot/>
   <ManagedFolderId/>
   <Comment/>
   <StorageQuota/>
   <FolderSize/>
   <HomePage/>
</ManagedFolderInformation>
```

 **ManagedFolderInformationType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[CanDelete](candelete.md) <br/> |顧客が管理対象のフォルダーを削除できるかどうかを示します。  <br/> |
|[CanRenameOrMove](canrenameormove.md) <br/> |指定された管理フォルダーの名前の変更やお客様が移動するかどうかを示します。  <br/> |
|[MustDisplayComment](mustdisplaycomment.md) <br/> |管理フォルダーのコメントを表示する必要があるかどうかを示します。  <br/> |
|[HasQuota](hasquota.md) <br/> |管理フォルダーがクォータを持つかどうかを示します。  <br/> |
|[IsManagedFoldersRoot](ismanagedfoldersroot.md) <br/> |管理フォルダーがすべての管理フォルダーのルートであるかどうかを示します。  <br/> |
|[ManagedFolderId](managedfolderid.md) <br/> |管理フォルダーのフォルダー ID が含まれています。  <br/> |
|[Comment](comment.md) <br/> |管理フォルダーに関連付けられているコメントが含まれています。  <br/> |
|[StorageQuota](storagequota.md) <br/> |管理フォルダーの記憶域のクォータについて説明します。  <br/> |
|[FolderSize](foldersize.md) <br/> |管理フォルダーのすべての内容の合計サイズを示します。  <br/> |
|[ホームページ](homepage.md) <br/> |管理フォルダーの既定のホーム ページとなる URL を指定します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Folder](folder.md) <br/> |Exchange ストア内のフォルダーを表します。 管理されたカスタム フォルダーは、**管理対象フォルダー**をという名前のフォルダーのサブフォルダーのみできます。  <br/> |
|[CalendarFolder](calendarfolder.md) <br/> |該当なし。  <br/> |
|[メッセージ](contactsfolder.md) <br/> |該当なし。  <br/> |
|[SearchFolder](searchfolder.md) <br/> |該当なし。  <br/> |
|[TasksFolder](tasksfolder.md) <br/> |該当なし。  <br/> |
   
## <a name="remarks"></a>注釈

MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空にすることができます。  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[CreateManagedFolder 操作](createmanagedfolder-operation.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)


[管理フォルダーを追加します。](http://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

