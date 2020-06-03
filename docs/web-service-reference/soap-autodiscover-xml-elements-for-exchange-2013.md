---
title: Exchange 2013 の SOAP 自動検出 XML 要素
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: ae18a5b3-ae44-4cff-8654-db8028565e01
description: Exchange の SOAP 自動検出 web サービスの XML 要素参照情報を検索します。
ms.openlocfilehash: 3b88429488dbecd4ed7c3adf56462f34fa0d4b17
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465185"
---
# <a name="soap-autodiscover-xml-elements-for-exchange-2013"></a><span data-ttu-id="982a6-103">Exchange 2013 の SOAP 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="982a6-103">SOAP Autodiscover XML elements for Exchange 2013</span></span>

<span data-ttu-id="982a6-104">Exchange の SOAP 自動検出 web サービスの XML 要素参照情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="982a6-104">Find XML element reference information for the SOAP Autodiscover web service in Exchange.</span></span>
  
<span data-ttu-id="982a6-105">このセクションのドキュメントは、クライアントとサーバー間で送信される SOAP 自動検出 XML 要素のインスタンスに基づいています。</span><span class="sxs-lookup"><span data-stu-id="982a6-105">The documentation in this section is based on the SOAP Autodiscover XML element instances that are sent between the client and server.</span></span> <span data-ttu-id="982a6-106">この XML インスタンスドキュメントは、SOAP 自動検出サービスをホストする仮想ディレクトリにある WSDL ファイルおよびスキーマファイルに基づいています。</span><span class="sxs-lookup"><span data-stu-id="982a6-106">This XML instance documentation is based on the WSDL and schema files that are located in the virtual directory that hosts the SOAP Autodiscover service.</span></span> <span data-ttu-id="982a6-107">認証されたユーザーは、次のいずれかのような URL を使用して、WSDL およびスキーマファイルを参照できます。</span><span class="sxs-lookup"><span data-stu-id="982a6-107">Authenticated users can browse to the WSDL and schema files by using a URL that is similar to one of the following:</span></span>
  
- <span data-ttu-id="982a6-108">WSDL ファイルの場所を指定し `http://<yourclientaccessserver>.com/autodiscover/services.wsdl` ます。`http://autodiscover.<yourclientaccessserver>.com/autodiscover/services.wsdl`</span><span class="sxs-lookup"><span data-stu-id="982a6-108">The location of the WSDL file: `http://<yourclientaccessserver>.com/autodiscover/services.wsdl` or `http://autodiscover.<yourclientaccessserver>.com/autodiscover/services.wsdl`</span></span>
    
- <span data-ttu-id="982a6-109">メッセージスキーマの場所を指定し `http://<yourclientaccessserver>.com/autodiscover/messages.xsd` ます。`http://autodiscover.<yourclientaccessserver>.com/autodiscover/messages.xsd`</span><span class="sxs-lookup"><span data-stu-id="982a6-109">The location of the messages schema: `http://<yourclientaccessserver>.com/autodiscover/messages.xsd` or `http://autodiscover.<yourclientaccessserver>.com/autodiscover/messages.xsd`</span></span> 
    
<span data-ttu-id="982a6-110">SOAP 自動検出の WSDL ファイルおよびスキーマファイルの場所は、Exchange のインストールによって異なります。</span><span class="sxs-lookup"><span data-stu-id="982a6-110">The location of the SOAP Autodiscover WSDL and schema files varies based on the Exchange installation.</span></span>
  
<span data-ttu-id="982a6-111">メッセージ .xsd スキーマファイルは、自動検出 SOAP ヘッダーと SOAP 本文で送信できる XML 要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="982a6-111">The messages.xsd schema file describes the XML elements that can be sent in an Autodiscover SOAP header and SOAP body.</span></span> <span data-ttu-id="982a6-112">このファイルは、特定の要求と応答メッセージの相互作用に対して XML 構造をどのように使用できるかについての一般的なロードマップを提供します。</span><span class="sxs-lookup"><span data-stu-id="982a6-112">This file provides a general roadmap of what the XML structure can be for a given request-response message interaction.</span></span> <span data-ttu-id="982a6-113">クライアントとサーバー間で送信される実際の XML 構造は、オプションと使用されるコンテキストに基づいています。</span><span class="sxs-lookup"><span data-stu-id="982a6-113">The actual XML structure that is sent between the client and server is based on the options and the context in which it is used.</span></span> <span data-ttu-id="982a6-114">スキーマファイルでは、可能な XML が定義されています。</span><span class="sxs-lookup"><span data-stu-id="982a6-114">The schema files define what XML is possible.</span></span> <span data-ttu-id="982a6-115">ネットワーク上で送信される実際の XML の範囲は、呼び出された操作、要求された情報、およびサーバー側の設定に基づいています。</span><span class="sxs-lookup"><span data-stu-id="982a6-115">The actual range of XML that is sent over the wire is based on which operation is called, the requested information, and the server-side settings.</span></span> 
  
## <a name="related-sections"></a><span data-ttu-id="982a6-116">関連情報</span><span class="sxs-lookup"><span data-stu-id="982a6-116">Related sections</span></span>

- [<span data-ttu-id="982a6-117">Exchange 用 SOAP 自動検出 Web サービス リファレンス</span><span class="sxs-lookup"><span data-stu-id="982a6-117">SOAP Autodiscover web service reference for Exchange</span></span>](soap-autodiscover-web-service-reference-for-exchange.md)    
- [<span data-ttu-id="982a6-118">Exchange 用 EWS リファレンス</span><span class="sxs-lookup"><span data-stu-id="982a6-118">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)    
- [<span data-ttu-id="982a6-119">Exchange 用ユニファイドメッセージング web サービスのリファレンス</span><span class="sxs-lookup"><span data-stu-id="982a6-119">Unified Messaging web service reference for Exchange</span></span>](unified-messaging-web-service-reference-for-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="982a6-120">関連項目</span><span class="sxs-lookup"><span data-stu-id="982a6-120">See also</span></span>

- [<span data-ttu-id="982a6-121">Exchange 用自動検出 Web サービス リファレンス</span><span class="sxs-lookup"><span data-stu-id="982a6-121">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
- [<span data-ttu-id="982a6-122">Exchange の自動検出</span><span class="sxs-lookup"><span data-stu-id="982a6-122">Autodiscover for Exchange</span></span>](../exchange-web-services/autodiscover-for-exchange.md)
- [<span data-ttu-id="982a6-123">Exchange で Web サービスの使用を開始する</span><span class="sxs-lookup"><span data-stu-id="982a6-123">Start using web services in Exchange</span></span>](../exchange-web-services/start-using-web-services-in-exchange.md)
    

