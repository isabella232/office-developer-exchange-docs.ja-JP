---
title: MessageClassifications
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MessageClassifications
api_type:
- schema
ms.assetid: 041b3d48-8f43-47f3-869f-72b66bef372a
description: MessageClassifications 要素は、条件または例外を適用するために、受信メッセージにスタンプする必要があるメッセージ分類を表します。
ms.openlocfilehash: 63481aa8903c4e9637870130eb9154118471c3b0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/01/2020
ms.locfileid: "44467971"
---
# <a name="messageclassifications"></a><span data-ttu-id="5be88-103">MessageClassifications</span><span class="sxs-lookup"><span data-stu-id="5be88-103">MessageClassifications</span></span>

<span data-ttu-id="5be88-104">**MessageClassifications**要素は、条件または例外を適用するために、受信メッセージにスタンプする必要があるメッセージ分類を表します。</span><span class="sxs-lookup"><span data-stu-id="5be88-104">The **MessageClassifications** element represents the message classifications that must be stamped on incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<MessageClassifications>
    <String/>
</MessageClassifications>
```

 <span data-ttu-id="5be88-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="5be88-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5be88-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="5be88-106">Attributes and elements</span></span>

<span data-ttu-id="5be88-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5be88-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5be88-108">属性</span><span class="sxs-lookup"><span data-stu-id="5be88-108">Attributes</span></span>

<span data-ttu-id="5be88-109">なし</span><span class="sxs-lookup"><span data-stu-id="5be88-109">None</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5be88-110">子要素</span><span class="sxs-lookup"><span data-stu-id="5be88-110">Child elements</span></span>

|<span data-ttu-id="5be88-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="5be88-111">**Element**</span></span>|<span data-ttu-id="5be88-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="5be88-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5be88-113">String</span><span class="sxs-lookup"><span data-stu-id="5be88-113">String</span></span>](string.md) <br/> |<span data-ttu-id="5be88-114">メッセージ分類を表します。</span><span class="sxs-lookup"><span data-stu-id="5be88-114">Represents a message classification.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5be88-115">親要素</span><span class="sxs-lookup"><span data-stu-id="5be88-115">Parent elements</span></span>

|<span data-ttu-id="5be88-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="5be88-116">**Element**</span></span>|<span data-ttu-id="5be88-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="5be88-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5be88-118">条件</span><span class="sxs-lookup"><span data-stu-id="5be88-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="5be88-119">ルールのルールの処理を開始するときに実行される条件を表します。</span><span class="sxs-lookup"><span data-stu-id="5be88-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="5be88-120">例外</span><span class="sxs-lookup"><span data-stu-id="5be88-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="5be88-121">受信トレイルールに対して使用可能なルールの例外条件をすべて表す例外を表します。</span><span class="sxs-lookup"><span data-stu-id="5be88-121">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5be88-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="5be88-122">Text value</span></span>

<span data-ttu-id="5be88-123">なし。</span><span class="sxs-lookup"><span data-stu-id="5be88-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5be88-124">注釈</span><span class="sxs-lookup"><span data-stu-id="5be88-124">Remarks</span></span>

<span data-ttu-id="5be88-125">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="5be88-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5be88-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="5be88-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5be88-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="5be88-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5be88-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5be88-128">Schema Name</span></span>  <br/> |<span data-ttu-id="5be88-129">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="5be88-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5be88-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5be88-130">Validation File</span></span>  <br/> |<span data-ttu-id="5be88-131">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="5be88-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5be88-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="5be88-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="5be88-133">正しい</span><span class="sxs-lookup"><span data-stu-id="5be88-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5be88-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="5be88-134">See also</span></span>



- [<span data-ttu-id="5be88-135">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="5be88-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

