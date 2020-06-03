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
description: DistinguishedFolderId 要素は、名前で参照できるフォルダーを識別します。 この要素を使用しない場合は、フォルダーを識別するために FolderId 要素を使用する必要があります。
ms.openlocfilehash: be883cbca00910b24e4c45ba047803e5a5024566
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462697"
---
# <a name="distinguishedfolderid"></a>DistinguishedFolderId

**DistinguishedFolderId**要素は、名前で参照できるフォルダーを識別します。 この要素を使用しない場合は、フォルダーを識別するために[FolderId](folderid.md)要素を使用する必要があります。 
  
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
|**Id** <br/> |既定のフォルダーを識別する文字列を格納します。 この属性は必須です。  <br/> |
|**ChangeKey** <br/> |**Id**属性によって識別されるフォルダーのバージョンを識別する文字列を格納します。 この属性は省略可能です。 この属性を使用して、適切なバージョンのフォルダーが使用されていることを確認します。  <br/> |
   
#### <a name="id-attribute-values"></a>Id 属性の値

|**値**|**説明**|
|:-----|:-----|
|予定表  <br/> |予定表フォルダーを表します。  <br/> |
|連絡先  <br/> |連絡先フォルダーを表します。  <br/> |
|deleteditems  <br/> |[削除済みアイテム] フォルダーを表します。  <br/> |
|下書き  <br/> |[下書き] フォルダーを表します。  <br/> |
|inbox  <br/> |受信トレイフォルダーを表します。  <br/> |
|雑誌  <br/> |履歴フォルダーを表します。  <br/> |
|notes  <br/> |メモフォルダーを表します。  <br/> |
|送信トレイ  <br/> |[送信トレイ] フォルダーを表します。  <br/> |
|sentitems  <br/> |[送信済みアイテム] フォルダーを表します。  <br/> |
|tasks  <br/> |[タスク] フォルダーを表します。  <br/> |
|msgfolderroot  <br/> |メッセージフォルダーのルートを表します。  <br/> |
|root  <br/> |メールボックスのルートを表します。  <br/> |
|junkemail  <br/> |[迷惑メール] フォルダーを表します。  <br/> |
|searchfolders  <br/> |[検索フォルダー] フォルダーを表します。  <br/> |
|voicemail  <br/> |ボイスメールフォルダーを表します。  <br/> |
|recoverableitemsroot  <br/> |[収集ルート] フォルダーを表します。  <br/> |
|recoverableitemsdeletions  <br/> |削除フォルダーを表します。  <br/> |
|recoverableitemsversions  <br/> |収集されたバージョンのフォルダーを表します。  <br/> |
|recoverableitemspurges  <br/> |[削除] [削除] フォルダーを表します。  <br/> |
|アーカイブ  <br/> |ルートアーカイブフォルダーを表します。  <br/> |
|archivemsgfolderroot  <br/> |ルートアーカイブメッセージフォルダーを表します。  <br/> |
|archivedeleteditems  <br/> |[削除済みアイテムのアーカイブ] フォルダーを表します。  <br/> |
|アーカイブ受信トレイ  <br/> |アーカイブ受信トレイフォルダーを表します。 ビルド番号15.00.0913.09 以降のバージョンの Exchange には、この値が含まれています。  <br/> |
|アーカイブアイテムのルート  <br/> |アーカイブの回復可能なアイテムのルートフォルダーを表します。  <br/> |
|archiverecoverableitemsdeletions  <br/> |[回復可能なアイテムの削除] フォルダーを表します。  <br/> |
|archiverecoverableitemsversions  <br/> |アーカイブの回復可能なアイテムのバージョンフォルダーを表します。  <br/> |
|archiverecoverableitemspurges  <br/> |[回復可能なアイテムの削除] フォルダーを表します。  <br/> |
|syncissues  <br/> |同期の失敗フォルダーを表します。  <br/> |
|競合  <br/> |[競合] フォルダーを表します。  <br/> |
|localfailures  <br/> |[ローカルの失敗] フォルダを表します。  <br/> |
|serverfailures  <br/> |[サーバーエラー] フォルダーを表します。  <br/> |
|受信者キャッシュ  <br/> |受信者のキャッシュフォルダーを表します。  <br/> |
|クイック連絡先  <br/> |[クイック連絡先] フォルダーを表します。  <br/> |
|conversationhistory  <br/> |[会話履歴] フォルダーを表します。  <br/> |
|adminauditlogs  <br/> |管理者監査ログフォルダーを表します。  <br/> |
|todosearch  <br/> |Todo 検索フォルダーを表します。  <br/> |
|mycontacts  <br/> |[個人用連絡先] フォルダーを表します。  <br/> |
|名簿  <br/> |ディレクトリフォルダを表します。  <br/> |
|imcontactlist  <br/> |IM 連絡先リストフォルダーを表します。  <br/> |
|peopleconnect  <br/> |People connect フォルダーを表します。  <br/> |
|使う  <br/> |[お気に入り] フォルダーを表します。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[メールボックス](mailbox.md) <br/> |プライマリ SMTP アドレスを識別します。 プロキシアドレスは使用できません。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ContextFolderId](contextfolderid.md) <br/> |フォルダーを使用する会話アクションを対象とするフォルダーを示します。  <br/> |
|[DestinationFolderId](destinationfolderid.md) <br/> |会話のコピーと移動の操作を行うための宛先フォルダーを示します。  <br/> |
|[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) <br/> | 新しいフォルダーまたはアイテムを作成するフォルダーを指定します。  <br/><br/>この要素の XPath 式は次のとおりです。<br/><br/>  `/CreateItem/ParentFolderId` <br/><br/>`/CreateFolder/ParentFolderId` <br/> |
|[ParentFolderIds](parentfolderids.md) <br/> |[FindItem 操作](finditem-operation.md)と[findfolder 操作](findfolder-operation.md)を検索するフォルダーを識別します。  <br/> |
|[BaseFolderIds](basefolderids.md) <br/> |検索フォルダーの内容を確認するために検索されるフォルダーのコレクションを表します。  <br/> |
|[FolderIds](folderids.md) <br/> |イベント通知のコピー、移動、取得、削除、または監視を行うフォルダーを識別するために使用されるフォルダー識別子の配列を格納します。  <br/> |
|[FolderChange](folderchange.md) <br/> |1つのフォルダーに対して実行される変更のコレクションを表します。  <br/> <br/>この要素の XPath 式を次に示します。<br/><br/>`/UpdateFolder/FolderChanges/FolderChange`<br/> |
|[ToFolderId](tofolderid.md) <br/> | コピーまたは移動されたアイテムまたはフォルダーの移動先フォルダーを表します。<br/><br/>この要素の XPath 式は次のとおりです。<br/><br/>`/MoveFolder/ToFolderId`<br/><br/>`/CopyFolder/ToFolderId`<br/><br/>`/MoveItem/ToFolderId`<br/><br/>`/CopyItem/ToFolderId` <br/> |
|[SavedItemFolderId](saveditemfolderid.md) <br/> | Exchange ストア内のアイテムを更新、送信、および作成する操作のターゲットフォルダーを指定します。<br/><br/>この要素の XPath 式は次のとおりです。<br/><br/>`/CreateItem/SavedItemFolderId`<br/><br/>`/UpdateItem/SavedItemFolderId`<br/><br/>`/SendItem/SavedItemFolderId` <br/> |
|[SyncFolderId](syncfolderid.md) <br/> |同期するアイテムを含むフォルダを表します。  <br/> |
|[UserConfigurationName](userconfigurationname.md) <br/> |ユーザー構成オブジェクトの名前を表します。 ユーザー構成オブジェクトの名前は、ユーザー構成オブジェクトの識別子です。  <br/> |
|[CopyToFolder](copytofolder.md) <br/> |電子メールアイテムがコピーされるフォルダーの ID を表します。  <br/> |
|[MoveToFolder](movetofolder.md) <br/> |電子メールアイテムの移動先となるフォルダーの ID を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

**DistinguishedFolderId**は、 **FolderId**に解決されます。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)
- [フォルダーの作成 (Exchange Web サービス)](https://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

