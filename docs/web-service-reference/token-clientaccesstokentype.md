---
title: トークン (ClientAccessTokenType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cddd6075-06b6-4858-9ffa-9db4d9d9b030
description: トークンの要素は、クライアントのアクセス トークンを指定します。
ms.openlocfilehash: 2e1f401141aef07a57a214968f6a6bafdf71f0dc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839715"
---
# <a name="token-clientaccesstokentype"></a><span data-ttu-id="86998-103">トークン (ClientAccessTokenType)</span><span class="sxs-lookup"><span data-stu-id="86998-103">Token (ClientAccessTokenType)</span></span>

<span data-ttu-id="86998-104">**トークン**の要素は、クライアントのアクセス トークンを指定します。</span><span class="sxs-lookup"><span data-stu-id="86998-104">The **Token** element specifies a client access token.</span></span> 
  
```XML
<Token>
   <Id/>
   <TokenType/>
   <TokenValue/>
   <TTL/>
</Token>
```

 <span data-ttu-id="86998-105">**ClientAccessTokenType**</span><span class="sxs-lookup"><span data-stu-id="86998-105">**ClientAccessTokenType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="86998-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="86998-106">Attributes and elements</span></span>

<span data-ttu-id="86998-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="86998-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="86998-108">属性</span><span class="sxs-lookup"><span data-stu-id="86998-108">Attributes</span></span>

<span data-ttu-id="86998-109">なし。</span><span class="sxs-lookup"><span data-stu-id="86998-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="86998-110">子要素</span><span class="sxs-lookup"><span data-stu-id="86998-110">Child elements</span></span>

<span data-ttu-id="86998-111">[ID (文字列)](id-string.md) | [TokenType](tokentype.md) | [TokenValue](tokenvalue.md) | [TTL](ttl.md)</span><span class="sxs-lookup"><span data-stu-id="86998-111">[ID (String)](id-string.md) | [TokenType](tokentype.md) | [TokenValue](tokenvalue.md) | [TTL](ttl.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="86998-112">親要素</span><span class="sxs-lookup"><span data-stu-id="86998-112">Parent elements</span></span>

[<span data-ttu-id="86998-113">GetClientAccessTokenResponseMessage</span><span class="sxs-lookup"><span data-stu-id="86998-113">GetClientAccessTokenResponseMessage</span></span>](getclientaccesstokenresponsemessage.md)
  
## <a name="remarks"></a><span data-ttu-id="86998-114">備考</span><span class="sxs-lookup"><span data-stu-id="86998-114">Remarks</span></span>

<span data-ttu-id="86998-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="86998-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="86998-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="86998-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="86998-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="86998-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="86998-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="86998-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="86998-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="86998-119">Schema name</span></span>  <br/> |<span data-ttu-id="86998-120">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="86998-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="86998-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="86998-121">Validation file</span></span>  <br/> |<span data-ttu-id="86998-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="86998-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="86998-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="86998-123">Can be empty</span></span>  <br/> ||
   

