---
title: Exchange 2013 の自動検出の XML 要素を SOAP
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: ae18a5b3-ae44-4cff-8654-db8028565e01
description: Exchange SOAP の自動検出 web サービスの XML 要素のリファレンス情報を検索します。
ms.openlocfilehash: 7201ef33060691df70b63d06b2045e1120b0610f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833517"
---
# <a name="soap-autodiscover-xml-elements-for-exchange-2013"></a><span data-ttu-id="20773-103">Exchange 2013 の自動検出の XML 要素を SOAP</span><span class="sxs-lookup"><span data-stu-id="20773-103">SOAP Autodiscover XML elements for Exchange 2013</span></span>

<span data-ttu-id="20773-104">Exchange SOAP の自動検出 web サービスの XML 要素のリファレンス情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="20773-104">Find XML element reference information for the SOAP Autodiscover web service in Exchange.</span></span>
  
<span data-ttu-id="20773-105">このセクションのドキュメントは、クライアントとサーバー間で送信される SOAP の自動検出の XML の要素インスタンスに基づいています。</span><span class="sxs-lookup"><span data-stu-id="20773-105">The documentation in this section is based on the SOAP Autodiscover XML element instances that are sent between the client and server.</span></span> <span data-ttu-id="20773-106">この XML インスタンス ドキュメントは、SOAP の自動検出サービスをホストする仮想ディレクトリに配置されている WSDL およびスキーマ ファイルに基づいています。</span><span class="sxs-lookup"><span data-stu-id="20773-106">This XML instance documentation is based on the WSDL and schema files that are located in the virtual directory that hosts the SOAP Autodiscover service.</span></span> <span data-ttu-id="20773-107">認証されたユーザーはことができます、次のいずれかのような URL を使用して、WSDL ファイルとスキーマ ファイルを参照してください。</span><span class="sxs-lookup"><span data-stu-id="20773-107">Authenticated users can browse to the WSDL and schema files by using a URL that is similar to one of the following:</span></span>
  
- <span data-ttu-id="20773-108">http://\<yourclientaccessserver\>.com/autodiscover/services.wsdl またはhttp://autodiscover.\<yourclientaccessserver\>.com/autodiscover/services.wsdl: WSDL ファイルの場所です。</span><span class="sxs-lookup"><span data-stu-id="20773-108">http://\<yourclientaccessserver\>.com/autodiscover/services.wsdl or http://autodiscover.\<yourclientaccessserver\>.com/autodiscover/services.wsdl — The location of the WSDL file.</span></span>
    
- <span data-ttu-id="20773-109">http://\<yourclientaccessserver\>.com/autodiscover/messages.xsd またはhttp://autodiscover.\<yourclientaccessserver\>.com/autodiscover/messages.xsd— メッセージのスキーマの場所です。</span><span class="sxs-lookup"><span data-stu-id="20773-109">http://\<yourclientaccessserver\>.com/autodiscover/messages.xsd or http://autodiscover.\<yourclientaccessserver\>.com/autodiscover/messages.xsd — The location of the messages schema.</span></span>
    
<span data-ttu-id="20773-110">SOAP の自動検出の WSDL ファイルとスキーマ ファイルの場所は、Exchange のインストールによって異なります。</span><span class="sxs-lookup"><span data-stu-id="20773-110">The location of the SOAP Autodiscover WSDL and schema files varies based on the Exchange installation.</span></span>
  
<span data-ttu-id="20773-111">Messages.xsd スキーマ ファイルでは、自動検出の SOAP ヘッダーと SOAP 本体に送信される XML 要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="20773-111">The messages.xsd schema file describes the XML elements that can be sent in an Autodiscover SOAP header and SOAP body.</span></span> <span data-ttu-id="20773-112">このファイルは、特定の要求-応答のメッセージのやり取りをすることができます [XML データ構造の全般的なロードマップを提供します。</span><span class="sxs-lookup"><span data-stu-id="20773-112">This file provides a general roadmap of what the XML structure can be for a given request-response message interaction.</span></span> <span data-ttu-id="20773-113">クライアントとサーバー間で送信される実際の XML 構造は、オプションとそれが使用されているコンテキストに基づきます。</span><span class="sxs-lookup"><span data-stu-id="20773-113">The actual XML structure that is sent between the client and server is based on the options and the context in which it is used.</span></span> <span data-ttu-id="20773-114">スキーマ ファイルは、どのような XML が使用可能なを定義します。</span><span class="sxs-lookup"><span data-stu-id="20773-114">The schema files define what XML is possible.</span></span> <span data-ttu-id="20773-115">実際の範囲の XML をネットワーク経由で送信されるは、どの操作が呼び出されると、要求された情報、およびサーバー側の設定に基づいています。</span><span class="sxs-lookup"><span data-stu-id="20773-115">The actual range of XML that is sent over the wire is based on which operation is called, the requested information, and the server-side settings.</span></span> 
  
## <a name="related-sections"></a><span data-ttu-id="20773-116">関連セクション</span><span class="sxs-lookup"><span data-stu-id="20773-116">Related sections</span></span>
<span data-ttu-id="20773-117"><a name="bk_RelatedSections"> </a></span><span class="sxs-lookup"><span data-stu-id="20773-117"></span></span>

- [<span data-ttu-id="20773-118">Exchange の自動検出 web サービスの参照が SOAP します。</span><span class="sxs-lookup"><span data-stu-id="20773-118">SOAP Autodiscover web service reference for Exchange</span></span>](soap-autodiscover-web-service-reference-for-exchange.md)
    
- <span data-ttu-id="20773-119">
  [Exchange 用 EWS リファレンス](ews-reference-for-exchange.md)</span><span class="sxs-lookup"><span data-stu-id="20773-119">[EWS reference for Exchange](ews-reference-for-exchange.md)</span></span>
    
- [<span data-ttu-id="20773-120">Exchange ユニファイド メッセージング web サービス リファレンス</span><span class="sxs-lookup"><span data-stu-id="20773-120">Unified Messaging web service reference for Exchange</span></span>](unified-messaging-web-service-reference-for-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="20773-121">関連項目</span><span class="sxs-lookup"><span data-stu-id="20773-121">See also</span></span>

- [<span data-ttu-id="20773-122">Exchange の自動検出 web サービスの参照</span><span class="sxs-lookup"><span data-stu-id="20773-122">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
- [<span data-ttu-id="20773-123">Exchange の自動検出</span><span class="sxs-lookup"><span data-stu-id="20773-123">Autodiscover for Exchange</span></span>](../exchange-web-services/autodiscover-for-exchange.md)
- [<span data-ttu-id="20773-124">Exchange で Web サービスの使用を開始する</span><span class="sxs-lookup"><span data-stu-id="20773-124">Start using web services in Exchange</span></span>](../exchange-web-services/start-using-web-services-in-exchange.md)
    

