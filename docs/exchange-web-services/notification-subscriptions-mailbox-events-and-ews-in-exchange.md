---
title: Exchange の通知サブスクリプション、メールボックス イベント、および EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 76136f28-0dad-4ecc-9dd7-a45a1861e4b0
description: Exchange の通知サブスクリプションと EWS のメールボックス イベントについて説明します。
localization_priority: Priority
ms.openlocfilehash: 00a0941e615f35a46bb77c00648b75fcd2a45286
ms.sourcegitcommit: 843a2e030a94b12aec70c553ca4e06e39ac02d82
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/09/2020
ms.locfileid: "49603842"
---
# <a name="notification-subscriptions-mailbox-events-and-ews-in-exchange"></a>Exchange の通知サブスクリプション、メールボックス イベント、および EWS

Exchange の通知サブスクリプションと EWS のメールボックス イベントについて説明します。
  
EWS マネージ API と Exchange Web Services (EWS) の両方を使用して、メールボックス、またはメールボックスの 1 つ以上のフォルダーでイベントが発生したときに通知を受信するようサブスクライブできます。ストリーミング通知、プル通知、プッシュ通知の 3 つのサブスクリプションの種類があります。これらのサブスクリプションの種類は、それぞれ異なる手法を使用して通知を受信または取得します。
  
## <a name="getting-notifications---what-are-my-options"></a>通知を取得する場合のオプション
<a name="bk_notiftypes"> </a>

EWS には、独立して動作し、クライアントにサーバーの変更を通知する 3 種類のサブスクリプションが含まれています。どのサブスクリプションの種類を選択しても、最終的にすべて同じ通知にアクセスすることになり、取得方法が異なるだけです。
  
**表 1 サブスクリプションの種類**

|**オプション**|**説明**|**適切かどうか**|
|:-----|:-----|:-----|
|ストリーミング通知  <br/> |特定の期間開いたままの状態の接続を経由した、サーバーから送信される通知。  <br/> |ストリーミング通知は通常、ほとんどのアプリケーションで推奨されます。プル通知およびプッシュ通知と同様のもので、両方のメリットを併せ持っています。通知サブスクリプションを確立した後、接続が最大で 30 分間開いたままになり、それによってサーバーがクライアントにプッシュ通知を行えるようになります。プル サブスクリプションのように更新を要求する必要はなく、プッシュ サブスクリプションのように Web サービス リスナー アプリケーションを作成する必要もありません。  <br/> |
|プル通知  <br/> |クライアントによって要求 (またはプル) される通知。  <br/> |プル通知は通常、クライアントがネットワークに確実に接続されているわけでない疎結合クライアントに最も適しています。プル通知は、クライアントがサーバーに頻繁に要求を送信して通知を受信するため、クライアントとサーバーの間の余分なトラフィックを確立してしまうことがあり、すべての要求が受信通知になるわけではありません。  <br/> |
|プッシュ通知  <br/> |コールバック アドレスを経由し、サーバーによってクライアント側の Web サービスに送信 (またはプッシュ) される通知。  <br/> |一般的に、プッシュ通知はプル通知よりも通知の遅延が小さく、サーバーのアクセスが信頼性の高いもので、クライアントが IP アドレス指定可能な密結合のクライアントに適しています。ただし、プッシュ通知は Exchange 2010 でストリーミング通知が登場して以来、使用されなくなっています。可能であれば、今後はプッシュ通知ではなく、ストリーミング通知を使用することをお勧めします。プッシュ通知ではリスナー アプリケーションを作成する必要があり、そこに通知がプッシュされます。この点はプル通知に比べて少し利点があり、書き込みのトラフィックが減少しますが、別のアプリケーションを必要とすることでオーバーヘッドが増加します。  <br/> |
   
## <a name="what-ews-events-can-i-subscribe-to"></a>サブスクライブできる EWS のイベント
<a name="bk_eventtypes"> </a>

クライアントがサブスクライブする EWS イベントの種類は、EWS マネージ APIの [EventType](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.eventtype%28v=exchg.80%29.aspx) 列挙型、または EWS の [EventType](https://msdn.microsoft.com/library/04b70f9e-c226-4130-958e-0db0275cf58b%28Office.15%29.aspx) 要素によって定義されます。次の EWS イベントがサブスクリプションに利用できます。 
  
- NewMail – 受信トレイに新しいメッセージが到着しました。
    
- Deleted - メッセージが受信トレイから物理的に削除されました。削除されたアイテムの通知に関する詳細については、「[Exchange の EWS を使用するアイテムの削除](deleting-items-by-using-ews-in-exchange.md)」 と 「[Exchange での EWS の削除に関連するメールボックス イベントのプル通知](pull-notifications-for-ews-deletion-related-mailbox-events-in-exchange.md)」を参照してください。
    
- Modified – アイテムまたはフォルダーが変更されました。
    
- Moved – アイテムまたはフォルダーが移動されました。 
    
- Copied – アイテムまたはフォルダーがコピーされました。
    
- Created – アイテムまたはフォルダーが作成されました。 
    
- FreeBusyChanged - ユーザーの空き時間情報が変更されました。
    
EWS イベントの別の種類である Status イベントは、[EventType](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.eventtype%28v=exchg.80%29.aspx) 要素によって定義されますが、このイベントにはサブスクライブしません。その代わり、ストリーミング通知とプッシュ通知のみに関するクライアントの状態を確認するために、そのイベントはサーバーによって送信されます。クライアントは、このイベントに応答する必要があり、そうしないとクライアントはタイムアウトになります。 
  
たいていの場合、1 つのユーザー アクションで、複数の通知が作成されます。このことを示すため、次の図では、いくつかの一般的なシナリオとそれぞれに作成された通知を図示しています。クライアントの設定によって受信する通知は変わってくるので、これは構成オプションと結果の通知すべてを網羅したリストではありません。
  
**図 1 通知サブスクリプションによって返されるイベントの種類**

![新規電子メールの受信、新規フォルダーの作成、フォルダーの移動など一般的なユーザー シナリオで送信される通知を示した表。](media/Exchange2013_Notifications_Events.png)
  
図 1 では、通知の処理が簡素化されています。実際には、単一のユーザーのアクションに対して複数の通知 (同じ種類の複数の通知も可) を作成できます。たとえば、フォルダーの移動操作では、変更されたフォルダー用に 1 つ、古い親フォルダー用に 1 つ、新しい親フォルダー用に 1 つ、で合わせて 3 つのフォルダー イベントが作成されます。1 回の操作で多数のイベントが発生する可能性があるため、[同期処理には数秒の待機時間を作成](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices)し、操作の途中ではなく、アクションが完了したときにのみ同期するようにします。
  
また、各ユーザーが選択した構成設定によって、作成される通知が変わってくることを認識しておくことも重要です。たとえば、新しい会議出席依頼を受信した場合、アイテムを読み上げる前でさえ、一部のユーザーの空き時間情報データは自動的に更新され、FreeBusyChanged イベントが作成されます。また、空き時間情報データが更新されず、会議を承諾した後まで FreeBusyChanged イベントが作成されないユーザーもいます。これらの設定は、サーバーによって作成される通知に大きな影響を与える可能性があります。
  
## <a name="how-do-ews-notifications-work"></a>EWS の通知のしくみ
<a name="bk_howwork"> </a>

EWS の通知は、サブスクリプションごとに処理されます。通常、メールボックスあたり 1 つのサブスクリプションがあり、メールボックスのサブスクリプション内で、一部またはすべてのフォルダーをサブスクライブできます。サブスクライブする通知の種類 (ストリーミング、プル、またはプッシュ) を決定し、受信したいイベントの種類 (NewMail、Created、Deleted、Modified など) を決定し、サブスクリプションを作成します。EWS のイベントは、非同期的にメールボックス サーバーからクライアントに送信されます。(以前、Exchange 2007 ではイベントは同期的で、Exchange 2010 ではイベントはクライアント アクセス サーバーに保存されていましたが、現在はそうではありません。)
  
サブスクリプションの種類によって、クライアントに通知が送信される方法が異なります。このセクションでは、サブスクリプションの種類ごとのしくみについて詳細に説明します。
  
### <a name="ews-streaming-notifications"></a>EWS のストリーミング通知
<a name="bk_streamnotif"> </a>

ストリーミング通知は、ストリーミング サブスクリプションの接続を開いているサーバーの分岐 get 要求に依存するため、接続がアクティブな間に発生するイベントは、クライアントにすぐにストリーミングされます。1 つの接続の間に複数の通知を送信でき、接続は一定時間が経過するまで開いている状態が維持されます (最大 30 分)。接続が切断されると、クライアントは分岐 get 要求をもう一度送信します。図 2 では、ストリーミングのサブスクリプションとストリーミング通知のしくみを示します。
  
**図 2 ストリーミング通知の概要**

![ストリーミング通知の動作方法を示す図。ストリーミング通知をセットアップするには、次を実行します。1. サブスクライブします。2. 接続を開きます。3. イベントを待機します。4. イベントを受信し、3 と 4 を繰り返します。5. 接続を閉じるか、そのままにします。6. サブスクリプションを解除するか、タイムアウトします。](media/Exchange2013_Notifications_StreamSub.png)
  
ストリーミングの通知を作成する方法の詳細については、「[Exchange での EWS を使用したメールボックス イベントに関するストリーム通知](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md)」を参照してください。
  
### <a name="ews-pull-notifications"></a>EWS プル通知
<a name="bk_pullnotif"> </a>

プル通知は、クライアントが管理する間隔で通知を要求するクライアントに依存します。これにより、通知のない GetEvents 応答が発生することがあります。図 3 は、プル サブスクリプションとプル通知のしくみを示しています。
  
**図 3 プル通知の概要**

![プル通知の動作方法を示す図。プル通知をセットアップするには、次を実行します。1. サブスクライブします。2. GetEvents を送信します。3. 応答を受信し、2 と 3 を繰り返します。4. 接続を閉じるか、そのままにします。5. サブスクリプションを解除するか、タイムアウトします。](media/Exchange2013_Notifications_PullSub.png)
  
プル通知を作成する方法の詳細については、「[Exchange での EWS を使用したメールボックス イベントに関するプル通知](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md)」を参照してください。
  
### <a name="ews-push-notifications"></a>EWS プッシュ通知
<a name="bk_pushnotif"> </a>

プッシュ通知は、通知をクライアントにプッシュするサーバーに依存します。通知がある場合にのみトラフィックがあります。図 4 は、プッシュ サブスクリプションとプッシュ通知のしくみを示しています。
  
**図 4 プッシュ通知の概要**

![プッシュ通知の動作方法を示す図。プッシュ通知をセットアップするには、次を実行します。1. リスナーを作成します。2. サブスクライブします。3. イベントを待機します。4. イベントを受信します。5. [OK] 応答を送信し、3、4、および 5 を繰り返します。6. サブスクリプションを解除するか、タイムアウトします。](media/Exchange2013_Notifications_PushSub.png)

[Exchange 2010 を使用したプッシュ通知](https://msdn.microsoft.com/library/db1f8523-fa44-483f-bdb6-ab5939b52eee%28Office.15%29.aspx)を利用している場合、[ストリーミング通知を利用する](https://code.msdn.microsoft.com/exchange/Exchange-2013-Set-push-82738cc5)ようアプリケーションをアップグレードすることを検討してください。こうすると、イベントを受信する別のアプリケーションが必要ありません。

  
## <a name="how-do-i-subscribe-to-notifications"></a>通知をサブスクライブする方法
<a name="bk_notifoperations"> </a>

作成するサブスクリプションの種類に応じて、通知のサブスクライブのために選択する様々なオプションがあります。
  
**表 2 通知をサブスクライブするための操作とメソッド**

|**サブスクリプションの種類**|**EWS 操作**|**EWS マネージ API メソッド**|**目的**|
|:-----|:-----|:-----|:-----|
|ストリーミング  <br/> |[サブスクライブ操作](https://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx) <br/> |[ExchangeService.BeginSubscribeToStreamingNotifications メソッド](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.beginsubscribetostreamingnotifications%28v=exchg.80%29.aspx) <br/> [ExchangeService.BeginSubscribeToStreamingNotificationsOnAllFolders メソッド](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.beginsubscribetostreamingnotificationsonallfolders%28v=exchg.80%29.aspx) <br/> [ExchangeService.SubscribeToStreamingNotificationsOnAllFolders メソッド](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetostreamingnotifications%28v=exchg.80%29.aspx) <br/> |ストリーミング通知をサブスクライブする要求を作成します。  <br/> |
|プル  <br/> |[サブスクライブ操作](https://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx) <br/> |[ExchangeService.BeginSubscribeToPullNotifications メソッド](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.beginsubscribetopullnotifications%28v=exchg.80%29.aspx) <br/> [ExchangeService.BeginSubscribeToPullNotificationsOnAllFolders メソッド](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.beginsubscribetopullnotificationsonallfolders%28v=exchg.80%29.aspx) <br/> [ExchangeService.SubscribeToPullNotifications メソッド](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) <br/> [ExchangeService.SubscribeToPullNotificationsOnAllFolders メソッド](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotificationsonallfolders%28v=exchg.80%29.aspx) <br/> |プル通知をサブスクライブする要求を作成します。  <br/> |
|プッシュ  <br/> |[サブスクライブ操作](https://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx) <br/> |[ExchangeService.BeginSubscribeToPushNotifications overloaded メドッド](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.beginsubscribetopushnotifications%28v=exchg.80%29.aspx) <br/> [ExchangeService.BeginSubscribeToPushNotificationsOnAllFolders overload メソッド](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.beginsubscribetopushnotificationsonallfolders%28v=exchg.80%29.aspx) <br/> [ExchangeService.SubscribeToPushNotifications overloaded メソッド](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopushnotifications%28v=exchg.80%29.aspx) <br/> [ExchangeService.SubscribeToPushNotificationsOnAllFolders overloaded メソッド](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopushnotificationsonallfolders%28v=exchg.80%29.aspx) <br/> |プッシュ通知をサブスクライブする要求を作成します。  <br/> |
   
## <a name="how-do-i-get-ews-events"></a>EWS のイベントを取得する方法
<a name="bk_getevents"> </a>

サブスクリプションが作成されると、実際のイベントがクライアントに送信される方法は、サブスクリプションの種類によって異なります。 
  
ストリーミング通知を行うためにはストリーミング サブスクリプション接続を作成する必要があり、作成するとサブスクリプションが接続に追加されます。 このプロセスの詳細は、「[Exchange での EWS を使用したメールボックス イベントに関するストリーム通知](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md)」で確認できます。 
  
プル通知では、サブスクリプションが作成されたときにサブスクリプション オブジェクトが初期化されるため、 **GetEvent** メソッドまたは操作を呼び出してサーバーからイベントを取得するだけで十分です。 この詳細は、「[Exchange での EWS を使用したメールボックス イベントに関するプル通知](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md)」で確認できます。 
  
以下の表には、イベントを取得するために必要な操作とクラスが一覧表示されています。 
  
**表 3 接続を作成してイベントを取得するための要素とクラス**

|**サブスクリプションの種類**|**EWS 操作**|**EWS マネージ API メソッド**|**目的**|
|:-----|:-----|:-----|:-----|
|ストリーミング  <br/> |[GetStreamingEvents の操作](https://msdn.microsoft.com/library/8da95423-72bc-4034-90a8-162eedcd059b%28Office.15%29.aspx) <br/> |[StreamingSubscriptionConnection.AddSubscription メソッド](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.streamingsubscriptionconnection.addsubscription%28v=exchg.80%29.aspx) <br/> |イベントが発生したときに応答する分岐 get 要求をサーバーで作成します。  <br/> |
|プル  <br/> |[GetEvents 操作](https://msdn.microsoft.com/library/f268efe5-9a1a-41a2-b6a6-51fcde7720a1%28Office.15%29.aspx) <br/> |[PullSubscription.GetEvents メソッド](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pullsubscription.getevents%28v=exchg.80%29.aspx) <br/> |サーバーからプル通知イベントを取得します。  <br/> |
|プッシュ  <br/> |該当なし。  <br/> |該当なし。  <br/> |プッシュ通知は、Web サービスのリスナー (サブスクリプション要求で指定されたコールバック URL) に自動的に送信されます。追加のメソッドまたは操作を呼び出す必要はありません。  <br/> |
   
## <a name="how-do-i-unsubscribe-to-notifications"></a>通知をアンサブスクライブする方法
<a name="bk_notifunsubscribe"> </a>

次の表は、サブスクリプションの種類ごとにアンサブスクライブする方法を示しています。
  
**表 4 通知をアンサブスクライブするための操作とメソッド**

|**サブスクリプションの種類**|**EWS**|**EWS Managed API**||
|:-----|:-----|:-----|:-----|
|ストリーミング  <br/> |[Unsubscribe 操作](https://msdn.microsoft.com/library/994a9d2b-1501-4804-90f0-12bd914496ec%28Office.15%29.aspx) <br/> |[StreamingSubscription.BeginUnsubscribe メソッド](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.streamingsubscription.beginunsubscribe%28v=exchg.80%29.aspx) <br/> [StreamingSubscription.EndUnsubscribe メソッド](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.streamingsubscription.endunsubscribe%28v=exchg.80%29.aspx) <br/> [StreamingSubscription.Unsubscribe メソッド](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.streamingsubscription.unsubscribe%28v=exchg.80%29.aspx) <br/> ||
|プル  <br/> |[Unsubscribe 操作](https://msdn.microsoft.com/library/994a9d2b-1501-4804-90f0-12bd914496ec%28Office.15%29.aspx) <br/> |[PullSubscription.BeginUnsubscribe メソッド](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pullsubscription.beginunsubscribe%28v=exchg.80%29.aspx) <br/> [PullSubscription.EndUnsubscribe メソッド](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pullsubscription.endunsubscribe%28v=exchg.80%29.aspx) <br/> [PullSubscription.Unsubscribe メソッド](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pullsubscription.unsubscribe%28v=exchg.80%29.aspx) <br/> ||
|プッシュ  <br/> |**SendNotificationResponseMessage** の [StatusFrequency](https://msdn.microsoft.com/library/917474e2-a426-4166-b825-53783a41dad4%28Office.15%29.aspx) 要素で [Unsubscribe](https://msdn.microsoft.com/library/2c6d681b-67ac-4331-bc6b-a2e709b638e3%28Office.15%29.aspx) を返します <br/> |該当なし。代わりにサブスクリプションをタイムアウトさせることができます。  <br/> ||
   
または、各サブスクリプションをタイムアウトさせることができます。 
  
**表 5 サブスクリプションのタイムアウト**

|**サブスクリプションの種類**|**EWS でのタイムアウトの値**|**EWS マネージ API でのタイムアウトの値**|**タイムアウトの処理**|
|:-----|:-----|:-----|:-----|
|ストリーミング  <br/> |[ConnectionTimeout](https://msdn.microsoft.com/library/14da68a0-bcca-4281-a774-47644baa4ee9%28Office.15%29.aspx) 要素  <br/> | *StreamingSubscriptionConnection* コンストラクターの  [lifetime](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.streamingsubscriptionconnection.streamingsubscriptionconnection%28v=exchg.80%29.aspx)  パラメーター  <br/> |EWS マネージ API では、タイムアウト値が経過した後に、[OnDisconnect](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.streamingsubscriptionconnection.ondisconnect%28v=exchg.80%29.aspx) イベントが発生します。 [StreamingSubscriptionConnection.Open](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.streamingsubscriptionconnection.open%28v=exchg.80%29.aspx) メソッドが呼び出されないと、接続は終了します。  <br/> EWS では、タイムアウト値が経過した後に、[GetUserConfigurationResponse](https://msdn.microsoft.com/library/5e418c91-c836-4de0-a80d-f0dad0c684d7%28Office.15%29.aspx) メッセージが Closed の [ConnectionStatus](https://msdn.microsoft.com/library/4300f9d6-8bf9-48c2-9f07-d80197864e17%28Office.15%29.aspx) 値を返します。  <br/> |
|プル  <br/> |[Timeout](https://msdn.microsoft.com/library/c2e1ca5a-6667-4f6f-aac4-89de33bddc54%28Office.15%29.aspx) 要素  <br/> | *SubscribeToPullNotification* メソッドの  [timeout](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx)  パラメーター  <br/> |タイムアウト値が経過した後、サーバーはサブスクリプションを削除します。  <br/> |
|プッシュ  <br/> |[StatusFrequency](https://msdn.microsoft.com/library/917474e2-a426-4166-b825-53783a41dad4%28Office.15%29.aspx) 要素  <br/> | *SubscribeToPushNotification* メソッドの  [frequency](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopushnotifications%28v=exchg.80%29.aspx)  パラメーター  <br/> |サーバーがプッシュ通知または状態の ping への応答を受信しない場合は、通知の送信を数回再試行してから、通知の送信を停止します。詳細については、「[StatusFrequency](https://msdn.microsoft.com/library/917474e2-a426-4166-b825-53783a41dad4%28Office.15%29.aspx)」をご覧ください。  <br/> |
   
## <a name="can-i-limit-subscriptions"></a>サブスクリプションの制限について
<a name="bk_limitsubs"> </a>

社内展開では、調整ポリシーの [EwsMaxSubscriptions 調整パラメーター](ews-throttling-in-exchange.md)を使用して、ユーザーごとのサブスクリプションの数を制限することができます。このポリシーは、すべてのユーザー、または特定のユーザーに適用できます。 **EwsMaxSubscriptions** 調整ポリシーは、Exchange Online では構成できません。 
  
## <a name="in-this-section"></a>このセクションの内容
<a name="bk_limitsubs"> </a>

- [Exchange での EWS を使用したメールボックス イベントに関するストリーム通知](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md)
    
- [Exchange での EWS を使用したメールボックス イベントに関するプル通知](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md)
    
- [Exchange の購読グループとメールボックス サーバー間のアフィニティを維持する](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md)
    
- [Exchange における EWS での通知関連エラーの処理](handling-notification-related-errors-in-ews-in-exchange.md)
    
## <a name="see-also"></a>関連項目

- [Exchange 用の Web サービス クライアントの開発](develop-web-service-clients-for-exchange.md)
- [Exchange web サービスの参照](../web-service-reference/web-services-reference-for-exchange.md)
- [Exchange で Web サービスの使用を開始する](start-using-web-services-in-exchange.md)
- [Exchange のメールボックス同期と EWS](mailbox-synchronization-and-ews-in-exchange.md)
- [プッシュ通知のサンプル アプリケーション](https://msdn.microsoft.com/library/db1f8523-fa44-483f-bdb6-ab5939b52eee%28Office.15%29.aspx)
    

