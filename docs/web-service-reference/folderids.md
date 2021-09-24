---
title: FolderIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FolderIds
api_type:
- schema
ms.assetid: 3ff9d15a-7220-4785-ae6b-583a7eb82005
description: FolderIds 要素には、コピー、移動、取得、削除、またはイベント通知を監視するフォルダーを識別するために使用されるフォルダー識別子の配列が含まれています。
ms.openlocfilehash: 7c0cf46d5fdaf35ec72cf3b5750b51edc5a8bfe0
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518366"
---
# <a name="folderids"></a>FolderIds

**FolderIds 要素には**、コピー、移動、取得、削除、またはイベント通知を監視するフォルダーを識別するために使用されるフォルダー識別子の配列が含まれています。 
  
```xml
<FolderIds>
   <FolderId/>
   <DistinguishedFolderId/>
</FolderIds>
```

 **NonEmptyArrayOfBaseFolderIdsType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |フォルダーの識別子と変更キーを格納します。  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |名前でMicrosoft Exchange Serverできるフォルダーを識別します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetFolder](getfolder.md) <br/> |フォルダー ストアからフォルダーを取得する要求Exchangeします。  <br/> 次に、この要素の XPath 式を示します。  `/GetFolder` <br/> |
|[DeleteFolder](deletefolder.md) <br/> |フォルダーストアからフォルダーを削除する要求をExchangeします。  <br/> 次に、この要素の XPath 式を示します。  `/DeleteFolder` <br/> |
|[EmptyFolder](emptyfolder.md) <br/> |フォルダーストアからフォルダーを削除する要求をExchangeします。  <br/> 次に、この要素の XPath 式を示します。  `/EmptyFolder` <br/> |
|[MoveFolder](movefolder.md) <br/> |フォルダーストア内のフォルダーを移動する要求Exchangeします。  <br/> 次に、この要素の XPath 式を示します。  `/MoveFolder` <br/> |
|[CopyFolder](copyfolder.md) <br/> |フォルダー ストア内のフォルダーをコピーする要求をExchangeします。  <br/> 次に、この要素の XPath 式を示します。  `/CopyFolder` <br/> |
|[PushSubscriptionRequest](pushsubscriptionrequest.md) <br/> |プッシュ ベースのイベント通知サブスクリプションのサブスクリプションを表します。  <br/> |
|[PullSubscriptionRequest](pullsubscriptionrequest.md) <br/> |プル ベースのイベント通知サブスクリプションのサブスクリプションを表します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされているコンピューター Microsoft Exchange Server EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages と https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ。型スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd;Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[GetFolder 操作](getfolder-operation.md)
  
[DeleteFolder 操作](deletefolder-operation.md)
  
[MoveFolder 操作](movefolder-operation.md)
  
[CopyFolder 操作](copyfolder-operation.md)
  
[サブスクライブ操作](subscribe-operation.md)

