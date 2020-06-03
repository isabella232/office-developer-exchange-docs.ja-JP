---
title: Exchange 用 POX 自動検出 Web サービス リファレンス
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 877152f0-f4b1-4f63-b2ce-924f4bdf2d20
description: Exchange の POX 自動検出サービスに関する参照情報を検索します。
ms.openlocfilehash: 3c0ca368f4427be7759e2db58fb418b4822dea8e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465654"
---
# <a name="pox-autodiscover-web-service-reference-for-exchange"></a><span data-ttu-id="223de-103">Exchange 用 POX 自動検出 Web サービス リファレンス</span><span class="sxs-lookup"><span data-stu-id="223de-103">POX Autodiscover web service reference for Exchange</span></span>

<span data-ttu-id="223de-104">Exchange の POX 自動検出サービスに関する参照情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="223de-104">Find reference information for the POX Autodiscover service in Exchange.</span></span>
  
<span data-ttu-id="223de-105">自動検出サービスは、アプリケーションが Exchange サーバーへの接続を作成するために使用する構成情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="223de-105">The Autodiscover service provides the configuration information that your application uses to create a connection to an Exchange server.</span></span> <span data-ttu-id="223de-106">"プレーン旧 XML" (POX) 自動検出サービスを使用すると、クライアントアプリケーションが Exchange に接続するために必要な設定を特定するために、XML ペイロードのみで構成されたメッセージを、それを囲む SOAP エンベロープを使用せずに送信できます。</span><span class="sxs-lookup"><span data-stu-id="223de-106">You can use the "plain old XML" (POX) Autodiscover service to send messages that consist only of XML payloads, without any enclosing SOAP envelopes, in order to locate the settings that a client application must have in order to connect to Exchange.</span></span>
  
> [!NOTE]
> <span data-ttu-id="223de-107">Exchange Server 2010 以降のバージョンの Exchange を対象とするクライアントでは、POX 自動検出サービスの代わりに SOAP 自動検出サービスを使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="223de-107">For clients that target versions of Exchange starting with Exchange Server 2010, we recommend that you use the SOAP Autodiscover service instead of the POX Autodiscover service.</span></span> <span data-ttu-id="223de-108">Exchange 2007 を対象とするクライアントは、POX 自動検出サービスを使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="223de-108">Clients that target Exchange 2007 have to use the POX Autodiscover service.</span></span> <span data-ttu-id="223de-109">.NET Framework を使用するクライアントには、堅牢で十分にテストされた POX 自動検出クライアントが含まれているため、EWS マネージ API を使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="223de-109">We recommend that clients that use the .NET Framework use the EWS Managed API because it contains a robust and well-tested POX Autodiscover client.</span></span> <span data-ttu-id="223de-110">EWS マネージ API の詳細については、「 [Ews マネージ api クライアントアプリケーションの概要](https://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="223de-110">For more information about the EWS Managed API, see [Get started with EWS Managed API client applications](https://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx).</span></span> 
  
<span data-ttu-id="223de-111">このセクションでは、POX 自動検出要求のリダイレクト時にクライアントとサーバー間で送信される XML 要素、および応答で返されるユーザー設定について説明します。</span><span class="sxs-lookup"><span data-stu-id="223de-111">This section provides information about the XML elements that are sent between the client and server during POX Autodiscover request redirections and the user settings that are returned in a response.</span></span> <span data-ttu-id="223de-112">XML 要素リファレンスには、要素が表す内容の概要と、要素を使用する可能性のある要素階層の説明が含まれています。</span><span class="sxs-lookup"><span data-stu-id="223de-112">The XML element reference contains summaries of what the elements represent and a description of the potential element hierarchies that use the element.</span></span> <span data-ttu-id="223de-113">このドキュメントでは、クライアントとサーバー間で送信される XML インスタンスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="223de-113">This documentation covers the XML instances that are sent between the client and server.</span></span> <span data-ttu-id="223de-114">POX 自動検出サービスには、明示的なスキーマがありません。</span><span class="sxs-lookup"><span data-stu-id="223de-114">The POX Autodiscover service does not have an explicit schema.</span></span>
  
<span data-ttu-id="223de-115">このセクションの記事では、POX 自動検出サービスを使用して自動検出構成情報を取得するために使用されるメッセージの例と説明を示します。</span><span class="sxs-lookup"><span data-stu-id="223de-115">The articles in this section provide examples and descriptions of the messages that are used to retrieve Autodiscover configuration information by using the POX Autodiscover service.</span></span> 
  
## <a name="in-this-section"></a><span data-ttu-id="223de-116">このセクションの内容</span><span class="sxs-lookup"><span data-stu-id="223de-116">In this section</span></span>
<span data-ttu-id="223de-117"><a name="bk_InThisSection"> </a></span><span class="sxs-lookup"><span data-stu-id="223de-117"><a name="bk_InThisSection"> </a></span></span>

- [<span data-ttu-id="223de-118">POX Exchange の自動検出要求</span><span class="sxs-lookup"><span data-stu-id="223de-118">POX Autodiscover request for Exchange</span></span>](pox-autodiscover-request-for-exchange.md)
    
- [<span data-ttu-id="223de-119">POX Exchange の自動検出応答</span><span class="sxs-lookup"><span data-stu-id="223de-119">POX Autodiscover response for Exchange</span></span>](pox-autodiscover-response-for-exchange.md)
    
- [<span data-ttu-id="223de-120">Exchange の POX 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="223de-120">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="223de-121">関連項目</span><span class="sxs-lookup"><span data-stu-id="223de-121">See also</span></span>

- [<span data-ttu-id="223de-122">Exchange 用自動検出 Web サービス リファレンス</span><span class="sxs-lookup"><span data-stu-id="223de-122">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
- [<span data-ttu-id="223de-123">Exchange の自動検出</span><span class="sxs-lookup"><span data-stu-id="223de-123">Autodiscover for Exchange</span></span>](../exchange-web-services/autodiscover-for-exchange.md)   
- [<span data-ttu-id="223de-124">Exchange 用 SOAP 自動検出 Web サービス リファレンス</span><span class="sxs-lookup"><span data-stu-id="223de-124">SOAP Autodiscover web service reference for Exchange</span></span>](soap-autodiscover-web-service-reference-for-exchange.md)
- [<span data-ttu-id="223de-125">Exchange で Web サービスの使用を開始する</span><span class="sxs-lookup"><span data-stu-id="223de-125">Start using web services in Exchange</span></span>](../exchange-web-services/start-using-web-services-in-exchange.md)
    

