---
title: SentToAddresses
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SentToAddresses
api_type:
- schema
ms.assetid: 086130d2-93b1-4de1-9553-10ec10322a0c
description: SentToAddresses 要素は、受信メッセージに適用する条件または例外の順序で送信された必要がある電子メール アドレスを示します。
ms.openlocfilehash: c5a4770ff22e08713e5cf40b9a81191d50a2f437
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833358"
---
# <a name="senttoaddresses"></a><span data-ttu-id="6d930-103">SentToAddresses</span><span class="sxs-lookup"><span data-stu-id="6d930-103">SentToAddresses</span></span>

<span data-ttu-id="6d930-104">**SentToAddresses**要素は、受信メッセージに適用する条件または例外の順序で送信された必要がある電子メール アドレスを示します。</span><span class="sxs-lookup"><span data-stu-id="6d930-104">The **SentToAddresses** element indicates the e-mail addresses that incoming messages have to have been sent to in order for the condition or exception to apply.</span></span> 
  
```XML
<SentToAddresses>
   <Address/>
</SentToAddresses>
```

 <span data-ttu-id="6d930-105">**ArrayOfEmailAddressesType**</span><span class="sxs-lookup"><span data-stu-id="6d930-105">**ArrayOfEmailAddressesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6d930-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="6d930-106">Attributes and elements</span></span>

<span data-ttu-id="6d930-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6d930-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6d930-108">属性</span><span class="sxs-lookup"><span data-stu-id="6d930-108">Attributes</span></span>

<span data-ttu-id="6d930-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6d930-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6d930-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6d930-110">Child elements</span></span>

|<span data-ttu-id="6d930-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="6d930-111">**Element**</span></span>|<span data-ttu-id="6d930-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="6d930-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6d930-113">アドレス (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="6d930-113">Address (EmailAddressType)</span></span>](address-emailaddresstype.md) <br/> |<span data-ttu-id="6d930-114">完全に解決された電子メール アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="6d930-114">Represents a fully resolved e-mail address.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6d930-115">親要素</span><span class="sxs-lookup"><span data-stu-id="6d930-115">Parent elements</span></span>

|<span data-ttu-id="6d930-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="6d930-116">**Element**</span></span>|<span data-ttu-id="6d930-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="6d930-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6d930-118">条件</span><span class="sxs-lookup"><span data-stu-id="6d930-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="6d930-119">条件を表しますが、満たされるとときに、ルールのルールの処理をトリガーします。</span><span class="sxs-lookup"><span data-stu-id="6d930-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="6d930-120">Exceptions</span><span class="sxs-lookup"><span data-stu-id="6d930-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="6d930-121">受信トレイ ルールの使用可能なルールの例外条件をすべてを表します。</span><span class="sxs-lookup"><span data-stu-id="6d930-121">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6d930-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="6d930-122">Text value</span></span>

<span data-ttu-id="6d930-123">なし。</span><span class="sxs-lookup"><span data-stu-id="6d930-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6d930-124">備考</span><span class="sxs-lookup"><span data-stu-id="6d930-124">Remarks</span></span>

<span data-ttu-id="6d930-125">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="6d930-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6d930-126">要素情報</span><span class="sxs-lookup"><span data-stu-id="6d930-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6d930-127">名前空間</span><span class="sxs-lookup"><span data-stu-id="6d930-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6d930-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6d930-128">Schema Name</span></span>  <br/> |<span data-ttu-id="6d930-129">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="6d930-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6d930-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6d930-130">Validation File</span></span>  <br/> |<span data-ttu-id="6d930-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6d930-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6d930-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="6d930-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="6d930-133">True</span><span class="sxs-lookup"><span data-stu-id="6d930-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6d930-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="6d930-134">See also</span></span>



- [<span data-ttu-id="6d930-135">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="6d930-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

