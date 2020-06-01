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
description: ManagedFolderInformation 要素には、管理されたカスタムフォルダーに関する情報が含まれています。
ms.openlocfilehash: ce15dcb15cccdce253494beefd2f4a2a7a0c0ad8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44450950"
---
# <a name="managedfolderinformation"></a>ManagedFolderInformation

**Managedfolderinformation**要素には、管理されたカスタムフォルダーに関する情報が含まれています。 
  
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
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[CanDelete](candelete.md) <br/> |管理フォルダーを顧客が削除できるかどうかを示します。  <br/> |
|[CanRenameOrMove](canrenameormove.md) <br/> |ユーザーが、特定の管理フォルダーの名前を変更するか、移動できるかどうかを示します。  <br/> |
|[On Displaycomment](mustdisplaycomment.md) <br/> |管理フォルダーのコメントを表示する必要があるかどうかを示します。  <br/> |
|[HasQuota](hasquota.md) <br/> |管理フォルダーにクォータがあるかどうかを示します。  <br/> |
|[Ismanagedフォルダーのルート](ismanagedfoldersroot.md) <br/> |管理フォルダーがすべての管理フォルダーのルートであるかどうかを示します。  <br/> |
|[ManagedFolderId](managedfolderid.md) <br/> |管理フォルダーのフォルダー ID を格納します。  <br/> |
|[Comment](comment.md) <br/> |管理フォルダーに関連付けられているコメントが保存されています。  <br/> |
|[StorageQuota](storagequota.md) <br/> |管理フォルダーの記憶域のクォータを示します。  <br/> |
|[FolderSize](foldersize.md) <br/> |管理フォルダーのすべてのコンテンツの合計サイズを示します。  <br/> |
|[HomePage](homepage.md) <br/> |管理フォルダーの既定のホームページとなる URL を指定します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Folder](folder.md) <br/> |Exchange ストア内のフォルダーを表します。 管理されたカスタムフォルダーは、**管理フォルダー**という名前のフォルダーのサブフォルダーにのみ設定できます。  <br/> |
|[CalendarFolder](calendarfolder.md) <br/> |該当なし。  <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |該当なし。  <br/> |
|[SearchFolder](searchfolder.md) <br/> |該当なし。  <br/> |
|[TasksFolder](tasksfolder.md) <br/> |なし。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[CreateManagedFolder 操作](createmanagedfolder-operation.md)


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)


[管理フォルダーの追加](https://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

