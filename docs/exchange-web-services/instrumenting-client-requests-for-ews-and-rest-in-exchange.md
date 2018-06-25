---
title: Exchange で EWS と REST のクライアントの要求をインストルメント化する
manager: sethgros
ms.date: 4/13/2016
ms.audience: Developer
localization_priority: Normal
ms.assetid: 330de503-498d-447e-b4a9-c20fc1699fd1
description: Exchange アプリケーションのモニターとトラブルシューティングに役立つ EWS と REST の要求と応答の HTTP ヘッダーについて説明します。
ms.openlocfilehash: bcf362952c29956729c44397043a56bf3603d0af
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759084"
---
# <a name="instrumenting-client-requests-for-ews-and-rest-in-exchange"></a>Exchange で EWS と REST のクライアントの要求をインストルメント化する

Exchange アプリケーションのモニターとトラブルシューティングに役立つ EWS と REST の要求と応答の HTTP ヘッダーについて説明します。
  
これまで起こったするでしょうか。 アプリケーションのユーザーは、予期しないエラーを報告します。 調査をするが、それを再現することはできません。 エラーがユーザーに表示されなくなったし、して残っているはほとんどの実用的なデータです。 フラストレーション、だと思いませんか。 このシナリオで事前に準備し、うまくいけば不満、将来的にしないようにする方法を見てみましょう。
  
## <a name="add-instrumentation-to-requests"></a>要求にインストルメンテーションを追加する

トラブルシューティングを容易にするために、要求に HTTP ヘッダーを追加することをお勧めします。後で必要になったら取得できるように、この情報をどこかに (ログ ファイルなど) 記録しておいてください。これは、ネットワーク トラフィックを調べるときに役立ちますが、Microsoft サポートに連絡して支援を求めるときにも役立ちます。
  
**表 1 です。トラブルシューティングのための要求ヘッダー**

|**HTTP ヘッダー (EWS)**|**EWS のマネージ API と同じ**|**メモ**|
|:-----|:-----|:-----|
|User-Agent  <br/> |[ExchangeService.UserAgent](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.useragent%28v=exchg.80%29.aspx) <br/> |クライアント アプリケーションを識別する一意の値を設定します。<br/><br/> 呼び出しの失敗のトラブルシューティングに役立つ、マイクロソフトでは、アプリケーションが送信するすべての要求に対して同じ値を使用して、必要がある問題が発生します。  <br/> |
|client-request-id  <br/> |[ExchangeService.ClientRequestId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.clientrequestid%28v=exchg.80%29.aspx) <br/> |これをアプリケーションに送信する要求ごとに異なる固有の値に設定します。<br/><br/> GUID を使用することをお勧めします。 この一意の識別子は、問題が生じたことは、2 つのシステム間での活動を関連付けるために使用します。  <br/> |
|return-client-request-id  <br/> |[ExchangeService.ReturnClientRequestId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.returnclientrequestid%28v=exchg.80%29.aspx) <br/> |設定を**true**に対応する応答にクライアントの要求の id の値を返す必要があることを Exchange サーバーに通知します。<br/><br/> ネットワーク トレースまたは EWS マネージ API トレースにおける要求と応答を関連付けるためには、これを使用します。  <br/> |
|X-ClientStatistics  <br/> |[ExchangeService.SendClientLatencies](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.sendclientlatencies%28v=exchg.80%29.aspx) <br/> |アプリケーションが Office 365 の一部として Exchange Online または Exchange Online をアクセスする場合は、マイクロソフトに[レポートの EWS の待ち時間](#bk_ReportLatency)を使用します。  <br/> |
   
## <a name="log-information-from-responses"></a>応答からのログ情報

クライアントが送信する要求にインストルメンテーションを追加できるのと同様、Exchange も HTTP ヘッダーの形式でインストルメンテーションを応答に追加します。クライアントはこの情報を要求のインストルメンテーションの情報とともにキャプチャする必要があります。
  
> [!NOTE]
> EWS のマネージ API を使用する場合、HTTP ヘッダーに直接相当するものはありません。 ただし、すべての HTTP 応答ヘッダーは、 [ExchangeService.HttpResponseHeaders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.httpresponseheaders%28v=exchg.80%29.aspx)プロパティを通じてアクセスできます。 
  
**表 2 になります。HTTP 応答ヘッダー**

|**HTTP ヘッダー**|**説明**|
|:-----|:-----|
|request-id  <br/> |この応答に対応する要求を表す、サーバーによって生成される ID。  <br/> |
|client-request-id  <br/> |要求でクライアントの要求の id のヘッダーの値。<br/><br/> このヘッダーは、要求には、 **true**の値を返すクライアント要求 id ヘッダーが含まれている場合のみです。  <br/> |
|X-FEServer  <br/> |要求を処理したクライアント アクセス サーバーの FQDN。  <br/> |
|X-TargetBEServer  <br/> |要求を処理したメールボックス サーバーの FQDN。  <br/> |
|X-DiagInfo  <br/> |要求に応じた追加の診断情報。  <br/> |
|x-ms-diagnostics  <br/> | このヘッダーは、OAuth 認証が要求に使用します。<br/><br/> OAuth 認証が失敗した理由を指定する明示的なエラー コードが含まれています。<br/><br/> 次の形式がかかります。`errorId;reason="reason"error_type="error type"`<br/><br/> **[理由**] フィールドは、人間が判読できる、エラーの説明です。<br/><br/> **ErrorId**フィールドは、整数、および、**エラー\_型**フィールドは、整数の文字列形式を次のように。<ul><li>2000000: 無効な\_署名</li><li>2000001: 無効な\_トークン</li><li>  2000002: トークン\_有効期限が切れて</li><li>2000003: 無効な\_リソース</li><li>2000004: 無効な\_テナント  </li><li>2000005: 無効な\_ユーザー</li><li>2000006: 無効な\_クライアント</li><li>2000007: 内部\_エラー</li><li>2000008: 無効な\_を与える</li></ul> |
   
## <a name="report-ews-latency-to-microsoft"></a>Microsoft への EWS の待機時間の報告
<a name="bk_ReportLatency"> </a>

アプリケーションは、Exchange Online に接続するのには、EWS のマネージ API または EWS を使用する場合は、マイクロソフトに直接 EWS 要求の待機時間を報告できます。 X ClientStatistics 要求ヘッダーを使用して、情報が渡されます。 EWS のマネージ API を使用する場合は、 [ExchangeService.SendClientLatencies](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.sendclientlatencies%28v=exchg.80%29.aspx)プロパティを**true**に設定を実行する必要があるすべてが。 EWS を使用する場合は、要求を発行し、応答を受け取るまでの時間を測定し、次の EWS 要求を次の形式を使用して、アプリケーションを送信する X ClientStatistics ヘッダーを追加する必要があります。
  
`X-ClientStatistics: MessageId=<value of request-id header>,ResponseTime=<time in milliseconds>,SoapAction=<EWS operation>`
  
Microsoft はこれらの待機時間の報告を保存し、Exchange Online の EWS のサービスを継続的に改善するために使用します。
  
## <a name="next-steps"></a>次の手順
<a name="bk_ReportLatency"> </a>

クライアントの実装をアプリケーションに追加した後より準備ができました問題が生じた場合。 そのような場合は、インストルメンテーション データを[アプリケーションのトラブルシューティング](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md)を使用できます。
  
## <a name="see-also"></a>関連項目

- [Exchange の EWS クライアントの設計の概要](ews-client-design-overview-for-exchange.md)
- [EWS のマネージ API アプリケーションのトラブルシューティングを行うには、要求と応答をトレースします。](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md)
- [Exchange の EWS アプリケーションのトラブルシューティングに使用するツールとリソース](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md)
    

