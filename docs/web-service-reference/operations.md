---
title: 業務
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
description: Operations 要素には、受信トレイに対して実行できるルール操作の配列が含まれています。
ms.openlocfilehash: 4bbec4ad6424f802bb6781a870d65f23705e88c4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462487"
---
# <a name="operations"></a><span data-ttu-id="0fd3f-103">業務</span><span class="sxs-lookup"><span data-stu-id="0fd3f-103">Operations</span></span>

<span data-ttu-id="0fd3f-104">**Operations**要素には、受信トレイに対して実行できるルール操作の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0fd3f-104">The **Operations** element contains an array of rule operations that can be performed on an Inbox.</span></span> 
  
[<span data-ttu-id="0fd3f-105">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="0fd3f-105">UpdateInboxRules</span></span>](updateinboxrules.md)
  
```XML
<Operations>
    <CreateRuleOperation/>
    <SetRuleOperation/>
    <DeleteRuleOperation/>
</Operations>
```

 <span data-ttu-id="0fd3f-106">**ArrayOfRuleOperationsType**</span><span class="sxs-lookup"><span data-stu-id="0fd3f-106">**ArrayOfRuleOperationsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0fd3f-107">属性と要素</span><span class="sxs-lookup"><span data-stu-id="0fd3f-107">Attributes and elements</span></span>

<span data-ttu-id="0fd3f-108">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0fd3f-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0fd3f-109">属性</span><span class="sxs-lookup"><span data-stu-id="0fd3f-109">Attributes</span></span>

<span data-ttu-id="0fd3f-110">なし。</span><span class="sxs-lookup"><span data-stu-id="0fd3f-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0fd3f-111">子要素</span><span class="sxs-lookup"><span data-stu-id="0fd3f-111">Child elements</span></span>

|<span data-ttu-id="0fd3f-112">**Element**</span><span class="sxs-lookup"><span data-stu-id="0fd3f-112">**Element**</span></span>|<span data-ttu-id="0fd3f-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="0fd3f-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0fd3f-114">CreateRuleOperation</span><span class="sxs-lookup"><span data-stu-id="0fd3f-114">CreateRuleOperation</span></span>](createruleoperation.md) <br/> |<span data-ttu-id="0fd3f-115">新しい受信トレイルールを作成する操作を表します。</span><span class="sxs-lookup"><span data-stu-id="0fd3f-115">Represents an operation to create a new Inbox rule.</span></span>  <br/> |
|[<span data-ttu-id="0fd3f-116">SetRuleOperation</span><span class="sxs-lookup"><span data-stu-id="0fd3f-116">SetRuleOperation</span></span>](setruleoperation.md) <br/> |<span data-ttu-id="0fd3f-117">受信トレイルールを更新する操作を表します。</span><span class="sxs-lookup"><span data-stu-id="0fd3f-117">Represents an operation to update an Inbox rule.</span></span>  <br/> |
|[<span data-ttu-id="0fd3f-118">DeleteRuleOperation</span><span class="sxs-lookup"><span data-stu-id="0fd3f-118">DeleteRuleOperation</span></span>](deleteruleoperation.md) <br/> |<span data-ttu-id="0fd3f-119">受信トレイルールを削除する操作を表します。</span><span class="sxs-lookup"><span data-stu-id="0fd3f-119">Represents an operation to delete an Inbox rule.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0fd3f-120">親要素</span><span class="sxs-lookup"><span data-stu-id="0fd3f-120">Parent elements</span></span>

|<span data-ttu-id="0fd3f-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="0fd3f-121">**Element**</span></span>|<span data-ttu-id="0fd3f-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="0fd3f-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0fd3f-123">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="0fd3f-123">UpdateInboxRules</span></span>](updateinboxrules.md) <br/> |<span data-ttu-id="0fd3f-124">サーバーストア内のメールボックスの受信トレイルールを更新する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="0fd3f-124">Defines a request to update the Inbox rules in a mailbox in the server store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0fd3f-125">注釈</span><span class="sxs-lookup"><span data-stu-id="0fd3f-125">Remarks</span></span>

<span data-ttu-id="0fd3f-126">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="0fd3f-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0fd3f-127">要素の情報</span><span class="sxs-lookup"><span data-stu-id="0fd3f-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0fd3f-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="0fd3f-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0fd3f-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0fd3f-129">Schema Name</span></span>  <br/> |<span data-ttu-id="0fd3f-130">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="0fd3f-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="0fd3f-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0fd3f-131">Validation File</span></span>  <br/> |<span data-ttu-id="0fd3f-132">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="0fd3f-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0fd3f-133">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="0fd3f-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="0fd3f-134">正しくない</span><span class="sxs-lookup"><span data-stu-id="0fd3f-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0fd3f-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="0fd3f-135">See also</span></span>



[<span data-ttu-id="0fd3f-136">UpdateInboxRules の操作</span><span class="sxs-lookup"><span data-stu-id="0fd3f-136">UpdateInboxRules operation</span></span>](updateinboxrules-operation.md)


- [<span data-ttu-id="0fd3f-137">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="0fd3f-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

