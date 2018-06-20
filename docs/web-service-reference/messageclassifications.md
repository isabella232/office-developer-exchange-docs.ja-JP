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
description: MessageClassifications 要素は、メッセージの分類を適用する場合の条件または例外の順序で受信したメッセージにスタンプする必要があることを表します。
ms.openlocfilehash: 402377907efbc9bb63d875f3f66b314dfc4b788d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832471"
---
# <a name="messageclassifications"></a><span data-ttu-id="100e0-103">MessageClassifications</span><span class="sxs-lookup"><span data-stu-id="100e0-103">MessageClassifications</span></span>

<span data-ttu-id="100e0-104">**MessageClassifications**要素は、メッセージの分類を適用する場合の条件または例外の順序で受信したメッセージにスタンプする必要があることを表します。</span><span class="sxs-lookup"><span data-stu-id="100e0-104">The **MessageClassifications** element represents the message classifications that must be stamped on incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<MessageClassifications>
    <String/>
</MessageClassifications>
```

 <span data-ttu-id="100e0-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="100e0-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="100e0-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="100e0-106">Attributes and elements</span></span>

<span data-ttu-id="100e0-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="100e0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="100e0-108">属性</span><span class="sxs-lookup"><span data-stu-id="100e0-108">Attributes</span></span>

<span data-ttu-id="100e0-109">なし</span><span class="sxs-lookup"><span data-stu-id="100e0-109">None</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="100e0-110">子要素</span><span class="sxs-lookup"><span data-stu-id="100e0-110">Child elements</span></span>

|<span data-ttu-id="100e0-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="100e0-111">**Element**</span></span>|<span data-ttu-id="100e0-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="100e0-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="100e0-113">String</span><span class="sxs-lookup"><span data-stu-id="100e0-113">String</span></span>](string.md) <br/> |<span data-ttu-id="100e0-114">メッセージの分類を表します。</span><span class="sxs-lookup"><span data-stu-id="100e0-114">Represents a message classification.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="100e0-115">親要素</span><span class="sxs-lookup"><span data-stu-id="100e0-115">Parent elements</span></span>

|<span data-ttu-id="100e0-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="100e0-116">**Element**</span></span>|<span data-ttu-id="100e0-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="100e0-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="100e0-118">条件</span><span class="sxs-lookup"><span data-stu-id="100e0-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="100e0-119">条件を表しますが、満たされるとときに、ルールのルールの処理をトリガーします。</span><span class="sxs-lookup"><span data-stu-id="100e0-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="100e0-120">Exceptions</span><span class="sxs-lookup"><span data-stu-id="100e0-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="100e0-121">受信トレイ ルールの使用可能なルールの例外条件をすべてを表す例外を表します。</span><span class="sxs-lookup"><span data-stu-id="100e0-121">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="100e0-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="100e0-122">Text value</span></span>

<span data-ttu-id="100e0-123">なし。</span><span class="sxs-lookup"><span data-stu-id="100e0-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="100e0-124">備考</span><span class="sxs-lookup"><span data-stu-id="100e0-124">Remarks</span></span>

<span data-ttu-id="100e0-125">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="100e0-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="100e0-126">要素情報</span><span class="sxs-lookup"><span data-stu-id="100e0-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="100e0-127">名前空間</span><span class="sxs-lookup"><span data-stu-id="100e0-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="100e0-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="100e0-128">Schema Name</span></span>  <br/> |<span data-ttu-id="100e0-129">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="100e0-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="100e0-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="100e0-130">Validation File</span></span>  <br/> |<span data-ttu-id="100e0-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="100e0-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="100e0-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="100e0-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="100e0-133">True</span><span class="sxs-lookup"><span data-stu-id="100e0-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="100e0-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="100e0-134">See also</span></span>



- [<span data-ttu-id="100e0-135">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="100e0-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

