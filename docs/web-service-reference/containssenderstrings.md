---
title: ContainsSenderStrings
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContainsSenderStrings
api_type:
- schema
ms.assetid: 3e16163f-cffe-4c4e-9a2a-00245d25ba96
description: ContainsSenderStrings 要素を適用する場合の条件または例外の順序で受信メッセージの From プロパティ内に表示する文字列を示します。
ms.openlocfilehash: d174c0d7e2cbfd5b671a825a867d3ee7e24c2f2a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759713"
---
# <a name="containssenderstrings"></a><span data-ttu-id="718e1-103">ContainsSenderStrings</span><span class="sxs-lookup"><span data-stu-id="718e1-103">ContainsSenderStrings</span></span>

<span data-ttu-id="718e1-104">**ContainsSenderStrings**要素**から**のプロパティに適用する条件または例外の順序で受信したメッセージに表示する文字列を示します。</span><span class="sxs-lookup"><span data-stu-id="718e1-104">The **ContainsSenderStrings** element indicates the strings that must appear in the **From** property of incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<ContainsSenderStrings>
    <String/>
</ContainsSenderStrings>
```

 <span data-ttu-id="718e1-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="718e1-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="718e1-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="718e1-106">Attributes and elements</span></span>

<span data-ttu-id="718e1-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="718e1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="718e1-108">属性</span><span class="sxs-lookup"><span data-stu-id="718e1-108">Attributes</span></span>

<span data-ttu-id="718e1-109">なし。</span><span class="sxs-lookup"><span data-stu-id="718e1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="718e1-110">子要素</span><span class="sxs-lookup"><span data-stu-id="718e1-110">Child elements</span></span>

|<span data-ttu-id="718e1-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="718e1-111">**Element**</span></span>|<span data-ttu-id="718e1-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="718e1-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="718e1-113">String</span><span class="sxs-lookup"><span data-stu-id="718e1-113">String</span></span>](string.md) <br/> |<span data-ttu-id="718e1-114">**** プロパティに適用する条件または例外の順序で受信したメッセージに表示する文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="718e1-114">Represents a string that must appear in the **From** property of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="718e1-115">親要素</span><span class="sxs-lookup"><span data-stu-id="718e1-115">Parent elements</span></span>

|<span data-ttu-id="718e1-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="718e1-116">**Element**</span></span>|<span data-ttu-id="718e1-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="718e1-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="718e1-118">条件</span><span class="sxs-lookup"><span data-stu-id="718e1-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="718e1-119">条件を表しますが、満たされるとときに、ルールのルールの処理をトリガーします。</span><span class="sxs-lookup"><span data-stu-id="718e1-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="718e1-120">Exceptions</span><span class="sxs-lookup"><span data-stu-id="718e1-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="718e1-121">受信トレイ ルールの使用可能なルールの例外条件をすべてを表す例外を表します。</span><span class="sxs-lookup"><span data-stu-id="718e1-121">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="718e1-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="718e1-122">Text value</span></span>

<span data-ttu-id="718e1-123">なし。</span><span class="sxs-lookup"><span data-stu-id="718e1-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="718e1-124">備考</span><span class="sxs-lookup"><span data-stu-id="718e1-124">Remarks</span></span>

<span data-ttu-id="718e1-125">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="718e1-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="718e1-126">要素情報</span><span class="sxs-lookup"><span data-stu-id="718e1-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="718e1-127">名前空間</span><span class="sxs-lookup"><span data-stu-id="718e1-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="718e1-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="718e1-128">Schema Name</span></span>  <br/> |<span data-ttu-id="718e1-129">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="718e1-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="718e1-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="718e1-130">Validation File</span></span>  <br/> |<span data-ttu-id="718e1-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="718e1-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="718e1-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="718e1-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="718e1-133">True</span><span class="sxs-lookup"><span data-stu-id="718e1-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="718e1-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="718e1-134">See also</span></span>



- [<span data-ttu-id="718e1-135">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="718e1-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

