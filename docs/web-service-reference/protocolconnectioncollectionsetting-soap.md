---
title: ProtocolConnectionCollectionSetting (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 51f84364-9a5f-4ef2-ba82-f6ef7c65f7cb
description: ProtocolConnectionCollectionSetting 要素は、サーバー プロトコルの接続の設定のコレクションを表します。
ms.openlocfilehash: d0342222c0390d3e49afe572af92a903b9643a2c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832914"
---
# <a name="protocolconnectioncollectionsetting-soap"></a><span data-ttu-id="5fab3-103">ProtocolConnectionCollectionSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5fab3-103">ProtocolConnectionCollectionSetting (SOAP)</span></span>

<span data-ttu-id="5fab3-104">**ProtocolConnectionCollectionSetting**要素は、サーバー プロトコルの接続の設定のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="5fab3-104">The **ProtocolConnectionCollectionSetting** element represents a collection of server protocol connection settings.</span></span> 
  
```XML
<ProtocolConnectionCollectionSetting/>
   <Name/>
   <ProtocolConnections/>
</ProtocolConnectionCollectionSetting>
```

 <span data-ttu-id="5fab3-105">**ProtocolConnectionCollectionSetting**</span><span class="sxs-lookup"><span data-stu-id="5fab3-105">**ProtocolConnectionCollectionSetting**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5fab3-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="5fab3-106">Attributes and elements</span></span>

<span data-ttu-id="5fab3-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5fab3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5fab3-108">属性</span><span class="sxs-lookup"><span data-stu-id="5fab3-108">Attributes</span></span>

<span data-ttu-id="5fab3-109">なし。</span><span class="sxs-lookup"><span data-stu-id="5fab3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5fab3-110">子要素</span><span class="sxs-lookup"><span data-stu-id="5fab3-110">Child elements</span></span>

|<span data-ttu-id="5fab3-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="5fab3-111">**Element**</span></span>|<span data-ttu-id="5fab3-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="5fab3-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5fab3-113">名 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5fab3-113">Name (SOAP)</span></span>](name-soap.md) <br/> |<span data-ttu-id="5fab3-114">設定の名前を表します。</span><span class="sxs-lookup"><span data-stu-id="5fab3-114">Represents the name of a setting.</span></span>  <br/> |
|[<span data-ttu-id="5fab3-115">ProtocolConnections (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5fab3-115">ProtocolConnections (SOAP)</span></span>](protocolconnections-soap.md) <br/> |<span data-ttu-id="5fab3-116">0 個以上のプロトコルの接続が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5fab3-116">Contains zero or more protocol connections.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5fab3-117">親要素</span><span class="sxs-lookup"><span data-stu-id="5fab3-117">Parent elements</span></span>

<span data-ttu-id="5fab3-118">なし。</span><span class="sxs-lookup"><span data-stu-id="5fab3-118">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="5fab3-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="5fab3-119">Text value</span></span>

<span data-ttu-id="5fab3-120">なし。</span><span class="sxs-lookup"><span data-stu-id="5fab3-120">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5fab3-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="5fab3-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5fab3-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="5fab3-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="5fab3-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5fab3-123">Schema Name</span></span>  <br/> |<span data-ttu-id="5fab3-124">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="5fab3-124">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="5fab3-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5fab3-125">Validation File</span></span>  <br/> |<span data-ttu-id="5fab3-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="5fab3-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5fab3-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="5fab3-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="5fab3-128">True</span><span class="sxs-lookup"><span data-stu-id="5fab3-128">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5fab3-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="5fab3-129">See also</span></span>



[<span data-ttu-id="5fab3-130">GetUserSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5fab3-130">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
  
[<span data-ttu-id="5fab3-131">GetDomainSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5fab3-131">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)
  
[<span data-ttu-id="5fab3-132">GetFederationInformation 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5fab3-132">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)

