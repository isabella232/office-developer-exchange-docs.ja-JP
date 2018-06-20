---
title: ルール
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Rules
api_type:
- schema
ms.assetid: 53f59054-8f68-4eaa-be9c-ccfc9383bcf2
description: ルール要素には、保護の規則の配列が含まれています。
ms.openlocfilehash: 5d511f977f3eb3273dc43f56356a059985b2a929
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833269"
---
# <a name="rules"></a><span data-ttu-id="64c0c-103">ルール</span><span class="sxs-lookup"><span data-stu-id="64c0c-103">Rules</span></span>

<span data-ttu-id="64c0c-104">**ルール**要素には、保護の規則の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="64c0c-104">The **Rules** element contains an array of protection rules.</span></span> 
  
```xml
<Rules>   <Rule/></Rules>
```

 <span data-ttu-id="64c0c-105">**ArrayOfProtectionRulesType**</span><span class="sxs-lookup"><span data-stu-id="64c0c-105">**ArrayOfProtectionRulesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="64c0c-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="64c0c-106">Attributes and elements</span></span>

<span data-ttu-id="64c0c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="64c0c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="64c0c-108">属性</span><span class="sxs-lookup"><span data-stu-id="64c0c-108">Attributes</span></span>

<span data-ttu-id="64c0c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="64c0c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="64c0c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="64c0c-110">Child elements</span></span>

|<span data-ttu-id="64c0c-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="64c0c-111">**Element**</span></span>|<span data-ttu-id="64c0c-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="64c0c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="64c0c-113">Rule</span><span class="sxs-lookup"><span data-stu-id="64c0c-113">Rule</span></span>](rule.md) <br/> |<span data-ttu-id="64c0c-114">1 つの保護ルールが含まれています。</span><span class="sxs-lookup"><span data-stu-id="64c0c-114">Contains a single protection rule.</span></span> <span data-ttu-id="64c0c-115">この要素に 0 回以上発生します。</span><span class="sxs-lookup"><span data-stu-id="64c0c-115">This element can occur zero or more times.</span></span> <span data-ttu-id="64c0c-116">この要素と保護のルールが定義されていない組織で 0 が発生します。</span><span class="sxs-lookup"><span data-stu-id="64c0c-116">This element occurs zero times when no protection rules are defined by the organization.</span></span> <span data-ttu-id="64c0c-117">1 つ以上の時間は、組織が少なくとも 1 つのルールが定義されている場合に発生します。</span><span class="sxs-lookup"><span data-stu-id="64c0c-117">It occurs one or more times if at least one rule is defined by the organization.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="64c0c-118">親要素</span><span class="sxs-lookup"><span data-stu-id="64c0c-118">Parent elements</span></span>

|<span data-ttu-id="64c0c-119">**要素**</span><span class="sxs-lookup"><span data-stu-id="64c0c-119">**Element**</span></span>|<span data-ttu-id="64c0c-120">**説明**</span><span class="sxs-lookup"><span data-stu-id="64c0c-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="64c0c-121">ProtectionRulesConfiguration</span><span class="sxs-lookup"><span data-stu-id="64c0c-121">ProtectionRulesConfiguration</span></span>](protectionrulesconfiguration.md) <br/> |<span data-ttu-id="64c0c-122">保護ルールのサービスのサービスの構成が含まれています。</span><span class="sxs-lookup"><span data-stu-id="64c0c-122">Contains service configuration for the protection rules service.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="64c0c-123">備考</span><span class="sxs-lookup"><span data-stu-id="64c0c-123">Remarks</span></span>

<span data-ttu-id="64c0c-124">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="64c0c-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="64c0c-125">要素情報</span><span class="sxs-lookup"><span data-stu-id="64c0c-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="64c0c-126">名前空間</span><span class="sxs-lookup"><span data-stu-id="64c0c-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="64c0c-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="64c0c-127">Schema Name</span></span>  <br/> |<span data-ttu-id="64c0c-128">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="64c0c-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="64c0c-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="64c0c-129">Validation File</span></span>  <br/> |<span data-ttu-id="64c0c-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="64c0c-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="64c0c-131">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="64c0c-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="64c0c-132">False</span><span class="sxs-lookup"><span data-stu-id="64c0c-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="64c0c-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="64c0c-133">See also</span></span>



- [<span data-ttu-id="64c0c-134">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="64c0c-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

