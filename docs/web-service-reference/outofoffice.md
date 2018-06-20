---
title: OutOfOffice
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OutOfOffice
api_type:
- schema
ms.assetid: fe1256ab-5c0f-467d-abb3-b38a2dc312ae
description: OutOfOffice 要素は、応答メッセージと応答メッセージを送信するための継続時間を表します。
ms.openlocfilehash: 4e1e06ee332c44aeba03e1343c8c3258a2c9631e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832675"
---
# <a name="outofoffice"></a><span data-ttu-id="521ab-103">OutOfOffice</span><span class="sxs-lookup"><span data-stu-id="521ab-103">OutOfOffice</span></span>

<span data-ttu-id="521ab-104">**OutOfOffice**要素は、応答メッセージと応答メッセージを送信するための継続時間を表します。</span><span class="sxs-lookup"><span data-stu-id="521ab-104">The **OutOfOffice** element represents the response message and a duration time for sending the response message.</span></span> 
  
```XML
<OutOfOffice>
   <ReplyBody/>
   <Duration/>
</OutOfOffice>
```

 <span data-ttu-id="521ab-105">**OutOfOfficeMailTip**</span><span class="sxs-lookup"><span data-stu-id="521ab-105">**OutOfOfficeMailTip**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="521ab-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="521ab-106">Attributes and elements</span></span>

<span data-ttu-id="521ab-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="521ab-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="521ab-108">属性</span><span class="sxs-lookup"><span data-stu-id="521ab-108">Attributes</span></span>

<span data-ttu-id="521ab-109">なし。</span><span class="sxs-lookup"><span data-stu-id="521ab-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="521ab-110">子要素</span><span class="sxs-lookup"><span data-stu-id="521ab-110">Child elements</span></span>

|<span data-ttu-id="521ab-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="521ab-111">**Element**</span></span>|<span data-ttu-id="521ab-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="521ab-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="521ab-113">ReplyBody</span><span class="sxs-lookup"><span data-stu-id="521ab-113">ReplyBody</span></span>](replybody.md) <br/> |<span data-ttu-id="521ab-114">Office (OOF) メッセージと、メッセージに使用する言語が含まれています。</span><span class="sxs-lookup"><span data-stu-id="521ab-114">Contains an Out of Office (OOF) message and the language used for the message.</span></span>  <br/> |
|[<span data-ttu-id="521ab-115">期間 (UserOofSettings)</span><span class="sxs-lookup"><span data-stu-id="521ab-115">Duration (UserOofSettings)</span></span>](duration-useroofsettings.md) <br/> |<span data-ttu-id="521ab-116">[OofState](oofstate.md)要素は、[スケジュール済] に設定されている場合に、不在の状態が有効になっている期間が含まれています。</span><span class="sxs-lookup"><span data-stu-id="521ab-116">Contains the duration that the OOF status is enabled if the [OofState](oofstate.md) element is set to Scheduled.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="521ab-117">親要素</span><span class="sxs-lookup"><span data-stu-id="521ab-117">Parent elements</span></span>

|<span data-ttu-id="521ab-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="521ab-118">**Element**</span></span>|<span data-ttu-id="521ab-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="521ab-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="521ab-120">メール ヒント</span><span class="sxs-lookup"><span data-stu-id="521ab-120">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="521ab-121">さまざまな種類のメール ヒントの値を表します。</span><span class="sxs-lookup"><span data-stu-id="521ab-121">Represents values for various types of mail tips.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="521ab-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="521ab-122">Text value</span></span>

<span data-ttu-id="521ab-123">なし。</span><span class="sxs-lookup"><span data-stu-id="521ab-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="521ab-124">備考</span><span class="sxs-lookup"><span data-stu-id="521ab-124">Remarks</span></span>

<span data-ttu-id="521ab-125">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="521ab-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="521ab-126">要素情報</span><span class="sxs-lookup"><span data-stu-id="521ab-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="521ab-127">名前空間</span><span class="sxs-lookup"><span data-stu-id="521ab-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="521ab-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="521ab-128">Schema Name</span></span>  <br/> |<span data-ttu-id="521ab-129">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="521ab-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="521ab-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="521ab-130">Validation File</span></span>  <br/> |<span data-ttu-id="521ab-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="521ab-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="521ab-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="521ab-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="521ab-133">False</span><span class="sxs-lookup"><span data-stu-id="521ab-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="521ab-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="521ab-134">See also</span></span>



- [<span data-ttu-id="521ab-135">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="521ab-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

