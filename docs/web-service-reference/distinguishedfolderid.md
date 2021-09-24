---
title: DistinguishedFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DistinguishedFolderId
api_type:
- schema
ms.assetid: 50018162-2941-4227-8a5b-d6b4686bb32f
description: DistinguishedFolderId 要素は、名前で参照できるフォルダーを識別します。 この要素を使用しない場合は、FolderId 要素を使用してフォルダーを識別する必要があります。
ms.openlocfilehash: 309db925bb783c435320aeb283915ece39da2271
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521998"
---
# <a name="distinguishedfolderid"></a>DistinguishedFolderId

**DistinguishedFolderId** 要素は、名前で参照できるフォルダーを識別します。 この要素を使用しない場合は [、FolderId](folderid.md) 要素を使用してフォルダーを識別する必要があります。 
  
```XML
<DistinguishedFolderId Id="" ChangeKey="">
   <Mailbox/>
</DistinguishedFolderId>
```

 **DistinguishedFolderIdType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**Id** <br/> |既定のフォルダーを識別する文字列が含まれます。 この属性は必須です。  <br/> |
|**ChangeKey** <br/> |Id 属性によって識別されるフォルダーのバージョンを識別する文字列が **含** まれます。 この属性は省略可能です。 フォルダーの正しいバージョンが使用されていることを確認するには、この属性を使用します。  <br/> |
   
#### <a name="id-attribute-values"></a>Id 属性値

|**値**|**説明**|
|:-----|:-----|
|予定表  <br/> |予定表フォルダーを表します。  <br/> |
|contacts  <br/> |連絡先フォルダーを表します。  <br/> |
|deleteditems  <br/> |[削除済みアイテム] フォルダーを表します。  <br/> |
|下書き  <br/> |下書きフォルダーを表します。  <br/> |
|inbox  <br/> |受信トレイ フォルダーを表します。  <br/> |
|ジャーナル  <br/> |[ジャーナル] フォルダーを表します。  <br/> |
|notes  <br/> |Notes フォルダーを表します。  <br/> |
|送信トレイ  <br/> |送信ボックス フォルダーを表します。  <br/> |
|sentitems  <br/> |[送信されたアイテム] フォルダーを表します。  <br/> |
|tasks  <br/> |タスク フォルダーを表します。  <br/> |
|msgfolderroot  <br/> |メッセージ フォルダーのルートを表します。  <br/> |
|root  <br/> |メールボックスのルートを表します。  <br/> |
|junkemail  <br/> |迷惑メール フォルダーを表します。  <br/> |
|searchfolders  <br/> |検索フォルダー フォルダーを表します。  <br/> |
|voicemail  <br/> |ボイス メール フォルダーを表します。  <br/> |
|recoverableitemsroot  <br/> |ゴミ箱のルート フォルダーを表します。  <br/> |
|recoverableitemsdeletions  <br/> |ゴミ箱の削除フォルダーを表します。  <br/> |
|recoverableitemsversions  <br/> |ゴミ箱のバージョン フォルダーを表します。  <br/> |
|recoverableitemspurges  <br/> |ゴミ箱の削除フォルダーを表します。  <br/> |
|archiveroot  <br/> |ルート アーカイブ フォルダーを表します。  <br/> |
|archivemsgfolderroot  <br/> |ルート アーカイブ メッセージ フォルダーを表します。  <br/> |
|archivedeleteditems  <br/> |アーカイブ削除済みアイテム フォルダーを表します。  <br/> |
|archiveinbox  <br/> |アーカイブ受信トレイ フォルダーを表します。 ビルド番号 15.00.0913.09 から始まるバージョンExchangeには、この値が含まれます。  <br/> |
|archiverecoverableitemsroot  <br/> |アーカイブ回復可能なアイテムのルート フォルダーを表します。  <br/> |
|archiverecoverableitemsdeletions  <br/> |アーカイブ回復可能なアイテムの削除フォルダーを表します。  <br/> |
|archiverecoverableitemsversions  <br/> |アーカイブ回復可能なアイテムのバージョン フォルダーを表します。  <br/> |
|archiverecoverableitemspurges  <br/> |アーカイブ回復可能なアイテムの削除フォルダーを表します。  <br/> |
|syncissues  <br/> |同期の問題フォルダーを表します。  <br/> |
|競合  <br/> |競合フォルダーを表します。  <br/> |
|localfailures  <br/> |ローカルエラー フォルダーを表します。  <br/> |
|serverfailures  <br/> |サーバーのエラー フォルダーを表します。  <br/> |
|recipientcache  <br/> |受信者キャッシュ フォルダーを表します。  <br/> |
|quickcontacts  <br/> |クイック連絡先フォルダーを表します。  <br/> |
|conversationhistory  <br/> |会話履歴フォルダーを表します。  <br/> |
|adminauditlogs  <br/> |管理者監査ログ フォルダーを表します。  <br/> |
|todosearch  <br/> |todo 検索フォルダーを表します。  <br/> |
|mycontacts  <br/> |[連絡先] フォルダーを表します。  <br/> |
|ディレクトリ  <br/> |ディレクトリ フォルダーを表します。  <br/> |
|imcontactlist  <br/> |IM 連絡先リスト フォルダーを表します。  <br/> |
|peopleconnect  <br/> |ユーザー接続フォルダーを表します。  <br/> |
|お気に入り  <br/> |[お気に入り] フォルダーを表します。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[メールボックス](mailbox.md) <br/> |プライマリ SMTP アドレスを識別します。 プロキシ アドレスは使用できません。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ContextFolderId](contextfolderid.md) <br/> |フォルダーを使用する会話アクションの対象となるフォルダーを示します。  <br/> |
|[DestinationFolderId](destinationfolderid.md) <br/> |会話のコピーおよび移動アクションの移動先フォルダーを示します。  <br/> |
|[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) <br/> | 新しいフォルダーまたはアイテムが作成されるフォルダーを識別します。  <br/><br/>この要素の XPath 式を次に示します。<br/><br/>  `/CreateItem/ParentFolderId` <br/><br/>`/CreateFolder/ParentFolderId` <br/> |
|[ParentFolderIds](parentfolderids.md) <br/> |FindItem 操作と [FindFolder 操作](finditem-operation.md) を検索する [フォルダーを識別します](findfolder-operation.md)。  <br/> |
|[BaseFolderIds](basefolderids.md) <br/> |検索フォルダーの内容を決定するために検索されるフォルダーのコレクションを表します。  <br/> |
|[FolderIds](folderids.md) <br/> |イベント通知をコピー、移動、取得、削除、または監視するフォルダーを識別するために使用されるフォルダー識別子の配列が含まれています。  <br/> |
|[FolderChange](folderchange.md) <br/> |1 つのフォルダーに対して実行する変更のコレクションを表します。  <br/> <br/>次に、この要素の XPath 式を示します。<br/><br/>`/UpdateFolder/FolderChanges/FolderChange`<br/> |
|[ToFolderId](tofolderid.md) <br/> | コピーまたは移動したアイテムまたはフォルダーの移動先フォルダーを表します。<br/><br/>この要素の XPath 式を次に示します。<br/><br/>`/MoveFolder/ToFolderId`<br/><br/>`/CopyFolder/ToFolderId`<br/><br/>`/MoveItem/ToFolderId`<br/><br/>`/CopyItem/ToFolderId` <br/> |
|[SavedItemFolderId](saveditemfolderid.md) <br/> | アイテムを更新、送信、および作成する操作のターゲット フォルダーを、Exchangeします。<br/><br/>この要素の XPath 式を次に示します。<br/><br/>`/CreateItem/SavedItemFolderId`<br/><br/>`/UpdateItem/SavedItemFolderId`<br/><br/>`/SendItem/SavedItemFolderId` <br/> |
|[SyncFolderId](syncfolderid.md) <br/> |同期するアイテムを含むフォルダーを表します。  <br/> |
|[UserConfigurationName](userconfigurationname.md) <br/> |ユーザー構成オブジェクトの名前を表します。 ユーザー構成オブジェクト名は、ユーザー構成オブジェクトの識別子です。  <br/> |
|[CopyToFolder](copytofolder.md) <br/> |電子メール アイテムをコピーするフォルダーの ID を表します。  <br/> |
|[MoveToFolder](movetofolder.md) <br/> |メール アイテムを移動するフォルダーの ID を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

**DistinguishedFolderId は** **FolderId に解決されます**。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)
- [フォルダーの作成 (Exchange Web サービス)](https://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

