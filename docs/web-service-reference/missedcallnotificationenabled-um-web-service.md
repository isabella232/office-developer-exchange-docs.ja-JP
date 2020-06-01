---
title: MissedCallNotificationEnabled (UM web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- MissedCallNotificationEnabled
api_type:
- schema
ms.assetid: 8e6bf0b1-ff76-474c-ac0f-621b6ab89212
description: MissedCallNotificationEnabled 要素には、GetUMProperties 操作 (UM web サービス) 要求に対する応答で不在着信通知が有効になっているかどうかを示す値が含まれています。
ms.openlocfilehash: e2f18027c56be1408c27d5f687fe90f8ffd724db
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/01/2020
ms.locfileid: "44468657"
---
# <a name="missedcallnotificationenabled-um-web-service"></a><span data-ttu-id="873fb-103">MissedCallNotificationEnabled (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="873fb-103">MissedCallNotificationEnabled (UM web service)</span></span>

<span data-ttu-id="873fb-104">**MissedCallNotificationEnabled**要素には、 [getumproperties 操作 (UM web サービス)](getumproperties-operation-um-web-service.md)要求に対する応答で不在着信通知が有効になっているかどうかを示す値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="873fb-104">The **MissedCallNotificationEnabled** element contains a value that indicates whether a missed call notification is enabled in a response to a [GetUMProperties operation (UM web service)](getumproperties-operation-um-web-service.md) request.</span></span> 
  
[<span data-ttu-id="873fb-105">GetUMPropertiesResponse (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="873fb-105">GetUMPropertiesResponse (UM web service)</span></span>](getumpropertiesresponse-um-web-service.md)
  
[<span data-ttu-id="873fb-106">MissedCallNotificationEnabled (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="873fb-106">MissedCallNotificationEnabled (UM web service)</span></span>](missedcallnotificationenabled-um-web-service.md)
  
```xml
<MissedCallNotificationEnabled/>
```

 <span data-ttu-id="873fb-107">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="873fb-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="873fb-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="873fb-108">Attributes and elements</span></span>

<span data-ttu-id="873fb-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="873fb-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="873fb-110">属性</span><span class="sxs-lookup"><span data-stu-id="873fb-110">Attributes</span></span>

<span data-ttu-id="873fb-111">なし。</span><span class="sxs-lookup"><span data-stu-id="873fb-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="873fb-112">子要素</span><span class="sxs-lookup"><span data-stu-id="873fb-112">Child elements</span></span>

<span data-ttu-id="873fb-113">なし。</span><span class="sxs-lookup"><span data-stu-id="873fb-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="873fb-114">親要素</span><span class="sxs-lookup"><span data-stu-id="873fb-114">Parent elements</span></span>

|<span data-ttu-id="873fb-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="873fb-115">**Element**</span></span>|<span data-ttu-id="873fb-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="873fb-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="873fb-117">GetUMPropertiesResponse (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="873fb-117">GetUMPropertiesResponse (UM web service)</span></span>](getumpropertiesresponse-um-web-service.md) <br/> |<span data-ttu-id="873fb-118">[Getumproperties 操作 (UM web サービス)](getumproperties-operation-um-web-service.md)要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="873fb-118">Defines a response to a [GetUMProperties operation (UM web service)](getumproperties-operation-um-web-service.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="873fb-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="873fb-119">Text value</span></span>

<span data-ttu-id="873fb-120">ブール型のテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="873fb-120">A Boolean text value is required.</span></span> <span data-ttu-id="873fb-121">指定可能な値は次のいずれかです。</span><span class="sxs-lookup"><span data-stu-id="873fb-121">The following are the possible values:</span></span>
  
- <span data-ttu-id="873fb-122">True</span><span class="sxs-lookup"><span data-stu-id="873fb-122">True</span></span>
    
- <span data-ttu-id="873fb-123">False</span><span class="sxs-lookup"><span data-stu-id="873fb-123">False</span></span>
    
## <a name="element-information"></a><span data-ttu-id="873fb-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="873fb-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="873fb-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="873fb-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="873fb-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="873fb-126">Schema Name</span></span>  <br/> |<span data-ttu-id="873fb-127">メッセージ</span><span class="sxs-lookup"><span data-stu-id="873fb-127">Messages</span></span>  <br/> |
|<span data-ttu-id="873fb-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="873fb-128">Validation File</span></span>  <br/> |<span data-ttu-id="873fb-129">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="873fb-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="873fb-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="873fb-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="873fb-131">正しくない</span><span class="sxs-lookup"><span data-stu-id="873fb-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="873fb-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="873fb-132">See also</span></span>



[<span data-ttu-id="873fb-133">GetUMProperties 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="873fb-133">GetUMProperties operation (UM web service)</span></span>](getumproperties-operation-um-web-service.md)
  
[<span data-ttu-id="873fb-134">SetMissedCallNotificationEnabled 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="873fb-134">SetMissedCallNotificationEnabled operation (UM web service)</span></span>](setmissedcallnotificationenabled-operation-um-web-service.md)

