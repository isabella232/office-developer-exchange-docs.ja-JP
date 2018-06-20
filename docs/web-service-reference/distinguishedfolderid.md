---
title: DistinguishedFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DistinguishedFolderId
api_type:
- schema
ms.assetid: 50018162-2941-4227-8a5b-d6b4686bb32f
description: DistinguishedFolderId 要素は、名前で参照可能なフォルダーを識別します。 この要素を使用しない場合は、フォルダーを識別するのにはフォルダー Id 要素を使用する必要があります。
ms.openlocfilehash: 834166be3d882fa8c0533cfcc2999600430b82ce
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760134"
---
# <a name="distinguishedfolderid"></a>DistinguishedFolderId

**DistinguishedFolderId**要素は、名前で参照可能なフォルダーを識別します。 この要素を使用しない場合は、フォルダーを識別するのには[フォルダー Id](folderid.md)要素を使用する必要があります。 
  
```XML
<DistinguishedFolderId Id="" ChangeKey="">
   <Mailbox/>
</DistinguishedFolderId>
```

 **DistinguishedFolderIdType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**Id** <br/> |既定のフォルダーを識別する文字列が含まれています。 この属性は、必要があります。  <br/> |
|**変更キー** <br/> |**Id**属性によって識別されるフォルダーのバージョンを識別する文字列が含まれています。 この属性は、省略可能です。 フォルダーの正しいバージョンを使用するかどうかを確認するには、この属性を使用します。  <br/> |
   
#### <a name="id-attribute-values"></a>Id 属性の値

|**値**|**説明**|
|:-----|:-----|
|予定表  <br/> |予定表フォルダーを表します。  <br/> |
|contacts  <br/> |連絡先フォルダーを表します。  <br/> |
|deleteditems  <br/> |削除済みアイテム フォルダーを表します。  <br/> |
|下書き  <br/> |[下書き] フォルダーを表します。  <br/> |
|[受信トレイ]  <br/> |受信トレイ フォルダーを表します。  <br/> |
|仕訳帳  <br/> |履歴フォルダーを表します。  <br/> |
|notes  <br/> |メモ フォルダーを表します。  <br/> |
|[送信トレイ] します。  <br/> |[送信トレイ] フォルダーを表します。  <br/> |
|送信済みアイテム  <br/> |送信済みアイテム フォルダーを表します。  <br/> |
|tasks  <br/> |タスク フォルダーを表します。  <br/> |
|msgfolderroot  <br/> |メッセージ フォルダーのルートを表します。  <br/> |
|root  <br/> |メールボックスのルートを表します。  <br/> |
|junkemail  <br/> |[迷惑メール フォルダーを表します。  <br/> |
|使用して  <br/> |検索フォルダー] フォルダーを表します。  <br/> |
|voicemail  <br/> |ボイス メール フォルダーを表します。  <br/> |
|recoverableitemsroot  <br/> |表す、ごみ箱をあさるルート フォルダーです。  <br/> |
|recoverableitemsdeletions  <br/> |表します、収集コンポーネント フォルダーを削除します。  <br/> |
|recoverableitemsversions  <br/> |表す、ごみ箱をあさるバージョンのフォルダーです。  <br/> |
|recoverableitemspurges  <br/> |表します、収集コンポーネント フォルダーを削除します。  <br/> |
|archiveroot  <br/> |アーカイブのルート フォルダーを表します。  <br/> |
|archivemsgfolderroot  <br/> |ルートフォルダーのアーカイブ メッセージを表します。  <br/> |
|archivedeleteditems  <br/> |アーカイブの削除済みアイテム フォルダーを表します。  <br/> |
|archiveinbox  <br/> |アーカイブ受信トレイ フォルダーを表します。 Exchange のビルド番号 15.00.0913.09 以降のバージョンには、この値が含まれます。  <br/> |
|archiverecoverableitemsroot  <br/> |アーカイブの回復可能な項目のルート フォルダーを表します。  <br/> |
|archiverecoverableitemsdeletions  <br/> |アーカイブの回復可能なアイテムの削除フォルダーを表します。  <br/> |
|archiverecoverableitemsversions  <br/> |アーカイブの回復可能な項目のバージョンのフォルダーを表します。  <br/> |
|archiverecoverableitemspurges  <br/> |アーカイブの回復可能なアイテムのパージのフォルダーを表します。  <br/> |
|syncissues  <br/> |同期の問題のフォルダーを表します。  <br/> |
|競合  <br/> |[競合] フォルダーを表します。  <br/> |
|localfailures  <br/> |ローカルの失敗フォルダーを表します。  <br/> |
|serverfailures  <br/> |サーバーの失敗フォルダーを表します。  <br/> |
|recipientcache  <br/> |受信者キャッシュ フォルダーを表します。  <br/> |
|quickcontacts  <br/> |クイック連絡先フォルダーを表します。  <br/> |
|conversationhistory  <br/> |会話の履歴フォルダーを表します。  <br/> |
|adminauditlogs  <br/> |管理監査ログのフォルダーを表します。  <br/> |
|todosearch  <br/> |Todo の検索フォルダーを表します。  <br/> |
|連絡先  <br/> |個人用の連絡先フォルダーを表します。  <br/> |
|ディレクトリ  <br/> |ディレクトリ ・ フォルダーを表します。  <br/> |
|imcontactlist  <br/> |IM の連絡先リスト フォルダーを表します。  <br/> |
|peopleconnect  <br/> |フォルダーの接続のユーザーを表します。  <br/> |
|お気に入り  <br/> |[お気に入り] フォルダーを表します。  <br/> |
   
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[メールボックス](mailbox.md) <br/> |プライマリ SMTP アドレスを識別します。 プロキシ アドレスを指定することはできません。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ContextFolderId](contextfolderid.md) <br/> |フォルダーを使用して対話操作を対象としているフォルダーを示します。  <br/> |
|[DestinationFolderId](destinationfolderid.md) <br/> |コピー先のフォルダーを指定し、対話操作を移動します。  <br/> |
|[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) <br/> | 新しいフォルダーまたはアイテムを作成するフォルダーを識別します。  <br/><br/>この要素への XPath 式は、次のように。<br/><br/>  `/CreateItem/ParentFolderId` <br/><br/>`/CreateFolder/ParentFolderId` <br/> |
|[ParentFolderIds](parentfolderids.md) <br/> |[FindItem 操作](finditem-operation.md)および[FindFolder 操作](findfolder-operation.md)を検索するフォルダーを識別します。  <br/> |
|[BaseFolderIds](basefolderids.md) <br/> |検索フォルダーの内容を判断するに検索するフォルダーのコレクションを表します。  <br/> |
|[FolderIds](folderids.md) <br/> |コピー、移動、取得、削除、またはイベント通知を監視するフォルダーを識別するために使用されるフォルダー識別子の配列が含まれています。  <br/> |
|[FolderChange](folderchange.md) <br/> |1 つのフォルダーで実行される変更のコレクションを表します。  <br/> <br/>この要素への XPath 式は、次のようにします。<br/><br/>`/UpdateFolder/FolderChanges/FolderChange`<br/> |
|[ToFolderId](tofolderid.md) <br/> | 先のフォルダーにコピーまたは移動されたアイテムまたはフォルダーを表します。<br/><br/>この要素への XPath 式は、次のように。<br/><br/>`/MoveFolder/ToFolderId`<br/><br/>`/CopyFolder/ToFolderId`<br/><br/>`/MoveItem/ToFolderId`<br/><br/>`/CopyItem/ToFolderId` <br/> |
|[SavedItemFolderId](saveditemfolderid.md) <br/> | 更新、送信、および Exchange ストア内の項目を作成する操作のターゲット フォルダーを識別します。<br/><br/>この要素への XPath 式は、次のように。<br/><br/>`/CreateItem/SavedItemFolderId`<br/><br/>`/UpdateItem/SavedItemFolderId`<br/><br/>`/SendItem/SavedItemFolderId` <br/> |
|[SyncFolderId](syncfolderid.md) <br/> |同期する項目を含むフォルダーを表します。  <br/> |
|[UserConfigurationName](userconfigurationname.md) <br/> |ユーザーの構成オブジェクトの名前を表します。 ユーザーの構成オブジェクトの名前は、ユーザーの構成オブジェクトの識別子です。  <br/> |
|[CopyToFolder](copytofolder.md) <br/> |アイテムをコピー、その電子メール フォルダーの ID を表します。  <br/> |
|[MoveToFolder](movetofolder.md) <br/> |アイテムに移動する電子メールのフォルダーの ID を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>備考

の**DistinguishedFolderId**は、**フォルダー Id**を解決します。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)
- [フォルダー (Exchange Web サービス) を作成します。](http://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

