---
title: ReplyBody
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ReplyBody
api_type:
- schema
ms.assetid: bb184144-3e4b-4419-a883-cc9fab1085e6
description: ReplyBody 要素には、Office (OOF) メッセージと、メッセージに使用する言語が含まれています。
ms.openlocfilehash: 8400dda1ee810781e129fcc44fd3cd5d6c15cbbe
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833116"
---
# <a name="replybody"></a><span data-ttu-id="6ba6c-103">ReplyBody</span><span class="sxs-lookup"><span data-stu-id="6ba6c-103">ReplyBody</span></span>

<span data-ttu-id="6ba6c-104">**ReplyBody**要素には、Office (OOF) メッセージと、メッセージに使用する言語が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6ba6c-104">The **ReplyBody** element contains an Out of Office (OOF) message and the language used for the message.</span></span> 
  
```XML
<ReplyBody xml:lang="">
   <Message/>
</ReplyBody>
```

 <span data-ttu-id="6ba6c-105">**ReplyBody**</span><span class="sxs-lookup"><span data-stu-id="6ba6c-105">**ReplyBody**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6ba6c-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="6ba6c-106">Attributes and elements</span></span>

<span data-ttu-id="6ba6c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6ba6c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6ba6c-108">属性</span><span class="sxs-lookup"><span data-stu-id="6ba6c-108">Attributes</span></span>

|<span data-ttu-id="6ba6c-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="6ba6c-109">**Attribute**</span></span>|<span data-ttu-id="6ba6c-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="6ba6c-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6ba6c-111">xml:lang</span><span class="sxs-lookup"><span data-stu-id="6ba6c-111">xml:lang</span></span>  <br/> |<span data-ttu-id="6ba6c-112">**ReplyBody**内容で使用する言語を指定します。</span><span class="sxs-lookup"><span data-stu-id="6ba6c-112">Specifies the language used in the **ReplyBody** contents.</span></span> <span data-ttu-id="6ba6c-113">この属性は、省略可能です。</span><span class="sxs-lookup"><span data-stu-id="6ba6c-113">This attribute is optional.</span></span> <span data-ttu-id="6ba6c-114">この属性に指定できる値は、IETF RFC 3066 で定義されます。</span><span class="sxs-lookup"><span data-stu-id="6ba6c-114">The possible values of this attribute are defined by IETF RFC 3066.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="6ba6c-115">子要素</span><span class="sxs-lookup"><span data-stu-id="6ba6c-115">Child elements</span></span>

|<span data-ttu-id="6ba6c-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="6ba6c-116">**Element**</span></span>|<span data-ttu-id="6ba6c-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="6ba6c-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6ba6c-118">メッセージ (可用性)</span><span class="sxs-lookup"><span data-stu-id="6ba6c-118">Message (Availability)</span></span>](message-availability.md) <br/> |<span data-ttu-id="6ba6c-119">不在 (oof) の応答が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6ba6c-119">Contains the out of office (OOF) response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6ba6c-120">親要素</span><span class="sxs-lookup"><span data-stu-id="6ba6c-120">Parent elements</span></span>

|<span data-ttu-id="6ba6c-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="6ba6c-121">**Element**</span></span>|<span data-ttu-id="6ba6c-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="6ba6c-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6ba6c-123">OutOfOffice</span><span class="sxs-lookup"><span data-stu-id="6ba6c-123">OutOfOffice</span></span>](outofoffice.md) <br/> |<span data-ttu-id="6ba6c-124">不在時の応答メッセージとメールボックスの応答メッセージを送信するための継続時間を定義します。</span><span class="sxs-lookup"><span data-stu-id="6ba6c-124">Defines the OOF response message and a duration time for sending the response message for a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6ba6c-125">テキスト値</span><span class="sxs-lookup"><span data-stu-id="6ba6c-125">Text value</span></span>

<span data-ttu-id="6ba6c-126">なし。</span><span class="sxs-lookup"><span data-stu-id="6ba6c-126">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6ba6c-127">備考</span><span class="sxs-lookup"><span data-stu-id="6ba6c-127">Remarks</span></span>

<span data-ttu-id="6ba6c-128">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="6ba6c-128">This element is required.</span></span>
  
<span data-ttu-id="6ba6c-129">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="6ba6c-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6ba6c-130">要素情報</span><span class="sxs-lookup"><span data-stu-id="6ba6c-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6ba6c-131">名前空間</span><span class="sxs-lookup"><span data-stu-id="6ba6c-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6ba6c-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6ba6c-132">Schema Name</span></span>  <br/> |<span data-ttu-id="6ba6c-133">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="6ba6c-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="6ba6c-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6ba6c-134">Validation File</span></span>  <br/> |<span data-ttu-id="6ba6c-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6ba6c-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6ba6c-136">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="6ba6c-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="6ba6c-137">False</span><span class="sxs-lookup"><span data-stu-id="6ba6c-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6ba6c-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="6ba6c-138">See also</span></span>



- [<span data-ttu-id="6ba6c-139">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="6ba6c-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

