---
title: OofStatus (UM web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- OofStatus
api_type:
- schema
ms.assetid: 0ba4225a-784e-4e6e-bd20-be45f0f7597c
description: OofStatus 要素には、GetUMProperties 操作 (UM web サービス) 要求を作成しているユーザーに対して、ユニファイドメッセージングの不在状態を indicaties する値が含まれています。
ms.openlocfilehash: 80b1d5aa508579eec14637ed10c322b5fbb670da
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460576"
---
# <a name="oofstatus-um-web-service"></a><span data-ttu-id="a8689-103">OofStatus (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="a8689-103">OofStatus (UM web service)</span></span>

<span data-ttu-id="a8689-104">**Oofstatus**要素には、 [getumproperties 操作 (UM web サービス)](getumproperties-operation-um-web-service.md)要求を作成しているユーザーに対して、ユニファイドメッセージングの不在状態を indicaties する値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a8689-104">The **OofStatus** element contains a value that indicaties the Unified Messaging Out of Office status for the user who is making a [GetUMProperties operation (UM web service)](getumproperties-operation-um-web-service.md) request.</span></span> 
  
[<span data-ttu-id="a8689-105">GetUMPropertiesResponse (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="a8689-105">GetUMPropertiesResponse (UM web service)</span></span>](getumpropertiesresponse-um-web-service.md)
  
[<span data-ttu-id="a8689-106">OofStatus (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="a8689-106">OofStatus (UM web service)</span></span>](oofstatus-um-web-service.md)
  
```xml
<GetUMPropertiesResponse>
    <OofStatus/>
  <MissedCallNotificationEnabled/>
  <PlayOnPhoneDialString/>
  <TelephoneAccessNumbers/>
  <TelephoneAccessFolderEmail/>
</GetUMPropertiesResponse>
```

 <span data-ttu-id="a8689-107">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="a8689-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a8689-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="a8689-108">Attributes and elements</span></span>

<span data-ttu-id="a8689-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a8689-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a8689-110">属性</span><span class="sxs-lookup"><span data-stu-id="a8689-110">Attributes</span></span>

<span data-ttu-id="a8689-111">なし。</span><span class="sxs-lookup"><span data-stu-id="a8689-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a8689-112">子要素</span><span class="sxs-lookup"><span data-stu-id="a8689-112">Child elements</span></span>

<span data-ttu-id="a8689-113">なし。</span><span class="sxs-lookup"><span data-stu-id="a8689-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a8689-114">親要素</span><span class="sxs-lookup"><span data-stu-id="a8689-114">Parent elements</span></span>

|<span data-ttu-id="a8689-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="a8689-115">**Element**</span></span>|<span data-ttu-id="a8689-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="a8689-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a8689-117">GetUMPropertiesResponse (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="a8689-117">GetUMPropertiesResponse (UM web service)</span></span>](getumpropertiesresponse-um-web-service.md) <br/> |<span data-ttu-id="a8689-118">[Getumproperties 操作 (UM web サービス)](getumproperties-operation-um-web-service.md)要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="a8689-118">Defines a response to a [GetUMProperties operation (UM web service)](getumproperties-operation-um-web-service.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a8689-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="a8689-119">Text value</span></span>

<span data-ttu-id="a8689-120">ブール型のテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="a8689-120">A Boolean text value is required.</span></span> <span data-ttu-id="a8689-121">指定可能な値は次のいずれかです。</span><span class="sxs-lookup"><span data-stu-id="a8689-121">The following are the possible values:</span></span>
  
- <span data-ttu-id="a8689-122">True</span><span class="sxs-lookup"><span data-stu-id="a8689-122">True</span></span>
    
- <span data-ttu-id="a8689-123">False</span><span class="sxs-lookup"><span data-stu-id="a8689-123">False</span></span>
    
## <a name="element-information"></a><span data-ttu-id="a8689-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="a8689-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a8689-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="a8689-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a8689-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a8689-126">Schema Name</span></span>  <br/> |<span data-ttu-id="a8689-127">メッセージ</span><span class="sxs-lookup"><span data-stu-id="a8689-127">Messages</span></span>  <br/> |
|<span data-ttu-id="a8689-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a8689-128">Validation File</span></span>  <br/> |<span data-ttu-id="a8689-129">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="a8689-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a8689-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="a8689-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="a8689-131">正しくない</span><span class="sxs-lookup"><span data-stu-id="a8689-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a8689-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="a8689-132">See also</span></span>



[<span data-ttu-id="a8689-133">GetUMProperties 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="a8689-133">GetUMProperties operation (UM web service)</span></span>](getumproperties-operation-um-web-service.md)
  
[<span data-ttu-id="a8689-134">GetUMPropertiesResponse (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="a8689-134">GetUMPropertiesResponse (UM web service)</span></span>](getumpropertiesresponse-um-web-service.md)

