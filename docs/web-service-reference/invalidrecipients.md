---
title: InvalidRecipients
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- InvalidRecipients
api_type:
- schema
ms.assetid: e4e7b50e-2fa9-4649-94a6-6002f341ecc4
description: InvalidRecipients 要素は、無効なフォルダー共有要求の受信者を表します。
ms.openlocfilehash: 99e0817f0ff873c4732b03cc7d68aa8e0070813c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465563"
---
# <a name="invalidrecipients"></a><span data-ttu-id="7eb3b-103">InvalidRecipients</span><span class="sxs-lookup"><span data-stu-id="7eb3b-103">InvalidRecipients</span></span>

<span data-ttu-id="7eb3b-104">**Invalidrecipients**要素は、無効なフォルダー共有要求の受信者を表します。</span><span class="sxs-lookup"><span data-stu-id="7eb3b-104">The **InvalidRecipients** element represents the recipients of a folder sharing request that are invalid.</span></span> 
  
```XML
<InvalidRecipients>
   <InvalidRecipient/>
</InvalidRecipients>
```

 <span data-ttu-id="7eb3b-105">**Arrayofinvalid受信者 Stype**</span><span class="sxs-lookup"><span data-stu-id="7eb3b-105">**ArrayOfInvalidRecipientsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7eb3b-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="7eb3b-106">Attributes and elements</span></span>

<span data-ttu-id="7eb3b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7eb3b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7eb3b-108">属性</span><span class="sxs-lookup"><span data-stu-id="7eb3b-108">Attributes</span></span>

<span data-ttu-id="7eb3b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="7eb3b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7eb3b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="7eb3b-110">Child elements</span></span>

|<span data-ttu-id="7eb3b-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="7eb3b-111">**Element**</span></span>|<span data-ttu-id="7eb3b-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="7eb3b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7eb3b-113">InvalidRecipient</span><span class="sxs-lookup"><span data-stu-id="7eb3b-113">InvalidRecipient</span></span>](invalidrecipient.md) <br/> |<span data-ttu-id="7eb3b-114">無効な受信者の SMTP アドレスと、受信者が無効である理由についての情報を格納します。</span><span class="sxs-lookup"><span data-stu-id="7eb3b-114">Contains the SMTP address of the invalid recipient and information about why the recipient is invalid.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7eb3b-115">親要素</span><span class="sxs-lookup"><span data-stu-id="7eb3b-115">Parent elements</span></span>

|<span data-ttu-id="7eb3b-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="7eb3b-116">**Element**</span></span>|<span data-ttu-id="7eb3b-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="7eb3b-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7eb3b-118">GetSharingMetadataResponse</span><span class="sxs-lookup"><span data-stu-id="7eb3b-118">GetSharingMetadataResponse</span></span>](getsharingmetadataresponse.md) <br/> |<span data-ttu-id="7eb3b-119">[Getsharingmetadata 操作](getsharingmetadata-operation.md)要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="7eb3b-119">Defines a response to a [GetSharingMetadata operation](getsharingmetadata-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="7eb3b-120">GetSharingMetadataResponseMessage</span><span class="sxs-lookup"><span data-stu-id="7eb3b-120">GetSharingMetadataResponseMessage</span></span>](getsharingmetadataresponsemessage.md) <br/> |<span data-ttu-id="7eb3b-121">1つの[Getsharingmetadata 操作](getsharingmetadata-operation.md)要求の状態と結果を格納します。</span><span class="sxs-lookup"><span data-stu-id="7eb3b-121">Contains the status and result of a single [GetSharingMetadata operation](getsharingmetadata-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7eb3b-122">注釈</span><span class="sxs-lookup"><span data-stu-id="7eb3b-122">Remarks</span></span>

<span data-ttu-id="7eb3b-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="7eb3b-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7eb3b-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="7eb3b-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7eb3b-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="7eb3b-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7eb3b-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7eb3b-126">Schema Name</span></span>  <br/> |<span data-ttu-id="7eb3b-127">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="7eb3b-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7eb3b-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7eb3b-128">Validation File</span></span>  <br/> |<span data-ttu-id="7eb3b-129">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="7eb3b-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7eb3b-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="7eb3b-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="7eb3b-131">正しくない</span><span class="sxs-lookup"><span data-stu-id="7eb3b-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7eb3b-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="7eb3b-132">See also</span></span>



[<span data-ttu-id="7eb3b-133">GetSharingMetadata 操作</span><span class="sxs-lookup"><span data-stu-id="7eb3b-133">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)


- [<span data-ttu-id="7eb3b-134">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="7eb3b-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

