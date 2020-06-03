---
title: Exchange の EWS XML 要素
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
api_name:
- Exchange
api_type:
- schema
ms.assetid: 4653466a-a596-456f-bbff-7da4ef1d18d3
description: Exchange 内の EWS XML 要素に関する参照情報を検索します。
localization_priority: Priority
ms.openlocfilehash: 29b90ad137141e30484ef804b6fcb6bb049ef3e8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526117"
---
# <a name="ews-xml-elements-in-exchange"></a><span data-ttu-id="0080e-103">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="0080e-103">EWS XML elements in Exchange</span></span>

<span data-ttu-id="0080e-104">Exchange 内の EWS XML 要素に関する参照情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="0080e-104">Find reference information for the EWS XML elements in Exchange.</span></span>
  
<span data-ttu-id="0080e-105">Exchange Web サービス (EWS) は SOAP ベースの web サービスです。これは、クライアントとサーバー間で送信される要求メッセージと応答メッセージが XML 要素で構成されることを意味します。</span><span class="sxs-lookup"><span data-stu-id="0080e-105">Exchange Web Services (EWS) is a SOAP-based web service, which means that the request and response messages that are sent between the client and server are comprised of XML elements.</span></span> <span data-ttu-id="0080e-106">このセクションのドキュメントは、クライアントとサーバー間で送信される XML インスタンスに基づいています。</span><span class="sxs-lookup"><span data-stu-id="0080e-106">The documentation in this section is based on the XML instances that are sent between the client and server.</span></span> <span data-ttu-id="0080e-107">XML インスタンスは、EWS をホストする仮想ディレクトリにある WSDL ファイルおよびスキーマファイルで定義されています。</span><span class="sxs-lookup"><span data-stu-id="0080e-107">The XML instances are defined in the WSDL and schema files that are located in the virtual directory that hosts EWS.</span></span> <span data-ttu-id="0080e-108">認証されたユーザーの場合は、次の Url を使用して WSDL およびスキーマファイルを参照でき \<yourclientaccessserver\> ます。ここで、はクライアントアクセスサーバーの名前です。</span><span class="sxs-lookup"><span data-stu-id="0080e-108">If you are an authenticated user, you can browse to the WSDL and schema files by using the following URLs, where \<yourclientaccessserver\> is the name of your Client Access server:</span></span>
  
- <span data-ttu-id="0080e-109">http:// \<yourclientaccessserver\> /ews/サービス wsdl ファイルの場所を指定します。</span><span class="sxs-lookup"><span data-stu-id="0080e-109">http://\<yourclientaccessserver\>.com/ews/services.wsdl — The location of the WSDL file.</span></span>
    
- <span data-ttu-id="0080e-110">http:// \<yourclientaccessserver\> /ews/メッセージ .xsd-メッセージスキーマの場所。</span><span class="sxs-lookup"><span data-stu-id="0080e-110">http://\<yourclientaccessserver\>.com/ews/messages.xsd — The location of the messages schema.</span></span>
    
- <span data-ttu-id="0080e-111">http:// \<yourclientaccessserver\> /ews/型 .xsd-types スキーマの場所。</span><span class="sxs-lookup"><span data-stu-id="0080e-111">http://\<yourclientaccessserver\>.com/ews/types.xsd — The location of the types schema.</span></span>
    
<span data-ttu-id="0080e-112">EWS XML 要素を記述するスキーマファイルは、要求と応答メッセージの相互作用に使用できる XML 構造の一般的なロードマップを提供します。</span><span class="sxs-lookup"><span data-stu-id="0080e-112">The schema files that describe the EWS XML elements provide a general roadmap of the XML structure that is possible for request-response message interactions.</span></span> <span data-ttu-id="0080e-113">クライアントとサーバー間で送信される実際の XML 構造は、呼び出される操作、要求された情報、およびサーバー側の設定によって異なります。</span><span class="sxs-lookup"><span data-stu-id="0080e-113">The actual XML structure that is sent between client and server varies according to the operation that is called, the information requested, and the server-side settings.</span></span>
  
<span data-ttu-id="0080e-114">EWS WSDL ファイルサービス wsdl は、wsdl 標準に完全に準拠していません。 wsdl サービス定義は含まれていません。</span><span class="sxs-lookup"><span data-stu-id="0080e-114">The EWS WSDL file, services.wsdl, does not fully conform to the WSDL standard because it does not include a WSDL service definition.</span></span> <span data-ttu-id="0080e-115">これは、EWS が事前に定義されたアドレスを持つコンピューターでホストされるように設計されていないためです。</span><span class="sxs-lookup"><span data-stu-id="0080e-115">This is because EWS is not designed to be hosted on a computer that has a predefined address.</span></span> <span data-ttu-id="0080e-116">自動検出サービスを使用して、EWS エンドポイントアドレスを取得できます。</span><span class="sxs-lookup"><span data-stu-id="0080e-116">You can use the Autodiscover service to get the EWS endpoint address.</span></span> <span data-ttu-id="0080e-117">一部のクライアント側オブジェクトモデルジェネレーターは、WSDL を解析し、wsdl ファイルに WSDL サービス定義が含まれていないため、エラーが発生することがあります。</span><span class="sxs-lookup"><span data-stu-id="0080e-117">Some client-side object model generators parse the WSDL and can encounter an error condition because the WSDL file does not contain a WSDL service definition.</span></span> <span data-ttu-id="0080e-118">オブジェクトモデルジェネレーターでエラーが発生した場合は、プレースホルダー WSDL サービス定義を挿入できます。</span><span class="sxs-lookup"><span data-stu-id="0080e-118">If your object model generator encounters an error, you can insert a placeholder WSDL service definition.</span></span>
  
> [!TIP]
> <span data-ttu-id="0080e-119">.NET Framework を使用してアプリケーションを開発している場合は、オブジェクトモデルジェネレーターではなく、 [EWS マネージ API](http://aka.ms/ews-managed-api-readme)を使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="0080e-119">If you are using the .NET Framework to develop your application, we recommend that you use the [EWS Managed API](http://aka.ms/ews-managed-api-readme), rather than an object model generator.</span></span> <span data-ttu-id="0080e-120">EWS マネージ API には、EWS XML のシリアル化と逆シリアル化を処理するための使いやすいオブジェクトモデルが用意されています。</span><span class="sxs-lookup"><span data-stu-id="0080e-120">The EWS Managed API provides an easy-to-use object model to handle the serialization and deserialization of the EWS XML.</span></span> <span data-ttu-id="0080e-121">詳細については、「 [EWS マネージ API クライアントアプリケーションの概要](https://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0080e-121">For more information, see [Get started with EWS Managed API client applications](https://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx).</span></span> 
  
<span data-ttu-id="0080e-122">メッセージ .xsd スキーマファイルには、SOAP 本文の最上位レベルの要素の要素定義が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0080e-122">The messages.xsd schema file contains the element definitions for the top-level elements in the SOAP body.</span></span> <span data-ttu-id="0080e-123">エラー応答コード以外の場合、メッセージ .xsd の定義のほとんどは操作に固有のものです。</span><span class="sxs-lookup"><span data-stu-id="0080e-123">With the exception of the error response codes, most of the definitions in messages.xsd are specific to an operation.</span></span> <span data-ttu-id="0080e-124">型 .xsd スキーマには、SOAP ヘッダーの定義と、操作間で共有されるすべての共通定義が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0080e-124">The types.xsd schema contains the definitions for the SOAP headers and all the common definitions that are shared across operations.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="0080e-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="0080e-125">See also</span></span>

- [<span data-ttu-id="0080e-126">Exchange 用 EWS リファレンス</span><span class="sxs-lookup"><span data-stu-id="0080e-126">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)
- [<span data-ttu-id="0080e-127">Exchange での EWS 操作</span><span class="sxs-lookup"><span data-stu-id="0080e-127">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
- [<span data-ttu-id="0080e-128">Exchange の EWS マネージ API、EWS、および Web サービスについて学ぶ</span><span class="sxs-lookup"><span data-stu-id="0080e-128">Explore the EWS Managed API, EWS, and web services in Exchange</span></span>](../exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)
- [<span data-ttu-id="0080e-129">Exchange で Web サービスの使用を開始する</span><span class="sxs-lookup"><span data-stu-id="0080e-129">Start using web services in Exchange</span></span>](../exchange-web-services/start-using-web-services-in-exchange.md)
- [<span data-ttu-id="0080e-130">Exchange の自動検出</span><span class="sxs-lookup"><span data-stu-id="0080e-130">Autodiscover for Exchange</span></span>](../exchange-web-services/autodiscover-for-exchange.md)
    

