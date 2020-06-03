---
title: TrackingPropertyType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TrackingPropertyType
api_type:
- schema
ms.assetid: 1d0f219b-1063-4eaa-9d3b-da384a544f89
description: TrackingPropertyType 要素は、メッセージ追跡レポートのプロパティを作成するために使用される文字列の名前と値のペアを表します。
ms.openlocfilehash: 7812b52dd57fed0a9b6f1a8fc4e77660932a60dc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468083"
---
# <a name="trackingpropertytype"></a><span data-ttu-id="ec2ac-103">TrackingPropertyType</span><span class="sxs-lookup"><span data-stu-id="ec2ac-103">TrackingPropertyType</span></span>

<span data-ttu-id="ec2ac-104">**TrackingPropertyType**要素は、メッセージ追跡レポートのプロパティを作成するために使用される文字列の名前と値のペアを表します。</span><span class="sxs-lookup"><span data-stu-id="ec2ac-104">The **TrackingPropertyType** element represents a name and value pair of strings that is used to create properties for message tracking reports.</span></span> 
  
[<span data-ttu-id="ec2ac-105">プロパティ (ArrayOfTrackingPropertiesType)</span><span class="sxs-lookup"><span data-stu-id="ec2ac-105">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md)
  
[<span data-ttu-id="ec2ac-106">TrackingPropertyType</span><span class="sxs-lookup"><span data-stu-id="ec2ac-106">TrackingPropertyType</span></span>](trackingpropertytype.md)
  
```xml
<TrackingPropertyType>
   <Name/>
   <Value/>
</TrackingPropertyType>
```

 <span data-ttu-id="ec2ac-107">**TrackingPropertyType**</span><span class="sxs-lookup"><span data-stu-id="ec2ac-107">**TrackingPropertyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ec2ac-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="ec2ac-108">Attributes and elements</span></span>

<span data-ttu-id="ec2ac-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ec2ac-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ec2ac-110">属性</span><span class="sxs-lookup"><span data-stu-id="ec2ac-110">Attributes</span></span>

<span data-ttu-id="ec2ac-111">なし。</span><span class="sxs-lookup"><span data-stu-id="ec2ac-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ec2ac-112">子要素</span><span class="sxs-lookup"><span data-stu-id="ec2ac-112">Child elements</span></span>

|<span data-ttu-id="ec2ac-113">**Element**</span><span class="sxs-lookup"><span data-stu-id="ec2ac-113">**Element**</span></span>|<span data-ttu-id="ec2ac-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="ec2ac-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ec2ac-115">Name (メッセージ追跡)</span><span class="sxs-lookup"><span data-stu-id="ec2ac-115">Name (Message Tracking)</span></span>](name-message-tracking.md) <br/> |<span data-ttu-id="ec2ac-116">メッセージ追跡レポートプロパティの名前を定義します。</span><span class="sxs-lookup"><span data-stu-id="ec2ac-116">Defines a name for the message tracking report property.</span></span>  <br/> |
|[<span data-ttu-id="ec2ac-117">値 (メッセージ追跡)</span><span class="sxs-lookup"><span data-stu-id="ec2ac-117">Value (Message Tracking)</span></span>](value-message-tracking.md) <br/> |<span data-ttu-id="ec2ac-118">メッセージ追跡レポートのプロパティの値を定義します。</span><span class="sxs-lookup"><span data-stu-id="ec2ac-118">Defines a value for the message tracking report property.</span></span> <span data-ttu-id="ec2ac-119">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="ec2ac-119">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ec2ac-120">親要素</span><span class="sxs-lookup"><span data-stu-id="ec2ac-120">Parent elements</span></span>

|<span data-ttu-id="ec2ac-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="ec2ac-121">**Element**</span></span>|<span data-ttu-id="ec2ac-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="ec2ac-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ec2ac-123">プロパティ (ArrayOfTrackingPropertiesType)</span><span class="sxs-lookup"><span data-stu-id="ec2ac-123">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md) <br/> |<span data-ttu-id="ec2ac-124">1つ以上の追跡プロパティの一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ec2ac-124">Contains a list of one or more tracking properties.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ec2ac-125">テキスト値</span><span class="sxs-lookup"><span data-stu-id="ec2ac-125">Text value</span></span>

<span data-ttu-id="ec2ac-126">なし。</span><span class="sxs-lookup"><span data-stu-id="ec2ac-126">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ec2ac-127">注釈</span><span class="sxs-lookup"><span data-stu-id="ec2ac-127">Remarks</span></span>

<span data-ttu-id="ec2ac-128">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="ec2ac-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ec2ac-129">要素の情報</span><span class="sxs-lookup"><span data-stu-id="ec2ac-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ec2ac-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="ec2ac-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ec2ac-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ec2ac-131">Schema Name</span></span>  <br/> |<span data-ttu-id="ec2ac-132">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="ec2ac-132">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ec2ac-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ec2ac-133">Validation File</span></span>  <br/> |<span data-ttu-id="ec2ac-134">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="ec2ac-134">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ec2ac-135">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="ec2ac-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="ec2ac-136">正しくない</span><span class="sxs-lookup"><span data-stu-id="ec2ac-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ec2ac-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="ec2ac-137">See also</span></span>



- [<span data-ttu-id="ec2ac-138">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="ec2ac-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

