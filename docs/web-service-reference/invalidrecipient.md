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
description: InvalidRecipient 要素には、無効な受信者の SMTP アドレスと、受信者が無効である理由に関する情報が含まれています。
ms.openlocfilehash: f301b31c1054625151ce90e41fca5e3efc21f473
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526551"
---
# <a name="invalidrecipient"></a><span data-ttu-id="bd5ce-103">InvalidRecipient</span><span class="sxs-lookup"><span data-stu-id="bd5ce-103">InvalidRecipient</span></span>

<span data-ttu-id="bd5ce-104">**Invalidrecipient**要素には、無効な受信者の SMTP アドレスと、受信者が無効である理由に関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="bd5ce-104">The **InvalidRecipient** element contains the SMTP address of the invalid recipient and information about why the recipient is invalid.</span></span> 
  
```XML
<InvalidRecipient>
   <SmtpAddress/>
   <ResponseCode/>
   <MessageText/>
</InvalidRecipient>

```

 <span data-ttu-id="bd5ce-105">**Invalid受信者の種類**</span><span class="sxs-lookup"><span data-stu-id="bd5ce-105">**InvalidRecipientType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bd5ce-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="bd5ce-106">Attributes and elements</span></span>

<span data-ttu-id="bd5ce-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="bd5ce-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bd5ce-108">属性</span><span class="sxs-lookup"><span data-stu-id="bd5ce-108">Attributes</span></span>

<span data-ttu-id="bd5ce-109">なし。</span><span class="sxs-lookup"><span data-stu-id="bd5ce-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bd5ce-110">子要素</span><span class="sxs-lookup"><span data-stu-id="bd5ce-110">Child elements</span></span>

|<span data-ttu-id="bd5ce-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="bd5ce-111">**Element**</span></span>|<span data-ttu-id="bd5ce-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="bd5ce-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bd5ce-113">SmtpAddress</span><span class="sxs-lookup"><span data-stu-id="bd5ce-113">SmtpAddress</span></span>](smtpaddress.md) <br/> |<span data-ttu-id="bd5ce-114">無効な受信者の SMTP アドレスを含みます。</span><span class="sxs-lookup"><span data-stu-id="bd5ce-114">Contains the SMTP address of the invalid recipient.</span></span> <span data-ttu-id="bd5ce-115">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="bd5ce-115">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="bd5ce-116">応答 Secmode (Invalid受信者応答 Secodetype)</span><span class="sxs-lookup"><span data-stu-id="bd5ce-116">ResponseCode (InvalidRecipientResponseCodeType)</span></span>](responsecode-invalidrecipientresponsecodetype.md) <br/> |<span data-ttu-id="bd5ce-117">要求で発生した特定のエラーを識別するエラーコードを提供します。</span><span class="sxs-lookup"><span data-stu-id="bd5ce-117">Provides an error code that identifies the specific error that the request encountered.</span></span> <span data-ttu-id="bd5ce-118">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="bd5ce-118">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="bd5ce-119">MessageText</span><span class="sxs-lookup"><span data-stu-id="bd5ce-119">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="bd5ce-120">応答の状態を説明するテキストを提供します。</span><span class="sxs-lookup"><span data-stu-id="bd5ce-120">Provides a text description of the status of the response.</span></span> <span data-ttu-id="bd5ce-121">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="bd5ce-121">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bd5ce-122">親要素</span><span class="sxs-lookup"><span data-stu-id="bd5ce-122">Parent elements</span></span>

|<span data-ttu-id="bd5ce-123">**要素**</span><span class="sxs-lookup"><span data-stu-id="bd5ce-123">**Element**</span></span>|<span data-ttu-id="bd5ce-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="bd5ce-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bd5ce-125">InvalidRecipients</span><span class="sxs-lookup"><span data-stu-id="bd5ce-125">InvalidRecipients</span></span>](invalidrecipients.md) <br/> |<span data-ttu-id="bd5ce-126">無効なフォルダー共有要求の受信者を表します。</span><span class="sxs-lookup"><span data-stu-id="bd5ce-126">Represents the recipients of a folder sharing request that are invalid.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="bd5ce-127">注釈</span><span class="sxs-lookup"><span data-stu-id="bd5ce-127">Remarks</span></span>

<span data-ttu-id="bd5ce-128">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="bd5ce-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bd5ce-129">要素の情報</span><span class="sxs-lookup"><span data-stu-id="bd5ce-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bd5ce-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="bd5ce-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bd5ce-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="bd5ce-131">Schema Name</span></span>  <br/> |<span data-ttu-id="bd5ce-132">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="bd5ce-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="bd5ce-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="bd5ce-133">Validation File</span></span>  <br/> |<span data-ttu-id="bd5ce-134">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="bd5ce-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bd5ce-135">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="bd5ce-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="bd5ce-136">正しくない</span><span class="sxs-lookup"><span data-stu-id="bd5ce-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bd5ce-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="bd5ce-137">See also</span></span>



[<span data-ttu-id="bd5ce-138">GetSharingMetadata 操作</span><span class="sxs-lookup"><span data-stu-id="bd5ce-138">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)


- [<span data-ttu-id="bd5ce-139">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="bd5ce-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

