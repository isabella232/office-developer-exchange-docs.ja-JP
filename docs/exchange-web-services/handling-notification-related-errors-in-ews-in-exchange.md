---
title: Exchange における EWS での通知関連エラーの処理
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 519e1e52-5f1f-4f06-931e-8c20a586a563
description: Exchange の EWS マネージ API または EWS を使用して、開発したアプリケーションの通知に関連するエラーを処理する方法を確認します。
ms.openlocfilehash: cb0c16a74e68b5a16ef0f2011f65b22675950f58
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758897"
---
# <a name="handling-notification-related-errors-in-ews-in-exchange"></a>Exchange における EWS での通知関連エラーの処理

Exchange の EWS マネージ API または EWS を使用して、開発したアプリケーションの通知に関連するエラーを処理する方法を確認します。
  
アプリケーションが通知をサブスクライブして取得する場合、通知に関連するエラーを処理する必要があります。これらのエラーは実行時、または EWS アプリケーションを開発するときに処理することができます。
  
**表 1. 通知に関連するエラーとその処理方法**

|エラー|発生するタイミング|処理方法|
|:-----|:-----|:-----|
|**ErrorExceededConnectionCount** |アカウントがストリーミング接続の接続制限に達したときに、接続を開いてイベントを取得する場合。 | <ul><li>[偽装](http://technet.microsoft.com/ja-JP/library/dd776119%28v=exchg.150%29.aspx)を使用して、[接続を開く](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md#bk_throttling)。</li><li>より少ない接続を使用してイベントを取得する。 [アフィニティを使用](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md)して、[同じグループに最大 200 のサブスクリプション ID を配置](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md#bk_howdoimaintain)することで、各接続のサブスクリプション数を最大にします。 これで、同じ接続を使用して、グループ全体のイベントを取得し、必要な接続の数を削減することができるようになります。</li><li>  オンプレミスの Exchange の web.config ファイルで HangingConnectionLimit の値を変更し、3 つの開いている接続の既定値をオーバーライドする。Exchange Online には、10 の既定の HangingConnectionLimit があり、これを構成することはできません。</li></ul> |
|**ErrorExceededSubscriptionCount** |作成するサブスクリプションが多すぎる場合。 [EwsMaxSubscriptions](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.data.directory.systemconfiguration.throttlingpolicy.ewsmaxsubscriptions%28v=exchg.150%29.aspx) 調整ポリシー パラメーターが、アカウントで作成できるサブスクリプションの最大数を決定します。 | <ul><li>[偽装](http://technet.microsoft.com/ja-JP/library/dd776119%28v=exchg.150%29.aspx)を使用して、[サブスクリプションを作成する](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md#bk_throttling)。</li><li>サブスクリプションの数を削減する。</li></ul> |
|**ErrorInvalidSubscriptionRequest** |1 つの要求から複数のメールボックスまたは複数のフォルダーに対してサブスクリプションを作成する場合。  |1 つの要求で 1 つのパブリック フォルダーまたは 1 つのメールボックスに対してサブスクリプションを作成する。| 
|**ErrorInvalidWatermark** |無効な基準値を使用してイベントを取得する場合。| <ul><li>前の応答で返されたサブスクリプション ID を確認する。</li><li>正しい **ExchangeService** オブジェクトのサブスクリプション ID を送信していることを確認する。</li><li>[新しいサブスクリプションを作成する](handling-notification-related-errors-in-ews-in-exchange.md#bk_recover)。</li></ul> |
|**ErrorMissedNotificationEvents** |以前のイベントがないイベントを取得する場合。   |拡張フォルダーのプロパティ **PR_LOCAL_COMMIT_TIME_MAX** (0x670a) と **PR_DELETED_COUNT_TOTAL** (0x670b) を比較し、どの変更がないのかを特定し、[新しいサブスクリプションを作成する](handling-notification-related-errors-in-ews-in-exchange.md#bk_recover)。  |
|**ErrorProxyRequestNotAllowed** |メールボックスが別のサイトに移動しているユーザーに対して、バッチ要求でイベントをサブスクライブする場合。   |[自動検出](autodiscover-for-exchange.md)を使用して、ExternalEwsUrl または EwsPartnerUrl を再検出し、新しいサブスクリプションを作成する。  |
|**ErrorReadEventsFailed** |見つからないサブスクリプションからイベントを取得する場合。  |[自動検出](autodiscover-for-exchange.md)を使用して、ExternalEwsUrl または EwsPartnerUrl を再検出し、新しいサブスクリプションを作成する。  |
|**ErrorServerBusy** | [調整](ews-throttling-in-exchange.md#bk_ThrottlingNotifications)制限を超過した場合。 調整に関する次の点に注意してください。<ul><li>[EwsMaxSubscriptions](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.data.directory.systemconfiguration.throttlingpolicy.ewsmaxsubscriptions%28v=exchg.150%29.aspx) 調整制限により、一度にアクティブにできるプッシュ、プル、またはストリーミングの通知サブスクリプションの最大数が指定されます。 これはメールボックスのサブスクリプションの値です。メールボックス サブスクリプション内にある個々のフォルダーのサブスクリプション数ではありません。 サービス メールボックスのバージョン 14.16.0135 および 14.15.0057.000 以降では、Exchange Online または Office 365 の一部としての Exchange Online によってホストされるメールボックスは、最大 20 のサブスクリプション、対象になる Exchange 2013 のオンプレミスのメールボックスは最大 5,000 のサブスクリプションを持つことができます。</li><li>[EwsMaxConcurrency](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.data.directory.systemconfiguration.throttlingpolicy.ewsmaxconcurrency%28v=exchg.150%29.aspx) 調整制限により、非ストリーミング接続のアクティブな要求の最大数が指定されます。既定値は 27 です。</li><li>開いているストリーミング接続の既定の制限値は 10 です。</li></ul> |<ul><li>[通知に関連する調整ポリシーの影響を考慮し](ews-throttling-in-exchange.md#bk_ThrottlingNotifications)、アプリケーションが調整されないようにアクティブなサブスクリプションとアクティブな接続の数を制限する。</li><li>より少ない接続を使用してイベントを取得する。 [同じグループに最大 200 のサブスクリプション ID を配置](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md)することで、各接続のサブスクリプション数を最大にします。 これで、同じ接続を使用して、グループ全体のイベントを取得し、必要な接続の数を削減することができるようになります。</li><li>web.config ファイルの HangingConnectionLimit の値を変更し、開くことができるストリーミング接続の既定値 10 をオーバーライドする。</li></ul>|
|**ErrorSubscriptionNotFound** |見つからないサブスクリプションのイベントを取得する場合。サブスクリプションの期限が切れているか、EWS のプロセスが再起動されている可能性があります。または無効なサブスクリプションが渡されました。 | <ul><li>前の応答で返されたのと同じサブスクリプション ID を使用していることを確認する。</li><li>正しい **ExchangeService** オブジェクトのサブスクリプション ID を送信していることを確認する。</li><li> [新しいサブスクリプションを作成する](handling-notification-related-errors-in-ews-in-exchange.md#bk_recover)。</li></ul> |
|**[ServiceLocalException](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.serviceresponseexception%28v=exchg.80%29.aspx)** |サブスクリプションの接続が別のフォルダーで開いている間に、新しいフォルダーにサブスクリプションを追加します。  |サブスクリプションを変更して、特定のフォルダーではなく、メールボックス内のすべてのフォルダーをサブスクライブする。  |
|**[ServiceResponseException](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.serviceresponseexception%28v=exchg.80%29.aspx)** |Exchange ストア内にないサブスクリプションのイベントを取得する場合。  | <ul><li>前の応答で返されたのと同じサブスクリプション ID を使用していることを確認する。</li><li>正しい **ExchangeService** オブジェクトのサブスクリプション ID を送信していることを確認する。</li></ul> |
   
## <a name="recovering-from-lost-subscriptions"></a>失われたサブスクリプションから回復する
<a name="bk_recover"> </a>

サブスクリプションが失われる、またはアクセスできなくなった場合は、新しいサブスクリプションを作成し、新しいサブスクリプションに古い基準値を含めないことをお勧めします。 古い基準値を使用して再度サブスクライブすると、イベントが線形にスキャンされるためコストがかかります。 代わりに、新しいサブスクリプションを作成し、フォルダーのプロパティを比較して、失われたサブスクリプションと新しいサブスクリプションの間で発生したコンテンツ変更を検索します。 確認することをお勧めする拡張フォルダー プロパティは、**PR_LOCAL_COMMIT_TIME_MAX** (0x670a0040) と **PR_DELETED_COUNT_TOTAL** (0x670b0003) です。 これを行うには、[拡張プロパティの定義を作成します](properties-and-extended-properties-in-ews-in-exchange.md)。
  
## <a name="see-also"></a>関連項目

- [Exchange の通知サブスクリプション、メールボックス イベント、および EWS](notification-subscriptions-mailbox-events-and-ews-in-exchange.md)
- [Exchange で EWS を使用し、メールボックス イベントに関するストリーミング通知を行う](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md)    
- [Exchange で EWS を使用し、メールボックス イベントに関するプル通知を行う](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md)    
- [サブスクリプション グループと Exchange のメールボックス サーバー間のアフィニティを維持する](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md)
    

