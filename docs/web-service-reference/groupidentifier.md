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
description: GroupIdentifier 要素は、アカウントがメンバーである Active Directory ディレクトリサービスオブジェクトグループの単一のセキュリティ識別子と属性を表します。
ms.openlocfilehash: 8b427b9228cc5e66f46f70389acf2fa4bcd283b3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530804"
---
# <a name="groupidentifier"></a><span data-ttu-id="70a70-103">GroupIdentifier</span><span class="sxs-lookup"><span data-stu-id="70a70-103">GroupIdentifier</span></span>

<span data-ttu-id="70a70-104">**GroupIdentifier**要素は、アカウントがメンバーである Active Directory ディレクトリサービスオブジェクトグループの単一のセキュリティ識別子と属性を表します。</span><span class="sxs-lookup"><span data-stu-id="70a70-104">The **GroupIdentifier** element represents a single security identifier and attribute for an Active Directory directory service object group of which the account is a member.</span></span> 
  
```xml
<GroupIdentifier>
   <SecurityIdentifier/>
</GroupIdentifier>
```

 <span data-ttu-id="70a70-105">**SidAndAttributesType**</span><span class="sxs-lookup"><span data-stu-id="70a70-105">**SidAndAttributesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="70a70-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="70a70-106">Attributes and elements</span></span>

<span data-ttu-id="70a70-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="70a70-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="70a70-108">属性</span><span class="sxs-lookup"><span data-stu-id="70a70-108">Attributes</span></span>

|<span data-ttu-id="70a70-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="70a70-109">**Attribute**</span></span>|<span data-ttu-id="70a70-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="70a70-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="70a70-111">**属性**</span><span class="sxs-lookup"><span data-stu-id="70a70-111">**Attributes**</span></span> <br/> |<span data-ttu-id="70a70-112">グループの属性が含まれます。</span><span class="sxs-lookup"><span data-stu-id="70a70-112">Contains group attributes.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="70a70-113">子要素</span><span class="sxs-lookup"><span data-stu-id="70a70-113">Child elements</span></span>

|<span data-ttu-id="70a70-114">**Element**</span><span class="sxs-lookup"><span data-stu-id="70a70-114">**Element**</span></span>|<span data-ttu-id="70a70-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="70a70-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="70a70-116">SecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="70a70-116">SecurityIdentifier</span></span>](securityidentifier.md) <br/> |<span data-ttu-id="70a70-117">グループを表すセキュリティ識別子 ([SID](sid.md)) のセキュリティ記述子定義言語 (SDDL) 形式を表します。</span><span class="sxs-lookup"><span data-stu-id="70a70-117">Represents the security descriptor definition language (SDDL) form of a security identifier ([SID](sid.md)) that represents the group.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="70a70-118">親要素</span><span class="sxs-lookup"><span data-stu-id="70a70-118">Parent elements</span></span>

|<span data-ttu-id="70a70-119">**要素**</span><span class="sxs-lookup"><span data-stu-id="70a70-119">**Element**</span></span>|<span data-ttu-id="70a70-120">**説明**</span><span class="sxs-lookup"><span data-stu-id="70a70-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="70a70-121">GroupSids</span><span class="sxs-lookup"><span data-stu-id="70a70-121">GroupSids</span></span>](groupsids.md) <br/> |<span data-ttu-id="70a70-122">トークンのシリアル化のためのアカウントトークンを構成する Active Directory グループオブジェクトのセキュリティ識別子のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="70a70-122">Represents a collection of Active Directory group object security identifiers that make up an account token for token serialization.</span></span> <span data-ttu-id="70a70-123">トークンのシリアル化はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="70a70-123">Token serialization is not supported.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="70a70-124">注釈</span><span class="sxs-lookup"><span data-stu-id="70a70-124">Remarks</span></span>

<span data-ttu-id="70a70-125">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="70a70-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="70a70-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="70a70-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="70a70-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="70a70-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="70a70-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="70a70-128">Schema Name</span></span>  <br/> |<span data-ttu-id="70a70-129">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="70a70-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="70a70-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="70a70-130">Validation File</span></span>  <br/> |<span data-ttu-id="70a70-131">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="70a70-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="70a70-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="70a70-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="70a70-133">正しくない</span><span class="sxs-lookup"><span data-stu-id="70a70-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="70a70-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="70a70-134">See also</span></span>



- [<span data-ttu-id="70a70-135">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="70a70-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

