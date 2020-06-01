---
title: 受信者 (Arrayof受信者 Stype)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Recipients
api_type:
- schema
ms.assetid: f4b71403-cbae-4176-8b2e-3597048c057b
description: Recipients 要素は、メッセージのコピーを受信する受信者のコレクションを表します。
ms.openlocfilehash: 0e18152a8143b888ad27f48137c06613694f5713
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463875"
---
# <a name="recipients-arrayofrecipientstype"></a><span data-ttu-id="e8e84-103">受信者 (Arrayof受信者 Stype)</span><span class="sxs-lookup"><span data-stu-id="e8e84-103">Recipients (ArrayOfRecipientsType)</span></span>

<span data-ttu-id="e8e84-104">**Recipients**要素は、メッセージのコピーを受信する受信者のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="e8e84-104">The **Recipients** element represents a collection of recipients that receive a copy of the message.</span></span> 
  
```XML
<Recipients>
   <Mailbox/>
</Recipients>
```

 <span data-ttu-id="e8e84-105">**Arrayof受信者 Stype**</span><span class="sxs-lookup"><span data-stu-id="e8e84-105">**ArrayOfRecipientsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e8e84-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="e8e84-106">Attributes and elements</span></span>

<span data-ttu-id="e8e84-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e8e84-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e8e84-108">属性</span><span class="sxs-lookup"><span data-stu-id="e8e84-108">Attributes</span></span>

<span data-ttu-id="e8e84-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e8e84-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e8e84-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e8e84-110">Child elements</span></span>

|<span data-ttu-id="e8e84-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="e8e84-111">**Element**</span></span>|<span data-ttu-id="e8e84-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="e8e84-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e8e84-113">メールボックス</span><span class="sxs-lookup"><span data-stu-id="e8e84-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="e8e84-114">メールが有効な Active Directory オブジェクトを識別します。</span><span class="sxs-lookup"><span data-stu-id="e8e84-114">Identifies a mail-enabled Active Directory object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e8e84-115">親要素</span><span class="sxs-lookup"><span data-stu-id="e8e84-115">Parent elements</span></span>

|<span data-ttu-id="e8e84-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="e8e84-116">**Element**</span></span>|<span data-ttu-id="e8e84-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="e8e84-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e8e84-118">GetMailTips</span><span class="sxs-lookup"><span data-stu-id="e8e84-118">GetMailTips</span></span>](getmailtips.md) <br/> |<span data-ttu-id="e8e84-119">取得するメールヒントの受信者と種類が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e8e84-119">Contains the recipients and types of mail tips to retrieve.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e8e84-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="e8e84-120">Text value</span></span>

<span data-ttu-id="e8e84-121">なし。</span><span class="sxs-lookup"><span data-stu-id="e8e84-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e8e84-122">注釈</span><span class="sxs-lookup"><span data-stu-id="e8e84-122">Remarks</span></span>

<span data-ttu-id="e8e84-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="e8e84-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e8e84-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="e8e84-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e8e84-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="e8e84-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e8e84-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e8e84-126">Schema Name</span></span>  <br/> |<span data-ttu-id="e8e84-127">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="e8e84-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="e8e84-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e8e84-128">Validation File</span></span>  <br/> |<span data-ttu-id="e8e84-129">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="e8e84-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e8e84-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="e8e84-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="e8e84-131">正しくない</span><span class="sxs-lookup"><span data-stu-id="e8e84-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e8e84-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="e8e84-132">See also</span></span>



- [<span data-ttu-id="e8e84-133">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="e8e84-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

