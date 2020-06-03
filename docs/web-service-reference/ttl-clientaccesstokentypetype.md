---
title: TTL (ClientAccessTokenTypeType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cc8f8caa-fced-49b6-9861-d112590b218a
description: TTL 要素は、トークンの time to live 値を示します。
ms.openlocfilehash: 0275e97ce02e41cc377f4003aee12c6fff0995e2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467390"
---
# <a name="ttl-clientaccesstokentypetype"></a><span data-ttu-id="08ae1-103">TTL (ClientAccessTokenTypeType)</span><span class="sxs-lookup"><span data-stu-id="08ae1-103">TTL (ClientAccessTokenTypeType)</span></span>

<span data-ttu-id="08ae1-104">**TTL**要素は、トークンの time to live 値を示します。</span><span class="sxs-lookup"><span data-stu-id="08ae1-104">The **TTL** element indicates the time to live value for the token.</span></span> 
  
```XML
<TTL></TTL>
```

 <span data-ttu-id="08ae1-105">**以外**</span><span class="sxs-lookup"><span data-stu-id="08ae1-105">**integer**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="08ae1-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="08ae1-106">Attributes and elements</span></span>

<span data-ttu-id="08ae1-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="08ae1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="08ae1-108">属性</span><span class="sxs-lookup"><span data-stu-id="08ae1-108">Attributes</span></span>

<span data-ttu-id="08ae1-109">なし。</span><span class="sxs-lookup"><span data-stu-id="08ae1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="08ae1-110">子要素</span><span class="sxs-lookup"><span data-stu-id="08ae1-110">Child elements</span></span>

<span data-ttu-id="08ae1-111">なし。</span><span class="sxs-lookup"><span data-stu-id="08ae1-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="08ae1-112">親要素</span><span class="sxs-lookup"><span data-stu-id="08ae1-112">Parent elements</span></span>

<span data-ttu-id="08ae1-113">[Tokenrequest](tokenrequest.md)  | [トークン](token.md)</span><span class="sxs-lookup"><span data-stu-id="08ae1-113">[TokenRequest](tokenrequest.md) | [Token](token.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="08ae1-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="08ae1-114">Text value</span></span>

<span data-ttu-id="08ae1-115">**TTL**要素のテキスト値は、トークンが有効である期間を示します。</span><span class="sxs-lookup"><span data-stu-id="08ae1-115">The text value for the **TTL** element indicates how long the token remains valid.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="08ae1-116">注釈</span><span class="sxs-lookup"><span data-stu-id="08ae1-116">Remarks</span></span>

<span data-ttu-id="08ae1-117">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="08ae1-117">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="08ae1-118">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="08ae1-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="08ae1-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="08ae1-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="08ae1-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="08ae1-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="08ae1-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="08ae1-121">Schema name</span></span>  <br/> |<span data-ttu-id="08ae1-122">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="08ae1-122">Types schema</span></span>  <br/> |
|<span data-ttu-id="08ae1-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="08ae1-123">Validation file</span></span>  <br/> |<span data-ttu-id="08ae1-124">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="08ae1-124">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="08ae1-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="08ae1-125">Can be empty</span></span>  <br/> |<span data-ttu-id="08ae1-126">false</span><span class="sxs-lookup"><span data-stu-id="08ae1-126">false</span></span>  <br/> |
   

