---
title: BccRecipient
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- BccRecipient
api_type:
- schema
ms.assetid: 4ef0cff5-8a5a-4d76-9d2b-938774d8fc1b
description: BccRecipient 要素は、電子メール メッセージのブラインド カーボン コピー (Bcc) を受信する受信者を表します。
ms.openlocfilehash: bed58536263196a61651493e92a4dcd1df3f5ec9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759492"
---
# <a name="bccrecipient"></a><span data-ttu-id="cf5f7-103">BccRecipient</span><span class="sxs-lookup"><span data-stu-id="cf5f7-103">BccRecipient</span></span>

<span data-ttu-id="cf5f7-104">**BccRecipient**要素は、電子メール メッセージのブラインド カーボン コピー (Bcc) を受信する受信者を表します。</span><span class="sxs-lookup"><span data-stu-id="cf5f7-104">The **BccRecipient** element represents a recipient to receive a blind carbon copy (Bcc) of an e-mail message.</span></span> 
  
```XML
<BccRecipient>true | false</BccRecipient>
```

 <span data-ttu-id="cf5f7-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="cf5f7-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cf5f7-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="cf5f7-106">Attributes and elements</span></span>

<span data-ttu-id="cf5f7-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="cf5f7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cf5f7-108">属性</span><span class="sxs-lookup"><span data-stu-id="cf5f7-108">Attributes</span></span>

<span data-ttu-id="cf5f7-109">なし。</span><span class="sxs-lookup"><span data-stu-id="cf5f7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cf5f7-110">子要素</span><span class="sxs-lookup"><span data-stu-id="cf5f7-110">Child elements</span></span>

<span data-ttu-id="cf5f7-111">なし。</span><span class="sxs-lookup"><span data-stu-id="cf5f7-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="cf5f7-112">親要素</span><span class="sxs-lookup"><span data-stu-id="cf5f7-112">Parent elements</span></span>

|<span data-ttu-id="cf5f7-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="cf5f7-113">**Element**</span></span>|<span data-ttu-id="cf5f7-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="cf5f7-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cf5f7-115">RecipientTrackingEvent</span><span class="sxs-lookup"><span data-stu-id="cf5f7-115">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="cf5f7-116">受信者の 1 つのイベントの情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="cf5f7-116">Contains information for a single event for a recipient.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="cf5f7-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="cf5f7-117">Text value</span></span>

<span data-ttu-id="cf5f7-118">この要素には、 **true**または**false**のいずれかができます。</span><span class="sxs-lookup"><span data-stu-id="cf5f7-118">This element can be either **true** or **false**.</span></span> <span data-ttu-id="cf5f7-119">**True**の値の場合、受信者がブラインドのカーボン コピーであることを示します**false**の値は、受信者は、視覚に障害のカーボン コピーではないことを示します。</span><span class="sxs-lookup"><span data-stu-id="cf5f7-119">A value of **true** indicates that the recipient is blind carbon copied; a value of **false** indicates that the recipient is not blind carbon copied.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="cf5f7-120">備考</span><span class="sxs-lookup"><span data-stu-id="cf5f7-120">Remarks</span></span>

<span data-ttu-id="cf5f7-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="cf5f7-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cf5f7-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="cf5f7-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cf5f7-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="cf5f7-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cf5f7-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="cf5f7-124">Schema Name</span></span>  <br/> |<span data-ttu-id="cf5f7-125">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="cf5f7-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="cf5f7-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="cf5f7-126">Validation File</span></span>  <br/> |<span data-ttu-id="cf5f7-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="cf5f7-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="cf5f7-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="cf5f7-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="cf5f7-129">False</span><span class="sxs-lookup"><span data-stu-id="cf5f7-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cf5f7-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="cf5f7-130">See also</span></span>



- [<span data-ttu-id="cf5f7-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="cf5f7-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

