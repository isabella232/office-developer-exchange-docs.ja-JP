---
title: MajorVersion (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 0b2a83cf-e173-4073-9603-b2ea3b36ec1a
description: MajorVersion 要素は、サーバーのメジャー バージョン番号を表します。
ms.openlocfilehash: ca619d4c36e17ca9a811019f0a13b45353cab1e2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832333"
---
# <a name="majorversion-soap"></a><span data-ttu-id="9734a-103">MajorVersion (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9734a-103">MajorVersion (SOAP)</span></span>

<span data-ttu-id="9734a-104">**MajorVersion**要素は、サーバーのメジャー バージョン番号を表します。</span><span class="sxs-lookup"><span data-stu-id="9734a-104">The **MajorVersion** element represents the major version number for the server.</span></span> 
  
```XML
<MajorVersion/>
```

 <span data-ttu-id="9734a-105">**int**</span><span class="sxs-lookup"><span data-stu-id="9734a-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9734a-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="9734a-106">Attributes and elements</span></span>

<span data-ttu-id="9734a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9734a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9734a-108">属性</span><span class="sxs-lookup"><span data-stu-id="9734a-108">Attributes</span></span>

<span data-ttu-id="9734a-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9734a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9734a-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9734a-110">Child elements</span></span>

<span data-ttu-id="9734a-111">なし。</span><span class="sxs-lookup"><span data-stu-id="9734a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9734a-112">親要素</span><span class="sxs-lookup"><span data-stu-id="9734a-112">Parent elements</span></span>

|<span data-ttu-id="9734a-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="9734a-113">**Element**</span></span>|<span data-ttu-id="9734a-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="9734a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9734a-115">ServerVersionInfo (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9734a-115">ServerVersionInfo (SOAP)</span></span>](serverversioninfo-soap.md) <br/> |<span data-ttu-id="9734a-116">要求を処理したサーバーのバージョンが含まれています。</span><span class="sxs-lookup"><span data-stu-id="9734a-116">Contains the version of the server that processed the request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9734a-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="9734a-117">Text value</span></span>

<span data-ttu-id="9734a-118">**MajorVersion**要素のテキスト値は、要求を処理したサーバーのメジャー バージョン番号を表す整数です。</span><span class="sxs-lookup"><span data-stu-id="9734a-118">The text value for the **MajorVersion** element is an integer that represents the major version number of the server that processed the request.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="9734a-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="9734a-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9734a-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="9734a-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="9734a-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9734a-121">Schema Name</span></span>  <br/> |<span data-ttu-id="9734a-122">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="9734a-122">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="9734a-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9734a-123">Validation File</span></span>  <br/> |<span data-ttu-id="9734a-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9734a-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9734a-125">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="9734a-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="9734a-126">True</span><span class="sxs-lookup"><span data-stu-id="9734a-126">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9734a-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="9734a-127">See also</span></span>



[<span data-ttu-id="9734a-128">GetUserSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9734a-128">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
  
[<span data-ttu-id="9734a-129">GetFederationInformation 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9734a-129">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)

