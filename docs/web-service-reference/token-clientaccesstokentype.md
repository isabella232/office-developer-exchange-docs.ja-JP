---
title: トークン (ClientAccessTokenType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cddd6075-06b6-4858-9ffa-9db4d9d9b030
description: Token 要素は、クライアントアクセストークンを指定します。
ms.openlocfilehash: d195e81d8d20eb2288e921c640c7b2898a5341ab
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467866"
---
# <a name="token-clientaccesstokentype"></a><span data-ttu-id="e8a1f-103">トークン (ClientAccessTokenType)</span><span class="sxs-lookup"><span data-stu-id="e8a1f-103">Token (ClientAccessTokenType)</span></span>

<span data-ttu-id="e8a1f-104">**Token**要素は、クライアントアクセストークンを指定します。</span><span class="sxs-lookup"><span data-stu-id="e8a1f-104">The **Token** element specifies a client access token.</span></span> 
  
```XML
<Token>
   <Id/>
   <TokenType/>
   <TokenValue/>
   <TTL/>
</Token>
```

 <span data-ttu-id="e8a1f-105">**ClientAccessTokenType**</span><span class="sxs-lookup"><span data-stu-id="e8a1f-105">**ClientAccessTokenType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e8a1f-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="e8a1f-106">Attributes and elements</span></span>

<span data-ttu-id="e8a1f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e8a1f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e8a1f-108">属性</span><span class="sxs-lookup"><span data-stu-id="e8a1f-108">Attributes</span></span>

<span data-ttu-id="e8a1f-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e8a1f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e8a1f-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e8a1f-110">Child elements</span></span>

<span data-ttu-id="e8a1f-111">[ID (文字列)](id-string.md)  | [TokenType](tokentype.md)  | [Tokenvalue](tokenvalue.md)  | [TTL](ttl.md)</span><span class="sxs-lookup"><span data-stu-id="e8a1f-111">[ID (String)](id-string.md) | [TokenType](tokentype.md) | [TokenValue](tokenvalue.md) | [TTL](ttl.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e8a1f-112">親要素</span><span class="sxs-lookup"><span data-stu-id="e8a1f-112">Parent elements</span></span>

[<span data-ttu-id="e8a1f-113">GetClientAccessTokenResponseMessage</span><span class="sxs-lookup"><span data-stu-id="e8a1f-113">GetClientAccessTokenResponseMessage</span></span>](getclientaccesstokenresponsemessage.md)
  
## <a name="remarks"></a><span data-ttu-id="e8a1f-114">注釈</span><span class="sxs-lookup"><span data-stu-id="e8a1f-114">Remarks</span></span>

<span data-ttu-id="e8a1f-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="e8a1f-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e8a1f-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="e8a1f-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e8a1f-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="e8a1f-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e8a1f-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="e8a1f-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e8a1f-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e8a1f-119">Schema name</span></span>  <br/> |<span data-ttu-id="e8a1f-120">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="e8a1f-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="e8a1f-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e8a1f-121">Validation file</span></span>  <br/> |<span data-ttu-id="e8a1f-122">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="e8a1f-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e8a1f-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="e8a1f-123">Can be empty</span></span>  <br/> ||
   

