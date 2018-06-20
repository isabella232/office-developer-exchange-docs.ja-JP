---
title: TokenType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 83c650eb-7ab8-480c-a7c9-df60072ee042
description: TokenType 要素では、トークンの種類を指定します。
ms.openlocfilehash: 5c8e880f035ed74776a7c77e4b4e60ca46d66d4e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839719"
---
# <a name="tokentype"></a><span data-ttu-id="b7bf4-103">TokenType</span><span class="sxs-lookup"><span data-stu-id="b7bf4-103">TokenType</span></span>

<span data-ttu-id="b7bf4-104">**TokenType**要素では、トークンの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="b7bf4-104">The **TokenType** element specifies the type of token.</span></span> 
  
```XML
<TokenType> CallerIdentity | ExtensionCallback | ScopedToken </TokenType>
```

 <span data-ttu-id="b7bf4-105">**ClientAccessTokenTypeType**</span><span class="sxs-lookup"><span data-stu-id="b7bf4-105">**ClientAccessTokenTypeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b7bf4-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="b7bf4-106">Attributes and elements</span></span>

<span data-ttu-id="b7bf4-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b7bf4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b7bf4-108">属性</span><span class="sxs-lookup"><span data-stu-id="b7bf4-108">Attributes</span></span>

<span data-ttu-id="b7bf4-109">なし。</span><span class="sxs-lookup"><span data-stu-id="b7bf4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b7bf4-110">子要素</span><span class="sxs-lookup"><span data-stu-id="b7bf4-110">Child elements</span></span>

<span data-ttu-id="b7bf4-111">なし。</span><span class="sxs-lookup"><span data-stu-id="b7bf4-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b7bf4-112">親要素</span><span class="sxs-lookup"><span data-stu-id="b7bf4-112">Parent elements</span></span>

<span data-ttu-id="b7bf4-113">[TokenRequest](tokenrequest.md) | [トークン](token.md)</span><span class="sxs-lookup"><span data-stu-id="b7bf4-113">[TokenRequest](tokenrequest.md) | [Token](token.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="b7bf4-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="b7bf4-114">Text value</span></span>

<span data-ttu-id="b7bf4-115">**TokenType**要素のテキスト値は、トークンの型です。</span><span class="sxs-lookup"><span data-stu-id="b7bf4-115">The text value of the **TokenType** element is the token type.</span></span> <span data-ttu-id="b7bf4-116">**CallerIdentity**のテキスト値は、トークンは、呼び出し元 id のトークンであることを示します。</span><span class="sxs-lookup"><span data-stu-id="b7bf4-116">The text value of **CallerIdentity** indicates that the token is a caller identity token.</span></span> <span data-ttu-id="b7bf4-117">**ExtensionCallback**のテキスト値は、トークンが、拡張機能コールバックであることを示します。</span><span class="sxs-lookup"><span data-stu-id="b7bf4-117">The text value of **ExtensionCallback** indicates that the token is for an extension callback.</span></span> <span data-ttu-id="b7bf4-118">**ScopedToken**のテキスト値は、クライアントのアクセス トークンがスコープのトークンであることを示します。</span><span class="sxs-lookup"><span data-stu-id="b7bf4-118">The text value of **ScopedToken** indicates that the client access token is a scoped token.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="b7bf4-119">備考</span><span class="sxs-lookup"><span data-stu-id="b7bf4-119">Remarks</span></span>

<span data-ttu-id="b7bf4-120">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="b7bf4-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b7bf4-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="b7bf4-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b7bf4-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="b7bf4-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b7bf4-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="b7bf4-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b7bf4-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b7bf4-124">Schema name</span></span>  <br/> |<span data-ttu-id="b7bf4-125">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="b7bf4-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="b7bf4-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b7bf4-126">Validation file</span></span>  <br/> |<span data-ttu-id="b7bf4-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b7bf4-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b7bf4-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="b7bf4-128">Can be empty</span></span>  <br/> |<span data-ttu-id="b7bf4-129">false</span><span class="sxs-lookup"><span data-stu-id="b7bf4-129">false</span></span>  <br/> |
   

