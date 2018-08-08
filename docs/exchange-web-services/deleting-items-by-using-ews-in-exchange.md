---
title: Exchange で EWS を使用してアイテムを削除する
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: c81e3160-e12b-47e0-b3d6-4be28537f301
description: Exchange で EWS マネージ API または EWS を使用して、アイテムを削除済みアイテム フォルダーまたはごみ箱に移動して削除する方法について説明します。
ms.openlocfilehash: a475ebc6677e5f5003cc790a2d4d2b83c513f309
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758904"
---
# <a name="deleting-items-by-using-ews-in-exchange"></a>Exchange で EWS を使用してアイテムを削除する

Exchange で EWS マネージ API または EWS を使用して、アイテムを削除済みアイテム フォルダーまたはごみ箱に移動して削除する方法について説明します。
  
アイテムを削除済みアイテム フォルダーに移動することと、ごみ箱に移動することにどんな違いがあるか考えたことがおありですか。 削除されたアイテムを処理する別のオプションや、アプリケーションでそれらのオプションを実装する方法について興味を持たれるかもしれません。 Exchange Web サービス (EWS) には、削除されたアイテムを処理する 3 つのオプションが含まれています。 この記事を読むことによって、それらの違いについての混乱をすべて解決できることでしょう。
  
## <a name="deleting-items---what-are-my-options"></a>アイテムを削除する場合のオプション
<a name="bk_DeletingItemsOptions"> </a>

アイテムを削除する際の全体的な概要を理解する前に、次の違いを認識することが重要です。
  
- 削除済みアイテム フォルダー - メールボックスでアイテムを削除すると、アイテムはここに移動されます。
    
- ごみ箱 (回復可能なアイテム フォルダー) - メールボックスからアイテムを削除すると、アイテムはここに移動されます。
    
図 1 と図 2 は、メールボックスのアイテムとフォルダーの削除処理がどのようなものかを示しています。 

**図 1. メールボックスからアイテムを削除する際のプロセス**

![削除されたアイテムの移動先を示す図。 削除されたアイテムは [削除済みアイテム] フォルダーに移動された後、アイテム保持ポリシーに従って [回復可能なアイテム] フォルダーに移動され、期限切れになった時点で完全に削除されます。](media/Ex_DeleteItems_Source.png)

<br/>

**図 2. メールボックスからフォルダーを削除する際のプロセス**

![削除されたフォルダーが [削除済みアイテム] フォルダーに移動された後、メールボックスから完全に削除される仕組みを示す図。](media/Ex_.png)
   
削除の「永続性」に応じて、アイテムとフォルダーは 3 つの方法で削除できます。
  
**表 1. EWS を使用してアイテムを削除する場合のオプション**

|**オプション**|**結果**|
|:-----|:-----|
|削除済みアイテム フォルダーに移動する  <br/> |これは、アイテムを削除する方法のなかで最も永続性が低いものです。<br/><br/>これは、自分の席の横にあるごみ箱に紙を捨てることに似ています。 必要であれば、もう一度簡単に取り出すことができます。<br/><br/>この操作を実行するには、削除済みアイテム フォルダーに移動するオプションを実装する任意の[削除操作](deleting-items-by-using-ews-in-exchange.md#bk_howdoIdeleteitems)を使用できます。<br/><br/>また、[MoveItem 操作](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) ([Item.Move()](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.item.move%28v=exchg.80%29.aspx)) または [MoveFolder 操作](http://msdn.microsoft.com/library/c7233966-6c87-4a14-8156-b1610760176d%28Office.15%29.aspx) ([Folder.Move()](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.move%28v=exchg.80%29.aspx)) を使用して、アイテムまたはフォルダーを削除済みアイテム フォルダーに移動することもできます。  <br/> |
|論理的な削除  <br/> |アイテムはごみ箱の削除フォルダーに移動されます。<br/><br/>これは、ごみ箱の中身を収集用のコンテナーに移して空にするのと同様です。 必要であれば、少し面倒ではありますが、そのアイテムにアクセスすることはまだ可能です。  <br/><br/>ごみ箱 (回復可能なアイテム フォルダーとも呼ばれる) および電子情報開示や訴訟ホールドなどのシナリオの詳細については、TechNet の「[回復可能なアイテム フォルダー](http://technet.microsoft.com/ja-JP/library/ee364755%28v=exchg.150%29.aspx)」を参照してください。<br/><br/>Exchange 2007 を対象とするアプリケーションの場合、論理的な削除はお勧めしません。 Exchange 2007 で論理的な削除を処理するには、アイテムで、そのアイテムが不特定の時間にごみ箱に移動されることを示すビットを設定します。<br/><br/>論理的な削除の走査、つまり [FindItem Operation](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) によって削除済みアイテム フォルダーに移動されたアイテムの検索は、Exchange Online、Office 365 の一部としての Exchange Online、Exchange 2010 以降のバージョンの Exchange ではサポートされていません。  <br/><br/>**注**: フォルダーを削除済みアイテム フォルダーへ移動することはできません。           |
|物理的な削除  <br/> |アイテムまたはフォルダーが完全に削除されます。<br/><br/>物理的に削除されたアイテムはごみ箱の Purges フォルダーに配置されます。 これは、ごみ収集車が収集用のコンテナーを空にするのと同じです。 Outlook または Outlook Web App のような電子メール クライアントからはこれらのアイテムにアクセスできず、メールボックスに保持設定がない限り、アイテムは一定期間後に完全に削除されます。<br/><br/>アイテムの保存期間については、TechNet の「[削除済みアイテムの保存期間と回復可能なアイテムのクォータを構成する](http://technet.microsoft.com/ja-JP/library/ee364752%28v=exchg.150%29.aspx)」の記事を参照してください。<br/><br/>**注**: フォルダーを物理的に削除する場合、そのフォルダーは Purges フォルダーには配置されません。 物理的に削除されたフォルダーは、メールボックスから削除されます。  |
   
削除済みアイテム フォルダーへの移動および物理的な削除のオプションはトランザクションです。これは、Web サービス呼び出しが完了するまでに、アイテムが削除済みアイテム フォルダーまたはごみ箱に移動されていることを意味します。
  
削除済みアイテムの格納に使用されるフォルダーのエコシステムについて理解するために、次の図は、削除済みアイテムを含めることができるフォルダーの階層を示しています。 フォルダー名は、**DistinguishedFolderIdNameType** スキーマの種類、または EWS マネージ API の **WellKnownFolderName** 列挙体の場合と同じように表示されています。 
  
**図 3. 削除済みアイテムを格納するフォルダーの階層**

![図は、削除されたアイテムをプライマリ メールボックスとアーカイブ メールボックスの両方に含めることのできるフォルダーのフォルダー階層を示しています。図では、各フォルダーは個別のフォルダー名で示されています。](media/Ex_FolderHierarchyDeletedItems.png)
  
**表 2. 削除済みアイテムを格納するフォルダー **

|**フォルダー名**|**導入バージョン**|**説明**|
|:-----|:-----|:-----|
|deleteditems  <br/> |Exchange 2007  <br/> |既定の削除済みアイテム フォルダー。アイテムは、論理的な削除によって削除されるか、物理的に削除されるまで、または保存期間が超えるまでこのフォルダーに残ります。次に、このアイテムはごみ箱内のフォルダーに移動されます。削除済みフォルダーは、削除済みアイテム フォルダーに配置されており、論理的な削除によって削除されるか、物理的に削除されるときに、メールボックスから完全に削除され、回復できなくなります。  <br/> |
|recoverableitemsroot  <br/> |Exchange 2010  <br/> |ごみ箱、つまり回復可能なアイテム フォルダーのルート。 Exchange 2010 の EWS では、ごみ箱へのアクセスが実装されています。 このフォルダーの表示名は、「回復可能なアイテム」です。  <br/> |
|recoverableitemsdeletions  <br/> |Exchange 2010  <br/> |メールボックスのメインごみ箱フォルダー。 アイテム保持ポリシーによって、論理的な削除によって削除されたアイテムおよび削除済みアイテム フォルダーから移動されたアイテムは、このフォルダーに配置されます。 このフォルダーの表示名は、「削除」です。  <br/> |
|recoverableitemsversions  <br/> |Exchange 2010  <br/> |以前のバージョンのアイテムが格納されます。 以前のバージョンのアイテムは、アイテムが更新されたときに作成されます。 下書きバージョンのアイテムはこのフォルダーに保存されません。 このフォルダーの表示名は、「バージョン」です。  <br/> |
|recoverableitemspurges  <br/> |Exchange 2010  <br/> |削除フォルダーから削除されるアイテムが格納されます。 記憶域で物理的に削除されたすべてのアイテムは、このフォルダーに移動されます。 このフォルダーの表示名は、「Purges」です。  <br/> |
|archiveddeletedtitems  <br/> |Exchange 2010  <br/> |アーカイブ メールボックスの既定の削除済みアイテム フォルダー。  <br/> |
|archiverecoverablesitemsroot  <br/> |Exchange 2010  <br/> |アーカイブ メールボックスのルートごみ箱フォルダー。論理的な削除によって削除されたアーカイブ アイテムは、このフォルダーのサブフォルダーに移動されます。  <br/> |
|archiverecoverableitemsdeletions  <br/> |Exchange 2010  <br/> |アーカイブ メールボックスのメインごみ箱フォルダー。ごみ箱に移動されたアーカイブ アイテムはここに配置されます。  <br/> |
|archiverecoverableitemsversions  <br/> |Exchange 2010  <br/> |以前のバージョンのアーカイブ アイテムが格納されます。  <br/> |
|archiverecoverableitemspurges  <br/> |Exchange 2010  <br/> |ごみ箱のアーカイブ削除フォルダーにある物理的に削除されたアイテムが格納されます。記憶域で物理的に削除されたすべてのアーカイブ アイテムは、このフォルダーに移動されます。  <br/> |
   
## <a name="how-do-i-delete-items"></a>アイテムを削除する方法
<a name="bk_howdoIdeleteitems"> </a>

次のいずれかを使用して、削除済みアイテム フォルダーにアイテムを移動するか、論理的な削除または物理的な削除を実行するかどうかを指定します。
  
- **DisposalType** の単純型 (EWS を使用して Exchange にアクセスする場合)。 
    
- [DeleteMode 列挙型](http://msdn.microsoft.com/ja-JP/library/exchange/microsoft.exchange.webservices.data.deletemode%28v=exchg.80%29.aspx) (EWS マネージ API を使用する場合)。
    
複数の異なる EWS 操作または EWS マネージ API メソッドを使用して、メールボックスからアイテムやフォルダーを削除できます。
  
**表 3. アイテムを削除するための EWS 操作と EWS マネージ API メソッド**

|**EWS 操作**|**EWS マネージ API メソッド**|**導入バージョン**|**機能**|
|:-----|:-----|:-----|:-----|
|[DeleteFolder 操作](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |[Folder.Delete メソッド](http://msdn.microsoft.com/ja-JP/library/exchange/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) <br/> |Exchange 2007  <br/> |メールボックスからフォルダーを削除します。EWS では、フォルダーをバッチ削除できます。EWS マネージ API では、呼び出しごとに 1 つのフォルダーのみを削除できます。  <br/> |
|[DeleteItem 操作](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |[Item.Delete メソッド](http://msdn.microsoft.com/ja-JP/library/exchange/microsoft.exchange.webservices.data.item.delete%28v=exchg.80%29.aspx)<br/><br/>[ExchangeService.DeleteItems メソッド](http://msdn.microsoft.com/ja-JP/library/exchange/microsoft.exchange.webservices.data.exchangeservice.deleteitems%28v=exchg.80%29.aspx) <br/> |Exchange 2007  <br/> |メールボックスからアイテムを削除します。  <br/> |
|[EmptyFolder 操作](http://msdn.microsoft.com/library/98161486-e2f2-480f-8d5d-708ba81b208a%28Office.15%29.aspx) <br/> |[Folder.Empty メソッド](http://msdn.microsoft.com/ja-JP/library/exchange/microsoft.exchange.webservices.data.folder.empty%28v=exchg.80%29.aspx) <br/> |Exchange 2010  <br/> |フォルダー内のすべての項目を削除します。必要に応じて、フォルダー内のすべてのサブフォルダーも削除します。  <br/> |
|[ApplyConversationAction 操作](http://msdn.microsoft.com/library/73d7943d-d361-4f8b-9948-d85f886efa1a%28Office.15%29.aspx) <br/> |[Conversation.EnableAlwaysDeleteItems メソッド](http://msdn.microsoft.com/ja-JP/library/exchange/microsoft.exchange.webservices.data.conversation.enablealwaysdeleteitems%28v=exchg.80%29.aspx)<br/><br/>[Conversation.DeleteItems メソッド](http://msdn.microsoft.com/ja-JP/library/exchange/microsoft.exchange.webservices.data.conversation.deleteitems%28v=exchg.80%29.aspx) <br/> |Exchange 2010  <br/> |会話の電子メール メッセージに対して削除処理アクションを設定し、それらが削除されるようにします。  <br/> |
|[DeleteUserConfiguration 操作](http://msdn.microsoft.com/library/93e44690-be2d-4fdb-96a8-4ded3c193aed%28Office.15%29.aspx) <br/> |[UserConfiguration.Delete メソッド](http://msdn.microsoft.com/ja-JP/library/exchange/microsoft.exchange.webservices.data.userconfiguration.delete%28v=exchg.80%29.aspx) <br/> |Exchange 2010  <br/> |アイテムに関連付けられているフォルダーを削除し、ごみ箱に移動します。  <br/> |
|[CreateItem 操作](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/> |[Appointment.Accept メソッド](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.accept%28v=exchg.80%29.aspx) <br/><br/>[Appointment.AcceptTentatively メソッド](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.accepttentatively%28v=exchg.80%29.aspx)<br/><br/>[Appointment.CancelMeeting メソッド](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.cancelmeeting%28v=exchg.80%29.aspx)<br/><br/>[Appointment.Decline](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.decline%28v=exchg.80%29.aspx)<br/><br/>[MeetingRequest.Accept メソッド](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.meetingrequest.accept%28v=exchg.80%29.aspx)<br/><br/>[MeetingRequest.AcceptTentatively メソッド](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.meetingrequest.accepttentatively%28v=exchg.80%29.aspx)<br/><br/>[MeetingRequest.Decline メソッド](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.meetingrequest.decline%28v=exchg.80%29.aspx) <br/> |Exchange 2007  <br/> |会議出席依頼への応答が送信されるか、応答が予定に設定されるたびに、アイテムを削除済みアイテム フォルダーに間接的に移動します。<br/><br/>削除の種類は、この操作では設定されません。 応答オブジェクトがサービスによって正常に処理されると、会議のメッセージは削除済みアイテム フォルダーに移動されます。  <br/> |
   
受信トレイ ルールを使用して、削除済みアイテム フォルダーにアイテムを移動することもできます。 たとえば、削除アクションを含む[ルールを作成する](inbox-management-and-ews-in-exchange.md)ことができます。 
  
アイテムを削除する場合の注意点:
  
- 定期的な発生アイテムを削除しても、削除済みアイテム フォルダーまたはごみ箱への移動は行われません。これにより、定期的なアイテムの定期的マスター アイテムが更新されます。
    
- 既定のフォルダーはメールボックスから削除できません。
    
- 会議または会議のメッセージ (会議出席依頼または会議の更新など) は削除しないでください。 代わりに、応答オブジェクトを使用してこれらのアイテムに対応します。 これで、関連付けられている予定表アイテムが更新され、レスポンダーまたは開催者のアクションが反映されます。
    
- アイテムが削除済みアイテムまたは削除フォルダーに移動されている場合、アイテムのキーの変更は更新されません。
    
- アイテムの物理的な削除を実行してから、[SyncFolderHierarchy 操作](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx)や [SyncFolderHierarchy](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderhierarchy%28v=exchg.80%29.aspx) EWS マネージ API メソッド、または [SyncFolderItems 操作](http://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx)や [SyncFolderItems](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderitems%28v=exchg.80%29.aspx) メソッドを呼び出すと、**Delete** 変更エントリが返されます。 アイテムを削除済みアイテム フォルダーに移動すると、**Update** 変更エントリが返されます。 これは、アイテムまたはフォルダーが新しい [ParentFolderId](http://msdn.microsoft.com/library/258f4b1f-367e-4c7d-9c29-eb775a2398c7%28Office.15%29.aspx) プロパティ値を持つためです。 削除済みアイテムの同期がシナリオの一部になっている場合は、[同期について参照してください](mailbox-synchronization-and-ews-in-exchange.md)。 
    
## <a name="find-out-more-about-deleting-items"></a>アイテムの削除についての詳細
<a name="findoutmore"> </a>

- [Exchange での EWS の削除に関連するメールボックス イベントのプル通知](pull-notifications-for-ews-deletion-related-mailbox-events-in-exchange.md)
    
- [Exchange における EWS での削除に関連するエラーの処理](handling-deletion-related-errors-in-ews-in-exchange.md)
    
## <a name="see-also"></a>関連項目

- [Exchange の EWS のフォルダーとアイテム](folders-and-items-in-ews-in-exchange.md)    
- [Exchange の Web サービス クライアントを開発する](develop-web-service-clients-for-exchange.md)    
- [回復可能なアイテム フォルダー](http://technet.microsoft.com/ja-JP/library/ee364755.aspx)    
- [Exchange Server 2010 での単一アイテムの回復](http://blogs.technet.com/b/exchange/archive/2009/09/25/3408389.aspx#_Single_Item_Recovery)    
- [Exchange 2013: Exchange サーバーからプログラムを使用して定期的なアイテムを削除する](http://code.msdn.microsoft.com/exchange/Exchange-2013-Delete-a-e1c7b89d)    
- [Exchange 2013: プログラムを使用して Exchange サーバー上のアカウントからタスクを削除する](http://code.msdn.microsoft.com/exchange/Exchange-2013-Delete-tasks-13824637)    
- [Exchange 2013: プログラムを使用して Exchange サーバー上のフォルダーを空にする](http://code.msdn.microsoft.com/exchange/Exchange-2013-Empty-6487df37)    
- [Exchange 2013: Exchange サーバーからプログラムを使用してフォルダーを削除する](http://code.msdn.microsoft.com/exchange/Exchange-2013-Delete-aa1a5823)    
- [Exchange 2013: Exchange サーバーからプログラムを使用して多くのアイテムを削除する](http://code.msdn.microsoft.com/exchange/Exchange-2013-Delete-many-064f8760)    
- [Exchange 2013: Exchange サーバーからプログラムを使用して連絡先を削除する](http://code.msdn.microsoft.com/exchange/Exchange-2013-Delete-3b8b0640)    
- [Exchange の EWS を使用して、予定を削除し、会議をキャンセルする](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)    
- [Exchange で EWS を使用して永続的なアプリケーションの設定を管理する](how-to-manage-persistent-application-settings-by-using-ews-in-exchange.md)
    

