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
description: RestrictGroupIdentifier 要素は、ユーザートークン内の制限されたグループのグループセキュリティ識別子 (SID) と属性を表します。
ms.openlocfilehash: c95af4e09324e96f4551a05490dc200aec0cbd46
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465367"
---
# <a name="restrictedgroupidentifier"></a><span data-ttu-id="8c294-103">RestrictedGroupIdentifier</span><span class="sxs-lookup"><span data-stu-id="8c294-103">RestrictedGroupIdentifier</span></span>

<span data-ttu-id="8c294-104">**RestrictGroupIdentifier**要素は、ユーザートークン内の制限されたグループのグループセキュリティ識別子 (SID) と属性を表します。</span><span class="sxs-lookup"><span data-stu-id="8c294-104">The **RestrictGroupIdentifier** element represents the group security identifier (SID) and attributes for a restricted group within a user token.</span></span> 
  
```xml
<RestrictedGroupIdentifier Attributes="">
   <SecurityIdentifier/>
</RestrictedGroupIdentifier>
```

 <span data-ttu-id="8c294-105">**SidAndAttributesType**</span><span class="sxs-lookup"><span data-stu-id="8c294-105">**SidAndAttributesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8c294-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="8c294-106">Attributes and elements</span></span>

<span data-ttu-id="8c294-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8c294-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8c294-108">属性</span><span class="sxs-lookup"><span data-stu-id="8c294-108">Attributes</span></span>

|<span data-ttu-id="8c294-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="8c294-109">**Attribute**</span></span>|<span data-ttu-id="8c294-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="8c294-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8c294-111">**属性**</span><span class="sxs-lookup"><span data-stu-id="8c294-111">**Attributes**</span></span> <br/> |<span data-ttu-id="8c294-112">グループの属性が含まれます。</span><span class="sxs-lookup"><span data-stu-id="8c294-112">Contains group attributes.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="8c294-113">子要素</span><span class="sxs-lookup"><span data-stu-id="8c294-113">Child elements</span></span>

|<span data-ttu-id="8c294-114">**Element**</span><span class="sxs-lookup"><span data-stu-id="8c294-114">**Element**</span></span>|<span data-ttu-id="8c294-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="8c294-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8c294-116">SecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="8c294-116">SecurityIdentifier</span></span>](securityidentifier.md) <br/> |<span data-ttu-id="8c294-117">セキュリティ識別子のセキュリティ記述子定義言語 (SDDL) 形式を表します。</span><span class="sxs-lookup"><span data-stu-id="8c294-117">Represents the security descriptor definition language (SDDL) form of a security identifier.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8c294-118">親要素</span><span class="sxs-lookup"><span data-stu-id="8c294-118">Parent elements</span></span>

|<span data-ttu-id="8c294-119">**要素**</span><span class="sxs-lookup"><span data-stu-id="8c294-119">**Element**</span></span>|<span data-ttu-id="8c294-120">**説明**</span><span class="sxs-lookup"><span data-stu-id="8c294-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8c294-121">RestrictedGroupSids</span><span class="sxs-lookup"><span data-stu-id="8c294-121">RestrictedGroupSids</span></span>](restrictedgroupsids.md) <br/> |<span data-ttu-id="8c294-122">ユーザートークン内の制限されたグループのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="8c294-122">Represents a collection of restricted groups within a user token.</span></span> <span data-ttu-id="8c294-123">トークンのシリアル化はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8c294-123">Token serialization is not supported.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8c294-124">注釈</span><span class="sxs-lookup"><span data-stu-id="8c294-124">Remarks</span></span>

<span data-ttu-id="8c294-125">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="8c294-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8c294-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="8c294-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8c294-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="8c294-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8c294-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8c294-128">Schema Name</span></span>  <br/> |<span data-ttu-id="8c294-129">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="8c294-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="8c294-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8c294-130">Validation File</span></span>  <br/> |<span data-ttu-id="8c294-131">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="8c294-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8c294-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="8c294-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="8c294-133">正しくない</span><span class="sxs-lookup"><span data-stu-id="8c294-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8c294-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="8c294-134">See also</span></span>



- [<span data-ttu-id="8c294-135">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="8c294-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

