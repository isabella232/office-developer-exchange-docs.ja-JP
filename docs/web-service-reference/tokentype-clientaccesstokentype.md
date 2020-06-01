---
title: TokenType (ClientAccessTokenType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 96103f15-a3e0-497c-af21-90adbf9a4b14
description: TokenType 要素は、GetClientAccessToken 応答で返されるクライアントアクセストークンの種類を識別します。
ms.openlocfilehash: 49ba2973967b12396e0c7f56129c89c40ccbcf97
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466053"
---
# <a name="tokentype-clientaccesstokentype"></a><span data-ttu-id="03490-103">TokenType (ClientAccessTokenType)</span><span class="sxs-lookup"><span data-stu-id="03490-103">TokenType (ClientAccessTokenType)</span></span>

<span data-ttu-id="03490-104">**TokenType**要素は、 **GetClientAccessToken**応答で返されるクライアントアクセストークンの種類を識別します。</span><span class="sxs-lookup"><span data-stu-id="03490-104">The **TokenType** element identifies the type of client access token that will be returned in the **GetClientAccessToken** response.</span></span> 
  
```XML
<TokenType>CallerIdentity | ExtensionCallback | ScopedToken</TokenType>
```

 <span data-ttu-id="03490-105">**ClientAccessTokenTypeType**</span><span class="sxs-lookup"><span data-stu-id="03490-105">**ClientAccessTokenTypeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="03490-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="03490-106">Attributes and elements</span></span>

<span data-ttu-id="03490-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="03490-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="03490-108">属性</span><span class="sxs-lookup"><span data-stu-id="03490-108">Attributes</span></span>

<span data-ttu-id="03490-109">なし。</span><span class="sxs-lookup"><span data-stu-id="03490-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="03490-110">子要素</span><span class="sxs-lookup"><span data-stu-id="03490-110">Child elements</span></span>

<span data-ttu-id="03490-111">なし。</span><span class="sxs-lookup"><span data-stu-id="03490-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="03490-112">親要素</span><span class="sxs-lookup"><span data-stu-id="03490-112">Parent elements</span></span>

<span data-ttu-id="03490-113">[Tokenrequest](tokenrequest.md)  | [トークン (ClientAccessTokenType)](token-clientaccesstokentype.md)</span><span class="sxs-lookup"><span data-stu-id="03490-113">[TokenRequest](tokenrequest.md) | [Token (ClientAccessTokenType)](token-clientaccesstokentype.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="03490-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="03490-114">Text value</span></span>

<span data-ttu-id="03490-115">**Calleridentity**のテキスト値は、呼び出し id クライアントアクセストークンが返されることを意味します。</span><span class="sxs-lookup"><span data-stu-id="03490-115">A text value of **CallerIdentity** means a caller identity client access token is returned.</span></span> <span data-ttu-id="03490-116">**Extensioncallback**というテキスト値は、拡張コールバッククライアントアクセストークンが返されることを示します。</span><span class="sxs-lookup"><span data-stu-id="03490-116">A text value of **ExtensionCallback** indicates that an extension callback client access token is returned.</span></span> <span data-ttu-id="03490-117">**ScopedToken**のテキスト値は、クライアントアクセストークンがスコープ付きのトークンであることを示します。</span><span class="sxs-lookup"><span data-stu-id="03490-117">A text value of **ScopedToken** indicates that the client access token is a scoped token.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="03490-118">注釈</span><span class="sxs-lookup"><span data-stu-id="03490-118">Remarks</span></span>

<span data-ttu-id="03490-119">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="03490-119">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="03490-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="03490-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="03490-121">要素の情報</span><span class="sxs-lookup"><span data-stu-id="03490-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="03490-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="03490-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="03490-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="03490-123">Schema name</span></span>  <br/> |<span data-ttu-id="03490-124">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="03490-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="03490-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="03490-125">Validation file</span></span>  <br/> |<span data-ttu-id="03490-126">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="03490-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="03490-127">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="03490-127">Can be empty</span></span>  <br/> |<span data-ttu-id="03490-128">false</span><span class="sxs-lookup"><span data-stu-id="03490-128">false</span></span>  <br/> |
   

