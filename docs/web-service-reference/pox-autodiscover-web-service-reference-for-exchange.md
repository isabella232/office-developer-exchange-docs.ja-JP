---
title: Exchange の POX の自動検出 web サービスの参照
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 877152f0-f4b1-4f63-b2ce-924f4bdf2d20
description: Exchange POX の自動検出サービスに関するリファレンス情報を検索します。
ms.openlocfilehash: a8797fe714fd23049094c3ec2475b93fec4282c0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832867"
---
# <a name="pox-autodiscover-web-service-reference-for-exchange"></a><span data-ttu-id="3d3bb-103">Exchange の POX の自動検出 web サービスの参照</span><span class="sxs-lookup"><span data-stu-id="3d3bb-103">POX Autodiscover web service reference for Exchange</span></span>

<span data-ttu-id="3d3bb-104">Exchange POX の自動検出サービスに関するリファレンス情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="3d3bb-104">Find reference information for the POX Autodiscover service in Exchange.</span></span>
  
<span data-ttu-id="3d3bb-105">自動検出サービスは、Exchange サーバーへの接続を作成するアプリケーションで使用される構成情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="3d3bb-105">The Autodiscover service provides the configuration information that your application uses to create a connection to an Exchange server.</span></span> <span data-ttu-id="3d3bb-106">"標準古い XML"を使用することができます (POX) の自動検出サービスを Exchange に接続するためにクライアント アプリケーションに必要な設定を見つけるためにせず、それを囲む、SOAP エンベロープの XML ペイロードのみを含むメッセージを送信します。</span><span class="sxs-lookup"><span data-stu-id="3d3bb-106">You can use the "plain old XML" (POX) Autodiscover service to send messages that consist only of XML payloads, without any enclosing SOAP envelopes, in order to locate the settings that a client application must have in order to connect to Exchange.</span></span>
  
> [!NOTE]
> <span data-ttu-id="3d3bb-107">バージョンの Exchange が Exchange Server 2010 で始まるを対象とするクライアントの場合は、POX の自動検出サービスではなく、SOAP の自動検出サービスを使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="3d3bb-107">For clients that target versions of Exchange starting with Exchange Server 2010, we recommend that you use the SOAP Autodiscover service instead of the POX Autodiscover service.</span></span> <span data-ttu-id="3d3bb-108">Exchange 2007 を対象とするクライアントでは、POX の自動検出サービスを使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3d3bb-108">Clients that target Exchange 2007 have to use the POX Autodiscover service.</span></span> <span data-ttu-id="3d3bb-109">.NET Framework を使用して、クライアントは、堅牢で十分にテストされた自動検出の POX クライアントが含まれているため、EWS のマネージ API を使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="3d3bb-109">We recommend that clients that use the .NET Framework use the EWS Managed API because it contains a robust and well-tested POX Autodiscover client.</span></span> <span data-ttu-id="3d3bb-110">EWS のマネージ API の詳細については、 [EWS のマネージ API のクライアント アプリケーションを使い始める](http://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3d3bb-110">For more information about the EWS Managed API, see [Get started with EWS Managed API client applications](http://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx).</span></span> 
  
<span data-ttu-id="3d3bb-111">このセクションでは、POX の自動検出要求のリダイレクトと、応答で返されるユーザーの設定中にクライアントとサーバー間で送信される XML 要素に関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="3d3bb-111">This section provides information about the XML elements that are sent between the client and server during POX Autodiscover request redirections and the user settings that are returned in a response.</span></span> <span data-ttu-id="3d3bb-112">XML 要素の参照には、要素が表す内容の概要と要素を使用している潜在的な要素階層の説明が含まれています。</span><span class="sxs-lookup"><span data-stu-id="3d3bb-112">The XML element reference contains summaries of what the elements represent and a description of the potential element hierarchies that use the element.</span></span> <span data-ttu-id="3d3bb-113">このドキュメントでは、クライアントとサーバー間で送信される XML インスタンスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="3d3bb-113">This documentation covers the XML instances that are sent between the client and server.</span></span> <span data-ttu-id="3d3bb-114">POX の自動検出サービスには、明示的なスキーマがありません。</span><span class="sxs-lookup"><span data-stu-id="3d3bb-114">The POX Autodiscover service does not have an explicit schema.</span></span>
  
<span data-ttu-id="3d3bb-115">このセクションの記事では、POX の自動検出サービスを使用して、自動検出の構成情報を取得するために使用されるメッセージの説明や例を提供します。</span><span class="sxs-lookup"><span data-stu-id="3d3bb-115">The articles in this section provide examples and descriptions of the messages that are used to retrieve Autodiscover configuration information by using the POX Autodiscover service.</span></span> 
  
## <a name="in-this-section"></a><span data-ttu-id="3d3bb-116">このセクションの内容</span><span class="sxs-lookup"><span data-stu-id="3d3bb-116">In this section</span></span>
<span data-ttu-id="3d3bb-117"><a name="bk_InThisSection"> </a></span><span class="sxs-lookup"><span data-stu-id="3d3bb-117"></span></span>

- [<span data-ttu-id="3d3bb-118">POX の自動検出要求の交換</span><span class="sxs-lookup"><span data-stu-id="3d3bb-118">POX Autodiscover request for Exchange</span></span>](pox-autodiscover-request-for-exchange.md)
    
- [<span data-ttu-id="3d3bb-119">POX Exchange の自動検出の応答</span><span class="sxs-lookup"><span data-stu-id="3d3bb-119">POX Autodiscover response for Exchange</span></span>](pox-autodiscover-response-for-exchange.md)
    
- [<span data-ttu-id="3d3bb-120">交換の POX の自動検出の XML 要素</span><span class="sxs-lookup"><span data-stu-id="3d3bb-120">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="3d3bb-121">関連項目</span><span class="sxs-lookup"><span data-stu-id="3d3bb-121">See also</span></span>

- [<span data-ttu-id="3d3bb-122">Exchange の自動検出 web サービスの参照</span><span class="sxs-lookup"><span data-stu-id="3d3bb-122">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
- [<span data-ttu-id="3d3bb-123">Exchange の自動検出</span><span class="sxs-lookup"><span data-stu-id="3d3bb-123">Autodiscover for Exchange</span></span>](../exchange-web-services/autodiscover-for-exchange.md)   
- [<span data-ttu-id="3d3bb-124">Exchange の自動検出 web サービスの参照が SOAP します。</span><span class="sxs-lookup"><span data-stu-id="3d3bb-124">SOAP Autodiscover web service reference for Exchange</span></span>](soap-autodiscover-web-service-reference-for-exchange.md)
- [<span data-ttu-id="3d3bb-125">Exchange で Web サービスの使用を開始する</span><span class="sxs-lookup"><span data-stu-id="3d3bb-125">Start using web services in Exchange</span></span>](../exchange-web-services/start-using-web-services-in-exchange.md)
    

