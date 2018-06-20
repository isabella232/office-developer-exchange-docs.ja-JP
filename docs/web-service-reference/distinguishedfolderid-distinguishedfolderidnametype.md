---
title: DistinguishedFolderId (DistinguishedFolderIdNameType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 915b2ee9-8284-4bf6-8995-1fd0785e9e48
description: DistinguishedFolderId 要素は、名前で参照可能なフォルダーを識別します。
ms.openlocfilehash: 1f5b97fc7ee7b93989762c26e4b979a8dfb884be
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760132"
---
# <a name="distinguishedfolderid-distinguishedfolderidnametype"></a>DistinguishedFolderId (DistinguishedFolderIdNameType)

**DistinguishedFolderId**要素は、名前で参照可能なフォルダーを識別します。 
  
```XML
<DistinguishedFolderId> calendar | contacts | deleteditems | drafts | inbox | journal | notes | outbox | sentitems | tasks | msgfolderroot | publicfoldersroot | root | junkemail | searchfolders | voicemail | recoverableitemsroot | recoverableitemsdeletions | recoverableitemsversions | recoverableitemspurges | archiveroot | archivemsgfolderroot | archivedeleteditems | archiverecoverableitemsroot | archiverecoverableitemsdeletions | archiverecoverableitemsversions | archiverecoverableitemspurges | syncissues | conflicts | localfailures | serverfailures | recipientcache | quickcontacts | conversationhistory | adminauditlogs | todosearch | mycontacts | directory | imcontactlist | peopleconnect</DistinguishedFolderId>
```

 **DistinguishedFolderIdNameType**
## <a name="attributes-and-elements"></a>属性および要素

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
|[メッセージ](contactsfolder.md) <br/> |連絡先フォルダーを指定します。  <br/> |
   
## <a name="text-value"></a>テキスト値

**DistinguishedFolderId 要素のテキスト値**

|**値**|**説明**|
|:-----|:-----|
|予定表  <br/> |予定表フォルダーの URL を示します。  <br/> |
|contacts  <br/> |連絡先フォルダーの URL を示します。  <br/> |
|deleteditems  <br/> |削除済みアイテム フォルダーの URL を示します。  <br/> |
|下書き  <br/> |[下書き] フォルダーの URL を示します。  <br/> |
|[受信トレイ]  <br/> |受信トレイ フォルダーの URL を示します。  <br/> |
|仕訳帳  <br/> |履歴フォルダーの URL を示します。  <br/> |
|notes  <br/> |メモ フォルダーの URL を示します。  <br/> |
|[送信トレイ] します。  <br/> |[送信トレイ] フォルダーの URL を示します。  <br/> |
|送信済みアイテム  <br/> |送信済みアイテム フォルダーの URL を示します。  <br/> |
|tasks  <br/> |[仕事] フォルダーの URL を示します。  <br/> |
|msgfolderroot  <br/> |メッセージのルート フォルダーの URL を示します。  <br/> |
|publicfoldersroot  <br/> |パブリック フォルダーのルート フォルダーの URL を示します。  <br/> |
|root  <br/> |ルート フォルダーの URL を示します。  <br/> |
|junkemail  <br/> |迷惑メール フォルダーの URL を示します。  <br/> |
|使用して  <br/> |検索フォルダーの URL を示します。  <br/> |
|voicemail  <br/> |ボイス メール フォルダーの URL を示します。  <br/> |
|recoverableitemsroot  <br/> |回復可能な項目のルート フォルダーの URL を示します。  <br/> |
|recoverableitemsdeletions  <br/> |回復可能な項目が削除されたフォルダーの URL を示します。  <br/> |
|recoverableitemsversions  <br/> |回復可能な項目のバージョンのフォルダーの URL を示します。  <br/> |
|recoverableitemspurges  <br/> |パージされた回復可能なアイテム] フォルダーの URL を示します。  <br/> |
|archiveroot  <br/> |アーカイブのルート フォルダーの URL を示します。  <br/> |
|archivemsgfolderroot  <br/> |ルート フォルダーには、アーカイブされたメッセージのフォルダーの URL を示します。  <br/> |
|archivedeleteditems  <br/> |アーカイブされた削除済みアイテム フォルダーの URL を示します。  <br/> |
|archiverecoverableitemsroot  <br/> |アーカイブの回復可能な項目のルート フォルダーの URL を示します。  <br/> |
|archiverecoverableitemsdeletions  <br/> |アーカイブの回復可能な削除済みアイテム フォルダーの URL を示します。  <br/> |
|archiverecoverableitemsversions  <br/> |アーカイブの回復可能な項目のバージョンのフォルダーの URL を示します。  <br/> |
|archiverecoverableitemspurges  <br/> |パージされたアーカイブの回復可能なアイテム] フォルダーの URL を示します。  <br/> |
|syncissues  <br/> |同期の失敗フォルダーの URL を示します。  <br/> |
|競合  <br/> |[競合] フォルダーの URL を示します。  <br/> |
|localfailures  <br/> |ローカルの失敗フォルダーの URL を示します。  <br/> |
|serverfailures  <br/> |サーバーの失敗フォルダーの URL を示します。  <br/> |
|recipientcache  <br/> |受信者キャッシュ フォルダーの URL を示します。  <br/> |
|quickcontacts  <br/> |クイック連絡先フォルダーの URL を示します。  <br/> |
|conversationhistory  <br/> |会話履歴フォルダーの URL を示します。  <br/> |
|adminauditlogs  <br/> |管理監査ログのフォルダーの URL を示します。  <br/> |
|todosearch  <br/> |検索タスク フォルダーの URL を示します。  <br/> |
|連絡先  <br/> |URL を示す、[連絡先] フォルダーです。  <br/> |
|ディレクトリ  <br/> |ディレクトリ ・ フォルダーの URL を示します。  <br/> |
   
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型のスキーマ  <br/> |
|検証ファイル  <br/> |types.xsd  <br/> |
|空にすることができます。  <br/> ||
   
## <a name="see-also"></a>関連項目

- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

