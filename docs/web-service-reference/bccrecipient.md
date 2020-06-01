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
description: BccRecipient 要素は、電子メールメッセージのブラインドカーボンコピー (Bcc) を受信するための受信者を表します。
ms.openlocfilehash: 8296af1d74338bdfb1f4cb7bc7449ad91a9cd531
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461528"
---
# <a name="bccrecipient"></a><span data-ttu-id="57c1d-103">BccRecipient</span><span class="sxs-lookup"><span data-stu-id="57c1d-103">BccRecipient</span></span>

<span data-ttu-id="57c1d-104">**BccRecipient**要素は、電子メールメッセージのブラインドカーボンコピー (bcc) を受信するための受信者を表します。</span><span class="sxs-lookup"><span data-stu-id="57c1d-104">The **BccRecipient** element represents a recipient to receive a blind carbon copy (Bcc) of an e-mail message.</span></span> 
  
```XML
<BccRecipient>true | false</BccRecipient>
```

 <span data-ttu-id="57c1d-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="57c1d-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="57c1d-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="57c1d-106">Attributes and elements</span></span>

<span data-ttu-id="57c1d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="57c1d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="57c1d-108">属性</span><span class="sxs-lookup"><span data-stu-id="57c1d-108">Attributes</span></span>

<span data-ttu-id="57c1d-109">なし。</span><span class="sxs-lookup"><span data-stu-id="57c1d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="57c1d-110">子要素</span><span class="sxs-lookup"><span data-stu-id="57c1d-110">Child elements</span></span>

<span data-ttu-id="57c1d-111">なし。</span><span class="sxs-lookup"><span data-stu-id="57c1d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="57c1d-112">親要素</span><span class="sxs-lookup"><span data-stu-id="57c1d-112">Parent elements</span></span>

|<span data-ttu-id="57c1d-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="57c1d-113">**Element**</span></span>|<span data-ttu-id="57c1d-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="57c1d-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="57c1d-115">受信者 Trackingイベント</span><span class="sxs-lookup"><span data-stu-id="57c1d-115">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="57c1d-116">受信者に対する1つのイベントに関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="57c1d-116">Contains information for a single event for a recipient.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="57c1d-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="57c1d-117">Text value</span></span>

<span data-ttu-id="57c1d-118">この要素は、 **true**または**false**のいずれかになります。</span><span class="sxs-lookup"><span data-stu-id="57c1d-118">This element can be either **true** or **false**.</span></span> <span data-ttu-id="57c1d-119">値**true**は、受信者がブラインドカーボンコピーされたことを示します。値が**false**の場合、受信者がブラインドカーボンコピーされていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="57c1d-119">A value of **true** indicates that the recipient is blind carbon copied; a value of **false** indicates that the recipient is not blind carbon copied.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="57c1d-120">注釈</span><span class="sxs-lookup"><span data-stu-id="57c1d-120">Remarks</span></span>

<span data-ttu-id="57c1d-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="57c1d-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="57c1d-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="57c1d-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="57c1d-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="57c1d-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="57c1d-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="57c1d-124">Schema Name</span></span>  <br/> |<span data-ttu-id="57c1d-125">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="57c1d-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="57c1d-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="57c1d-126">Validation File</span></span>  <br/> |<span data-ttu-id="57c1d-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="57c1d-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="57c1d-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="57c1d-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="57c1d-129">正しくない</span><span class="sxs-lookup"><span data-stu-id="57c1d-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="57c1d-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="57c1d-130">See also</span></span>



- [<span data-ttu-id="57c1d-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="57c1d-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

