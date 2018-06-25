---
title: DeliveryRestricted
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeliveryRestricted
api_type:
- schema
ms.assetid: 05989915-121c-4f26-93cc-af8d454ab442
description: DeliveryRestricted 要素は、配信の制限が、送信者のメッセージを防ぐため、受信者に到達できないかどうかを示します。
ms.openlocfilehash: ba1c6e00b93c9e442a427fe98a5e15bf5fe1effd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760008"
---
# <a name="deliveryrestricted"></a><span data-ttu-id="aae40-103">DeliveryRestricted</span><span class="sxs-lookup"><span data-stu-id="aae40-103">DeliveryRestricted</span></span>

<span data-ttu-id="aae40-104">**DeliveryRestricted**要素は、配信の制限が、送信者のメッセージを防ぐため、受信者に到達できないかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="aae40-104">The **DeliveryRestricted** element indicates whether delivery restrictions will prevent the sender's message from reaching the recipient.</span></span> 
  
```XML
<DeliveryRestricted>true | false</DeliveryRestricted>
```

 <span data-ttu-id="aae40-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="aae40-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="aae40-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="aae40-106">Attributes and elements</span></span>

<span data-ttu-id="aae40-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="aae40-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="aae40-108">属性</span><span class="sxs-lookup"><span data-stu-id="aae40-108">Attributes</span></span>

<span data-ttu-id="aae40-109">なし。</span><span class="sxs-lookup"><span data-stu-id="aae40-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="aae40-110">子要素</span><span class="sxs-lookup"><span data-stu-id="aae40-110">Child elements</span></span>

<span data-ttu-id="aae40-111">なし。</span><span class="sxs-lookup"><span data-stu-id="aae40-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="aae40-112">親要素</span><span class="sxs-lookup"><span data-stu-id="aae40-112">Parent elements</span></span>

|<span data-ttu-id="aae40-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="aae40-113">**Element**</span></span>|<span data-ttu-id="aae40-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="aae40-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aae40-115">メール ヒント</span><span class="sxs-lookup"><span data-stu-id="aae40-115">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="aae40-116">さまざまな種類のメール ヒントの値を表します。</span><span class="sxs-lookup"><span data-stu-id="aae40-116">Represents values for various types of mail tips.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="aae40-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="aae40-117">Text value</span></span>

<span data-ttu-id="aae40-118">この要素のテキスト値は、配信の制限は送信者のメッセージを防ぐため、受信者に到達できない場合**true** 。</span><span class="sxs-lookup"><span data-stu-id="aae40-118">The text value of this element is **true** if delivery restrictions will prevent the sender's message from reaching the recipient.</span></span> <span data-ttu-id="aae40-119">値は、配信の制限できなくなる、送信者のメッセージが受信者に届かない場合**は false** 。</span><span class="sxs-lookup"><span data-stu-id="aae40-119">The value is **false** if delivery restrictions will not prevent the sender's message from reaching the recipient.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="aae40-120">備考</span><span class="sxs-lookup"><span data-stu-id="aae40-120">Remarks</span></span>

<span data-ttu-id="aae40-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="aae40-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="aae40-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="aae40-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="aae40-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="aae40-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="aae40-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="aae40-124">Schema Name</span></span>  <br/> |<span data-ttu-id="aae40-125">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="aae40-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="aae40-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="aae40-126">Validation File</span></span>  <br/> |<span data-ttu-id="aae40-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="aae40-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="aae40-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="aae40-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="aae40-129">False</span><span class="sxs-lookup"><span data-stu-id="aae40-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="aae40-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="aae40-130">See also</span></span>

- [<span data-ttu-id="aae40-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="aae40-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

