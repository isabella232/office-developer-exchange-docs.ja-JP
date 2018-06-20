---
title: Exchange の EWS を使用するアイテムの削除
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: c81e3160-e12b-47e0-b3d6-4be28537f301
description: Exchange で EWS マネージ API または EWS を使用して、アイテムを削除済みアイテム フォルダーまたはごみ箱に移動して削除する方法について説明します。
ms.openlocfilehash: a475ebc6677e5f5003cc790a2d4d2b83c513f309
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19758904"
---
# <a name="deleting-items-by-using-ews-in-exchange"></a>Exchange の EWS を使用するアイテムの削除

Exchange で EWS マネージ API または EWS を使用して、アイテムを削除済みアイテム フォルダーまたはごみ箱に移動して削除する方法について説明します。
  
確認することは今まで自分では、削除済みアイテム フォルダーにアイテムを移動し、移動する間の違い、ごみ箱をあさるか。 興味がある項目を削除する処理と、アプリケーションでこれらのオプションを実装する方法のさまざまなオプションがあります。 Exchange Web サービス (EWS) には、アイテムの削除処理の 3 つのオプションが含まれています。 この資料はうまくいけば、それらの違いについて混乱をオフにします。
  
## <a name="deleting-items---what-are-my-options"></a>項目の削除のオプションは何ですか。
<a name="bk_DeletingItemsOptions"> </a>

アイテムを削除するための全体の展望を理解する前に、次の違いを認識することが重要です。
  
- 削除済みアイテム フォルダー、メールボックス内のアイテムを削除すると、これは、どこにいます。
    
- ごみ箱をあさる (別名、回復可能なアイテム] フォルダー) - これは、どこでこれらのメールボックスからアイテムを削除するとします。
    
図 1 と図 2 は、メールボックスのアイテムとフォルダーの削除処理がどのようなものかを示しています。  

**図 1 です。メールボックスからアイテムを削除するためのプロセス**

![削除されると、位置を示す図のアイテムを移動します。 削除済みアイテムは、[削除済みアイテム] フォルダーに移動し、リテンション ・ ポリシー、有効期限が切れるし、permantently が削除されたは、場所ごとの回復可能なアイテムのフォルダーに移動し、します。](media/Ex_DeleteItems_Source.png)

<br/>

**図 2 になります。メールボックスからフォルダーを削除するためのプロセス**

![図は、削除されたフォルダーが [削除済みアイテム] フォルダーに移動した後に、メールボックスから完全に削除される方法を示しています。](media/Ex_.png)
   
削除の「永続性」に応じて、アイテムとフォルダーは 3 つの方法で削除できます。
  
**EWS を使用して項目を削除するためのオプションを表 1:**

|**オプション**|**動作します。**|
|:-----|:-----|
|削除済みアイテム フォルダーに移動する  <br/> |これは、項目を削除するのには最低限の永続的です。<br/><br/>これは、自分の席でごみ箱に用紙を配置することに似ています。 簡単に取得できますする必要がある場合、もう一度。<br/><br/>この操作を実行するのには [削除済みアイテム フォルダー オプションへの移行を実装するすべての[削除操作](deleting-items-by-using-ews-in-exchange.md#bk_howdoIdeleteitems)を使用することができます。<br/><br/>アイテムまたはフォルダーを削除済みアイテム フォルダーに移動するのに、 [MoveItem 操作](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx)( [Item.Move()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.move%28v=exchg.80%29.aspx)) や、 [MoveFolder 操作](http://msdn.microsoft.com/library/c7233966-6c87-4a14-8156-b1610760176d%28Office.15%29.aspx)( [Folder.Move()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.move%28v=exchg.80%29.aspx)) を使用することもできます。  <br/> |
|論理的な削除  <br/> |削除フォルダーにアイテムを移動、ごみ箱をあさる。<br/><br/>こみ、コンテナーに、ごみ箱を空にするのと同様です。 必要がある場合でも、アイテムにアクセスすることができます、だけで、もう少し複雑になります。  <br/><br/>詳細については、ごみ箱をあさる (回復可能なアイテムのフォルダーとも呼ばれます) し、電子的証拠開示や訴訟の保留などのシナリオは、TechNet の[回復可能なアイテム] フォルダー](http://technet.microsoft.com/en-us/library/ee364755%28v=exchg.150%29.aspx)を参照してください。<br/><br/>ソフト削除はされていない Exchange 2007 を対象とするアプリケーションをお勧めします。 Exchange 2007 では、ソフトの削除は、アイテムに、少しの設定に移動することを示すために、ごみ箱をあさる時に、指定されていません。<br/><br/>Exchange オンラインのバージョンの Exchange が Exchange 2010 で始まる、Office 365 の一部として Exchange Online では、ソフト削除走査、またはされているソフト、 [FindItem 操作](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)で削除された項目の検索はサポートされていません。  <br/><br/>**注**: フォルダーは、ソフト削除することはできません。           |
|物理的な削除  <br/> |アイテムまたはフォルダーが完全に削除されます。<br/><br/>ハード削除済みアイテム フォルダーに配置されます、パージのごみ箱をあさる。 リサイクルのトラックがこみリサイクル コンテナーを空にするときと同様です。 アイテムは、Outlook または Outlook Web App では、ような電子メール クライアントからはアクセスできませんし、一定期間の後、アイテムを完全に削除する保留リストのメールボックスの設定がない限り、します。<br/><br/>詳細を参照することで、「[削除済みアイテム保存期間の構成と回復可能なアイテム クォータ](http://technet.microsoft.com/en-us/library/ee364752%28v=exchg.150%29.aspx)アイテムの保存期間について。<br/><br/>**注**: ハード削除されると、[パージ] フォルダーにフォルダーは入れられません。 ハード削除されたフォルダーは、メールボックスから削除されます。  |
   
削除済みアイテム フォルダーへの移動および物理的な削除のオプションはトランザクションです。これは、Web サービス呼び出しが完了するまでに、アイテムが削除済みアイテム フォルダーまたはごみ箱に移動されていることを意味します。
  
削除済みアイテムの格納に使用されるフォルダーのエコシステムを理解するために、次の図は、[削除済みアイテムを含めることができるフォルダーの階層を示します。 フォルダー名は、 **DistinguishedFolderIdNameType**スキーマの種類、または EWS のマネージ API の**WellKnownFolderName**列挙体に表示されるとおりです。 
  
**図 3 です。削除済みアイテムを含むフォルダーの階層**

![図は、削除されたアイテムをプライマリ メールボックスとアーカイブ メールボックスの両方に含めることのできるフォルダーのフォルダー階層を示しています。図では、各フォルダーは個別のフォルダー名で示されています。](media/Ex_FolderHierarchyDeletedItems.png)
  
**表 2: 削除済みアイテムを含むフォルダー**

|**フォルダー名**|**導入されました。**|**説明**|
|:-----|:-----|:-----|
|deleteditems  <br/> |Exchange 2007  <br/> |既定の削除済みアイテム フォルダー。アイテムは、論理的な削除によって削除されるか、物理的に削除されるまで、または保存期間が超えるまでこのフォルダーに残ります。次に、このアイテムはごみ箱内のフォルダーに移動されます。削除済みフォルダーは、削除済みアイテム フォルダーに配置されており、論理的な削除によって削除されるか、物理的に削除されるときに、メールボックスから完全に削除され、回復できなくなります。  <br/> |
|recoverableitemsroot  <br/> |Exchange 2010  <br/> |ルート、収集、または、回復可能なアイテム] フォルダーです。 収集機能アクセスは、Exchange 2010 内で実装されています。 このフォルダーの表示名は、[回復可能なアイテム] です。  <br/> |
|recoverableitemsdeletions  <br/> |Exchange 2010  <br/> |メインごみ箱をあさるメールボックスのフォルダーです。 ソフト削除済みアイテムおよびアイテム保持ポリシーによって、削除済みアイテム フォルダーから移動したアイテムは、このフォルダーに配置されます。 このフォルダーの表示名は、「削除」です。  <br/> |
|recoverableitemsversions  <br/> |Exchange 2010  <br/> |アイテムの以前のバージョンが格納されます。 アイテムの以前のバージョンは、項目が更新されたときに作成されます。 下書きアイテムのバージョンはこのフォルダーに保存されません。 このフォルダーの表示名は、「バージョン」です。  <br/> |
|recoverableitemspurges  <br/> |Exchange 2010  <br/> |削除フォルダーから削除されるアイテムが格納されます。 ハード削除ストアのすべての項目は、このフォルダーに移動されます。 このフォルダーの表示名は、「パージ」です。  <br/> |
|archiveddeletedtitems  <br/> |Exchange 2010  <br/> |アーカイブ メールボックスの既定の削除済みアイテム フォルダー。  <br/> |
|archiverecoverablesitemsroot  <br/> |Exchange 2010  <br/> |アーカイブ メールボックスのルートごみ箱フォルダー。論理的な削除によって削除されたアーカイブ アイテムは、このフォルダーのサブフォルダーに移動されます。  <br/> |
|archiverecoverableitemsdeletions  <br/> |Exchange 2010  <br/> |アーカイブ メールボックスのメインごみ箱フォルダー。ごみ箱に移動されたアーカイブ アイテムはここに配置されます。  <br/> |
|archiverecoverableitemsversions  <br/> |Exchange 2010  <br/> |以前のバージョンのアーカイブ アイテムが格納されます。  <br/> |
|archiverecoverableitemspurges  <br/> |Exchange 2010  <br/> |ごみ箱のアーカイブ削除フォルダーにある物理的に削除されたアイテムが格納されます。記憶域で物理的に削除されたすべてのアーカイブ アイテムは、このフォルダーに移動されます。  <br/> |
   
## <a name="how-do-i-delete-items"></a>アイテムを削除する方法
<a name="bk_howdoIdeleteitems"> </a>

次のいずれかを使用して、削除済みアイテム フォルダーにアイテムを移動するか、論理的な削除または物理的な削除を実行するかどうかを指定します。
  
- **DisposalType**単純型、EWS を使用して Exchange にアクセスする場合。 
    
- [DeleteMode 列挙型](http://msdn.microsoft.com/en-us/library/exchange/microsoft.exchange.webservices.data.deletemode%28v=exchg.80%29.aspx)EWS のマネージ API を使用する場合。
    
複数の異なる EWS 操作または EWS マネージ API メソッドを使用して、メールボックスからアイテムやフォルダーを削除できます。
  
**表 3: EWS 操作および削除するアイテムの EWS のマネージ API のメソッド**

|**EWS 操作**|**EWS マネージ API メソッド**|**導入されました。**|**できること**|
|:-----|:-----|:-----|:-----|
|[DeleteFolder 操作](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |[Folder.Delete メソッド](http://msdn.microsoft.com/en-us/library/exchange/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) <br/> |Exchange 2007  <br/> |メールボックスからフォルダーを削除します。EWS では、フォルダーをバッチ削除できます。EWS マネージ API では、呼び出しごとに 1 つのフォルダーのみを削除できます。  <br/> |
|[DeleteItem の操作](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |[Item.Delete メソッド](http://msdn.microsoft.com/en-us/library/exchange/microsoft.exchange.webservices.data.item.delete%28v=exchg.80%29.aspx)<br/><br/>[ExchangeService.DeleteItems メソッド](http://msdn.microsoft.com/en-us/library/exchange/microsoft.exchange.webservices.data.exchangeservice.deleteitems%28v=exchg.80%29.aspx) <br/> |Exchange 2007  <br/> |メールボックスからアイテムを削除します。  <br/> |
|[EmptyFolder 操作](http://msdn.microsoft.com/library/98161486-e2f2-480f-8d5d-708ba81b208a%28Office.15%29.aspx) <br/> |[Folder.Empty メソッド](http://msdn.microsoft.com/en-us/library/exchange/microsoft.exchange.webservices.data.folder.empty%28v=exchg.80%29.aspx) <br/> |Exchange 2010  <br/> |フォルダー内のすべての項目を削除し、必要に応じて、フォルダー内のすべてのサブフォルダーを削除します。  <br/> |
|[ApplyConversationAction 操作](http://msdn.microsoft.com/library/73d7943d-d361-4f8b-9948-d85f886efa1a%28Office.15%29.aspx) <br/> |[Conversation.EnableAlwaysDeleteItems メソッド](http://msdn.microsoft.com/en-us/library/exchange/microsoft.exchange.webservices.data.conversation.enablealwaysdeleteitems%28v=exchg.80%29.aspx)<br/><br/>[Conversation.DeleteItems メソッド](http://msdn.microsoft.com/en-us/library/exchange/microsoft.exchange.webservices.data.conversation.deleteitems%28v=exchg.80%29.aspx) <br/> |Exchange 2010  <br/> |会話の電子メール メッセージに対して削除処理アクションを設定し、それらが削除されるようにします。  <br/> |
|[DeleteUserConfiguration 操作](http://msdn.microsoft.com/library/93e44690-be2d-4fdb-96a8-4ded3c193aed%28Office.15%29.aspx) <br/> |[UserConfiguration.Delete メソッド](http://msdn.microsoft.com/en-us/library/exchange/microsoft.exchange.webservices.data.userconfiguration.delete%28v=exchg.80%29.aspx) <br/> |Exchange 2010  <br/> |アイテムに関連付けられているフォルダーを削除し、ごみ箱に移動します。  <br/> |
|
  [CreateItem 操作](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/> |[Appointment.Accept メソッド](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.accept%28v=exchg.80%29.aspx) <br/><br/>[Appointment.AcceptTentatively メソッド](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.accepttentatively%28v=exchg.80%29.aspx)<br/><br/>[Appointment.CancelMeeting メソッド](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.cancelmeeting%28v=exchg.80%29.aspx)<br/><br/>[Appointment.Decline](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.decline%28v=exchg.80%29.aspx)<br/><br/>[MeetingRequest.Accept メソッド](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.meetingrequest.accept%28v=exchg.80%29.aspx)<br/><br/>[MeetingRequest.AcceptTentatively メソッド](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.meetingrequest.accepttentatively%28v=exchg.80%29.aspx)<br/><br/>[MeetingRequest.Decline メソッド](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.meetingrequest.decline%28v=exchg.80%29.aspx) <br/> |Exchange 2007  <br/> |直接移動しないアイテム削除済みアイテム フォルダーに会議出席依頼への応答が送信されたか、応答が予定に設定します。<br/><br/>削除の種類は、この操作では設定されていません。 会議のメッセージは、応答オブジェクトは、サービスが正常に処理するときに、削除済みアイテム フォルダーに移動されます。  <br/> |
   
受信トレイ ルールを使用して削除済みアイテム フォルダーにアイテムを移動することもできます。 たとえば、[ルールを作成](inbox-management-and-ews-in-exchange.md)削除処理ができます。 
  
アイテムを削除する場合の注意点:
  
- 定期的な発生アイテムを削除しても、削除済みアイテム フォルダーまたはごみ箱への移動は行われません。これにより、定期的なアイテムの定期的マスター アイテムが更新されます。
    
- 既定のフォルダーはメールボックスから削除できません。
    
- 会議または会議出席依頼、または会議の更新など、会議のメッセージを削除しないでください。 代わりに、応答オブジェクトを使用してこれらの項目に対応します。 この方法では、開催者が、応答側のアクションを反映するために関連付けられている予定表アイテムが更新されます。
    
- アイテムが削除済みアイテムまたは削除フォルダーに移動すると、項目のキーの変更は更新されません。
    
- ハードを実行する場合、項目の削除し、 [SyncFolderHierarchy 操作](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx)または[SyncFolderHierarchy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderhierarchy%28v=exchg.80%29.aspx) EWS のマネージ API のメソッド、またはメソッドを呼び出して、 [SyncFolderItems 操作](http://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx)または[SyncFolderItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderitems%28v=exchg.80%29.aspx) **削除**の変更エントリが返されます。 削除済みアイテム フォルダーにアイテムを移動すると、**更新プログラム**の変更エントリが返されます。 アイテムまたはフォルダーに新しい[ParentFolderId](http://msdn.microsoft.com/library/258f4b1f-367e-4c7d-9c29-eb775a2398c7%28Office.15%29.aspx)プロパティの値を持つためにです。 [同期の詳細について](mailbox-synchronization-and-ews-in-exchange.md)削除済みアイテムを同期する場合は、自分のシナリオの一部です。 
    
## <a name="find-out-more-about-deleting-items"></a>アイテムの削除についての詳細
<a name="findoutmore"> </a>

- [EWS の [メールボックスの削除に関連するイベントの通知を Exchange でプルします。](pull-notifications-for-ews-deletion-related-mailbox-events-in-exchange.md)
    
- [Exchange EWS での削除に関連するエラーの処理](handling-deletion-related-errors-in-ews-in-exchange.md)
    
## <a name="see-also"></a>関連項目

- [Exchange の EWS のフォルダーとアイテム](folders-and-items-in-ews-in-exchange.md)    
- [Exchange の Web サービス クライアントを開発する](develop-web-service-clients-for-exchange.md)    
- [回復可能な項目] フォルダー](http://technet.microsoft.com/en-us/library/ee364755.aspx)    
- [Exchange Server 2010 での単一アイテムの回復](http://blogs.technet.com/b/exchange/archive/2009/09/25/3408389.aspx#_Single_Item_Recovery)    
- [Exchange 2013: 一連の定期的なプログラムを使用して Exchange のサーバーから削除します。](http://code.msdn.microsoft.com/exchange/Exchange-2013-Delete-a-e1c7b89d)    
- [Exchange 2013: のタスクからの Exchange サーバー上のアカウントからのプログラムで削除します。](http://code.msdn.microsoft.com/exchange/Exchange-2013-Delete-tasks-13824637)    
- [空の Exchange サーバー上のフォルダーにプログラムを使用して Exchange 2013。](http://code.msdn.microsoft.com/exchange/Exchange-2013-Empty-6487df37)    
- [Exchange 2013: フォルダーを削除プログラムを使用して Exchange サーバーから](http://code.msdn.microsoft.com/exchange/Exchange-2013-Delete-aa1a5823)    
- [Exchange 2013: 多数のアイテムを削除プログラムを使用して Exchange サーバーから](http://code.msdn.microsoft.com/exchange/Exchange-2013-Delete-many-064f8760)    
- [Exchange 2013: 連絡先を削除してプログラムを使用して Exchange サーバーから](http://code.msdn.microsoft.com/exchange/Exchange-2013-Delete-3b8b0640)    
- [予定を削除して、Exchange で EWS を使用して会議をキャンセル](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)    
- [EWS を使用して Exchange 内で永続的なアプリケーションの設定を管理します。](how-to-manage-persistent-application-settings-by-using-ews-in-exchange.md)
    

