---
title: AlternateMailboxes (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 9a0859c5-fa23-4496-9b63-15c97818f857
description: AlternateMailboxes 要素は、メールボックスを別のコレクションを表します。
ms.openlocfilehash: 31662ebdcb8286feb506e59c10d45055d71d6652
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759315"
---
# <a name="alternatemailboxes-soap"></a><span data-ttu-id="32498-103">AlternateMailboxes (SOAP)</span><span class="sxs-lookup"><span data-stu-id="32498-103">AlternateMailboxes (SOAP)</span></span>

<span data-ttu-id="32498-104">**AlternateMailboxes**要素は、メールボックスを別のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="32498-104">The **AlternateMailboxes** element represents a collection of alternate mailboxes.</span></span> 
  
```XML
<AlternateMailboxes>
   <AlternateMailbox/>
</AlternateMailboxes>
```

 <span data-ttu-id="32498-105">**AlternateMailboxes**</span><span class="sxs-lookup"><span data-stu-id="32498-105">**AlternateMailboxes**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="32498-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="32498-106">Attributes and elements</span></span>

<span data-ttu-id="32498-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="32498-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="32498-108">属性</span><span class="sxs-lookup"><span data-stu-id="32498-108">Attributes</span></span>

<span data-ttu-id="32498-109">なし。</span><span class="sxs-lookup"><span data-stu-id="32498-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="32498-110">子要素</span><span class="sxs-lookup"><span data-stu-id="32498-110">Child elements</span></span>

|<span data-ttu-id="32498-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="32498-111">**Element**</span></span>|<span data-ttu-id="32498-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="32498-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="32498-113">AlternateMailbox (SOAP)</span><span class="sxs-lookup"><span data-stu-id="32498-113">AlternateMailbox (SOAP)</span></span>](alternatemailbox-soap.md) <br/> |<span data-ttu-id="32498-114">別のメールボックスを表します。</span><span class="sxs-lookup"><span data-stu-id="32498-114">Represents an alternate mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="32498-115">親要素</span><span class="sxs-lookup"><span data-stu-id="32498-115">Parent elements</span></span>

|<span data-ttu-id="32498-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="32498-116">**Element**</span></span>|<span data-ttu-id="32498-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="32498-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="32498-118">AlternateMailboxCollectionSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="32498-118">AlternateMailboxCollectionSetting (SOAP)</span></span>](alternatemailboxcollectionsetting-soap.md) <br/> |<span data-ttu-id="32498-119">代替メールボックスの設定のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="32498-119">Contains a collection of alternate mailbox settings.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="32498-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="32498-120">Text value</span></span>

<span data-ttu-id="32498-121">なし。</span><span class="sxs-lookup"><span data-stu-id="32498-121">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="32498-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="32498-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="32498-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="32498-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="32498-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="32498-124">Schema Name</span></span>  <br/> |<span data-ttu-id="32498-125">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="32498-125">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="32498-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="32498-126">Validation File</span></span>  <br/> |<span data-ttu-id="32498-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="32498-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="32498-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="32498-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="32498-129">True</span><span class="sxs-lookup"><span data-stu-id="32498-129">True</span></span>  <br/> |
   

