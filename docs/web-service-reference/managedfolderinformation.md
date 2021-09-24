---
title: ManagedFolderInformation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ManagedFolderInformation
api_type:
- schema
ms.assetid: dea980eb-8303-47fe-a380-20a8efc9ead6
description: ManagedFolderInformation 要素には、管理されたカスタム フォルダーに関する情報が含まれている。
ms.openlocfilehash: f25daeff82b4a30574a627f290c2fcd336a38a6c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59524799"
---
# <a name="managedfolderinformation"></a>ManagedFolderInformation

**ManagedFolderInformation 要素には**、管理されたカスタム フォルダーに関する情報が含まれている。 
  
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
|[CanRenameOrMove](canrenameormove.md) <br/> |特定の管理フォルダーの名前を変更するか、顧客が移動できるかどうかを示します。  <br/> |
|[MustDisplayComment](mustdisplaycomment.md) <br/> |管理フォルダーのコメントを表示する必要があるかどうかを示します。  <br/> |
|[HasQuota](hasquota.md) <br/> |管理フォルダーにクォータが設定されているかどうかを示します。  <br/> |
|[IsManagedFoldersRoot](ismanagedfoldersroot.md) <br/> |管理フォルダーがすべての管理フォルダーのルートであるかどうかを示します。  <br/> |
|[ManagedFolderId](managedfolderid.md) <br/> |管理フォルダーのフォルダー ID を格納します。  <br/> |
|[コメント](comment.md) <br/> |管理フォルダーに関連付けられているコメントが含まれる。  <br/> |
|[StorageQuota](storagequota.md) <br/> |管理フォルダーの記憶域クォータについて説明します。  <br/> |
|[FolderSize](foldersize.md) <br/> |管理フォルダーのすべてのコンテンツの合計サイズを示します。  <br/> |
|[HomePage](homepage.md) <br/> |管理フォルダーの既定のホーム ページになる URL を指定します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Folder](folder.md) <br/> |フォルダー ストア内のフォルダー Exchangeします。 管理されたカスタム フォルダーには、管理フォルダーという名前のフォルダー **のサブフォルダーのみを指定できます**。  <br/> |
|[CalendarFolder](calendarfolder.md) <br/> |なし。  <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |なし。  <br/> |
|[SearchFolder](searchfolder.md) <br/> |なし。  <br/> |
|[TasksFolder](tasksfolder.md) <br/> |なし。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空の場合  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[CreateManagedFolder 操作](createmanagedfolder-operation.md)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)


[管理フォルダーの追加](https://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

