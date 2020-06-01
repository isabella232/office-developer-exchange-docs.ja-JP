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
description: Rules 要素には、保護ルールの配列が含まれています。
ms.openlocfilehash: d848abfe0c97d07836f28bc75806f506c5433d44
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464939"
---
# <a name="rules"></a><span data-ttu-id="4763b-103">ルール</span><span class="sxs-lookup"><span data-stu-id="4763b-103">Rules</span></span>

<span data-ttu-id="4763b-104">**Rules**要素には、保護ルールの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="4763b-104">The **Rules** element contains an array of protection rules.</span></span> 
  
```xml
<Rules>   <Rule/></Rules>
```

 <span data-ttu-id="4763b-105">**ArrayOfProtectionRulesType**</span><span class="sxs-lookup"><span data-stu-id="4763b-105">**ArrayOfProtectionRulesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4763b-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="4763b-106">Attributes and elements</span></span>

<span data-ttu-id="4763b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4763b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4763b-108">属性</span><span class="sxs-lookup"><span data-stu-id="4763b-108">Attributes</span></span>

<span data-ttu-id="4763b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="4763b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4763b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="4763b-110">Child elements</span></span>

|<span data-ttu-id="4763b-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="4763b-111">**Element**</span></span>|<span data-ttu-id="4763b-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="4763b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4763b-113">Rule</span><span class="sxs-lookup"><span data-stu-id="4763b-113">Rule</span></span>](rule.md) <br/> |<span data-ttu-id="4763b-114">1つの保護ルールを含みます。</span><span class="sxs-lookup"><span data-stu-id="4763b-114">Contains a single protection rule.</span></span> <span data-ttu-id="4763b-115">この要素は0回以上発生する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="4763b-115">This element can occur zero or more times.</span></span> <span data-ttu-id="4763b-116">組織によって保護ルールが定義されていない場合、この要素は0回発生します。</span><span class="sxs-lookup"><span data-stu-id="4763b-116">This element occurs zero times when no protection rules are defined by the organization.</span></span> <span data-ttu-id="4763b-117">組織によって少なくとも1つのルールが定義されている場合は、1回以上発生します。</span><span class="sxs-lookup"><span data-stu-id="4763b-117">It occurs one or more times if at least one rule is defined by the organization.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4763b-118">親要素</span><span class="sxs-lookup"><span data-stu-id="4763b-118">Parent elements</span></span>

|<span data-ttu-id="4763b-119">**要素**</span><span class="sxs-lookup"><span data-stu-id="4763b-119">**Element**</span></span>|<span data-ttu-id="4763b-120">**説明**</span><span class="sxs-lookup"><span data-stu-id="4763b-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4763b-121">Protectionルールの構成</span><span class="sxs-lookup"><span data-stu-id="4763b-121">ProtectionRulesConfiguration</span></span>](protectionrulesconfiguration.md) <br/> |<span data-ttu-id="4763b-122">保護ルールサービスのサービス構成が保存されています。</span><span class="sxs-lookup"><span data-stu-id="4763b-122">Contains service configuration for the protection rules service.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4763b-123">注釈</span><span class="sxs-lookup"><span data-stu-id="4763b-123">Remarks</span></span>

<span data-ttu-id="4763b-124">この要素を記述するスキーマは、Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="4763b-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4763b-125">要素の情報</span><span class="sxs-lookup"><span data-stu-id="4763b-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4763b-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="4763b-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4763b-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4763b-127">Schema Name</span></span>  <br/> |<span data-ttu-id="4763b-128">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="4763b-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="4763b-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4763b-129">Validation File</span></span>  <br/> |<span data-ttu-id="4763b-130">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="4763b-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4763b-131">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="4763b-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="4763b-132">正しくない</span><span class="sxs-lookup"><span data-stu-id="4763b-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4763b-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="4763b-133">See also</span></span>



- [<span data-ttu-id="4763b-134">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="4763b-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

