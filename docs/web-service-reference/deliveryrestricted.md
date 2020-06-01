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
description: DeliveryRestricted 要素は、配信の制限によって送信者のメッセージが受信者に届かないようにするかどうかを示します。
ms.openlocfilehash: 58fc85873326179d7745db4ba7d4854a76ced6a7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462690"
---
# <a name="deliveryrestricted"></a><span data-ttu-id="8a926-103">DeliveryRestricted</span><span class="sxs-lookup"><span data-stu-id="8a926-103">DeliveryRestricted</span></span>

<span data-ttu-id="8a926-104">**Deliveryrestricted**要素は、配信の制限によって送信者のメッセージが受信者に届かないようにするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8a926-104">The **DeliveryRestricted** element indicates whether delivery restrictions will prevent the sender's message from reaching the recipient.</span></span> 
  
```XML
<DeliveryRestricted>true | false</DeliveryRestricted>
```

 <span data-ttu-id="8a926-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="8a926-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8a926-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="8a926-106">Attributes and elements</span></span>

<span data-ttu-id="8a926-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8a926-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8a926-108">属性</span><span class="sxs-lookup"><span data-stu-id="8a926-108">Attributes</span></span>

<span data-ttu-id="8a926-109">なし。</span><span class="sxs-lookup"><span data-stu-id="8a926-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8a926-110">子要素</span><span class="sxs-lookup"><span data-stu-id="8a926-110">Child elements</span></span>

<span data-ttu-id="8a926-111">なし。</span><span class="sxs-lookup"><span data-stu-id="8a926-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8a926-112">親要素</span><span class="sxs-lookup"><span data-stu-id="8a926-112">Parent elements</span></span>

|<span data-ttu-id="8a926-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="8a926-113">**Element**</span></span>|<span data-ttu-id="8a926-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="8a926-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8a926-115">メールヒント</span><span class="sxs-lookup"><span data-stu-id="8a926-115">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="8a926-116">さまざまな種類のメールヒントの値を表します。</span><span class="sxs-lookup"><span data-stu-id="8a926-116">Represents values for various types of mail tips.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8a926-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="8a926-117">Text value</span></span>

<span data-ttu-id="8a926-118">この要素のテキスト値は、配信の制限によって送信者のメッセージが受信者に届かないようにする場合は**true**です。</span><span class="sxs-lookup"><span data-stu-id="8a926-118">The text value of this element is **true** if delivery restrictions will prevent the sender's message from reaching the recipient.</span></span> <span data-ttu-id="8a926-119">配信の制限によって送信者のメッセージが受信者に到達できない場合、値は**false**になります。</span><span class="sxs-lookup"><span data-stu-id="8a926-119">The value is **false** if delivery restrictions will not prevent the sender's message from reaching the recipient.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="8a926-120">注釈</span><span class="sxs-lookup"><span data-stu-id="8a926-120">Remarks</span></span>

<span data-ttu-id="8a926-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="8a926-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8a926-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="8a926-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8a926-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="8a926-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8a926-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8a926-124">Schema Name</span></span>  <br/> |<span data-ttu-id="8a926-125">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="8a926-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="8a926-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8a926-126">Validation File</span></span>  <br/> |<span data-ttu-id="8a926-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="8a926-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8a926-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="8a926-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="8a926-129">正しくない</span><span class="sxs-lookup"><span data-stu-id="8a926-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8a926-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="8a926-130">See also</span></span>

- [<span data-ttu-id="8a926-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="8a926-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

