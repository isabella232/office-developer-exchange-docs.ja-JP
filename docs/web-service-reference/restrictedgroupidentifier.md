---
title: RestrictedGroupIdentifier
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RestrictedGroupIdentifier
api_type:
- schema
ms.assetid: a3ea3c81-9f99-4836-8cb4-2384ea63f093
description: RestrictGroupIdentifier 要素は、グループのセキュリティ識別子 (SID) とユーザーのトークン内の制限されたグループの属性を表します。
ms.openlocfilehash: c6db8672b2afa855e83f2e9a2bf84c9ff33bdc7a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833206"
---
# <a name="restrictedgroupidentifier"></a><span data-ttu-id="13ecb-103">RestrictedGroupIdentifier</span><span class="sxs-lookup"><span data-stu-id="13ecb-103">RestrictedGroupIdentifier</span></span>

<span data-ttu-id="13ecb-104">**RestrictGroupIdentifier**要素は、グループのセキュリティ識別子 (SID) とユーザーのトークン内の制限されたグループの属性を表します。</span><span class="sxs-lookup"><span data-stu-id="13ecb-104">The **RestrictGroupIdentifier** element represents the group security identifier (SID) and attributes for a restricted group within a user token.</span></span> 
  
```xml
<RestrictedGroupIdentifier Attributes="">
   <SecurityIdentifier/>
</RestrictedGroupIdentifier>
```

 <span data-ttu-id="13ecb-105">**SidAndAttributesType**</span><span class="sxs-lookup"><span data-stu-id="13ecb-105">**SidAndAttributesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="13ecb-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="13ecb-106">Attributes and elements</span></span>

<span data-ttu-id="13ecb-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="13ecb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="13ecb-108">属性</span><span class="sxs-lookup"><span data-stu-id="13ecb-108">Attributes</span></span>

|<span data-ttu-id="13ecb-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="13ecb-109">**Attribute**</span></span>|<span data-ttu-id="13ecb-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="13ecb-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="13ecb-111">**Attributes**</span><span class="sxs-lookup"><span data-stu-id="13ecb-111">**Attributes**</span></span> <br/> |<span data-ttu-id="13ecb-112">グループの属性が含まれています。</span><span class="sxs-lookup"><span data-stu-id="13ecb-112">Contains group attributes.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="13ecb-113">子要素</span><span class="sxs-lookup"><span data-stu-id="13ecb-113">Child elements</span></span>

|<span data-ttu-id="13ecb-114">**要素**</span><span class="sxs-lookup"><span data-stu-id="13ecb-114">**Element**</span></span>|<span data-ttu-id="13ecb-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="13ecb-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="13ecb-116">SecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="13ecb-116">SecurityIdentifier</span></span>](securityidentifier.md) <br/> |<span data-ttu-id="13ecb-117">セキュリティ id のセキュリティ記述子定義言語 (SDDL) 形式を表します。</span><span class="sxs-lookup"><span data-stu-id="13ecb-117">Represents the security descriptor definition language (SDDL) form of a security identifier.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="13ecb-118">親要素</span><span class="sxs-lookup"><span data-stu-id="13ecb-118">Parent elements</span></span>

|<span data-ttu-id="13ecb-119">**要素**</span><span class="sxs-lookup"><span data-stu-id="13ecb-119">**Element**</span></span>|<span data-ttu-id="13ecb-120">**説明**</span><span class="sxs-lookup"><span data-stu-id="13ecb-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="13ecb-121">RestrictedGroupSids</span><span class="sxs-lookup"><span data-stu-id="13ecb-121">RestrictedGroupSids</span></span>](restrictedgroupsids.md) <br/> |<span data-ttu-id="13ecb-122">ユーザー トークン内の制限されたグループのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="13ecb-122">Represents a collection of restricted groups within a user token.</span></span> <span data-ttu-id="13ecb-123">トークンのシリアル化はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="13ecb-123">Token serialization is not supported.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="13ecb-124">備考</span><span class="sxs-lookup"><span data-stu-id="13ecb-124">Remarks</span></span>

<span data-ttu-id="13ecb-125">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="13ecb-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="13ecb-126">要素情報</span><span class="sxs-lookup"><span data-stu-id="13ecb-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="13ecb-127">名前空間</span><span class="sxs-lookup"><span data-stu-id="13ecb-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="13ecb-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="13ecb-128">Schema Name</span></span>  <br/> |<span data-ttu-id="13ecb-129">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="13ecb-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="13ecb-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="13ecb-130">Validation File</span></span>  <br/> |<span data-ttu-id="13ecb-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="13ecb-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="13ecb-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="13ecb-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="13ecb-133">False</span><span class="sxs-lookup"><span data-stu-id="13ecb-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="13ecb-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="13ecb-134">See also</span></span>



- [<span data-ttu-id="13ecb-135">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="13ecb-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

