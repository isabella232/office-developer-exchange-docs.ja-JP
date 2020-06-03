---
title: TokenType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 83c650eb-7ab8-480c-a7c9-df60072ee042
description: TokenType 要素は、トークンの種類を指定します。
ms.openlocfilehash: a42849dce9ed0253c3c5d4d4e899367b8e105594
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459883"
---
# <a name="tokentype"></a><span data-ttu-id="2a068-103">TokenType</span><span class="sxs-lookup"><span data-stu-id="2a068-103">TokenType</span></span>

<span data-ttu-id="2a068-104">**TokenType**要素は、トークンの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="2a068-104">The **TokenType** element specifies the type of token.</span></span> 
  
```XML
<TokenType> CallerIdentity | ExtensionCallback | ScopedToken </TokenType>
```

 <span data-ttu-id="2a068-105">**ClientAccessTokenTypeType**</span><span class="sxs-lookup"><span data-stu-id="2a068-105">**ClientAccessTokenTypeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2a068-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="2a068-106">Attributes and elements</span></span>

<span data-ttu-id="2a068-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2a068-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2a068-108">属性</span><span class="sxs-lookup"><span data-stu-id="2a068-108">Attributes</span></span>

<span data-ttu-id="2a068-109">なし。</span><span class="sxs-lookup"><span data-stu-id="2a068-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2a068-110">子要素</span><span class="sxs-lookup"><span data-stu-id="2a068-110">Child elements</span></span>

<span data-ttu-id="2a068-111">なし。</span><span class="sxs-lookup"><span data-stu-id="2a068-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2a068-112">親要素</span><span class="sxs-lookup"><span data-stu-id="2a068-112">Parent elements</span></span>

<span data-ttu-id="2a068-113">[Tokenrequest](tokenrequest.md)  | [トークン](token.md)</span><span class="sxs-lookup"><span data-stu-id="2a068-113">[TokenRequest](tokenrequest.md) | [Token](token.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="2a068-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="2a068-114">Text value</span></span>

<span data-ttu-id="2a068-115">**TokenType**要素のテキスト値は、トークンの種類です。</span><span class="sxs-lookup"><span data-stu-id="2a068-115">The text value of the **TokenType** element is the token type.</span></span> <span data-ttu-id="2a068-116">**Calleridentity**のテキスト値は、トークンが発信者番号トークンであることを示します。</span><span class="sxs-lookup"><span data-stu-id="2a068-116">The text value of **CallerIdentity** indicates that the token is a caller identity token.</span></span> <span data-ttu-id="2a068-117">**Extensioncallback**のテキスト値は、トークンが拡張機能コールバック用であることを示します。</span><span class="sxs-lookup"><span data-stu-id="2a068-117">The text value of **ExtensionCallback** indicates that the token is for an extension callback.</span></span> <span data-ttu-id="2a068-118">**ScopedToken**のテキスト値は、クライアントアクセストークンがスコープ付きのトークンであることを示します。</span><span class="sxs-lookup"><span data-stu-id="2a068-118">The text value of **ScopedToken** indicates that the client access token is a scoped token.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="2a068-119">注釈</span><span class="sxs-lookup"><span data-stu-id="2a068-119">Remarks</span></span>

<span data-ttu-id="2a068-120">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="2a068-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="2a068-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="2a068-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2a068-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="2a068-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2a068-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="2a068-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2a068-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2a068-124">Schema name</span></span>  <br/> |<span data-ttu-id="2a068-125">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="2a068-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="2a068-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2a068-126">Validation file</span></span>  <br/> |<span data-ttu-id="2a068-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="2a068-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2a068-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="2a068-128">Can be empty</span></span>  <br/> |<span data-ttu-id="2a068-129">false</span><span class="sxs-lookup"><span data-stu-id="2a068-129">false</span></span>  <br/> |
   

