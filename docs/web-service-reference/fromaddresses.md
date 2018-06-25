---
title: FromAddresses
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FromAddresses
api_type:
- schema
ms.assetid: b219f315-c20a-4633-af3e-94bd3e4526b6
description: FromAddresses 要素は、元の条件または例外を適用する順序で受信したメッセージを送信する必要がある電子メール アドレスを示します。
ms.openlocfilehash: 40ecb1f3e16ad961b8e4c38d5aa9d15f4f74469a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760606"
---
# <a name="fromaddresses"></a><span data-ttu-id="6c0ae-103">FromAddresses</span><span class="sxs-lookup"><span data-stu-id="6c0ae-103">FromAddresses</span></span>

<span data-ttu-id="6c0ae-104">**FromAddresses**要素は、元の条件または例外を適用する順序で受信したメッセージを送信する必要がある電子メール アドレスを示します。</span><span class="sxs-lookup"><span data-stu-id="6c0ae-104">The **FromAddresses** element indicates the e-mail addresses from which incoming messages must be sent in order for the condition or exception to apply.</span></span> 
  
```XML
<FromAddresses>
   <Address/>
</FromAddresses>
```

 <span data-ttu-id="6c0ae-105">**ArrayOfEmailAddressesType**</span><span class="sxs-lookup"><span data-stu-id="6c0ae-105">**ArrayOfEmailAddressesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6c0ae-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="6c0ae-106">Attributes and elements</span></span>

<span data-ttu-id="6c0ae-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6c0ae-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6c0ae-108">属性</span><span class="sxs-lookup"><span data-stu-id="6c0ae-108">Attributes</span></span>

<span data-ttu-id="6c0ae-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6c0ae-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6c0ae-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6c0ae-110">Child elements</span></span>

|<span data-ttu-id="6c0ae-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="6c0ae-111">**Element**</span></span>|<span data-ttu-id="6c0ae-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="6c0ae-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6c0ae-113">アドレス (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="6c0ae-113">Address (EmailAddressType)</span></span>](address-emailaddresstype.md) <br/> |<span data-ttu-id="6c0ae-114">完全に解決された電子メール アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="6c0ae-114">Represents a fully resolved e-mail address.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6c0ae-115">親要素</span><span class="sxs-lookup"><span data-stu-id="6c0ae-115">Parent elements</span></span>

|<span data-ttu-id="6c0ae-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="6c0ae-116">**Element**</span></span>|<span data-ttu-id="6c0ae-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="6c0ae-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6c0ae-118">条件</span><span class="sxs-lookup"><span data-stu-id="6c0ae-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="6c0ae-119">条件を表しますが、満たされるとときに、ルールのルールの処理をトリガーします。</span><span class="sxs-lookup"><span data-stu-id="6c0ae-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="6c0ae-120">Exceptions</span><span class="sxs-lookup"><span data-stu-id="6c0ae-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="6c0ae-121">受信トレイ ルールの使用可能なルールの例外条件をすべてを表します。</span><span class="sxs-lookup"><span data-stu-id="6c0ae-121">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6c0ae-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="6c0ae-122">Text value</span></span>

<span data-ttu-id="6c0ae-123">なし。</span><span class="sxs-lookup"><span data-stu-id="6c0ae-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6c0ae-124">備考</span><span class="sxs-lookup"><span data-stu-id="6c0ae-124">Remarks</span></span>

<span data-ttu-id="6c0ae-125">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="6c0ae-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6c0ae-126">要素情報</span><span class="sxs-lookup"><span data-stu-id="6c0ae-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6c0ae-127">名前空間</span><span class="sxs-lookup"><span data-stu-id="6c0ae-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6c0ae-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6c0ae-128">Schema Name</span></span>  <br/> |<span data-ttu-id="6c0ae-129">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="6c0ae-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6c0ae-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6c0ae-130">Validation File</span></span>  <br/> |<span data-ttu-id="6c0ae-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6c0ae-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6c0ae-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="6c0ae-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="6c0ae-133">True</span><span class="sxs-lookup"><span data-stu-id="6c0ae-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6c0ae-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="6c0ae-134">See also</span></span>



- [<span data-ttu-id="6c0ae-135">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="6c0ae-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

