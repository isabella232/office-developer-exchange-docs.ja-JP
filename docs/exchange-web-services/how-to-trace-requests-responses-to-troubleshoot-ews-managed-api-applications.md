---
title: EWS のマネージ API アプリケーションのトラブルシューティングを行うには、要求と応答をトレースします。
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 186c1d1d-b8dc-4914-b3cd-6fada7ecd877
description: EWS のマネージ API アプリケーションで発生したエラーのトラブルシューティングを行うには、EWS の要求と応答をトレースする方法を確認します。
ms.openlocfilehash: 056a1f84c4172b0404975d6fc35f9ecd7395ecdb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759057"
---
# <a name="trace-requests-and-responses-to-troubleshoot-ews-managed-api-apps"></a>EWS のマネージ API アプリケーションのトラブルシューティングを行うには、要求と応答をトレースします。

EWS のマネージ API アプリケーションで発生したエラーのトラブルシューティングを行うには、EWS の要求と応答をトレースする方法を確認します。
  
Web サービス ベースのアプリケーションのデバッグは困難へのアクセスがない可能性がリモート コンピューター上のプロセスの一部が実行されるためです。 サーバー上でコードをステップ実行することはできません、XML 要求とエラーが発生して、アプリケーションのどの部分を決定するには、クライアントとサーバー間で送信される応答を参照してくださいすることがあります。 
  
XML 要求と応答へのアクセスが既にある場合は、EWS を使用する場合は、問題をトラブルシューティングするために要求に、サーバーの応答を確認するようにコードにブレークポイントを配置できます。 EWS のマネージ API を使用する場合は、EWS の要求と応答に直接アクセスがありません。 ただし、 [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)オブジェクトのトレース メソッドを使用するには、XML 要求と応答をキャプチャして、コードが動作しない原因を特定するのには XML を使用することができますし。 

たとえば、プロパティを正しく設定されていない場合、予期しない応答を取得する可能性があり、エラーを識別するには、XML 要求と応答を確認するのにはトレース出力を使用することができます。 EWS のマネージ API からのトレース出力は、EWS アプリケーションを作成するのには XML の要求を手動で構築するにも役立ちます。 EWS を使用する場合は、EWS のマネージ API を使用して、小規模なアプリケーションを作成に、トレースおよび EWS 要求を構築するため、XML 要求の情報を使用します。 
  
## <a name="enabling-tracing-on-the-exchangeservice-object"></a>ExchangeService オブジェクトのトレースを有効にする
<a name="bk_EnableTracing"> </a>

トレースを有効にするには、アプリケーションの[ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)オブジェクトを作成し、次の例に示すように、トレースのプロパティを設定します。 
  
```cs
ExchangeService service = new ExchangeService(ExchangeVersion.Exchange2010);
service.TraceListener = ITraceListenerInstance;
// Optional flags to indicate the requests and responses to trace.
service.TraceFlags = TraceFlags.EwsRequest | TraceFlags.EwsResponse
service.TraceEnabled = true;

```

[TraceEnabled](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.traceenabled%28v=exchg.80%29.aspx)プロパティを**true**に設定した後、トレース フラグに一致するすべての要求が指定されたトレース リスナーに送信されます。 1 つのトレース フラグを指定することができます。 または論理**OR**で組み合わせることにより複数のトレース フラグを指定することができます。 [TraceFlags 列挙体](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.traceflags%28v=exchg.80%29.aspx)を使用するには EWS および自動検出の要求と応答の値を指定します。 
  
## <a name="implementing-a-tracelistener-object"></a>TraceListener オブジェクトを実装する
<a name="bk_traceListener"> </a>

[TraceEnabled](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.traceenabled%28v=exchg.80%29.aspx)プロパティを設定するには**true** XML 要求と、[コンソール] ウィンドウなど、アプリケーションへの応答を出力します。 トレース出力を制御し、ファイルに保存する場合は、 [TraceListener クラス](http://msdn.microsoft.com/en-us/library/system.diagnostics.tracelistener.aspx)オブジェクトを実装することをお勧めします。 次のコード例は、 [ITraceListener](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itracelistener%28v=exchg.80%29.aspx)インターフェイスを実装し、XML またはテキスト ファイルにトレースされた要求と応答を格納する単純なオブジェクトを示しています。 
  
```cs
class TraceListener : ITraceListener
{
    #region ITraceListener Members
    public void Trace(string traceType, string traceMessage)
    {
      CreateXMLTextFile(traceType, traceMessage.ToString());
    }
    #endregion
    private void CreateXMLTextFile(string fileName, string traceContent)
    {
      // Create a new XML file for the trace information.
      try
      {
        // If the trace data is valid XML, create an XmlDocument object and save.
        XmlDocument xmlDoc = new XmlDocument();
        xmlDoc.Load(traceContent);
        xmlDoc.Save(fileName + ".xml");
      }
      catch
      {
        // If the trace data is not valid XML, save it as a text document.
        System.IO.File.WriteAllText(fileName + ".txt", traceContent);
      }
    }
}

```

## <a name="see-also"></a>関連項目

- [Exchange で Web サービスの使用を開始する](start-using-web-services-in-exchange.md)
- [自動検出のエラー メッセージの処理](handling-autodiscover-error-messages.md)    
- [EWS のマネージ API のアセンブリを参照します。](how-to-reference-the-ews-managed-api-assembly.md)    
- [EWS のマネージ API を使用して通信 EWS](how-to-communicate-with-ews-by-using-the-ews-managed-api.md)
    

