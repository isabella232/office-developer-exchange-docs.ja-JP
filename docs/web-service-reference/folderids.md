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
description: FolderIds 要素には、コピー、移動、取得、削除、またはイベント通知を監視するフォルダーを識別するために使用されるフォルダー識別子の配列が含まれています。
ms.openlocfilehash: 911a74ca778ee988c270c16c67620a40656d82d8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760565"
---
# <a name="folderids"></a>FolderIds

**FolderIds**要素には、コピー、移動、取得、削除、またはイベント通知を監視するフォルダーを識別するために使用されるフォルダー識別子の配列が含まれています。 
  
```xml
<FolderIds>
   <FolderId/>
   <DistinguishedFolderId/>
</FolderIds>
```

 **NonEmptyArrayOfBaseFolderIdsType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[フォルダー Id](folderid.md) <br/> |フォルダーの識別子と変更キーが含まれています。  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |名前で参照できる Microsoft Exchange Server のフォルダーを識別します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetFolder](getfolder.md) <br/> |Exchange ストアからフォルダーを取得する要求を定義します。  <br/> この要素への XPath 式は、次のようにします。`/GetFolder` <br/> |
|[DeleteFolder](deletefolder.md) <br/> |Exchange ストアからフォルダーを削除する要求を定義します。  <br/> この要素への XPath 式は、次のようにします。`/DeleteFolder` <br/> |
|[EmptyFolder](emptyfolder.md) <br/> |Exchange ストアからフォルダーを削除する要求を定義します。  <br/> この要素への XPath 式は、次のようにします。`/EmptyFolder` <br/> |
|[MoveFolder](movefolder.md) <br/> |Exchange ストア内のフォルダーを移動する要求を定義します。  <br/> この要素への XPath 式は、次のようにします。`/MoveFolder` <br/> |
|[CopyFolder](copyfolder.md) <br/> |Exchange ストア内のフォルダーをコピーするのには要求を定義します。  <br/> この要素への XPath 式は、次のようにします。`/CopyFolder` <br/> |
|[PushSubscriptionRequest](pushsubscriptionrequest.md) <br/> |プッシュ ベースのイベント通知サブスクリプションをサブスクリプションを表します。  <br/> |
|[PullSubscriptionRequest](pullsubscriptionrequest.md) <br/> |プル ベースのイベント通知サブスクリプションをサブスクリプションを表します。  <br/> |
   
## <a name="remarks"></a>備考

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages と http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |メッセージ スキーマです。タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd です。Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目




  [GetFolder 操作](getfolder-operation.md)
  
[DeleteFolder 操作](deletefolder-operation.md)
  
[MoveFolder 操作](movefolder-operation.md)
  
[CopyFolder 操作](copyfolder-operation.md)
  
[サブスクライブ操作](subscribe-operation.md)

