---
title: InvalidRecipient
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- InvalidRecipient
api_type:
- schema
ms.assetid: 9e2d3433-22d7-444b-9883-e5649297d8fe
description: InvalidRecipient 要素には、受信者が有効な理由については、無効な受信者の SMTP アドレスが含まれています。
ms.openlocfilehash: 800056666e486e9337dcd1c2786f7e6db1e060bb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831961"
---
# <a name="invalidrecipient"></a><span data-ttu-id="a6684-103">InvalidRecipient</span><span class="sxs-lookup"><span data-stu-id="a6684-103">InvalidRecipient</span></span>

<span data-ttu-id="a6684-104">**InvalidRecipient**要素には、受信者が有効な理由については、無効な受信者の SMTP アドレスが含まれています。</span><span class="sxs-lookup"><span data-stu-id="a6684-104">The **InvalidRecipient** element contains the SMTP address of the invalid recipient and information about why the recipient is invalid.</span></span> 
  
```XML
<InvalidRecipient>
   <SmtpAddress/>
   <ResponseCode/>
   <MessageText/>
</InvalidRecipient>

```

 <span data-ttu-id="a6684-105">**InvalidRecipientType**</span><span class="sxs-lookup"><span data-stu-id="a6684-105">**InvalidRecipientType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a6684-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="a6684-106">Attributes and elements</span></span>

<span data-ttu-id="a6684-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a6684-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a6684-108">属性</span><span class="sxs-lookup"><span data-stu-id="a6684-108">Attributes</span></span>

<span data-ttu-id="a6684-109">なし。</span><span class="sxs-lookup"><span data-stu-id="a6684-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a6684-110">子要素</span><span class="sxs-lookup"><span data-stu-id="a6684-110">Child elements</span></span>

|<span data-ttu-id="a6684-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="a6684-111">**Element**</span></span>|<span data-ttu-id="a6684-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="a6684-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a6684-113">SmtpAddress</span><span class="sxs-lookup"><span data-stu-id="a6684-113">SmtpAddress</span></span>](smtpaddress.md) <br/> |<span data-ttu-id="a6684-114">無効な受信者の SMTP アドレスが含まれています。</span><span class="sxs-lookup"><span data-stu-id="a6684-114">Contains the SMTP address of the invalid recipient.</span></span> <span data-ttu-id="a6684-115">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="a6684-115">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="a6684-116">ResponseCode (InvalidRecipientResponseCodeType)</span><span class="sxs-lookup"><span data-stu-id="a6684-116">ResponseCode (InvalidRecipientResponseCodeType)</span></span>](responsecode-invalidrecipientresponsecodetype.md) <br/> |<span data-ttu-id="a6684-117">要求で発生した特定のエラーを識別するエラー コードを提供します。</span><span class="sxs-lookup"><span data-stu-id="a6684-117">Provides an error code that identifies the specific error that the request encountered.</span></span> <span data-ttu-id="a6684-118">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="a6684-118">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="a6684-119">MessageText</span><span class="sxs-lookup"><span data-stu-id="a6684-119">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="a6684-120">応答のステータスの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="a6684-120">Provides a text description of the status of the response.</span></span> <span data-ttu-id="a6684-121">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="a6684-121">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a6684-122">親要素</span><span class="sxs-lookup"><span data-stu-id="a6684-122">Parent elements</span></span>

|<span data-ttu-id="a6684-123">**要素**</span><span class="sxs-lookup"><span data-stu-id="a6684-123">**Element**</span></span>|<span data-ttu-id="a6684-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="a6684-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a6684-125">InvalidRecipients</span><span class="sxs-lookup"><span data-stu-id="a6684-125">InvalidRecipients</span></span>](invalidrecipients.md) <br/> |<span data-ttu-id="a6684-126">無効な要求を共有フォルダーの受信者を表します。</span><span class="sxs-lookup"><span data-stu-id="a6684-126">Represents the recipients of a folder sharing request that are invalid.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a6684-127">備考</span><span class="sxs-lookup"><span data-stu-id="a6684-127">Remarks</span></span>

<span data-ttu-id="a6684-128">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="a6684-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a6684-129">要素情報</span><span class="sxs-lookup"><span data-stu-id="a6684-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a6684-130">名前空間</span><span class="sxs-lookup"><span data-stu-id="a6684-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a6684-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a6684-131">Schema Name</span></span>  <br/> |<span data-ttu-id="a6684-132">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="a6684-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="a6684-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a6684-133">Validation File</span></span>  <br/> |<span data-ttu-id="a6684-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a6684-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a6684-135">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="a6684-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="a6684-136">False</span><span class="sxs-lookup"><span data-stu-id="a6684-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a6684-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="a6684-137">See also</span></span>



[<span data-ttu-id="a6684-138">GetSharingMetadata 操作</span><span class="sxs-lookup"><span data-stu-id="a6684-138">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)


- [<span data-ttu-id="a6684-139">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="a6684-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

