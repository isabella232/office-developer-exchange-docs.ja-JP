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
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759189"
---
# <a name="tools-and-resources-for-troubleshooting-ews-applications-for-exchange"></a>Exchange の EWS アプリケーションのトラブルシューティングに使用するツールとリソース

EWS マネージ API アプリケーションまたは EWS アプリケーションのトラブルシューティングに役立つリソースを紹介します。
  
物事は計画どおりに進まないことがあります。ときには EWS の要求が失敗することや、予期しない結果が生じることがあります。これは、特に理由が明らかでないときにはイライラするかもしれません。この状況に陥らないことが何よりですが、もしものために、この記事では問題のトラブルシューティングに役立つツールとリソースに関する情報をご提供します。
  
> [!NOTE]
> この記事では、一般的なトラブルシューティングのアドバイスと、トラブルシューティング情報のソースを提供します。 残念なことに、トラブルシューティング手順の詳細について説明することはできません。 特定のエラーをトラブルシューティングする際の支援については、「[次の手順](#bk_NextSteps)」をご参照ください。 
  
## <a name="examine-the-soap-requests-and-responses"></a>SOAP の要求と応答を調べる

物事が適切に動作しないときには、何が起こっているかが確認できると、とても助かります。 EWS または EWS マネージ API に関わる問題を調査しているときに最初に調べることは、アプリケーションがネットワークを通じて送信している要求とサーバーが送り返してきた応答を調べることです。
  
EWS マネージ API には[組み込みのトレース機能](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md)があるため、SOAP の要求と応答を簡単に調べることができます。 EWS を使用している場合、同様のトレース機能にアクセスできるかどうかは、要求の送信に使用しているプラットフォームやクラスによって決まります。 ただし、[Network Monitor](http://www.microsoft.com/en-us/download/details.aspx?id=4865) や [Fiddler](http://www.telerik.com/fiddler) などのネットワーク トレース ツールは、ネットワーク トラフィックを調べたり、要求と応答のペイロードを表示したりするためにいつでも使用できます。 
  
さらに、[クライアントの要求をインストルメント化する](instrumenting-client-requests-for-ews-and-rest-in-exchange.md)ことで、要求と応答から得られる情報の質が高まります。 
  
要求と応答を手に入れたら、次の点について自問してください。それらは正しいように見えるか。アプリケーションは期待どおりの値を送信しているか。応答に矛盾がないか。
  
## <a name="examine-error-codes"></a>エラー コードを調べる

エラー コードは、一見無意味に見えるものであっても、問題を特定するために非常に役立つことがあります。 クライアントが[調整されている](ews-throttling-in-exchange.md)ことをエラーが示していないか。 おそらく[構成情報を更新する](how-to-refresh-configuration-information-by-using-autodiscover.md)ための自動検出の呼び出しが適切であるか。 
  
特定のエラー処理の詳細については、次の記事をご参照ください。
  
- [自動検出のエラー メッセージの処理](handling-autodiscover-error-messages.md)
    
- [Exchange の EWS での通知に関連するエラーの処理](handling-notification-related-errors-in-ews-in-exchange.md)
    
- [Exchange の EWS での同期に関連するエラーの処理](handling-synchronization-related-errors-in-ews-in-exchange.md)
    
- [Exchange の EWS での削除に関連するエラーの処理](handling-deletion-related-errors-in-ews-in-exchange.md)
    
## <a name="verify-versions"></a>バージョンを確認する

EWS 操作に関連するコンポーネントは数種類あり、それらのコンポーネントのバージョンが結果に影響することがあります。
  
**表 1. EWS プロセスに影響する可能性のあるバージョン付きコンポーネント**

|**コンポーネント**|**EWS マネージ API**|**EWS**|**メモ**|
|:-----|:-----|:-----|:-----|
|要求されるサーバーのバージョン  <br/> |[ExchangeServiceBase.RequestedServerVersion](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservicebase.requestedserverversion%28v=exchg.80%29.aspx) プロパティ  <br/> |[RequestServerVersion](http://msdn.microsoft.com/library/af4032d5-42b3-463e-9d0a-8236d78e5b75%28Office.15%29.aspx) 要素  <br/> |この値により、EWS 要求の処理に使用される EWS スキーマのバージョンが制御されます。ここで指定されたスキーマのバージョンが、送信する要求に適していることを確認します。一部のプロパティと操作は、以前のスキーマのバージョンでは利用できません。  <br/> |
|サーバーのバージョン  <br/> |[ExchangeServiceBase.ServerInfo](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservicebase.serverinfo%28v=exchg.80%29.aspx) プロパティ  <br/> |[ServerVersionInfo](http://msdn.microsoft.com/library/c04a6872-ca27-432b-aac2-36b023d0afc6%28Office.15%29.aspx) 要素  <br/> |この値は EWS の応答でサーバーから返され、応答を処理したサーバーのバージョンを表します。この値が期待していたものであることを確認します。可能な場合は、Exchange サーバーが Exchange のメジャー バージョンに向けた最新の更新プログラムを実行していることを確認します。  <br/> |
|EWS マネージ API のバージョン  <br/> |Microsoft.Exchange.WebServices.dll ファイルの製品バージョン プロパティ。  <br/> |該当なし  <br/> |EWS マネージ API を使用している場合は、[最新のバージョン](http://aka.ms/ews-managed-api-readme)を使用していることを確認します。  <br/> |
   
## <a name="verify-access"></a>アクセスを確認する

EWS は既定で有効化されていますが、[既定値は変更可能](how-to-control-access-to-ews-in-exchange.md)です。 [Get-OrganizationConfig](http://technet.microsoft.com/ja-JP/library/bb124754.aspx) コマンドレットを使用して EWS がサーバー上で有効化されていることを確認し、[Get-CASMailbox](http://technet.microsoft.com/ja-JP/library/aa997571.aspx) コマンドレットを使用して EWS がユーザーのメールボックスに対して有効化されていることを確認します。 また、EWS の許可または禁止リストについて両方のコマンドレットの応答を調べて、目的のアプリケーションが EWS の使用を禁止されていないことも確認します。 
  
さらに、EWS 仮想ディレクトリの[既定の認証設定](http://technet.microsoft.com/ja-JP/library/gg247612%28v=exchg.150%29.aspx)が変更されていないことも確認する必要があります。 
  
## <a name="try-another-ews-client"></a>別の EWS クライアントを試してみる

ときには別のクライアントから同じ要求を試してみて、結果を比較することが役立つことがあります。別のクライアントの結果が異なっているならば、違いは何でしょうか。成功した要求と失敗した要求の違いを見つけることは、特定の要求が失敗する理由を説明する際に役立つことがあります。
  
テストに使用する別のクライアントを記述することもできますが、その必要はありません。 [EWSEditor](http://ewseditor.codeplex.com/) は、EWS マネージ API と EWS を使用するサンプル クライアントです。 このクライアントはダウンロードが可能です (ソース コードを含む)。これを使用して、目的のアプリケーションで失敗したものと同じ要求を試してみることができます。 
  
## <a name="examine-iis-logs"></a>IIS のログを調べる

Exchange サーバーにアクセスしている場合は、クライアント アクセス サーバー上のインターネット インフォメーション サービス (IIS) が提供するログ記録機能により、失敗に関する詳細な情報が得られます。ただし、IIS のログは HTTP エラーを受信した場合にのみ役立つものだという点に注意してください。
  
IIS には、2 種類のログ記録方式があります。[IIS ログ記録](http://www.iis.net/learn/manage/provisioning-and-managing-iis/configure-logging-in-iis)と[失敗した要求のトレース](http://www.iis.net/learn/troubleshoot/using-failed-request-tracing/troubleshooting-failed-requests-using-tracing-in-iis)です。 IIS のログを扱う場合は、いくつかの組み込み EWS クエリが含まれている [Log Parser Studio](http://blogs.technet.com/b/exchange/archive/2012/03/07/introducing-log-parser-studio.aspx) を使用できます。
  
## <a name="next-steps"></a>次の手順
<a name="bk_NextSteps"> </a>

トラブルシューティングに使用できるツールとリソースについて理解すると、それらのツールが提示する情報を理解するための支援が必要になることでしょう。 次に、支援を得るためのオプションを示します。
  
- [MSDN の Exchange Server 開発者フォーラム](http://social.msdn.microsoft.com/Forums/en-US/home?category=exchangeserver) — MSDN Exchange Server 開発者コミュニティに質問してください。 
    
- [StackOverflow](http://stackoverflow.com/tags/ews) — StackOverflow コミュニティに質問してください。 投稿には必ず "ews" のタグを付けてください。 
    
- [Microsoft サポート](http://support.microsoft.com/ph/730/en-us) — Microsoft サポート担当者にお問い合わせください。 
    
## <a name="see-also"></a>関連項目


次の記事をご覧ください。
  
- [Exchange の Web サービス クライアントを開発する](develop-web-service-clients-for-exchange.md)
    
- [要求と応答をトレースして、EWS マネージ API アプリケーションのトラブルシューティングを行う](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md)
    
- [Exchange で EWS と REST のクライアントの要求をインストルメント化する](instrumenting-client-requests-for-ews-and-rest-in-exchange.md)
    
- [Exchange での EWS 調整](ews-throttling-in-exchange.md)
    
- [自動検出を使用して構成情報を更新する](how-to-refresh-configuration-information-by-using-autodiscover.md)
    
- [自動検出のエラー メッセージの処理](handling-autodiscover-error-messages.md)
    
- [Exchange の EWS での通知に関連するエラーの処理](handling-notification-related-errors-in-ews-in-exchange.md)
    
- [Exchange の EWS での同期に関連するエラーの処理](handling-synchronization-related-errors-in-ews-in-exchange.md)
    
- [Exchange の EWS での削除に関連するエラーの処理](handling-deletion-related-errors-in-ews-in-exchange.md)
    
- [IIS のログ記録の構成](http://www.iis.net/learn/manage/provisioning-and-managing-iis/configure-logging-in-iis)
    
- [IIS 7 のトレースを使用して失敗した要求をトラブルシューティングする](http://www.iis.net/learn/troubleshoot/using-failed-request-tracing/troubleshooting-failed-requests-using-tracing-in-iis)
    
- [概要: Log Parser Studio](http://blogs.technet.com/b/exchange/archive/2012/03/07/introducing-log-parser-studio.aspx)
    
- [Exchange 仮想ディレクトリの既定の設定](http://technet.microsoft.com/ja-JP/library/gg247612%28v=exchg.150%29.aspx)
    
次のものをダウンロードしてください。
  
- [Microsoft ネットワーク モニター 3.4](http://www.microsoft.com/en-us/download/details.aspx?id=4865)
    
- [Fiddler](http://www.telerik.com/fiddler)
    
- [EWSEditor](http://ewseditor.codeplex.com/)
    
- [Exchange Web サービス マネージ API](http://go.microsoft.com/fwlink/?LinkID=255472)
    

