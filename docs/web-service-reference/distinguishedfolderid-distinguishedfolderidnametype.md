---
title: DistinguishedFolderId (DistinguishedFolderIdNameType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 915b2ee9-8284-4bf6-8995-1fd0785e9e48
description: DistinguishedFolderId 要素は、名前で参照できるフォルダーを識別します。
ms.openlocfilehash: 23d1dead5a97fe8b2ceb29235f4b784f667d2ee1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59526441"
---
# <a name="distinguishedfolderid-distinguishedfolderidnametype"></a>DistinguishedFolderId (DistinguishedFolderIdNameType)

**DistinguishedFolderId** 要素は、名前で参照できるフォルダーを識別します。 
  
```XML
<DistinguishedFolderId> calendar | contacts | deleteditems | drafts | inbox | journal | notes | outbox | sentitems | tasks | msgfolderroot | publicfoldersroot | root | junkemail | searchfolders | voicemail | recoverableitemsroot | recoverableitemsdeletions | recoverableitemsversions | recoverableitemspurges | archiveroot | archivemsgfolderroot | archivedeleteditems | archiverecoverableitemsroot | archiverecoverableitemsdeletions | archiverecoverableitemsversions | archiverecoverableitemspurges | syncissues | conflicts | localfailures | serverfailures | recipientcache | quickcontacts | conversationhistory | adminauditlogs | todosearch | mycontacts | directory | imcontactlist | peopleconnect</DistinguishedFolderId>
```

 **DistinguishedFolderIdNameType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Folder](folder.md) <br/> |汎用フォルダーを指定します。  <br/> |
|[CalendarFolder](calendarfolder.md) <br/> |予定表フォルダーを指定します。  <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |連絡先フォルダーを指定します。  <br/> |
   
## <a name="text-value"></a>テキスト値

**DistinguishedFolderId 要素のテキスト値**

|**値**|**説明**|
|:-----|:-----|
|予定表  <br/> |予定表フォルダーの URL を示します。  <br/> |
|contacts  <br/> |連絡先フォルダーの URL を示します。  <br/> |
|deleteditems  <br/> |削除済みアイテム フォルダーの URL を示します。  <br/> |
|下書き  <br/> |下書きフォルダーの URL を示します。  <br/> |
|inbox  <br/> |受信トレイ フォルダーの URL を示します。  <br/> |
|ジャーナル  <br/> |ジャーナル フォルダーの URL を示します。  <br/> |
|notes  <br/> |メモ フォルダーの URL を示します。  <br/> |
|送信トレイ  <br/> |送信ボックス フォルダーの URL を示します。  <br/> |
|sentitems  <br/> |送信されたアイテム フォルダーの URL を示します。  <br/> |
|tasks  <br/> |タスク フォルダーの URL を示します。  <br/> |
|msgfolderroot  <br/> |メッセージ ルート フォルダーの URL を示します。  <br/> |
|publicfoldersroot  <br/> |パブリック フォルダーのルート フォルダーの URL を示します。  <br/> |
|root  <br/> |ルート フォルダーの URL を示します。  <br/> |
|junkemail  <br/> |迷惑メール フォルダーの URL を示します。  <br/> |
|searchfolders  <br/> |検索フォルダーの URL を示します。  <br/> |
|voicemail  <br/> |ボイス メール フォルダーの URL を示します。  <br/> |
|recoverableitemsroot  <br/> |回復可能なアイテムのルート フォルダーの URL を示します。  <br/> |
|recoverableitemsdeletions  <br/> |削除された回復可能なアイテム フォルダーの URL を示します。  <br/> |
|recoverableitemsversions  <br/> |回復可能なアイテムのバージョン フォルダーの URL を示します。  <br/> |
|recoverableitemspurges  <br/> |削除された回復可能なアイテム フォルダーの URL を示します。  <br/> |
|archiveroot  <br/> |アーカイブ ルート フォルダーの URL を示します。  <br/> |
|archivemsgfolderroot  <br/> |アーカイブされたメッセージ フォルダーのルート フォルダーの URL を示します。  <br/> |
|archivedeleteditems  <br/> |アーカイブされた削除済みアイテム フォルダーの URL を示します。  <br/> |
|archiverecoverableitemsroot  <br/> |アーカイブされた回復可能なアイテムのルート フォルダーの URL を示します。  <br/> |
|archiverecoverableitemsdeletions  <br/> |アーカイブされた回復可能な削除済みアイテム フォルダーの URL を示します。  <br/> |
|archiverecoverableitemsversions  <br/> |アーカイブされた回復可能なアイテムのバージョン フォルダーの URL を示します。  <br/> |
|archiverecoverableitemspurges  <br/> |アーカイブされた削除済み回復可能なアイテム フォルダーの URL を示します。  <br/> |
|syncissues  <br/> |同期の問題フォルダーの URL を示します。  <br/> |
|競合  <br/> |競合フォルダーの URL を示します。  <br/> |
|localfailures  <br/> |ローカルエラー フォルダーの URL を示します。  <br/> |
|serverfailures  <br/> |サーバー障害フォルダーの URL を示します。  <br/> |
|recipientcache  <br/> |受信者キャッシュ フォルダーの URL を示します。  <br/> |
|quickcontacts  <br/> |クイック連絡先フォルダーの URL を示します。  <br/> |
|conversationhistory  <br/> |会話履歴フォルダーの URL を示します。  <br/> |
|adminauditlogs  <br/> |管理監査ログ フォルダーの URL を示します。  <br/> |
|todosearch  <br/> |検索先フォルダーの URL を示します。  <br/> |
|mycontacts  <br/> |連絡先フォルダーの URL を示します。  <br/> |
|ディレクトリ  <br/> |ディレクトリ フォルダーの URL を示します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |types.xsd  <br/> |
|空にできる  <br/> ||
   
## <a name="see-also"></a>関連項目

- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

