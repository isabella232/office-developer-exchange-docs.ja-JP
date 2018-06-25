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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832991"
---
# <a name="recipients-arrayofrecipientstype"></a><span data-ttu-id="c514f-103">受信者 (ArrayOfRecipientsType)</span><span class="sxs-lookup"><span data-stu-id="c514f-103">Recipients (ArrayOfRecipientsType)</span></span>

<span data-ttu-id="c514f-104">**宛先**の要素は、メッセージのコピーを受け取る受信者のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="c514f-104">The **Recipients** element represents a collection of recipients that receive a copy of the message.</span></span> 
  
```XML
<Recipients>
   <Mailbox/>
</Recipients>
```

 <span data-ttu-id="c514f-105">**ArrayOfRecipientsType**</span><span class="sxs-lookup"><span data-stu-id="c514f-105">**ArrayOfRecipientsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c514f-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="c514f-106">Attributes and elements</span></span>

<span data-ttu-id="c514f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c514f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c514f-108">属性</span><span class="sxs-lookup"><span data-stu-id="c514f-108">Attributes</span></span>

<span data-ttu-id="c514f-109">なし。</span><span class="sxs-lookup"><span data-stu-id="c514f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c514f-110">子要素</span><span class="sxs-lookup"><span data-stu-id="c514f-110">Child elements</span></span>

|<span data-ttu-id="c514f-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="c514f-111">**Element**</span></span>|<span data-ttu-id="c514f-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="c514f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c514f-113">メールボックス</span><span class="sxs-lookup"><span data-stu-id="c514f-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="c514f-114">メールが有効な Active Directory のオブジェクトを識別します。</span><span class="sxs-lookup"><span data-stu-id="c514f-114">Identifies a mail-enabled Active Directory object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c514f-115">親要素</span><span class="sxs-lookup"><span data-stu-id="c514f-115">Parent elements</span></span>

|<span data-ttu-id="c514f-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="c514f-116">**Element**</span></span>|<span data-ttu-id="c514f-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="c514f-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c514f-118">GetMailTips</span><span class="sxs-lookup"><span data-stu-id="c514f-118">GetMailTips</span></span>](getmailtips.md) <br/> |<span data-ttu-id="c514f-119">受信者とメール ヒントの種類を取得するのにが含まれています。</span><span class="sxs-lookup"><span data-stu-id="c514f-119">Contains the recipients and types of mail tips to retrieve.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c514f-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="c514f-120">Text value</span></span>

<span data-ttu-id="c514f-121">なし。</span><span class="sxs-lookup"><span data-stu-id="c514f-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c514f-122">備考</span><span class="sxs-lookup"><span data-stu-id="c514f-122">Remarks</span></span>

<span data-ttu-id="c514f-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="c514f-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c514f-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="c514f-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c514f-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="c514f-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c514f-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c514f-126">Schema Name</span></span>  <br/> |<span data-ttu-id="c514f-127">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="c514f-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="c514f-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c514f-128">Validation File</span></span>  <br/> |<span data-ttu-id="c514f-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c514f-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c514f-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="c514f-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="c514f-131">False</span><span class="sxs-lookup"><span data-stu-id="c514f-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c514f-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="c514f-132">See also</span></span>



- [<span data-ttu-id="c514f-133">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="c514f-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

