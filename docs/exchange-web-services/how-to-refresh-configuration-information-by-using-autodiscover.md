---
title: 自動検出を使用して構成情報を更新する
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: c2f3c6a5-e8ea-4375-b41a-686a6f238d33
description: 自動検出を使用して、Exchange 接続の構成情報をいつまたどのように更新するかについて説明します。
ms.openlocfilehash: 764909fbe5e4cd62ba6e05bfa4b2c417ef41a9ae
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353057"
---
# <a name="refresh-configuration-information-by-using-autodiscover"></a>自動検出を使用して構成情報を更新する

自動検出を使用して、Exchange 接続の構成情報をいつまたどのように更新するかについて説明します。
  
EWS アプリケーションを初めて実行するとき、自動検出は、ユーザーの Exchange メールボックスに接続するために必要な情報を収集する優れた方法です。しかし、自動検出は初めての使用だけに適しているわけではありません。定期的に自動検出を使用することで、アプリケーションを Exchange 展開の変化に対応させ、接続状態を保持することができます。
  
## <a name="cache-autodiscover-endpoint-and-ews-settings"></a>自動検出エンドポイントおよび EWS 設定のキャッシュ
<a name="bk_CacheSettings"> </a>

自動検出を定期的に使用することをお勧めしますが、これを行うには考慮すべき事項があります。環境の変化に対する迅速な対応と、数多く生成される不要なネットワーク トラフィックとのバランスをとるのが理想的です。アプリケーションが初めて自動検出応答に成功した場合、EWS 要求を送信するたびに自動検出プロセスを繰り返さなくてもいいように、次の情報を保存してください。
  
**表 1. 自動検出要求に関してキャッシュする情報**

|**キャッシュする設定**|**有効期間**|**詳細**|
|:-----|:-----|:-----|
|自動検出エンドポイント  <br/> |動作中  <br/> |正常な応答が返された自動検出エンドポイントを保存すると、[自動検出エンドポイントの一覧を生成](how-to-generate-a-list-of-autodiscover-endpoints.md)して、正常な応答を取得するまで自動検出プロセスを繰り返す必要はありません。<br/><br/> **注**: EWS のマネージ API は、自動検出エンドポイントのキャッシュをサポートしていません。           |
|EWS URL および自動検出応答から取得したその他の設定  <br/> |24 時間  <br/> |EWS URL およびその他の関連設定を保存することによって、EWS 要求ごとに、またはアプリケーションを再起動するときに、[新しい自動検出要求を送信する](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)必要はありません。 ただし、EWS URL が動作するとしても、より最適なサーバーが使用可能な場合があります。<br/><br/> たとえば、ユーザーのメールボックスが新しいメールボックス サーバーに移動され、新しい優先 EWS エンドポイントが生成されるという場合です。 最後の自動検出要求から 24 時間後に新しい自動検出要求を送信して、ユーザーの設定を更新することをお勧めします。 この時間は、アプリケーションの要件を満たすように調整することができます。  <br/> |
   
## <a name="refresh-cached-configuration-information"></a>キャッシュされた構成情報を更新する
<a name="bk_RefreshConfig"> </a>

情報をキャッシュしたので、今度はそのキャッシュを最新の状態に保つ方法について調べてみましょう。次の場合に、キャッシュされた情報を更新することをお勧めします。
  
- 情報の有効期間の期限が切れている場合。
    
- [接続に関連するエラー](#bk_ConnectionErrors)が発生した場合。 
    
キャッシュされた情報を更新するには、キャッシュされた自動検出エンドポイントに自動検出要求を送信し、次の操作を行います。
  
- 要求が成功したら、応答の EWS エンドポイントとキャッシュされた EWS エンドポイントを比較し、次の操作を行います。
    
  - 2 つのエンドポイントが異なる場合は、新しい EWS エンドポイントを使用します。エラーから回復するために更新する場合は、新しいエンドポイントを使用して失敗した要求を再試行してください。
    
  - 2 つのエンドポイントが同じ場合は、元の EWS エンドポイントを引き続き使用します。エラーから回復するために更新する場合は、必要に応じてエラーを処理します。
    
- 要求が失敗した場合は、[自動検出プロセス](autodiscover-for-exchange.md)を最初から開始します。正常な応答を取得したら、キャッシュされた自動検出エンドポイントを、正常な自動検出エンドポイントに置き換え、新しい EWS エンドポイントを引き続き使用します。正常な応答を取得できなかった場合は、引き続き元の自動検出エンドポイントと EWS エンドポイントを使用します。エラーから回復するために更新する場合は、必要に応じてエラーを処理します。 
    
次の図は、このプロセスを視覚的に表したものです。
  
**図 1. 自動検出を使用して構成情報を更新するプロセス**

![模式図は自動検出が構成情報を更新する方法を示しています。](media/Ex15_Autodiscover_Refresh_Flowchart.png)
  
### <a name="connection-related-errors"></a>接続に関連するエラー
<a name="bk_ConnectionErrors"> </a>

キャッシュされた構成情報を更新すると、すべてではありませんが、一部のエラーを解決することができます。 
  
**表 2. キャッシュの更新によって解決するエラー**

|**エラー**|**EWS マネージ API の実装**|**注**|
|:-----|:-----|:-----|
|DNS またはネットワーク障害のエラー<br/><br/> 例: Host name could not be found. (ホスト名が見つかりませんでした。)  <br/> |[ServiceRemoteException](https://msdn.microsoft.com/library/Microsoft.Exchange.WebServices.Data.ServiceRemoteException.aspx) <br/> |サーバーが見つからないか、サーバーにアクセスできなかったことを示すすべてのエラーは、自動検出を試みることによって解決される場合があります。 <br/><br/> キャッシュされた EWS エンドポイントが有効ではなくなった可能性があります。自動検出によって新しいサーバーに誘導できる場合があります。  <br/> |
|HTTP の状態エラー<br/><br/> 例: 503 Service Unavailable (503 サービスを利用できません)  <br/> |[ServiceRemoteException](https://msdn.microsoft.com/library/Microsoft.Exchange.WebServices.Data.ServiceRemoteException.aspx) <br/> |HTTP の状態エラーはさまざまな理由で発生します。<br/><br/> ただし、自動検出を実行して、ユーザーが新しい EWS エンドポイントを利用できるかどうか調べることをお勧めします。  <br/> |
|EWS のエラー コード <br/><br/> 例: ErrorConnectionFailed <br/> |[ResponseCodeType](../web-service-reference/responsecode.md) <br/> | ほとんどの EWS のエラー コードは、構成情報の更新の根拠にはなりません。<br/><br/> ただし、次のエラー コードは、構成情報を更新する必要があることを明確に示しています。<br/>- **ErrorConnectionFailed** <br/>- **ErrorMailboxMoveInProgress** <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange の自動検出](autodiscover-for-exchange.md)  
- [自動検出エンドポイントの一覧を生成する](how-to-generate-a-list-of-autodiscover-endpoints.md)   
- [自動検出を使用して Exchange からユーザー設定を取得する](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
    

