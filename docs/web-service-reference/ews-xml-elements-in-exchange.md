---
title: Exchange での EWS の XML 要素
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Exchange
api_type:
- schema
ms.assetid: 4653466a-a596-456f-bbff-7da4ef1d18d3
description: Exchange EWS XML のリファレンス情報について要素を検索します。
ms.openlocfilehash: 046a985ae4696616d28a0891ffe0aa8cc0552307
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760354"
---
# <a name="ews-xml-elements-in-exchange"></a><span data-ttu-id="31ade-103">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="31ade-103">EWS XML elements in Exchange</span></span>

<span data-ttu-id="31ade-104">Exchange EWS XML のリファレンス情報について要素を検索します。</span><span class="sxs-lookup"><span data-stu-id="31ade-104">Find reference information for the EWS XML elements in Exchange.</span></span>
  
<span data-ttu-id="31ade-105">Exchange Web サービス (EWS) では、SOAP ベースの web サービス、クライアントとサーバー間で送信される要求と応答メッセージは、XML 要素で構成することを意味します。</span><span class="sxs-lookup"><span data-stu-id="31ade-105">Exchange Web Services (EWS) is a SOAP-based web service, which means that the request and response messages that are sent between the client and server are comprised of XML elements.</span></span> <span data-ttu-id="31ade-106">このセクションのドキュメントは、クライアントとサーバー間で送信される XML インスタンスに基づいています。</span><span class="sxs-lookup"><span data-stu-id="31ade-106">The documentation in this section is based on the XML instances that are sent between the client and server.</span></span> <span data-ttu-id="31ade-107">XML インスタンスは、EWS をホストする仮想ディレクトリに配置されている WSDL およびスキーマ ファイルで定義されます。</span><span class="sxs-lookup"><span data-stu-id="31ade-107">The XML instances are defined in the WSDL and schema files that are located in the virtual directory that hosts EWS.</span></span> <span data-ttu-id="31ade-108">次の Url を使用して、WSDL ファイルとスキーマ ファイルを参照することが認証されたユーザーの場合は、場所\<yourclientaccessserver\>は、クライアント アクセス サーバーの名前。</span><span class="sxs-lookup"><span data-stu-id="31ade-108">If you are an authenticated user, you can browse to the WSDL and schema files by using the following URLs, where \<yourclientaccessserver\> is the name of your Client Access server:</span></span>
  
- <span data-ttu-id="31ade-109">http://\<yourclientaccessserver\>.com/ews/services.wsdl: WSDL ファイルの場所です。</span><span class="sxs-lookup"><span data-stu-id="31ade-109">http://\<yourclientaccessserver\>.com/ews/services.wsdl — The location of the WSDL file.</span></span>
    
- <span data-ttu-id="31ade-110">http://\<yourclientaccessserver\>.com/ews/messages.xsd-メッセージのスキーマの場所です。</span><span class="sxs-lookup"><span data-stu-id="31ade-110">http://\<yourclientaccessserver\>.com/ews/messages.xsd — The location of the messages schema.</span></span>
    
- <span data-ttu-id="31ade-111">http://\<yourclientaccessserver\>.com/ews/types.xsd-タイプのスキーマの場所です。</span><span class="sxs-lookup"><span data-stu-id="31ade-111">http://\<yourclientaccessserver\>.com/ews/types.xsd — The location of the types schema.</span></span>
    
<span data-ttu-id="31ade-112">EWS の XML 要素を記述するスキーマ ファイルは、要求-応答メッセージのやり取りの可能な XML データ構造の全般的なロードマップを提供します。</span><span class="sxs-lookup"><span data-stu-id="31ade-112">The schema files that describe the EWS XML elements provide a general roadmap of the XML structure that is possible for request-response message interactions.</span></span> <span data-ttu-id="31ade-113">クライアントとサーバー間で送信される実際の XML 構造は、操作と呼ばれる、要求された情報をサーバー側の設定によって異なります。</span><span class="sxs-lookup"><span data-stu-id="31ade-113">The actual XML structure that is sent between client and server varies according to the operation that is called, the information requested, and the server-side settings.</span></span>
  
<span data-ttu-id="31ade-114">EWS の WSDL ファイル、services.wsdl、完全に準拠していない標準の WSDL サービスの WSDL 定義が含まれていないためです。</span><span class="sxs-lookup"><span data-stu-id="31ade-114">The EWS WSDL file, services.wsdl, does not fully conform to the WSDL standard because it does not include a WSDL service definition.</span></span> <span data-ttu-id="31ade-115">これは、EWS が定義済みのアドレスを持つコンピューターでホストされるように設計されていませんので。</span><span class="sxs-lookup"><span data-stu-id="31ade-115">This is because EWS is not designed to be hosted on a computer that has a predefined address.</span></span> <span data-ttu-id="31ade-116">自動検出サービスを使用すると、EWS のエンドポイントのアドレスを取得します。</span><span class="sxs-lookup"><span data-stu-id="31ade-116">You can use the Autodiscover service to get the EWS endpoint address.</span></span> <span data-ttu-id="31ade-117">いくつかクライアント側オブジェクト モデルのジェネレーターでは、WSDL を解析し、WSDL ファイルにはサービスの WSDL 定義が含まれていないために、エラー状態が発生することができます。</span><span class="sxs-lookup"><span data-stu-id="31ade-117">Some client-side object model generators parse the WSDL and can encounter an error condition because the WSDL file does not contain a WSDL service definition.</span></span> <span data-ttu-id="31ade-118">オブジェクト モデルのジェネレーターには、エラーが発生すると、サービスの WSDL 定義のプレース ホルダーを挿入できます。</span><span class="sxs-lookup"><span data-stu-id="31ade-118">If your object model generator encounters an error, you can insert a placeholder WSDL service definition.</span></span>
  
> [!TIP]
> <span data-ttu-id="31ade-119">アプリケーションを開発するのには.NET Framework を使用する場合、オブジェクト モデルのジェネレーターではなく、 [EWS のマネージ API](http://aka.ms/ews-managed-api-readme)を使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="31ade-119">If you are using the .NET Framework to develop your application, we recommend that you use the [EWS Managed API](http://aka.ms/ews-managed-api-readme), rather than an object model generator.</span></span> <span data-ttu-id="31ade-120">EWS のマネージ API では、EWS の XML を逆シリアル化とシリアル化を処理するために使用するオブジェクト モデルを提供します。</span><span class="sxs-lookup"><span data-stu-id="31ade-120">The EWS Managed API provides an easy-to-use object model to handle the serialization and deserialization of the EWS XML.</span></span> <span data-ttu-id="31ade-121">詳細については、 [EWS のマネージ API のクライアント アプリケーションを使い始める](http://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="31ade-121">For more information, see [Get started with EWS Managed API client applications](http://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx).</span></span> 
  
<span data-ttu-id="31ade-122">Messages.xsd スキーマ ファイルには、SOAP 本文内の最上位の要素の要素定義が含まれています。</span><span class="sxs-lookup"><span data-stu-id="31ade-122">The messages.xsd schema file contains the element definitions for the top-level elements in the SOAP body.</span></span> <span data-ttu-id="31ade-123">エラー応答コードを除いては、messages.xsd 内の定義のほとんどは、操作に固有です。</span><span class="sxs-lookup"><span data-stu-id="31ade-123">With the exception of the error response codes, most of the definitions in messages.xsd are specific to an operation.</span></span> <span data-ttu-id="31ade-124">Types.xsd スキーマには、SOAP ヘッダーの定義と操作の間で共有されているすべての一般的な定義が含まれています。</span><span class="sxs-lookup"><span data-stu-id="31ade-124">The types.xsd schema contains the definitions for the SOAP headers and all the common definitions that are shared across operations.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="31ade-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="31ade-125">See also</span></span>

- <span data-ttu-id="31ade-126">
  [Exchange 用 EWS リファレンス](ews-reference-for-exchange.md)</span><span class="sxs-lookup"><span data-stu-id="31ade-126">[EWS reference for Exchange](ews-reference-for-exchange.md)</span></span>
- [<span data-ttu-id="31ade-127">Exchange での EWS の操作</span><span class="sxs-lookup"><span data-stu-id="31ade-127">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
- [<span data-ttu-id="31ade-128">Exchange、EWS の管理 API、EWS、および web サービスを探索します。</span><span class="sxs-lookup"><span data-stu-id="31ade-128">Explore the EWS Managed API, EWS, and web services in Exchange</span></span>](../exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)
- [<span data-ttu-id="31ade-129">Exchange で Web サービスの使用を開始する</span><span class="sxs-lookup"><span data-stu-id="31ade-129">Start using web services in Exchange</span></span>](../exchange-web-services/start-using-web-services-in-exchange.md)
- [<span data-ttu-id="31ade-130">Exchange の自動検出</span><span class="sxs-lookup"><span data-stu-id="31ade-130">Autodiscover for Exchange</span></span>](../exchange-web-services/autodiscover-for-exchange.md)
    

