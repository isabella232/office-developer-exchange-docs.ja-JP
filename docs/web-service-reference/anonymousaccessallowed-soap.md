---
title: AnonymousAccessAllowed (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: bf819a65-30f2-4881-a34f-cb30a9c2b6a7
description: AnonymousAccessAllowed 要素は、場所を共有するドキュメントに認証済みのユーザーが必要かどうかを示します。
ms.openlocfilehash: 7ca208aa0d75b254463400a5e207079d722fc0a3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759328"
---
# <a name="anonymousaccessallowed-soap"></a><span data-ttu-id="27253-103">AnonymousAccessAllowed (SOAP)</span><span class="sxs-lookup"><span data-stu-id="27253-103">AnonymousAccessAllowed (SOAP)</span></span>

<span data-ttu-id="27253-104">**AnonymousAccessAllowed**要素は、場所を共有するドキュメントに認証済みのユーザーが必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="27253-104">The **AnonymousAccessAllowed** element indicates whether a document sharing location requires an authenticated user.</span></span> 
  
```XML
<AnonymousAccessAllowed /> 
```

 <span data-ttu-id="27253-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="27253-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="27253-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="27253-106">Attributes and elements</span></span>

<span data-ttu-id="27253-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="27253-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="27253-108">属性</span><span class="sxs-lookup"><span data-stu-id="27253-108">Attributes</span></span>

<span data-ttu-id="27253-109">なし。</span><span class="sxs-lookup"><span data-stu-id="27253-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="27253-110">子要素</span><span class="sxs-lookup"><span data-stu-id="27253-110">Child elements</span></span>

<span data-ttu-id="27253-111">なし。</span><span class="sxs-lookup"><span data-stu-id="27253-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="27253-112">親要素</span><span class="sxs-lookup"><span data-stu-id="27253-112">Parent elements</span></span>

|<span data-ttu-id="27253-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="27253-113">**Element**</span></span>|<span data-ttu-id="27253-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="27253-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="27253-115">DocumentSharingLocation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="27253-115">DocumentSharingLocation (SOAP)</span></span>](documentsharinglocation-soap.md) <br/> |<span data-ttu-id="27253-116">場所を共有するドキュメントの場所およびメタデータの情報を表します。</span><span class="sxs-lookup"><span data-stu-id="27253-116">Represents location and metadata information for a document sharing location.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="27253-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="27253-117">Text value</span></span>

<span data-ttu-id="27253-118">**AnonymousAccessAllowed**要素のブール値は、共有の場所に認証されたユーザーが必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="27253-118">The Boolean value of the **AnonymousAccessAllowed** element indicates whether the sharing location requires an authenticated user.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="27253-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="27253-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="27253-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="27253-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="27253-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="27253-121">Schema Name</span></span>  <br/> |<span data-ttu-id="27253-122">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="27253-122">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="27253-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="27253-123">Validation File</span></span>  <br/> |<span data-ttu-id="27253-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="27253-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="27253-125">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="27253-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="27253-126">True</span><span class="sxs-lookup"><span data-stu-id="27253-126">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="27253-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="27253-127">See also</span></span>

- [<span data-ttu-id="27253-128">GetUserSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="27253-128">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
- [<span data-ttu-id="27253-129">Exchange の自動検出 web サービスの参照</span><span class="sxs-lookup"><span data-stu-id="27253-129">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
- [<span data-ttu-id="27253-130">Exchange 2013 の自動検出の XML 要素を SOAP</span><span class="sxs-lookup"><span data-stu-id="27253-130">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

