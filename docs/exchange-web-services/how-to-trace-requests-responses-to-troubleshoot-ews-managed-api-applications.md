---
title: EWS マネージ API アプリのトラブルシューティングのための要求と応答のトレース
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 186c1d1d-b8dc-4914-b3cd-6fada7ecd877
description: Ews の要求と応答をトレースして、EWS マネージ API アプリケーションでエラーのトラブルシューティングを行う方法について説明します。
localization_priority: Priority
ms.openlocfilehash: dd225030d62a2e8211b7063ee78a59fd1a070263
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455857"
---
# <a name="trace-requests-and-responses-to-troubleshoot-ews-managed-api-apps"></a>EWS マネージ API アプリのトラブルシューティングのための要求と応答のトレース

Ews の要求と応答をトレースして、EWS マネージ API アプリケーションでエラーのトラブルシューティングを行う方法について説明します。
  
アクセス権のないリモートコンピューターで処理の一部が実行されるため、web サービスベースのアプリケーションをデバッグするのは困難な場合があります。 サーバー上ではコードをステップ実行できないため、クライアントとサーバー間で送信される XML 要求と応答を確認すると、アプリケーションのどの部分がエラーの原因なのかを特定しやすくなります。 
  
EWS を使用している場合は、XML 要求と応答へのアクセス権が既に付与されています。問題のトラブルシューティングを行うために、要求に対するサーバーの応答を確認するブレークポイントをコードに含めることができます。 EWS マネージ API を使用している場合は、EWS 要求と応答に直接アクセスすることはできません。 ただし、 [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)オブジェクトのトレースメソッドを使用すると、xml 要求と応答をキャプチャできます。その後、xml を使用して、コードが動作していない理由を特定できます。 

たとえば、プロパティが正しく設定されていない場合は、予期しない応答が返される可能性があります。また、トレース出力を使用して、XML 要求と応答を参照し、エラーを識別できます。 Ews マネージ API のトレース出力は、EWS アプリケーションを作成するための XML 要求を手動で構築するのにも役立ちます。 EWS を使用している場合は、EWS マネージ API を使用して小規模なアプリケーションを作成し、それをトレースしてから、その XML 要求情報を使用して EWS 要求の作成に役立てることができます。 
  
## <a name="enabling-tracing-on-the-exchangeservice-object"></a>ExchangeService オブジェクトのトレースを有効にする
<a name="bk_EnableTracing"> </a>

トレースを有効にするには、アプリケーションの[ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)オブジェクトを作成し、次の例に示すように、トレースのプロパティを設定します。 
  
```cs
ExchangeService service = new ExchangeService(ExchangeVersion.Exchange2010);
service.TraceListener = ITraceListenerInstance;
// Optional flags to indicate the requests and responses to trace.
service.TraceFlags = TraceFlags.EwsRequest | TraceFlags.EwsResponse
service.TraceEnabled = true;

```

[Traceenabled](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.traceenabled%28v=exchg.80%29.aspx)プロパティを**true**に設定すると、トレースフラグに一致するすべての要求が、指定したトレースリスナーに送信されます。 1 つのトレース フラグを指定することができ、またはトレース フラグを論理 **OR** と組み合わせることにより、複数のトレース フラグを指定することができます。 [Traceflags 列挙](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.traceflags%28v=exchg.80%29.aspx)を使用して、EWS の値を指定したり、自動検出の要求と応答を指定したりできます。 
  
## <a name="implementing-a-tracelistener-object"></a>TraceListener オブジェクトを実装する
<a name="bk_traceListener"> </a>

[Traceenabled](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.traceenabled%28v=exchg.80%29.aspx)プロパティを**true**に設定すると、XML 要求とアプリケーションに対する応答 (コンソールウィンドウなど) が出力されます。 トレース出力を制御してファイルに保存する場合は、 [TraceListener クラス](https://msdn.microsoft.com/library/system.diagnostics.tracelistener.aspx)オブジェクトを実装することをお勧めします。 次のコード例は、 [ITraceListener](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itracelistener%28v=exchg.80%29.aspx)インターフェイスを実装し、トレースされた要求と応答を XML またはテキストファイルに格納する簡単なオブジェクトを示しています。 
  
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
- [EWS マネージ API アセンブリの参照](how-to-reference-the-ews-managed-api-assembly.md)    
- [EWS マネージ API を使用して EWS と通信する](how-to-communicate-with-ews-by-using-the-ews-managed-api.md)
    

