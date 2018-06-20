---
title: RemoveOutlookRuleBlob
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RemoveOutlookRuleBlob
api_type:
- schema
ms.assetid: 69614475-8bd3-4475-b988-614fe9cad8ef
description: RemoveOutlookRuleBlob 要素では、Microsoft Outlook のルールの blob を削除するかどうかを示します。
ms.openlocfilehash: 45336e296c39161704ce6e0d51fba1d2c61797b1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833102"
---
# <a name="removeoutlookruleblob"></a><span data-ttu-id="80d75-103">RemoveOutlookRuleBlob</span><span class="sxs-lookup"><span data-stu-id="80d75-103">RemoveOutlookRuleBlob</span></span>

<span data-ttu-id="80d75-104">**RemoveOutlookRuleBlob**要素では、Microsoft Outlook のルールの blob を削除するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="80d75-104">The **RemoveOutlookRuleBlob** element indicates whether to remove the Microsoft Outlook rule blob.</span></span> 
  
[<span data-ttu-id="80d75-105">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="80d75-105">UpdateInboxRules</span></span>](updateinboxrules.md)
  
[<span data-ttu-id="80d75-106">RemoveOutlookRuleBlob</span><span class="sxs-lookup"><span data-stu-id="80d75-106">RemoveOutlookRuleBlob</span></span>](removeoutlookruleblob.md)
  
```XML
<RemoveOutlookRuleBlob>true | false</RemoveOutlookRuleBlob>
```

 <span data-ttu-id="80d75-107">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="80d75-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="80d75-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="80d75-108">Attributes and elements</span></span>

<span data-ttu-id="80d75-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="80d75-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="80d75-110">属性</span><span class="sxs-lookup"><span data-stu-id="80d75-110">Attributes</span></span>

<span data-ttu-id="80d75-111">なし。</span><span class="sxs-lookup"><span data-stu-id="80d75-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="80d75-112">子要素</span><span class="sxs-lookup"><span data-stu-id="80d75-112">Child elements</span></span>

<span data-ttu-id="80d75-113">なし。</span><span class="sxs-lookup"><span data-stu-id="80d75-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="80d75-114">親要素</span><span class="sxs-lookup"><span data-stu-id="80d75-114">Parent elements</span></span>

|<span data-ttu-id="80d75-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="80d75-115">**Element**</span></span>|<span data-ttu-id="80d75-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="80d75-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="80d75-117">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="80d75-117">UpdateInboxRules</span></span>](updateinboxrules.md) <br/> |<span data-ttu-id="80d75-118">サーバー ストア内のメールボックスの受信トレイ ルールを更新する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="80d75-118">Defines a request to update the Inbox rules in a mailbox in the server store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="80d75-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="80d75-119">Text value</span></span>

<span data-ttu-id="80d75-120">**True**の場合、テキスト値は、Outlook のルールの blob を削除する必要があることを示します。</span><span class="sxs-lookup"><span data-stu-id="80d75-120">A text value of **true** indicates that the Outlook rule blob should be removed.</span></span> <span data-ttu-id="80d75-121">テキスト値が**false**のでは、Outlook のルールの blob を削除されないことを示します。</span><span class="sxs-lookup"><span data-stu-id="80d75-121">A text value of **false** indicates that the Outlook rule blob should not be removed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="80d75-122">備考</span><span class="sxs-lookup"><span data-stu-id="80d75-122">Remarks</span></span>

<span data-ttu-id="80d75-123">**True**に、受信トレイ ルールの更新プログラムでは、この要素を設定します。</span><span class="sxs-lookup"><span data-stu-id="80d75-123">Set this element to **true** to allow for an Inbox rule update.</span></span> 
  
<span data-ttu-id="80d75-124">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="80d75-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="80d75-125">要素情報</span><span class="sxs-lookup"><span data-stu-id="80d75-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="80d75-126">名前空間</span><span class="sxs-lookup"><span data-stu-id="80d75-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="80d75-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="80d75-127">Schema Name</span></span>  <br/> |<span data-ttu-id="80d75-128">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="80d75-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="80d75-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="80d75-129">Validation File</span></span>  <br/> |<span data-ttu-id="80d75-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="80d75-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="80d75-131">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="80d75-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="80d75-132">True</span><span class="sxs-lookup"><span data-stu-id="80d75-132">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="80d75-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="80d75-133">See also</span></span>



[<span data-ttu-id="80d75-134">UpdateInboxRules の操作</span><span class="sxs-lookup"><span data-stu-id="80d75-134">UpdateInboxRules operation</span></span>](updateinboxrules-operation.md)


- [<span data-ttu-id="80d75-135">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="80d75-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

