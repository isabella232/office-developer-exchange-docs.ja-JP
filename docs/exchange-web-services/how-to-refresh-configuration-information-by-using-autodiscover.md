---
title: 自動検出を使用して構成情報を更新します。
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: c2f3c6a5-e8ea-4375-b41a-686a6f238d33
description: 自動検出を使用して、Exchange 接続の構成情報をいつまたどのように更新するかについて説明します。
ms.openlocfilehash: ef3b61781cbafa6e7b873336a050c0b8c33a28ec
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759070"
---
# <a name="refresh-configuration-information-by-using-autodiscover"></a>自動検出を使用して構成情報を更新します。

自動検出を使用して、Exchange 接続の構成情報をいつまたどのように更新するかについて説明します。
  
EWS アプリケーションを初めて実行するとき、自動検出は、ユーザーの Exchange メールボックスに接続するために必要な情報を収集する優れた方法です。しかし、自動検出は初めての使用だけに適しているわけではありません。定期的に自動検出を使用することで、アプリケーションを Exchange 展開の変化に対応させ、接続状態を保持することができます。
  
## <a name="cache-autodiscover-endpoint-and-ews-settings"></a>自動検出エンドポイントおよび EWS 設定のキャッシュ
<a name="bk_CacheSettings"> </a>

自動検出を定期的に使用することをお勧めしますが、これを行うには考慮すべき事項があります。環境の変化に対する迅速な対応と、数多く生成される不要なネットワーク トラフィックとのバランスをとるのが理想的です。アプリケーションが初めて自動検出応答に成功した場合、EWS 要求を送信するたびに自動検出プロセスを繰り返さなくてもいいように、次の情報を保存してください。
  
**表 1 です。自動検出要求をキャッシュするための情報**

|**キャッシュを設定します。**|**に対して無効です。**|**詳細情報**|
|:-----|:-----|:-----|
|自動検出エンドポイント  <br/> |動作中  <br/> |正常な応答が返されますが、自動検出エンドポイントを保存すると、[自動検出エンドポイントの一覧を生成して](how-to-generate-a-list-of-autodiscover-endpoints.md)、正常な応答を取得するまでにしようとしてのプロセスを繰り返す必要はありません。<br/><br/> **注**:「EWS のマネージ API が自動検出エンドポイント キャッシュをサポートしていますいません。           |
|EWS URL および自動検出応答から取得したその他の設定  <br/> |24 時間  <br/> |EWS の URL とその他を保存することによって関連の EWS 要求ごとに[新しい自動検出要求の送信](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)をする必要がないか、アプリケーションが再起動するかどうかの設定をします。 ただし、EWS の URL は、ユーザーの動作する場合でもサーバーがあることがより最適です。<br/><br/> など、ユーザーのメールボックスは、EWS 端点を優先に、新しいメールボックス サーバーに移動しました可能性があります。 最後の自動検出の要求から 24 時間経過後、新しい自動検出要求を送信することによって、ユーザーの設定を更新することをお勧めします。 この時間は、アプリケーションの要件を満たすように調整できます。  <br/> |
   
## <a name="refresh-cached-configuration-information"></a>キャッシュされた構成情報を更新する
<a name="bk_RefreshConfig"> </a>

情報をキャッシュしたので、今度はそのキャッシュを最新の状態に保つ方法について調べてみましょう。次の場合に、キャッシュされた情報を更新することをお勧めします。
  
- 情報の有効期間の期限が切れている場合。
    
- の[接続に関連するエラー](#bk_ConnectionErrors)が発生します。 
    
キャッシュされた情報を更新するには、キャッシュされた自動検出エンドポイントに自動検出要求を送信し、次の操作を行います。
  
- 要求が成功したら、応答の EWS エンドポイントとキャッシュされた EWS エンドポイントを比較し、次の操作を行います。
    
  - 2 つのエンドポイントが異なる場合は、新しい EWS エンドポイントを使用します。エラーから回復するために更新する場合は、新しいエンドポイントを使用して失敗した要求を再試行してください。
    
  - 2 つのエンドポイントが同じ場合は、元の EWS エンドポイントを引き続き使用します。エラーから回復するために更新する場合は、必要に応じてエラーを処理します。
    
- 要求が失敗した場合、[自動検出プロセス](autodiscover-for-exchange.md)を最初から開始します。 正常な応答を取得した後は、自動検出エンドポイントが成功し、新しい EWS エンドポイントを使用する続行すると自動検出エンドポイントのキャッシュを交換してください。 正常な応答が得られなかった場合は、引き続き元の自動検出エンドポイントとエンドポイントの EWS を使用します。 エラーから回復するのには更新する場合は、必要に応じてエラーを処理します。 
    
次の図は、このプロセスを視覚的に表したものです。
  
**図 1 です。自動検出を使用して構成情報を更新するためのプロセス**

![模式図は自動検出が構成情報を更新する方法を示しています。](media/Ex15_Autodiscover_Refresh_Flowchart.png)
  
### <a name="connection-related-errors"></a>接続に関連するエラー
<a name="bk_ConnectionErrors"> </a>

キャッシュされた構成情報を更新すると、すべてではありませんが、一部のエラーを解決することができます。  
  
**表 2 になります。エラーが、キャッシュを更新することで解決**

|**Error**|**EWS のマネージ API の実装**|**メモ**|
|:-----|:-----|:-----|
|DNS またはネットワークのエラー<br/><br/> 例: ホスト名が見つかりませんでした。  <br/> |[ServiceRemoteException](https://msdn.microsoft.com/library/Microsoft.Exchange.WebServices.Data.ServiceRemoteException.aspx) <br/> |自動検出を試みることによって、サーバーが見つかりませんでしたか、到達できませんでしたを示す、エラーを解決する可能性があります。 <br/><br/> EWS エンドポイントのキャッシュが有効な場合は、不要になった場合があり、自動検出できる新しいサーバーをポイントすることがあります。  <br/> |
|HTTP 状態のエラー<br/><br/> 例: 503 サービスを利用できません。  <br/> |[ServiceRemoteException](https://msdn.microsoft.com/library/Microsoft.Exchange.WebServices.Data.ServiceRemoteException.aspx) <br/> |HTTP ステータス エラーは、さまざまな理由で発生します。<br/><br/> ただしは、新しい EWS エンドポイントが、ユーザーが利用できるかどうかを自動検出を実行することをお勧めです。  <br/> |
|EWS エラー コード <br/><br/> 例: ErrorConnectionFailed <br/> |[ResponseCodeType](https://msdn.microsoft.com/library/Microsoft.Exchange.WebServices.Data.ResponseCodeType.aspx) <br/> | EWS エラー コードのほとんどは保証するもので、構成情報を更新します。<br/><br/> ただし、次を具体的に指定の構成情報を更新する必要があること。<br/>- **ErrorConnectionFailed** <br/>- **ErrorMailboxMoveInProgress** <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange の自動検出](autodiscover-for-exchange.md)  
- [自動検出エンドポイントの一覧を生成します。](how-to-generate-a-list-of-autodiscover-endpoints.md)   
- [Exchange から自動検出を使用してユーザー設定を取得します。](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
    

