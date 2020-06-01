---
title: 文字列
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
description: この要素は、条件または例外を適用するために、受信メッセージの From プロパティに表示する必要がある文字列を示します。
ms.openlocfilehash: e7b78f1311d288db7969a0024bde84433e18d37f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458979"
---
# <a name="containssenderstrings"></a><span data-ttu-id="7d369-103">文字列</span><span class="sxs-lookup"><span data-stu-id="7d369-103">ContainsSenderStrings</span></span>

<span data-ttu-id="7d369-104">この**要素は、条件**または例外を適用するために、受信メッセージの**From**プロパティに表示する必要がある文字列を示します。</span><span class="sxs-lookup"><span data-stu-id="7d369-104">The **ContainsSenderStrings** element indicates the strings that must appear in the **From** property of incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<ContainsSenderStrings>
    <String/>
</ContainsSenderStrings>
```

 <span data-ttu-id="7d369-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="7d369-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7d369-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="7d369-106">Attributes and elements</span></span>

<span data-ttu-id="7d369-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7d369-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7d369-108">属性</span><span class="sxs-lookup"><span data-stu-id="7d369-108">Attributes</span></span>

<span data-ttu-id="7d369-109">なし。</span><span class="sxs-lookup"><span data-stu-id="7d369-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7d369-110">子要素</span><span class="sxs-lookup"><span data-stu-id="7d369-110">Child elements</span></span>

|<span data-ttu-id="7d369-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="7d369-111">**Element**</span></span>|<span data-ttu-id="7d369-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="7d369-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7d369-113">String</span><span class="sxs-lookup"><span data-stu-id="7d369-113">String</span></span>](string.md) <br/> |<span data-ttu-id="7d369-114">条件または例外を適用するために、受信メッセージの**From**プロパティに表示する必要がある文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="7d369-114">Represents a string that must appear in the **From** property of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7d369-115">親要素</span><span class="sxs-lookup"><span data-stu-id="7d369-115">Parent elements</span></span>

|<span data-ttu-id="7d369-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="7d369-116">**Element**</span></span>|<span data-ttu-id="7d369-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="7d369-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7d369-118">条件</span><span class="sxs-lookup"><span data-stu-id="7d369-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="7d369-119">ルールのルールの処理を開始するときに実行される条件を表します。</span><span class="sxs-lookup"><span data-stu-id="7d369-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="7d369-120">例外</span><span class="sxs-lookup"><span data-stu-id="7d369-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="7d369-121">受信トレイルールに対して使用可能なルールの例外条件をすべて表す例外を表します。</span><span class="sxs-lookup"><span data-stu-id="7d369-121">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7d369-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="7d369-122">Text value</span></span>

<span data-ttu-id="7d369-123">なし。</span><span class="sxs-lookup"><span data-stu-id="7d369-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7d369-124">注釈</span><span class="sxs-lookup"><span data-stu-id="7d369-124">Remarks</span></span>

<span data-ttu-id="7d369-125">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="7d369-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7d369-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="7d369-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7d369-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="7d369-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7d369-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7d369-128">Schema Name</span></span>  <br/> |<span data-ttu-id="7d369-129">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="7d369-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7d369-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7d369-130">Validation File</span></span>  <br/> |<span data-ttu-id="7d369-131">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="7d369-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7d369-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="7d369-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="7d369-133">正しい</span><span class="sxs-lookup"><span data-stu-id="7d369-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7d369-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="7d369-134">See also</span></span>



- [<span data-ttu-id="7d369-135">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="7d369-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

