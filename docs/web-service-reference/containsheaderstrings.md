---
title: ContainsHeaderStrings
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContainsHeaderStrings
api_type:
- schema
ms.assetid: 5f68427b-990a-4a27-bfb3-fce3115b02d7
description: ContainsHeaderStrings 要素を適用する場合の条件または例外の順序で受信メッセージのヘッダーに表示される文字列を示します。
ms.openlocfilehash: 360870d63853a0e79f801cc2f17473b1a1b28c25
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759705"
---
# <a name="containsheaderstrings"></a><span data-ttu-id="5d117-103">ContainsHeaderStrings</span><span class="sxs-lookup"><span data-stu-id="5d117-103">ContainsHeaderStrings</span></span>

<span data-ttu-id="5d117-104">**ContainsHeaderStrings**要素を適用する場合の条件または例外の順序で受信メッセージのヘッダーに表示される文字列を示します。</span><span class="sxs-lookup"><span data-stu-id="5d117-104">The **ContainsHeaderStrings** element indicates the strings that must appear in the headers of incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<ContainsHeaderStrings>
    <String/>
</ContainsHeaderStrings>
```

 <span data-ttu-id="5d117-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="5d117-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5d117-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="5d117-106">Attributes and elements</span></span>

<span data-ttu-id="5d117-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5d117-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5d117-108">属性</span><span class="sxs-lookup"><span data-stu-id="5d117-108">Attributes</span></span>

<span data-ttu-id="5d117-109">なし。</span><span class="sxs-lookup"><span data-stu-id="5d117-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5d117-110">子要素</span><span class="sxs-lookup"><span data-stu-id="5d117-110">Child elements</span></span>

|<span data-ttu-id="5d117-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="5d117-111">**Element**</span></span>|<span data-ttu-id="5d117-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="5d117-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5d117-113">String</span><span class="sxs-lookup"><span data-stu-id="5d117-113">String</span></span>](string.md) <br/> |<span data-ttu-id="5d117-114">適用する場合の条件または例外の順序でメッセージ ヘッダーに表示される文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="5d117-114">Represents a string that must appear in message headers in order for the condition or exception to apply.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5d117-115">親要素</span><span class="sxs-lookup"><span data-stu-id="5d117-115">Parent elements</span></span>

|<span data-ttu-id="5d117-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="5d117-116">**Element**</span></span>|<span data-ttu-id="5d117-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="5d117-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5d117-118">条件</span><span class="sxs-lookup"><span data-stu-id="5d117-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="5d117-119">条件を表しますが、満たされるとときに、ルールのルールの処理をトリガーします。</span><span class="sxs-lookup"><span data-stu-id="5d117-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="5d117-120">Exceptions</span><span class="sxs-lookup"><span data-stu-id="5d117-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="5d117-121">受信トレイ ルールの使用可能なルールの例外条件をすべてを表す例外を表します。</span><span class="sxs-lookup"><span data-stu-id="5d117-121">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5d117-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="5d117-122">Text value</span></span>

<span data-ttu-id="5d117-123">なし。</span><span class="sxs-lookup"><span data-stu-id="5d117-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5d117-124">備考</span><span class="sxs-lookup"><span data-stu-id="5d117-124">Remarks</span></span>

<span data-ttu-id="5d117-125">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="5d117-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5d117-126">要素情報</span><span class="sxs-lookup"><span data-stu-id="5d117-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5d117-127">名前空間</span><span class="sxs-lookup"><span data-stu-id="5d117-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5d117-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5d117-128">Schema Name</span></span>  <br/> |<span data-ttu-id="5d117-129">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="5d117-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5d117-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5d117-130">Validation File</span></span>  <br/> |<span data-ttu-id="5d117-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="5d117-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5d117-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="5d117-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="5d117-133">True</span><span class="sxs-lookup"><span data-stu-id="5d117-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5d117-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="5d117-134">See also</span></span>



- [<span data-ttu-id="5d117-135">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="5d117-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

