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
description: MajorVersion 要素は、サーバーのメジャーバージョン番号を表します。
ms.openlocfilehash: 2c564b110ec7497a2e9c92a00bfb7f376a657849
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44531008"
---
# <a name="majorversion-soap"></a><span data-ttu-id="ff399-103">MajorVersion (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ff399-103">MajorVersion (SOAP)</span></span>

<span data-ttu-id="ff399-104">**MajorVersion**要素は、サーバーのメジャーバージョン番号を表します。</span><span class="sxs-lookup"><span data-stu-id="ff399-104">The **MajorVersion** element represents the major version number for the server.</span></span> 
  
```XML
<MajorVersion/>
```

 <span data-ttu-id="ff399-105">**int**</span><span class="sxs-lookup"><span data-stu-id="ff399-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ff399-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="ff399-106">Attributes and elements</span></span>

<span data-ttu-id="ff399-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ff399-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ff399-108">属性</span><span class="sxs-lookup"><span data-stu-id="ff399-108">Attributes</span></span>

<span data-ttu-id="ff399-109">なし。</span><span class="sxs-lookup"><span data-stu-id="ff399-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ff399-110">子要素</span><span class="sxs-lookup"><span data-stu-id="ff399-110">Child elements</span></span>

<span data-ttu-id="ff399-111">なし。</span><span class="sxs-lookup"><span data-stu-id="ff399-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ff399-112">親要素</span><span class="sxs-lookup"><span data-stu-id="ff399-112">Parent elements</span></span>

|<span data-ttu-id="ff399-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="ff399-113">**Element**</span></span>|<span data-ttu-id="ff399-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="ff399-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ff399-115">ServerVersionInfo (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ff399-115">ServerVersionInfo (SOAP)</span></span>](serverversioninfo-soap.md) <br/> |<span data-ttu-id="ff399-116">要求を処理したサーバーのバージョンが保存されています。</span><span class="sxs-lookup"><span data-stu-id="ff399-116">Contains the version of the server that processed the request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ff399-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="ff399-117">Text value</span></span>

<span data-ttu-id="ff399-118">**MajorVersion**要素のテキスト値は、要求を処理したサーバーのメジャーバージョン番号を表す整数型 (integer) の値です。</span><span class="sxs-lookup"><span data-stu-id="ff399-118">The text value for the **MajorVersion** element is an integer that represents the major version number of the server that processed the request.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="ff399-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="ff399-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ff399-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="ff399-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="ff399-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ff399-121">Schema Name</span></span>  <br/> |<span data-ttu-id="ff399-122">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="ff399-122">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="ff399-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ff399-123">Validation File</span></span>  <br/> |<span data-ttu-id="ff399-124">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="ff399-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ff399-125">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="ff399-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="ff399-126">正しい</span><span class="sxs-lookup"><span data-stu-id="ff399-126">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ff399-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="ff399-127">See also</span></span>



[<span data-ttu-id="ff399-128">GetUserSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ff399-128">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
  
[<span data-ttu-id="ff399-129">GetFederationInformation 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ff399-129">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)

