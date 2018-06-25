---
title: TokenType (ClientAccessTokenType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 96103f15-a3e0-497c-af21-90adbf9a4b14
description: TokenType 要素は、GetClientAccessToken の応答で返されるクライアントのアクセス トークンの種類を識別します。
ms.openlocfilehash: c9adb60acf76fefebd58e2fd3bc899332a63dbee
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839725"
---
# <a name="tokentype-clientaccesstokentype"></a><span data-ttu-id="2b81a-103">TokenType (ClientAccessTokenType)</span><span class="sxs-lookup"><span data-stu-id="2b81a-103">TokenType (ClientAccessTokenType)</span></span>

<span data-ttu-id="2b81a-104">**TokenType**要素は、 **GetClientAccessToken**の応答で返されるクライアントのアクセス トークンの種類を識別します。</span><span class="sxs-lookup"><span data-stu-id="2b81a-104">The **TokenType** element identifies the type of client access token that will be returned in the **GetClientAccessToken** response.</span></span> 
  
```XML
<TokenType>CallerIdentity | ExtensionCallback | ScopedToken</TokenType>
```

 <span data-ttu-id="2b81a-105">**ClientAccessTokenTypeType**</span><span class="sxs-lookup"><span data-stu-id="2b81a-105">**ClientAccessTokenTypeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2b81a-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="2b81a-106">Attributes and elements</span></span>

<span data-ttu-id="2b81a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2b81a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2b81a-108">属性</span><span class="sxs-lookup"><span data-stu-id="2b81a-108">Attributes</span></span>

<span data-ttu-id="2b81a-109">なし。</span><span class="sxs-lookup"><span data-stu-id="2b81a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2b81a-110">子要素</span><span class="sxs-lookup"><span data-stu-id="2b81a-110">Child elements</span></span>

<span data-ttu-id="2b81a-111">なし。</span><span class="sxs-lookup"><span data-stu-id="2b81a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2b81a-112">親要素</span><span class="sxs-lookup"><span data-stu-id="2b81a-112">Parent elements</span></span>

<span data-ttu-id="2b81a-113">[TokenRequest](tokenrequest.md) | [(ClientAccessTokenType) をトークン](token-clientaccesstokentype.md)</span><span class="sxs-lookup"><span data-stu-id="2b81a-113">[TokenRequest](tokenrequest.md) | [Token (ClientAccessTokenType)](token-clientaccesstokentype.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="2b81a-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="2b81a-114">Text value</span></span>

<span data-ttu-id="2b81a-115">**CallerIdentity**のテキスト値は、呼び出し元 id のクライアントのアクセス トークンが返されますを意味します。</span><span class="sxs-lookup"><span data-stu-id="2b81a-115">A text value of **CallerIdentity** means a caller identity client access token is returned.</span></span> <span data-ttu-id="2b81a-116">**ExtensionCallback**のテキスト値は、拡張機能コールバック クライアントのアクセス トークンが返されることを示します。</span><span class="sxs-lookup"><span data-stu-id="2b81a-116">A text value of **ExtensionCallback** indicates that an extension callback client access token is returned.</span></span> <span data-ttu-id="2b81a-117">テキスト値が**ScopedToken**のクライアントのアクセス トークンがスコープのトークンであることを示します。</span><span class="sxs-lookup"><span data-stu-id="2b81a-117">A text value of **ScopedToken** indicates that the client access token is a scoped token.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="2b81a-118">備考</span><span class="sxs-lookup"><span data-stu-id="2b81a-118">Remarks</span></span>

<span data-ttu-id="2b81a-119">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="2b81a-119">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="2b81a-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="2b81a-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2b81a-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="2b81a-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2b81a-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="2b81a-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2b81a-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2b81a-123">Schema name</span></span>  <br/> |<span data-ttu-id="2b81a-124">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="2b81a-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="2b81a-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2b81a-125">Validation file</span></span>  <br/> |<span data-ttu-id="2b81a-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2b81a-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2b81a-127">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="2b81a-127">Can be empty</span></span>  <br/> |<span data-ttu-id="2b81a-128">false</span><span class="sxs-lookup"><span data-stu-id="2b81a-128">false</span></span>  <br/> |
   

