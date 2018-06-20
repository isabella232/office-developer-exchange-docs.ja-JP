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
description: InvalidRecipients 要素は、無効な要求を共有フォルダーの受信者を表します。
ms.openlocfilehash: 02ad8935bde347c563875bf5bfb31968b70d81b6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831966"
---
# <a name="invalidrecipients"></a><span data-ttu-id="d080f-103">InvalidRecipients</span><span class="sxs-lookup"><span data-stu-id="d080f-103">InvalidRecipients</span></span>

<span data-ttu-id="d080f-104">**InvalidRecipients**要素は、無効な要求を共有フォルダーの受信者を表します。</span><span class="sxs-lookup"><span data-stu-id="d080f-104">The **InvalidRecipients** element represents the recipients of a folder sharing request that are invalid.</span></span> 
  
```XML
<InvalidRecipients>
   <InvalidRecipient/>
</InvalidRecipients>
```

 <span data-ttu-id="d080f-105">**ArrayOfInvalidRecipientsType**</span><span class="sxs-lookup"><span data-stu-id="d080f-105">**ArrayOfInvalidRecipientsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d080f-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="d080f-106">Attributes and elements</span></span>

<span data-ttu-id="d080f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d080f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d080f-108">属性</span><span class="sxs-lookup"><span data-stu-id="d080f-108">Attributes</span></span>

<span data-ttu-id="d080f-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d080f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d080f-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d080f-110">Child elements</span></span>

|<span data-ttu-id="d080f-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="d080f-111">**Element**</span></span>|<span data-ttu-id="d080f-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="d080f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d080f-113">InvalidRecipient</span><span class="sxs-lookup"><span data-stu-id="d080f-113">InvalidRecipient</span></span>](invalidrecipient.md) <br/> |<span data-ttu-id="d080f-114">受信者が有効な理由については、無効な受信者の SMTP アドレスが含まれています。</span><span class="sxs-lookup"><span data-stu-id="d080f-114">Contains the SMTP address of the invalid recipient and information about why the recipient is invalid.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d080f-115">親要素</span><span class="sxs-lookup"><span data-stu-id="d080f-115">Parent elements</span></span>

|<span data-ttu-id="d080f-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="d080f-116">**Element**</span></span>|<span data-ttu-id="d080f-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="d080f-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d080f-118">GetSharingMetadataResponse</span><span class="sxs-lookup"><span data-stu-id="d080f-118">GetSharingMetadataResponse</span></span>](getsharingmetadataresponse.md) <br/> |<span data-ttu-id="d080f-119">[GetSharingMetadata 操作](getsharingmetadata-operation.md)要求に対する応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="d080f-119">Defines a response to a [GetSharingMetadata operation](getsharingmetadata-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="d080f-120">GetSharingMetadataResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d080f-120">GetSharingMetadataResponseMessage</span></span>](getsharingmetadataresponsemessage.md) <br/> |<span data-ttu-id="d080f-121">状態および 1 つの結果が含まれています[GetSharingMetadata の操作](getsharingmetadata-operation.md)を要求します。</span><span class="sxs-lookup"><span data-stu-id="d080f-121">Contains the status and result of a single [GetSharingMetadata operation](getsharingmetadata-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d080f-122">備考</span><span class="sxs-lookup"><span data-stu-id="d080f-122">Remarks</span></span>

<span data-ttu-id="d080f-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="d080f-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d080f-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="d080f-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d080f-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="d080f-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d080f-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d080f-126">Schema Name</span></span>  <br/> |<span data-ttu-id="d080f-127">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="d080f-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d080f-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d080f-128">Validation File</span></span>  <br/> |<span data-ttu-id="d080f-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d080f-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d080f-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d080f-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="d080f-131">False</span><span class="sxs-lookup"><span data-stu-id="d080f-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d080f-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="d080f-132">See also</span></span>



[<span data-ttu-id="d080f-133">GetSharingMetadata 操作</span><span class="sxs-lookup"><span data-stu-id="d080f-133">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)


- [<span data-ttu-id="d080f-134">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="d080f-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

