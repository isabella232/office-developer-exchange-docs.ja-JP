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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455857"
---
# <a name="trace-requests-and-responses-to-troubleshoot-ews-managed-api-apps"></a><span data-ttu-id="19a83-103">EWS マネージ API アプリのトラブルシューティングのための要求と応答のトレース</span><span class="sxs-lookup"><span data-stu-id="19a83-103">Trace requests and responses to troubleshoot EWS Managed API apps</span></span>

<span data-ttu-id="19a83-104">Ews の要求と応答をトレースして、EWS マネージ API アプリケーションでエラーのトラブルシューティングを行う方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="19a83-104">Find out how to trace EWS requests and responses to troubleshoot errors in your EWS Managed API application.</span></span>
  
<span data-ttu-id="19a83-105">アクセス権のないリモートコンピューターで処理の一部が実行されるため、web サービスベースのアプリケーションをデバッグするのは困難な場合があります。</span><span class="sxs-lookup"><span data-stu-id="19a83-105">Debugging a web service-based application can be difficult because part of the processing is performed on a remote computer that you might not have access to.</span></span> <span data-ttu-id="19a83-106">サーバー上ではコードをステップ実行できないため、クライアントとサーバー間で送信される XML 要求と応答を確認すると、アプリケーションのどの部分がエラーの原因なのかを特定しやすくなります。</span><span class="sxs-lookup"><span data-stu-id="19a83-106">Because you cannot step through the code on the server, it can be helpful to see the XML requests and responses that are sent between the client and the server to determine which part of the application is causing an error.</span></span> 
  
<span data-ttu-id="19a83-107">EWS を使用している場合は、XML 要求と応答へのアクセス権が既に付与されています。問題のトラブルシューティングを行うために、要求に対するサーバーの応答を確認するブレークポイントをコードに含めることができます。</span><span class="sxs-lookup"><span data-stu-id="19a83-107">If you are using EWS, you already have access to the XML request and response; you can put a break point in your code to review the server's response to your request in order to troubleshoot an issue.</span></span> <span data-ttu-id="19a83-108">EWS マネージ API を使用している場合は、EWS 要求と応答に直接アクセスすることはできません。</span><span class="sxs-lookup"><span data-stu-id="19a83-108">If you're using the EWS Managed API, you don't have direct access to the EWS request and response.</span></span> <span data-ttu-id="19a83-109">ただし、 [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)オブジェクトのトレースメソッドを使用すると、xml 要求と応答をキャプチャできます。その後、xml を使用して、コードが動作していない理由を特定できます。</span><span class="sxs-lookup"><span data-stu-id="19a83-109">However, you can use tracing methods on the [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object to capture the XML request and response, and you can then use the XML to determine why your code is not working.</span></span> 

<span data-ttu-id="19a83-110">たとえば、プロパティが正しく設定されていない場合は、予期しない応答が返される可能性があります。また、トレース出力を使用して、XML 要求と応答を参照し、エラーを識別できます。</span><span class="sxs-lookup"><span data-stu-id="19a83-110">For example, if you did not set a property correctly, you might get an unexpected response, and you can use the trace output to look at the XML request and response to identify the error.</span></span> <span data-ttu-id="19a83-111">Ews マネージ API のトレース出力は、EWS アプリケーションを作成するための XML 要求を手動で構築するのにも役立ちます。</span><span class="sxs-lookup"><span data-stu-id="19a83-111">The trace output from the EWS Managed API can also help you manually build the XML request to create your EWS application.</span></span> <span data-ttu-id="19a83-112">EWS を使用している場合は、EWS マネージ API を使用して小規模なアプリケーションを作成し、それをトレースしてから、その XML 要求情報を使用して EWS 要求の作成に役立てることができます。</span><span class="sxs-lookup"><span data-stu-id="19a83-112">If you are using EWS, you can create a small application by using EWS Managed API, trace it, and then use the XML request information to help you build your EWS request.</span></span> 
  
## <a name="enabling-tracing-on-the-exchangeservice-object"></a><span data-ttu-id="19a83-113">ExchangeService オブジェクトのトレースを有効にする</span><span class="sxs-lookup"><span data-stu-id="19a83-113">Enabling tracing on the ExchangeService object</span></span>
<span data-ttu-id="19a83-114"><a name="bk_EnableTracing"> </a></span><span class="sxs-lookup"><span data-stu-id="19a83-114"><a name="bk_EnableTracing"> </a></span></span>

<span data-ttu-id="19a83-115">トレースを有効にするには、アプリケーションの[ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)オブジェクトを作成し、次の例に示すように、トレースのプロパティを設定します。</span><span class="sxs-lookup"><span data-stu-id="19a83-115">To enable tracing, create an [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object for your application, and set the tracing properties as shown in the following example.</span></span> 
  
```cs
ExchangeService service = new ExchangeService(ExchangeVersion.Exchange2010);
service.TraceListener = ITraceListenerInstance;
// Optional flags to indicate the requests and responses to trace.
service.TraceFlags = TraceFlags.EwsRequest | TraceFlags.EwsResponse
service.TraceEnabled = true;

```

<span data-ttu-id="19a83-116">[Traceenabled](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.traceenabled%28v=exchg.80%29.aspx)プロパティを**true**に設定すると、トレースフラグに一致するすべての要求が、指定したトレースリスナーに送信されます。</span><span class="sxs-lookup"><span data-stu-id="19a83-116">After you set the [TraceEnabled](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.traceenabled%28v=exchg.80%29.aspx) property to **true**, all requests that match the trace flags will be sent to the specified trace listener.</span></span> <span data-ttu-id="19a83-117">1 つのトレース フラグを指定することができ、またはトレース フラグを論理 **OR** と組み合わせることにより、複数のトレース フラグを指定することができます。</span><span class="sxs-lookup"><span data-stu-id="19a83-117">You can specify a single trace flag, or you can specify multiple trace flags by combining them with a logical **OR**.</span></span> <span data-ttu-id="19a83-118">[Traceflags 列挙](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.traceflags%28v=exchg.80%29.aspx)を使用して、EWS の値を指定したり、自動検出の要求と応答を指定したりできます。</span><span class="sxs-lookup"><span data-stu-id="19a83-118">You can use the [TraceFlags enumeration](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.traceflags%28v=exchg.80%29.aspx) to specify values for EWS and for Autodiscover requests and responses.</span></span> 
  
## <a name="implementing-a-tracelistener-object"></a><span data-ttu-id="19a83-119">TraceListener オブジェクトを実装する</span><span class="sxs-lookup"><span data-stu-id="19a83-119">Implementing a TraceListener object</span></span>
<span data-ttu-id="19a83-120"><a name="bk_traceListener"> </a></span><span class="sxs-lookup"><span data-stu-id="19a83-120"><a name="bk_traceListener"> </a></span></span>

<span data-ttu-id="19a83-121">[Traceenabled](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.traceenabled%28v=exchg.80%29.aspx)プロパティを**true**に設定すると、XML 要求とアプリケーションに対する応答 (コンソールウィンドウなど) が出力されます。</span><span class="sxs-lookup"><span data-stu-id="19a83-121">You can set the [TraceEnabled](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.traceenabled%28v=exchg.80%29.aspx) property to **true** to output the XML requests and responses to your application, such as a console window.</span></span> <span data-ttu-id="19a83-122">トレース出力を制御してファイルに保存する場合は、 [TraceListener クラス](https://msdn.microsoft.com/library/system.diagnostics.tracelistener.aspx)オブジェクトを実装することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="19a83-122">If you want to control the trace output and save it to a file, we recommend that you implement a [TraceListener class](https://msdn.microsoft.com/library/system.diagnostics.tracelistener.aspx) object.</span></span> <span data-ttu-id="19a83-123">次のコード例は、 [ITraceListener](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itracelistener%28v=exchg.80%29.aspx)インターフェイスを実装し、トレースされた要求と応答を XML またはテキストファイルに格納する簡単なオブジェクトを示しています。</span><span class="sxs-lookup"><span data-stu-id="19a83-123">The following code example shows a simple object that implements the [ITraceListener](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itracelistener%28v=exchg.80%29.aspx) interface and stores the traced requests and responses in XML or text files.</span></span> 
  
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

## <a name="see-also"></a><span data-ttu-id="19a83-124">関連項目</span><span class="sxs-lookup"><span data-stu-id="19a83-124">See also</span></span>

- [<span data-ttu-id="19a83-125">Exchange で Web サービスの使用を開始する</span><span class="sxs-lookup"><span data-stu-id="19a83-125">Start using web services in Exchange</span></span>](start-using-web-services-in-exchange.md)
- [<span data-ttu-id="19a83-126">自動検出のエラー メッセージの処理</span><span class="sxs-lookup"><span data-stu-id="19a83-126">Handling Autodiscover error messages</span></span>](handling-autodiscover-error-messages.md)    
- [<span data-ttu-id="19a83-127">EWS マネージ API アセンブリの参照</span><span class="sxs-lookup"><span data-stu-id="19a83-127">Reference the EWS Managed API assembly</span></span>](how-to-reference-the-ews-managed-api-assembly.md)    
- [<span data-ttu-id="19a83-128">EWS マネージ API を使用して EWS と通信する</span><span class="sxs-lookup"><span data-stu-id="19a83-128">Communicate with EWS by using the EWS Managed API</span></span>](how-to-communicate-with-ews-by-using-the-ews-managed-api.md)
    

