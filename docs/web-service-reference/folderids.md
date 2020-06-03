---
title: FolderIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FolderIds
api_type:
- schema
ms.assetid: 3ff9d15a-7220-4785-ae6b-583a7eb82005
description: FolderIds 要素には、イベント通知のコピー、移動、取得、削除、または監視を行うフォルダーを識別するために使用されるフォルダー識別子の配列が含まれています。
ms.openlocfilehash: ff0476f72c7da088bd2b39f58ab560dcc82197e4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530994"
---
# <a name="folderids"></a>FolderIds

**FolderIds**要素には、イベント通知のコピー、移動、取得、削除、または監視を行うフォルダーを識別するために使用されるフォルダー識別子の配列が含まれています。 
  
```xml
<FolderIds>
   <FolderId/>
   <DistinguishedFolderId/>
</FolderIds>
```

 **非 Emptyarrayofbasefolderidstype**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |フォルダーの識別子と変更キーが含まれています。  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |名前で参照できる Microsoft Exchange Server フォルダーを識別します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetFolder](getfolder.md) <br/> |Exchange ストアからフォルダーを取得するための要求を定義します。  <br/> この要素の XPath 式を次に示します。`/GetFolder` <br/> |
|[DeleteFolder](deletefolder.md) <br/> |Exchange ストアからフォルダーを削除するための要求を定義します。  <br/> この要素の XPath 式を次に示します。`/DeleteFolder` <br/> |
|[EmptyFolder](emptyfolder.md) <br/> |Exchange ストアからフォルダーを削除するための要求を定義します。  <br/> この要素の XPath 式を次に示します。`/EmptyFolder` <br/> |
|[MoveFolder](movefolder.md) <br/> |Exchange ストア内のフォルダーを移動する要求を定義します。  <br/> この要素の XPath 式を次に示します。`/MoveFolder` <br/> |
|[CopyFolder](copyfolder.md) <br/> |Exchange ストア内のフォルダーをコピーするための要求を定義します。  <br/> この要素の XPath 式を次に示します。`/CopyFolder` <br/> |
|[PushSubscriptionRequest](pushsubscriptionrequest.md) <br/> |プッシュベースのイベント通知サブスクリプションのサブスクリプションを表します。  <br/> |
|[PullSubscriptionRequest](pullsubscriptionrequest.md) <br/> |プルベースのイベント通知サブスクリプションに対するサブスクリプションを表します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages と https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |メッセージスキーマ。Types スキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd。型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[GetFolder 操作](getfolder-operation.md)
  
[DeleteFolder 操作](deletefolder-operation.md)
  
[MoveFolder 操作](movefolder-operation.md)
  
[CopyFolder 操作](copyfolder-operation.md)
  
[サブスクライブ操作](subscribe-operation.md)

