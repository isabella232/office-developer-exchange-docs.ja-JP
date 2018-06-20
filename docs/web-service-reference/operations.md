---
title: 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: ITPro
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Operations
api_type:
- schema
ms.assetid: d8cd41b1-28ae-4c95-9ff6-8b25c8e18306
description: 操作要素には、受信トレイで実行可能なルール操作の配列が含まれています。
ms.openlocfilehash: 1030703d5e496be391d557e99e1420f9fddfdb36
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832655"
---
# <a name="operations"></a><span data-ttu-id="312f4-103">操作</span><span class="sxs-lookup"><span data-stu-id="312f4-103">Operations</span></span>

<span data-ttu-id="312f4-104">**操作**要素には、受信トレイで実行可能なルール操作の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="312f4-104">The **Operations** element contains an array of rule operations that can be performed on an Inbox.</span></span> 
  
[<span data-ttu-id="312f4-105">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="312f4-105">UpdateInboxRules</span></span>](updateinboxrules.md)
  
```XML
<Operations>
    <CreateRuleOperation/>
    <SetRuleOperation/>
    <DeleteRuleOperation/>
</Operations>
```

 <span data-ttu-id="312f4-106">**ArrayOfRuleOperationsType**</span><span class="sxs-lookup"><span data-stu-id="312f4-106">**ArrayOfRuleOperationsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="312f4-107">属性および要素</span><span class="sxs-lookup"><span data-stu-id="312f4-107">Attributes and elements</span></span>

<span data-ttu-id="312f4-108">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="312f4-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="312f4-109">属性</span><span class="sxs-lookup"><span data-stu-id="312f4-109">Attributes</span></span>

<span data-ttu-id="312f4-110">なし。</span><span class="sxs-lookup"><span data-stu-id="312f4-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="312f4-111">子要素</span><span class="sxs-lookup"><span data-stu-id="312f4-111">Child elements</span></span>

|<span data-ttu-id="312f4-112">**要素**</span><span class="sxs-lookup"><span data-stu-id="312f4-112">**Element**</span></span>|<span data-ttu-id="312f4-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="312f4-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="312f4-114">CreateRuleOperation</span><span class="sxs-lookup"><span data-stu-id="312f4-114">CreateRuleOperation</span></span>](createruleoperation.md) <br/> |<span data-ttu-id="312f4-115">新しい受信トレイ ルールを作成する操作を表します。</span><span class="sxs-lookup"><span data-stu-id="312f4-115">Represents an operation to create a new Inbox rule.</span></span>  <br/> |
|[<span data-ttu-id="312f4-116">SetRuleOperation</span><span class="sxs-lookup"><span data-stu-id="312f4-116">SetRuleOperation</span></span>](setruleoperation.md) <br/> |<span data-ttu-id="312f4-117">受信トレイ ルールを更新する操作を表します。</span><span class="sxs-lookup"><span data-stu-id="312f4-117">Represents an operation to update an Inbox rule.</span></span>  <br/> |
|[<span data-ttu-id="312f4-118">DeleteRuleOperation</span><span class="sxs-lookup"><span data-stu-id="312f4-118">DeleteRuleOperation</span></span>](deleteruleoperation.md) <br/> |<span data-ttu-id="312f4-119">受信トレイ ルールを削除する操作を表します。</span><span class="sxs-lookup"><span data-stu-id="312f4-119">Represents an operation to delete an Inbox rule.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="312f4-120">親要素</span><span class="sxs-lookup"><span data-stu-id="312f4-120">Parent elements</span></span>

|<span data-ttu-id="312f4-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="312f4-121">**Element**</span></span>|<span data-ttu-id="312f4-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="312f4-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="312f4-123">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="312f4-123">UpdateInboxRules</span></span>](updateinboxrules.md) <br/> |<span data-ttu-id="312f4-124">サーバー ストア内のメールボックスの受信トレイ ルールを更新する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="312f4-124">Defines a request to update the Inbox rules in a mailbox in the server store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="312f4-125">備考</span><span class="sxs-lookup"><span data-stu-id="312f4-125">Remarks</span></span>

<span data-ttu-id="312f4-126">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="312f4-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="312f4-127">要素情報</span><span class="sxs-lookup"><span data-stu-id="312f4-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="312f4-128">名前空間</span><span class="sxs-lookup"><span data-stu-id="312f4-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="312f4-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="312f4-129">Schema Name</span></span>  <br/> |<span data-ttu-id="312f4-130">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="312f4-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="312f4-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="312f4-131">Validation File</span></span>  <br/> |<span data-ttu-id="312f4-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="312f4-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="312f4-133">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="312f4-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="312f4-134">False</span><span class="sxs-lookup"><span data-stu-id="312f4-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="312f4-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="312f4-135">See also</span></span>



[<span data-ttu-id="312f4-136">UpdateInboxRules の操作</span><span class="sxs-lookup"><span data-stu-id="312f4-136">UpdateInboxRules operation</span></span>](updateinboxrules-operation.md)


- [<span data-ttu-id="312f4-137">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="312f4-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

