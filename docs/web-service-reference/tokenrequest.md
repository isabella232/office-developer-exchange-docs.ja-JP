---
title: TokenRequest
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 54f45f8e-c02b-4ead-b15a-38b30872c362
description: TokenRequest 要素は、1 つのトークン要求を指定します。
ms.openlocfilehash: b7e814cbcf34912f79bded57874dbc8e4ce28176
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839723"
---
# <a name="tokenrequest"></a><span data-ttu-id="729b8-103">TokenRequest</span><span class="sxs-lookup"><span data-stu-id="729b8-103">TokenRequest</span></span>

<span data-ttu-id="729b8-104">**TokenRequest**要素は、1 つのトークン要求を指定します。</span><span class="sxs-lookup"><span data-stu-id="729b8-104">The **TokenRequest** element specifies a single token request.</span></span> 
  
```XML
<TokenRequest>
   <Id/>
   <TokenType/>
</TokenRequest>
```

 <span data-ttu-id="729b8-105">**ClientAccessTokenRequestType**</span><span class="sxs-lookup"><span data-stu-id="729b8-105">**ClientAccessTokenRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="729b8-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="729b8-106">Attributes and elements</span></span>

<span data-ttu-id="729b8-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="729b8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="729b8-108">属性</span><span class="sxs-lookup"><span data-stu-id="729b8-108">Attributes</span></span>

<span data-ttu-id="729b8-109">なし。</span><span class="sxs-lookup"><span data-stu-id="729b8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="729b8-110">子要素</span><span class="sxs-lookup"><span data-stu-id="729b8-110">Child elements</span></span>

<span data-ttu-id="729b8-111">[ID (文字列)](id-string.md) | [TokenType (ClientAccessTokenType)](tokentype-clientaccesstokentype.md)</span><span class="sxs-lookup"><span data-stu-id="729b8-111">[ID (String)](id-string.md) | [TokenType (ClientAccessTokenType)](tokentype-clientaccesstokentype.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="729b8-112">親要素</span><span class="sxs-lookup"><span data-stu-id="729b8-112">Parent elements</span></span>

[<span data-ttu-id="729b8-113">TokenRequests</span><span class="sxs-lookup"><span data-stu-id="729b8-113">TokenRequests</span></span>](tokenrequests.md)
  
## <a name="remarks"></a><span data-ttu-id="729b8-114">備考</span><span class="sxs-lookup"><span data-stu-id="729b8-114">Remarks</span></span>

<span data-ttu-id="729b8-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="729b8-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="729b8-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="729b8-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="729b8-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="729b8-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="729b8-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="729b8-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="729b8-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="729b8-119">Schema name</span></span>  <br/> |<span data-ttu-id="729b8-120">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="729b8-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="729b8-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="729b8-121">Validation file</span></span>  <br/> |<span data-ttu-id="729b8-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="729b8-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="729b8-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="729b8-123">Can be empty</span></span>  <br/> |<span data-ttu-id="729b8-124">false</span><span class="sxs-lookup"><span data-stu-id="729b8-124">false</span></span>  <br/> |
   

