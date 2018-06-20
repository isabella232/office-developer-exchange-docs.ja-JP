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
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19758897"
---
# <a name="handling-notification-related-errors-in-ews-in-exchange"></a>Exchange における EWS での通知関連エラーの処理

Exchange の EWS マネージ API または EWS を使用して、開発したアプリケーションの通知に関連するエラーを処理する方法を確認します。
  
アプリケーションが通知をサブスクライブして取得する場合、通知に関連するエラーを処理する必要があります。これらのエラーは実行時、または EWS アプリケーションを開発するときに処理することができます。
  
**表 1 です。通知に関連するエラーと、それらを処理する方法**

|エラー|発生するタイミング|処理方法|
|:-----|:-----|:-----|
|**ErrorExceededConnectionCount** |アカウントがストリーミング接続の接続制限に達したときに、接続を開いてイベントを取得する場合。 | <ul><li>接続を[開く](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md#bk_throttling)には、[偽装](http://technet.microsoft.com/en-us/library/dd776119%28v=exchg.150%29.aspx)を使用します。</li><li>接続数を使用して、イベントを取得します。 [アフィニティを使用して](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md)、[最大 200 のサブスクリプション Id が同じグループ内で配置すること](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md#bk_howdoimaintain)によって、各接続でのサブスクリプションの数を最大化します。 必要な接続の数を減らし、グループ全体のイベントを取得するのには、同じ接続を使用できます。</li><li>  オンプレミスの Exchange の web.config ファイルで HangingConnectionLimit の値を変更し、3 つの開いている接続の既定値をオーバーライドする。Exchange Online には、10 の既定の HangingConnectionLimit があり、これを構成することはできません。</li></ul> |
|**ErrorExceededSubscriptionCount** |多数のサブスクリプションを作成します。 [EwsMaxSubscriptions](http://msdn.microsoft.com/en-us/library/microsoft.exchange.data.directory.systemconfiguration.throttlingpolicy.ewsmaxsubscriptions%28v=exchg.150%29.aspx)のポリシー パラメーターの調整では、アカウントが作成できるサブスクリプションの最大数を決定します。 | <ul><li>[サブスクリプションを作成](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md#bk_throttling)するのには、[偽装](http://technet.microsoft.com/en-us/library/dd776119%28v=exchg.150%29.aspx)を使用します。</li><li>サブスクリプションの数を削減する。</li></ul> |
|**ErrorInvalidSubscriptionRequest** |1 つの要求から複数のメールボックスまたは複数のフォルダーに対してサブスクリプションを作成する場合。  |1 つの要求で 1 つのパブリック フォルダーまたは 1 つのメールボックスに対してサブスクリプションを作成する。| 
|**ErrorInvalidWatermark** |無効な基準値を使用してイベントを取得する場合。| <ul><li>前の応答で返されたサブスクリプション ID を確認する。</li><li>適切な**ExchangeService**オブジェクトのサブスクリプション ID を送信することを確認します。</li><li>[新しいサブスクリプションを作成](handling-notification-related-errors-in-ews-in-exchange.md#bk_recover)しています。</li></ul> |
|**ErrorMissedNotificationEvents** |以前のイベントがないイベントを取得する場合。    |拡張フォルダー プロパティがどのような変更を確認するには、 **PR_LOCAL_COMMIT_TIME_MAX** (0x670a) と**PR_DELETED_COUNT_TOTAL** (0x670b) が失敗した、および[新しいサブスクリプションを作成する](handling-notification-related-errors-in-ews-in-exchange.md#bk_recover)と比較します。  |
|**ErrorProxyRequestNotAllowed** |メールボックスが別のサイトに移動しているユーザーに対して、バッチ要求でイベントをサブスクライブする場合。   |[自動検出](autodiscover-for-exchange.md)を使用して、ExternalEwsUrl または EwsPartnerUrl を再検出して、新しいサブスクリプションを作成します。  |
|**ErrorReadEventsFailed** |見つからないサブスクリプションからイベントを取得する場合。  |[自動検出](autodiscover-for-exchange.md)を使用して、ExternalEwsUrl または EwsPartnerUrl を再検出して、新しいサブスクリプションを作成します。  |
|**ErrorServerBusy** | [調整](ews-throttling-in-exchange.md#bk_ThrottlingNotifications)の制限を超えてください。 次に関する制限に注意します。<ul><li>[EwsMaxSubscriptions](http://msdn.microsoft.com/en-us/library/microsoft.exchange.data.directory.systemconfiguration.throttlingpolicy.ewsmaxsubscriptions%28v=exchg.150%29.aspx)の制限の調整は、プッシュ、プル、または、一度にアクティブにできる通知サブスクリプションのストリームの最大数を指定します。 これは、メールボックスのサブスクリプション、サブスクリプションのメールボックスの個別のフォルダーのサブスクリプションの数の値です。 サービス メールボックスのバージョン 14.16.0135 および 14.15.0057.000 以降では、Office 365 の一部として、Exchange のオンラインまたは Exchange のオンラインでホストされているメールボックスは最大 20 個のサブスクリプションを持つことができ、対象の Exchange 2013 のオンプレミスのメールボックスは、最大 5,000 のサブスクリプションを持つことができます。</li><li>調整制限の[EwsMaxConcurrency](http://msdn.microsoft.com/en-us/library/microsoft.exchange.data.directory.systemconfiguration.throttlingpolicy.ewsmaxconcurrency%28v=exchg.150%29.aspx)は、非ストリーミング接続のアクティブな要求の最大数を識別し、27 の既定値を持ちます。</li><li>開いているストリーミング接続の既定の制限値は 10 です。</li></ul> |<ul><li>[通知に関連する調整ポリシーの影響を考慮すると](ews-throttling-in-exchange.md#bk_ThrottlingNotifications)アクティブなサブスクリプションとアクティブな接続の数を制限するため、アプリケーションが制限されていません。</li><li>接続数を使用して、イベントを取得します。 [最大 200 のサブスクリプション Id が同じグループ内で配置すること](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md)によって、各接続でのサブスクリプションの数を最大化します。 必要な接続の数を減らし、グループ全体のイベントを取得するのには、同じ接続を使用できます。</li><li>web.config ファイルの HangingConnectionLimit の値を変更し、開くことができるストリーミング接続の既定値 10 をオーバーライドする。</li></ul>|
|**ErrorSubscriptionNotFound** |見つからないサブスクリプションのイベントを取得する場合。サブスクリプションの期限が切れているか、EWS のプロセスが再起動されている可能性があります。または無効なサブスクリプションが渡されました。 | <ul><li>前の応答で返された同じサブスクリプション ID を使用していることを確認します。</li><li>適切な**ExchangeService**オブジェクトのサブスクリプション ID を送信することを確認します。</li><li> [新しいサブスクリプションを作成](handling-notification-related-errors-in-ews-in-exchange.md#bk_recover)しています。</li></ul> |
|**[ServiceLocalException](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponseexception%28v=exchg.80%29.aspx)** |サブスクリプションの接続が別のフォルダーで開いている間に、新しいフォルダーにサブスクリプションを追加します。  |サブスクリプションを変更して、特定のフォルダーではなく、メールボックス内のすべてのフォルダーをサブスクライブする。  |
|**[ServiceResponseException](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponseexception%28v=exchg.80%29.aspx)** |Exchange ストア内にないサブスクリプションのイベントを取得する場合。  | <ul><li>前の応答で返された同じサブスクリプション ID を使用していることを確認します。</li><li>適切な**ExchangeService**オブジェクトのサブスクリプション ID を送信することを確認します。</li></ul> |
   
## <a name="recovering-from-lost-subscriptions"></a>失われたサブスクリプションから回復する。
<a name="bk_recover"> </a>

サブスクリプションまたは失われると、アクセスが不要になった、新しいサブスクリプションを作成し、古い透かしは新しいサブスクリプションに含まことをお勧めします。 古いウォーターマークを使用してサブスクライブすると、イベントを線形にスキャンはコストがかかる。 代わりに、新しいサブスクリプションを作成し、コンテンツを変更するためにフォルダーのプロパティを比較する失われたサブスクリプションとサブスクリプションの新規の間に発生します。 拡張フォルダー プロパティを確認することをお勧めする**PR_LOCAL_COMMIT_TIME_MAX** (0x670a0040)、 **PR_DELETED_COUNT_TOTAL** (0x670b0003) です。 [拡張プロパティの定義を作成すること](properties-and-extended-properties-in-ews-in-exchange.md)によってこれを行うことができます。
  
## <a name="see-also"></a>関連項目

- [Notification subscriptions, mailbox events, and EWS in Exchange](notification-subscriptions-mailbox-events-and-ews-in-exchange.md)
- [Exchange の EWS を使用してメールボックスのイベントに関する通知をストリーム](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md)    
- [EWS を使用して Exchange でメールボックスのイベントに関する通知をプルします。](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md)    
- [Exchange の購読グループとメールボックス サーバー間のアフィニティを維持します。](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md)
    

