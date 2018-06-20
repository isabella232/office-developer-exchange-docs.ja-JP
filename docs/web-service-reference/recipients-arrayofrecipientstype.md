---
title: 受信者 (ArrayOfRecipientsType)
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
description: 宛先の要素は、メッセージのコピーを受け取る受信者のコレクションを表します。
ms.openlocfilehash: b24a029bfacd6cc40e85a201b8ca90efd7790e9f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832991"
---
# <a name="recipients-arrayofrecipientstype"></a><span data-ttu-id="727c8-103">受信者 (ArrayOfRecipientsType)</span><span class="sxs-lookup"><span data-stu-id="727c8-103">Recipients (ArrayOfRecipientsType)</span></span>

<span data-ttu-id="727c8-104">**宛先**の要素は、メッセージのコピーを受け取る受信者のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="727c8-104">The **Recipients** element represents a collection of recipients that receive a copy of the message.</span></span> 
  
```XML
<Recipients>
   <Mailbox/>
</Recipients>
```

 <span data-ttu-id="727c8-105">**ArrayOfRecipientsType**</span><span class="sxs-lookup"><span data-stu-id="727c8-105">**ArrayOfRecipientsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="727c8-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="727c8-106">Attributes and elements</span></span>

<span data-ttu-id="727c8-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="727c8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="727c8-108">属性</span><span class="sxs-lookup"><span data-stu-id="727c8-108">Attributes</span></span>

<span data-ttu-id="727c8-109">なし。</span><span class="sxs-lookup"><span data-stu-id="727c8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="727c8-110">子要素</span><span class="sxs-lookup"><span data-stu-id="727c8-110">Child elements</span></span>

|<span data-ttu-id="727c8-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="727c8-111">**Element**</span></span>|<span data-ttu-id="727c8-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="727c8-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="727c8-113">メールボックス</span><span class="sxs-lookup"><span data-stu-id="727c8-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="727c8-114">メールが有効な Active Directory のオブジェクトを識別します。</span><span class="sxs-lookup"><span data-stu-id="727c8-114">Identifies a mail-enabled Active Directory object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="727c8-115">親要素</span><span class="sxs-lookup"><span data-stu-id="727c8-115">Parent elements</span></span>

|<span data-ttu-id="727c8-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="727c8-116">**Element**</span></span>|<span data-ttu-id="727c8-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="727c8-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="727c8-118">GetMailTips</span><span class="sxs-lookup"><span data-stu-id="727c8-118">GetMailTips</span></span>](getmailtips.md) <br/> |<span data-ttu-id="727c8-119">受信者とメール ヒントの種類を取得するのにが含まれています。</span><span class="sxs-lookup"><span data-stu-id="727c8-119">Contains the recipients and types of mail tips to retrieve.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="727c8-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="727c8-120">Text value</span></span>

<span data-ttu-id="727c8-121">なし。</span><span class="sxs-lookup"><span data-stu-id="727c8-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="727c8-122">備考</span><span class="sxs-lookup"><span data-stu-id="727c8-122">Remarks</span></span>

<span data-ttu-id="727c8-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="727c8-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="727c8-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="727c8-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="727c8-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="727c8-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="727c8-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="727c8-126">Schema Name</span></span>  <br/> |<span data-ttu-id="727c8-127">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="727c8-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="727c8-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="727c8-128">Validation File</span></span>  <br/> |<span data-ttu-id="727c8-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="727c8-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="727c8-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="727c8-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="727c8-131">False</span><span class="sxs-lookup"><span data-stu-id="727c8-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="727c8-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="727c8-132">See also</span></span>



- [<span data-ttu-id="727c8-133">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="727c8-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

