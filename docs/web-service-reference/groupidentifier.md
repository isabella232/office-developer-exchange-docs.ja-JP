---
title: GroupIdentifier
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GroupIdentifier
api_type:
- schema
ms.assetid: bdc6fc1e-4979-42da-a35b-e3017988c7d3
description: GroupIdentifier 要素は、1 つのセキュリティ識別子と、アカウントがメンバーとして含まれている Active Directory ディレクトリ サービス オブジェクト グループの属性を表します。
ms.openlocfilehash: d73d72979762238ca09496cfbd6636b4ff44a969
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831767"
---
# <a name="groupidentifier"></a><span data-ttu-id="c55ed-103">GroupIdentifier</span><span class="sxs-lookup"><span data-stu-id="c55ed-103">GroupIdentifier</span></span>

<span data-ttu-id="c55ed-104">**GroupIdentifier**要素は、1 つのセキュリティ識別子と、アカウントがメンバーとして含まれている Active Directory ディレクトリ サービス オブジェクト グループの属性を表します。</span><span class="sxs-lookup"><span data-stu-id="c55ed-104">The **GroupIdentifier** element represents a single security identifier and attribute for an Active Directory directory service object group of which the account is a member.</span></span> 
  
```xml
<GroupIdentifier>
   <SecurityIdentifier/>
</GroupIdentifier>
```

 <span data-ttu-id="c55ed-105">**SidAndAttributesType**</span><span class="sxs-lookup"><span data-stu-id="c55ed-105">**SidAndAttributesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c55ed-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="c55ed-106">Attributes and elements</span></span>

<span data-ttu-id="c55ed-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c55ed-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c55ed-108">属性</span><span class="sxs-lookup"><span data-stu-id="c55ed-108">Attributes</span></span>

|<span data-ttu-id="c55ed-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="c55ed-109">**Attribute**</span></span>|<span data-ttu-id="c55ed-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="c55ed-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c55ed-111">**Attributes**</span><span class="sxs-lookup"><span data-stu-id="c55ed-111">**Attributes**</span></span> <br/> |<span data-ttu-id="c55ed-112">グループの属性が含まれています。</span><span class="sxs-lookup"><span data-stu-id="c55ed-112">Contains group attributes.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="c55ed-113">子要素</span><span class="sxs-lookup"><span data-stu-id="c55ed-113">Child elements</span></span>

|<span data-ttu-id="c55ed-114">**要素**</span><span class="sxs-lookup"><span data-stu-id="c55ed-114">**Element**</span></span>|<span data-ttu-id="c55ed-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="c55ed-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c55ed-116">SecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="c55ed-116">SecurityIdentifier</span></span>](securityidentifier.md) <br/> |<span data-ttu-id="c55ed-117">グループを表すセキュリティ識別子 ([SID](sid.md)) のセキュリティ記述子定義言語 (SDDL) 形式を表します。</span><span class="sxs-lookup"><span data-stu-id="c55ed-117">Represents the security descriptor definition language (SDDL) form of a security identifier ([SID](sid.md)) that represents the group.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c55ed-118">親要素</span><span class="sxs-lookup"><span data-stu-id="c55ed-118">Parent elements</span></span>

|<span data-ttu-id="c55ed-119">**要素**</span><span class="sxs-lookup"><span data-stu-id="c55ed-119">**Element**</span></span>|<span data-ttu-id="c55ed-120">**説明**</span><span class="sxs-lookup"><span data-stu-id="c55ed-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c55ed-121">GroupSids</span><span class="sxs-lookup"><span data-stu-id="c55ed-121">GroupSids</span></span>](groupsids.md) <br/> |<span data-ttu-id="c55ed-122">アカウント トークンのトークンのシリアル化を構成する Active Directory グループ オブジェクト セキュリティ識別子のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="c55ed-122">Represents a collection of Active Directory group object security identifiers that make up an account token for token serialization.</span></span> <span data-ttu-id="c55ed-123">トークンのシリアル化はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c55ed-123">Token serialization is not supported.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c55ed-124">備考</span><span class="sxs-lookup"><span data-stu-id="c55ed-124">Remarks</span></span>

<span data-ttu-id="c55ed-125">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="c55ed-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c55ed-126">要素情報</span><span class="sxs-lookup"><span data-stu-id="c55ed-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c55ed-127">名前空間</span><span class="sxs-lookup"><span data-stu-id="c55ed-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c55ed-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c55ed-128">Schema Name</span></span>  <br/> |<span data-ttu-id="c55ed-129">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="c55ed-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="c55ed-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c55ed-130">Validation File</span></span>  <br/> |<span data-ttu-id="c55ed-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c55ed-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c55ed-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="c55ed-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="c55ed-133">False</span><span class="sxs-lookup"><span data-stu-id="c55ed-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c55ed-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="c55ed-134">See also</span></span>



- [<span data-ttu-id="c55ed-135">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="c55ed-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

