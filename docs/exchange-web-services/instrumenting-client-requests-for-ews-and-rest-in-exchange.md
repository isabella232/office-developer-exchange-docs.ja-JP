---
title: Exchange で EWS と REST のクライアントの要求をインストルメント化する
manager: sethgros
ms.date: 4/13/2016
ms.audience: Developer
localization_priority: Normal
ms.assetid: 330de503-498d-447e-b4a9-c20fc1699fd1
description: Exchange アプリケーションのモニターとトラブルシューティングに役立つ EWS と REST の要求と応答の HTTP ヘッダーについて説明します。
ms.openlocfilehash: 3a8ce889ec7a6b9e70ec25a95ac248902f48ca6c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456305"
---
# <a name="instrumenting-client-requests-for-ews-and-rest-in-exchange"></a>Exchange で EWS と REST のクライアントの要求をインストルメント化する

Exchange アプリケーションのモニターとトラブルシューティングに役立つ EWS と REST の要求と応答の HTTP ヘッダーについて説明します。
  
次のような経験があるかもしれません。 アプリケーションのユーザーが予期しないエラーを報告します。 調査しようとしましたが、再現できません。 エラーがユーザーに現れなくなり、役に立つデータはほとんどありません。 これはストレスのたまる状況です。 このようなシナリオに対して事前に準備し、今後のストレス回避に役立つ可能性のある方法を説明します。
  
## <a name="add-instrumentation-to-requests"></a>要求にインストルメンテーションを追加する

トラブルシューティングを容易にするために、要求に HTTP ヘッダーを追加することをお勧めします。後で必要になったら取得できるように、この情報をどこかに (ログ ファイルなど) 記録しておいてください。これは、ネットワーク トラフィックを調べるときに役立ちますが、Microsoft サポートに連絡して支援を求めるときにも役立ちます。
  
**表 1. トラブルシューティングのための要求ヘッダー**

|**HTTP ヘッダー (EWS)**|**EWS マネージ API の同等物**|**メモ**|
|:-----|:-----|:-----|
|User-Agent  <br/> |[ExchangeService.UserAgent](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.useragent%28v=exchg.80%29.aspx) <br/> |クライアント アプリケーションを識別する一意の値に設定します。<br/><br/> アプリケーションが送信するすべての要求に同じ値を使用すると、呼び出しの失敗が発生した場合に、Microsoft がトラブルシューティングを行うのに役立ちます。  <br/> |
|client-request-id  <br/> |[ExchangeService.ClientRequestId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.clientrequestid%28v=exchg.80%29.aspx) <br/> |アプリケーションが送信する要求ごとに異なる一意の値に設定します。<br/><br/> GUID を使用することをお勧めします。 この一意の識別子は、問題が発生した場合に 2 つのシステムの間でアクティビティを関連付けるために使用されます。  <br/> |
|return-client-request-id  <br/> |[ExchangeService.ReturnClientRequestId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.returnclientrequestid%28v=exchg.80%29.aspx) <br/> |**true** に設定することで、対応する応答で client-request-id の値を返す必要があることを Exchange サーバーに通知します。<br/><br/> これを使用して、ネットワーク トレースまたは EWS マネージ API のトレースで要求と応答を関連付けることができます。  <br/> |
|X-ClientStatistics  <br/> |[ExchangeService.SendClientLatencies](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.sendclientlatencies%28v=exchg.80%29.aspx) <br/> |アプリケーションが Exchange Online または Office 365 の一部としての Exchange Online にアクセスしている場合に、Microsoft に [EWS の待機時間を報告](#bk_ReportLatency)するために使用されます。  <br/> |
   
## <a name="log-information-from-responses"></a>応答からのログ情報

クライアントが送信する要求にインストルメンテーションを追加できるのと同様、Exchange も HTTP ヘッダーの形式でインストルメンテーションを応答に追加します。クライアントはこの情報を要求のインストルメンテーションの情報とともにキャプチャする必要があります。
  
> [!NOTE]
> EWS マネージ API を使用している場合、HTTP ヘッダーに直接相当するものはありません。 しかし、すべての HTTP 応答ヘッダーに、[ExchangeService.HttpResponseHeaders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.httpresponseheaders%28v=exchg.80%29.aspx) プロパティ経由でアクセスできます。 
  
**表 2. HTTP 応答ヘッダー**

|**HTTP ヘッダー**|**説明**|
|:-----|:-----|
|request-id  <br/> |この応答に対応する要求を表す、サーバーによって生成される ID。  <br/> |
|client-request-id  <br/> |要求の client-request-id ヘッダーの値。<br/><br/> このヘッダーは、要求に **true** の値を持つ return-client-request-id ヘッダーが含まれる場合にのみ存在します。  <br/> |
|X-FEServer  <br/> |要求を処理したクライアント アクセス サーバーの FQDN。  <br/> |
|X-TargetBEServer  <br/> |要求を処理したメールボックス サーバーの FQDN。  <br/> |
|X-DiagInfo  <br/> |要求に応じた追加の診断情報。  <br/> |
|x-ms-diagnostics  <br/> | このヘッダーは、要求で OAuth 認証が使用される場合にのみ適用されます。<br/><br/> これには、OAuth 認証が失敗した理由を指定する明示的なエラー コードが含まれます。<br/><br/> 次の形式を使用します。`errorId;reason="reason"error_type="error type"`<br/><br/> **reason** フィールドは、人間が理解しやすい形式でエラーを説明したものです。<br/><br/> **errorId** フィールドは整数、**error\_type** フィールドは整数の文字列表現であり、次のようになります。<ul><li>2000000: invalid\_signature</li><li>2000001: invalid\_token</li><li>  2000002: token\_expired</li><li>2000003: invalid\_resource</li><li>2000004: invalid\_tenant  </li><li>2000005: invalid\_user</li><li>2000006: invalid\_client</li><li>2000007: internal\_error</li><li>2000008: invalid\_grant</li></ul> |
   
## <a name="report-ews-latency-to-microsoft"></a>Microsoft への EWS の待機時間の報告
<a name="bk_ReportLatency"> </a>

アプリケーションが EWS マネージ API または EWS を使用して Exchange Online に接続する場合に、EWS 要求の要求の待機時間を Microsoft に直接報告できます。 情報は、X-ClientStatistics 要求ヘッダーを使用して渡されます。 EWS マネージ API を使用する場合、必要なのは [ExchangeService.SendClientLatencies](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.sendclientlatencies%28v=exchg.80%29.aspx) プロパティを **true** に設定することだけです。 EWS を使用する場合は、要求を発行してから応答を受け取るまでの時間を測定し、アプリケーションが送信するその次の EWS 要求に X-ClientStatistics ヘッダーを追加する必要があります。使用する形式は次のとおりです。
  
`X-ClientStatistics: MessageId=<value of request-id header>,ResponseTime=<time in milliseconds>,SoapAction=<EWS operation>`
  
Microsoft はこれらの待機時間の報告を保存し、Exchange Online の EWS のサービスを継続的に改善するために使用します。
  
## <a name="next-steps"></a>次の手順
<a name="bk_ReportLatency"> </a>

クライアントのインストルメンテーションをアプリケーションに追加したので、問題が発生した場合の準備がより一層整いました。 問題が発生した場合は、インストルメンテーション データを使用して[アプリケーションのトラブルシューティング](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md)を行うことができます。
  
## <a name="see-also"></a>関連項目

- [Exchange の EWS クライアントの設計の概要](ews-client-design-overview-for-exchange.md)
- [「EWS のマネージ API アプリケーションのトラブルシューティングを行うには、要求と応答をトレースします。」](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md)
- [Exchange の EWS アプリケーションのトラブルシューティングに使用するツールとリソース](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md)
    

