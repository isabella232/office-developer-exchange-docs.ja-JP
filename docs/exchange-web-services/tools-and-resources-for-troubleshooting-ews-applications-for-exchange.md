---
title: Exchange の EWS アプリケーションのトラブルシューティングに使用するツールとリソース
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: ee7fcd05-35d7-47bf-bac4-e719c49c11fe
description: EWS マネージ API アプリケーションまたは EWS アプリケーションのトラブルシューティングに役立つリソースを紹介します。
ms.openlocfilehash: d8d8ea736ca3b896642ad06f5987caeba8d8d059
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759189"
---
# <a name="tools-and-resources-for-troubleshooting-ews-applications-for-exchange"></a>Exchange の EWS アプリケーションのトラブルシューティングに使用するツールとリソース

EWS マネージ API アプリケーションまたは EWS アプリケーションのトラブルシューティングに役立つリソースを紹介します。
  
物事は計画どおりに進まないことがあります。ときには EWS の要求が失敗することや、予期しない結果が生じることがあります。これは、特に理由が明らかでないときにはイライラするかもしれません。この状況に陥らないことが何よりですが、もしものために、この記事では問題のトラブルシューティングに役立つツールとリソースに関する情報をご提供します。
  
> [!NOTE]
> トラブルシューティング情報のソースに関する一般的なトラブルシューティングのアドバイスが掲載されています。 残念ながら詳細なトラブルシューティング手順を提供することはできません。 詳細については、特定のエラーのトラブルシューティング、[次の手順](#bk_NextSteps)を参照してください。 
  
## <a name="examine-the-soap-requests-and-responses"></a>SOAP の要求と応答を調べる

プログラムが正しく実行されない、何が起こっているを確認することに本当に役立ちます。 EWS または EWS のマネージ API の問題を調査する場合に、照会の最初の行は、アプリケーションがネットワーク経由で送信される要求と、サーバーが送信する応答を調べることです。
  
EWS のマネージ API を簡単に SOAP 要求と応答の検証の[組み込みトレース機能の](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md)使用します。 EWS を使用する場合がありますか、どのようなプラットフォームや、要求の送信に使用するクラスによって、同様のトレース機能にアクセスできない場合があります。 ただし、ネットワーク トラフィックを検査し、要求と応答のペイロードを表示する常に[ネットワーク モニター](http://www.microsoft.com/en-us/download/details.aspx?id=4865)または[Fiddler](http://www.telerik.com/fiddler)のようなネットワーク トレース ツールを使用することができます。 
  
さらに、要求と応答で使用できる情報を強化するために[、クライアントの要求をインストルメント化](instrumenting-client-requests-for-ews-and-rest-in-exchange.md)をすることができます。 
  
要求と応答を手に入れたら、次の点について自問してください。それらは正しいように見えるか。アプリケーションは期待どおりの値を送信しているか。応答に矛盾がないか。
  
## <a name="examine-error-codes"></a>エラー コードを調べる

場合がありますもしない場合は、一見無意味にエラー コードは、問題を特定することに長い道を移動できます。 エラーは、クライアントが[抑制](ews-throttling-in-exchange.md)されていることを示していますか。 おそらく[構成情報を更新](how-to-refresh-configuration-information-by-using-autodiscover.md)するのには自動検出の呼び出しは、順番ですか。 
  
特定のエラー処理の詳細については、次の記事を参照してください。
  
- [自動検出のエラー メッセージの処理](handling-autodiscover-error-messages.md)
    
- [Exchange における EWS での通知関連エラーの処理](handling-notification-related-errors-in-ews-in-exchange.md)
    
- [Exchange EWS での同期に関連するエラーの処理](handling-synchronization-related-errors-in-ews-in-exchange.md)
    
- [Exchange EWS での削除に関連するエラーの処理](handling-deletion-related-errors-in-ews-in-exchange.md)
    
## <a name="verify-versions"></a>バージョンを確認する

EWS 操作に関連するコンポーネントは数種類あり、それらのコンポーネントのバージョンが結果に影響することがあります。
  
**表 1 です。EWS のプロセスに影響を与えることができますが、バージョン管理されるコンポーネント**

|**コンポーネント**|**EWS Managed API**|**EWS**|**メモ**|
|:-----|:-----|:-----|:-----|
|要求されるサーバーのバージョン  <br/> |[ExchangeServiceBase.RequestedServerVersion](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.exchangeservicebase.requestedserverversion%28v=exchg.80%29.aspx)プロパティ  <br/> |[RequestServerVersion](http://msdn.microsoft.com/library/af4032d5-42b3-463e-9d0a-8236d78e5b75%28Office.15%29.aspx)要素  <br/> |この値により、EWS 要求の処理に使用される EWS スキーマのバージョンが制御されます。ここで指定されたスキーマのバージョンが、送信する要求に適していることを確認します。一部のプロパティと操作は、以前のスキーマのバージョンでは利用できません。  <br/> |
|サーバーのバージョン  <br/> |[ExchangeServiceBase.ServerInfo](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.exchangeservicebase.serverinfo%28v=exchg.80%29.aspx)プロパティ  <br/> |[ServerVersionInfo](http://msdn.microsoft.com/library/c04a6872-ca27-432b-aac2-36b023d0afc6%28Office.15%29.aspx)要素  <br/> |この値は EWS の応答でサーバーから返され、応答を処理したサーバーのバージョンを表します。この値が期待していたものであることを確認します。可能な場合は、Exchange サーバーが Exchange のメジャー バージョンに向けた最新の更新プログラムを実行していることを確認します。  <br/> |
|EWS マネージ API のバージョン  <br/> |Microsoft.Exchange.WebServices.dll ファイルの製品バージョン プロパティ。  <br/> |適用できません  <br/> |EWS のマネージ API を使用している場合は、[最新バージョン](http://aka.ms/ews-managed-api-readme)を使っていることを確認します。  <br/> |
   
## <a name="verify-access"></a>アクセスを確認する

既定では[既定の設定を変更する](how-to-control-access-to-ews-in-exchange.md)には、EWS が有効です。 [Get OrganizationConfig](http://technet.microsoft.com/en-us/library/bb124754.aspx)コマンドレットをサーバーでは、EWS が有効になっているかどうかを確認し、ユーザーのメールボックスで EWS が有効であるかどうかを確認するのには、 [Get CASMailbox](http://technet.microsoft.com/en-us/library/aa997571.aspx)コマンドレットを使用します。 また、EWS の両方のコマンドレットの応答を許可または禁止リスト、し、EWS を使用してから、アプリケーションがブロックされていないことを確認を確認します。 
  
EWS 仮想ディレクトリの[既定の認証設定](http://technet.microsoft.com/en-us/library/gg247612%28v=exchg.150%29.aspx)が変更されていないことも確認する必要があります。 
  
## <a name="try-another-ews-client"></a>別の EWS クライアントを試してみる

ときには別のクライアントから同じ要求を試してみて、結果を比較することが役立つことがあります。別のクライアントの結果が異なっているならば、違いは何でしょうか。成功した要求と失敗した要求の違いを見つけることは、特定の要求が失敗する理由を説明する際に役立つことがあります。
  
テストするのには別のクライアントを記述することが確かに、中にする必要はありません。 [EWSEditor](http://ewseditor.codeplex.com/)は、EWS のマネージ API と EWS を使用するサンプル クライアントです。 (ソース コードを含む) のクライアントをダウンロードして使用して、アプリケーションで失敗するのと同じ要求を実行してください。 
  
## <a name="examine-iis-logs"></a>IIS のログを調べる

Exchange サーバーにアクセスしている場合は、クライアント アクセス サーバー上のインターネット インフォメーション サービス (IIS) が提供するログ記録機能により、失敗に関する詳細な情報が得られます。ただし、IIS のログは HTTP エラーを受信した場合にのみ役立つものだという点に注意してください。
  
IIS には、ログの 2 つの異なる方法が用意されています: [IIS ログの収集](http://www.iis.net/learn/manage/provisioning-and-managing-iis/configure-logging-in-iis)および[失敗した要求をトレース](http://www.iis.net/learn/troubleshoot/using-failed-request-tracing/troubleshooting-failed-requests-using-tracing-in-iis)します。 IIS ログを操作するには、[ログ パーサー Studio](http://blogs.technet.com/b/exchange/archive/2012/03/07/introducing-log-parser-studio.aspx)EWS の組み込みのクエリの数が含まれますを使用できます。
  
## <a name="next-steps"></a>次の手順
<a name="bk_NextSteps"> </a>

ツールとトラブルシューティングに使用できるリソースについて説明しました、これでは、これらのツールによって提供される情報を理解するヘルプを必要があります。 ヘルプを取得するためのいくつかのオプションは、次のように。
  
- [Msdn フォーラムを Exchange Server の開発](http://social.msdn.microsoft.com/Forums/en-US/home?category=exchangeserver): Exchange Server の MSDN 開発コミュニティの質問です。 
    
- [StackOverflow](http://stackoverflow.com/tags/ews) -StackOverflow のコミュニティに質問します。 「Ews」で自分投稿にタグ付けすることを確認します。 
    
- [マイクロソフトのサポート](http://support.microsoft.com/ph/730/en-us)などについてマイクロソフトのサポート担当者に問い合わせてください。 
    
## <a name="see-also"></a>関連項目


次の記事を参照してください。
  
- [Exchange の Web サービス クライアントを開発する](develop-web-service-clients-for-exchange.md)
    
- [EWS のマネージ API アプリケーションのトラブルシューティングを行うには、要求と応答をトレースします。](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md)
    
- [EWS および他の Exchange クライアントの要求を実装](instrumenting-client-requests-for-ews-and-rest-in-exchange.md)
    
- [EWS の交換で調整](ews-throttling-in-exchange.md)
    
- [自動検出を使用して構成情報を更新します。](how-to-refresh-configuration-information-by-using-autodiscover.md)
    
- [自動検出のエラー メッセージの処理](handling-autodiscover-error-messages.md)
    
- [Exchange における EWS での通知関連エラーの処理](handling-notification-related-errors-in-ews-in-exchange.md)
    
- [Exchange EWS での同期に関連するエラーの処理](handling-synchronization-related-errors-in-ews-in-exchange.md)
    
- [Exchange EWS での削除に関連するエラーの処理](handling-deletion-related-errors-in-ews-in-exchange.md)
    
- [IIS のログを構成します。](http://www.iis.net/learn/manage/provisioning-and-managing-iis/configure-logging-in-iis)
    
- [失敗した要求のトレースを使用して IIS 7 でのトラブルシューティング](http://www.iis.net/learn/troubleshoot/using-failed-request-tracing/troubleshooting-failed-requests-using-tracing-in-iis)
    
- [ログ パーサー Studio の導入:](http://blogs.technet.com/b/exchange/archive/2012/03/07/introducing-log-parser-studio.aspx)
    
- [Exchange 仮想ディレクトリの既定の設定](http://technet.microsoft.com/en-us/library/gg247612%28v=exchg.150%29.aspx)
    
次のものをダウンロードしてください。
  
- [Microsoft ネットワーク モニターの 3.4](http://www.microsoft.com/en-us/download/details.aspx?id=4865)
    
- [Fiddler](http://www.telerik.com/fiddler)
    
- [EWSEditor](http://ewseditor.codeplex.com/)
    
- [Exchange Web サービスの管理 API](http://go.microsoft.com/fwlink/?LinkID=255472)
    

