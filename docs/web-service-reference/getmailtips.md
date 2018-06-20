---
title: GetMailTips
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetMailTips
api_type:
- schema
ms.assetid: 4a24ff79-f1ae-43a1-9ac2-49baf3eaa173
description: GetMailTips 要素を取得するには、受信者とメール ヒントの種類を表します。
ms.openlocfilehash: aad3b3d9dd578d0c92bf7d48ee8b78b58c63e23d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760785"
---
# <a name="getmailtips"></a><span data-ttu-id="fef28-103">GetMailTips</span><span class="sxs-lookup"><span data-stu-id="fef28-103">GetMailTips</span></span>

<span data-ttu-id="fef28-104">**GetMailTips**要素を取得するには、受信者とメール ヒントの種類を表します。</span><span class="sxs-lookup"><span data-stu-id="fef28-104">The **GetMailTips** element represents the recipients and types of mail tips to retrieve.</span></span> 
  
```XML
<GetMailTips>
   <SendingAs/>
   <Recipients/>
   <MailTipsRequested/>
</GetMailTips>
```

 <span data-ttu-id="fef28-105">**GetMailTipsType**</span><span class="sxs-lookup"><span data-stu-id="fef28-105">**GetMailTipsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fef28-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="fef28-106">Attributes and elements</span></span>

<span data-ttu-id="fef28-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="fef28-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fef28-108">属性</span><span class="sxs-lookup"><span data-stu-id="fef28-108">Attributes</span></span>

<span data-ttu-id="fef28-109">なし。</span><span class="sxs-lookup"><span data-stu-id="fef28-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fef28-110">子要素</span><span class="sxs-lookup"><span data-stu-id="fef28-110">Child elements</span></span>

|<span data-ttu-id="fef28-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="fef28-111">**Element**</span></span>|<span data-ttu-id="fef28-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="fef28-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fef28-113">SendingAs</span><span class="sxs-lookup"><span data-stu-id="fef28-113">SendingAs</span></span>](sendingas.md) <br/> |<span data-ttu-id="fef28-114">として送信しようとしてユーザーの電子メール アドレスが含まれています。</span><span class="sxs-lookup"><span data-stu-id="fef28-114">Contains an e-mail address that a user is trying to send as.</span></span>  <br/> |
|[<span data-ttu-id="fef28-115">受信者 (ArrayOfRecipientsType)</span><span class="sxs-lookup"><span data-stu-id="fef28-115">Recipients (ArrayOfRecipientsType)</span></span>](recipients-arrayofrecipientstype.md) <br/> |<span data-ttu-id="fef28-116">メール ヒントを確認するのには受信者の一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="fef28-116">Contains a list of recipients to check for mail tips.</span></span>  <br/> |
|[<span data-ttu-id="fef28-117">MailTipsRequested</span><span class="sxs-lookup"><span data-stu-id="fef28-117">MailTipsRequested</span></span>](mailtipsrequested.md) <br/> |<span data-ttu-id="fef28-118">サービスから要求されたメール ヒントの種類が含まれています。</span><span class="sxs-lookup"><span data-stu-id="fef28-118">Contains the types of mail tips requested from the service.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fef28-119">親要素</span><span class="sxs-lookup"><span data-stu-id="fef28-119">Parent elements</span></span>

<span data-ttu-id="fef28-120">なし。</span><span class="sxs-lookup"><span data-stu-id="fef28-120">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="fef28-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="fef28-121">Text value</span></span>

<span data-ttu-id="fef28-122">なし。</span><span class="sxs-lookup"><span data-stu-id="fef28-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="fef28-123">備考</span><span class="sxs-lookup"><span data-stu-id="fef28-123">Remarks</span></span>

<span data-ttu-id="fef28-124">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="fef28-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fef28-125">要素情報</span><span class="sxs-lookup"><span data-stu-id="fef28-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fef28-126">名前空間</span><span class="sxs-lookup"><span data-stu-id="fef28-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="fef28-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="fef28-127">Schema Name</span></span>  <br/> |<span data-ttu-id="fef28-128">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="fef28-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="fef28-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="fef28-129">Validation File</span></span>  <br/> |<span data-ttu-id="fef28-130">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="fef28-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fef28-131">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="fef28-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="fef28-132">False</span><span class="sxs-lookup"><span data-stu-id="fef28-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fef28-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="fef28-133">See also</span></span>



- [<span data-ttu-id="fef28-134">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="fef28-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

