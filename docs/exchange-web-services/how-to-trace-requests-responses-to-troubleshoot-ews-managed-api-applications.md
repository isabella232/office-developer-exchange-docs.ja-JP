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
# <a name="trace-requests-and-responses-to-troubleshoot-ews-managed-api-apps"></a><span data-ttu-id="b3b2f-103">EWS のマネージ API アプリケーションのトラブルシューティングを行うには、要求と応答をトレースします。</span><span class="sxs-lookup"><span data-stu-id="b3b2f-103">Trace requests and responses to troubleshoot EWS Managed API apps</span></span>

<span data-ttu-id="b3b2f-104">EWS のマネージ API アプリケーションで発生したエラーのトラブルシューティングを行うには、EWS の要求と応答をトレースする方法を確認します。</span><span class="sxs-lookup"><span data-stu-id="b3b2f-104">Find out how to trace EWS requests and responses to troubleshoot errors in your EWS Managed API application.</span></span>
  
<span data-ttu-id="b3b2f-105">Web サービス ベースのアプリケーションのデバッグは困難へのアクセスがない可能性がリモート コンピューター上のプロセスの一部が実行されるためです。</span><span class="sxs-lookup"><span data-stu-id="b3b2f-105">Debugging a web service-based application can be difficult because part of the processing is performed on a remote computer that you might not have access to.</span></span> <span data-ttu-id="b3b2f-106">サーバー上でコードをステップ実行することはできません、XML 要求とエラーが発生して、アプリケーションのどの部分を決定するには、クライアントとサーバー間で送信される応答を参照してくださいすることがあります。</span><span class="sxs-lookup"><span data-stu-id="b3b2f-106">Because you cannot step through the code on the server, it can be helpful to see the XML requests and responses that are sent between the client and the server to determine which part of the application is causing an error.</span></span> 
  
<span data-ttu-id="b3b2f-107">XML 要求と応答へのアクセスが既にある場合は、EWS を使用する場合は、問題をトラブルシューティングするために要求に、サーバーの応答を確認するようにコードにブレークポイントを配置できます。</span><span class="sxs-lookup"><span data-stu-id="b3b2f-107">If you are using EWS, you already have access to the XML request and response; you can put a break point in your code to review the server's response to your request in order to troubleshoot an issue.</span></span> <span data-ttu-id="b3b2f-108">EWS のマネージ API を使用する場合は、EWS の要求と応答に直接アクセスがありません。</span><span class="sxs-lookup"><span data-stu-id="b3b2f-108">If you're using the EWS Managed API, you don't have direct access to the EWS request and response.</span></span> <span data-ttu-id="b3b2f-109">ただし、 [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)オブジェクトのトレース メソッドを使用するには、XML 要求と応答をキャプチャして、コードが動作しない原因を特定するのには XML を使用することができますし。</span><span class="sxs-lookup"><span data-stu-id="b3b2f-109">However, you can use tracing methods on the [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object to capture the XML request and response, and you can then use the XML to determine why your code is not working.</span></span> 

<span data-ttu-id="b3b2f-110">たとえば、プロパティを正しく設定されていない場合、予期しない応答を取得する可能性があり、エラーを識別するには、XML 要求と応答を確認するのにはトレース出力を使用することができます。</span><span class="sxs-lookup"><span data-stu-id="b3b2f-110">For example, if you did not set a property correctly, you might get an unexpected response, and you can use the trace output to look at the XML request and response to identify the error.</span></span> <span data-ttu-id="b3b2f-111">EWS のマネージ API からのトレース出力は、EWS アプリケーションを作成するのには XML の要求を手動で構築するにも役立ちます。</span><span class="sxs-lookup"><span data-stu-id="b3b2f-111">The trace output from the EWS Managed API can also help you manually build the XML request to create your EWS application.</span></span> <span data-ttu-id="b3b2f-112">EWS を使用する場合は、EWS のマネージ API を使用して、小規模なアプリケーションを作成に、トレースおよび EWS 要求を構築するため、XML 要求の情報を使用します。</span><span class="sxs-lookup"><span data-stu-id="b3b2f-112">If you are using EWS, you can create a small application by using EWS Managed API, trace it, and then use the XML request information to help you build your EWS request.</span></span> 
  
## <a name="enabling-tracing-on-the-exchangeservice-object"></a><span data-ttu-id="b3b2f-113">ExchangeService オブジェクトのトレースを有効にする</span><span class="sxs-lookup"><span data-stu-id="b3b2f-113">Enabling tracing on the ExchangeService object</span></span>
<span data-ttu-id="b3b2f-114"><a name="bk_EnableTracing"> </a></span><span class="sxs-lookup"><span data-stu-id="b3b2f-114"></span></span>

<span data-ttu-id="b3b2f-115">トレースを有効にするには、アプリケーションの[ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)オブジェクトを作成し、次の例に示すように、トレースのプロパティを設定します。</span><span class="sxs-lookup"><span data-stu-id="b3b2f-115">To enable tracing, create an [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object for your application, and set the tracing properties as shown in the following example.</span></span> 
  
```cs
ExchangeService service = new ExchangeService(ExchangeVersion.Exchange2010);
service.TraceListener = ITraceListenerInstance;
// Optional flags to indicate the requests and responses to trace.
service.TraceFlags = TraceFlags.EwsRequest | TraceFlags.EwsResponse
service.TraceEnabled = true;

```

<span data-ttu-id="b3b2f-116">[TraceEnabled](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.traceenabled%28v=exchg.80%29.aspx)プロパティを**true**に設定した後、トレース フラグに一致するすべての要求が指定されたトレース リスナーに送信されます。</span><span class="sxs-lookup"><span data-stu-id="b3b2f-116">After you set the [TraceEnabled](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.traceenabled%28v=exchg.80%29.aspx) property to **true**, all requests that match the trace flags will be sent to the specified trace listener.</span></span> <span data-ttu-id="b3b2f-117">1 つのトレース フラグを指定することができます。 または論理**OR**で組み合わせることにより複数のトレース フラグを指定することができます。</span><span class="sxs-lookup"><span data-stu-id="b3b2f-117">You can specify a single trace flag, or you can specify multiple trace flags by combining them with a logical **OR**.</span></span> <span data-ttu-id="b3b2f-118">[TraceFlags 列挙体](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.traceflags%28v=exchg.80%29.aspx)を使用するには EWS および自動検出の要求と応答の値を指定します。</span><span class="sxs-lookup"><span data-stu-id="b3b2f-118">You can use the [TraceFlags enumeration](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.traceflags%28v=exchg.80%29.aspx) to specify values for EWS and for Autodiscover requests and responses.</span></span> 
  
## <a name="implementing-a-tracelistener-object"></a><span data-ttu-id="b3b2f-119">TraceListener オブジェクトを実装する</span><span class="sxs-lookup"><span data-stu-id="b3b2f-119">Implementing a TraceListener object</span></span>
<span data-ttu-id="b3b2f-120"><a name="bk_traceListener"> </a></span><span class="sxs-lookup"><span data-stu-id="b3b2f-120"></span></span>

<span data-ttu-id="b3b2f-121">[TraceEnabled](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.traceenabled%28v=exchg.80%29.aspx)プロパティを設定するには**true** XML 要求と、[コンソール] ウィンドウなど、アプリケーションへの応答を出力します。</span><span class="sxs-lookup"><span data-stu-id="b3b2f-121">You can set the [TraceEnabled](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.traceenabled%28v=exchg.80%29.aspx) property to **true** to output the XML requests and responses to your application, such as a console window.</span></span> <span data-ttu-id="b3b2f-122">トレース出力を制御し、ファイルに保存する場合は、 [TraceListener クラス](http://msdn.microsoft.com/en-us/library/system.diagnostics.tracelistener.aspx)オブジェクトを実装することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="b3b2f-122">If you want to control the trace output and save it to a file, we recommend that you implement a [TraceListener class](http://msdn.microsoft.com/en-us/library/system.diagnostics.tracelistener.aspx) object.</span></span> <span data-ttu-id="b3b2f-123">次のコード例は、 [ITraceListener](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itracelistener%28v=exchg.80%29.aspx)インターフェイスを実装し、XML またはテキスト ファイルにトレースされた要求と応答を格納する単純なオブジェクトを示しています。</span><span class="sxs-lookup"><span data-stu-id="b3b2f-123">The following code example shows a simple object that implements the [ITraceListener](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itracelistener%28v=exchg.80%29.aspx) interface and stores the traced requests and responses in XML or text files.</span></span> 
  
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

## <a name="see-also"></a><span data-ttu-id="b3b2f-124">関連項目</span><span class="sxs-lookup"><span data-stu-id="b3b2f-124">See also</span></span>

- [<span data-ttu-id="b3b2f-125">Exchange で Web サービスの使用を開始する</span><span class="sxs-lookup"><span data-stu-id="b3b2f-125">Start using web services in Exchange</span></span>](start-using-web-services-in-exchange.md)
- [<span data-ttu-id="b3b2f-126">自動検出のエラー メッセージの処理</span><span class="sxs-lookup"><span data-stu-id="b3b2f-126">Handling Autodiscover error messages</span></span>](handling-autodiscover-error-messages.md)    
- [<span data-ttu-id="b3b2f-127">EWS のマネージ API のアセンブリを参照します。</span><span class="sxs-lookup"><span data-stu-id="b3b2f-127">Reference the EWS Managed API assembly</span></span>](how-to-reference-the-ews-managed-api-assembly.md)    
- [<span data-ttu-id="b3b2f-128">EWS のマネージ API を使用して通信 EWS</span><span class="sxs-lookup"><span data-stu-id="b3b2f-128">Communicate with EWS by using the EWS Managed API</span></span>](how-to-communicate-with-ews-by-using-the-ews-managed-api.md)
    

