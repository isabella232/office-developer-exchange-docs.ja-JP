---
title: Members (MemberListType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Members
api_type:
- schema
ms.assetid: cbd38049-2ef7-40bf-9bec-0469af0f58ec
description: Members 要素は、配布リストのメンバーの一覧を提供します。
ms.openlocfilehash: 2cdfb81dfbc223db365d49ed44d4893339eb4653
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462431"
---
# <a name="members-memberlisttype"></a><span data-ttu-id="c7943-103">Members (MemberListType)</span><span class="sxs-lookup"><span data-stu-id="c7943-103">Members (MemberListType)</span></span>

<span data-ttu-id="c7943-104">**Members**要素は、配布リストのメンバーの一覧を提供します。</span><span class="sxs-lookup"><span data-stu-id="c7943-104">The **Members** element provides the list of members for a distribution list.</span></span> 
  
```xml
<Members>
   <Member/>
</Members>
```

<span data-ttu-id="c7943-105">**MemberListType**</span><span class="sxs-lookup"><span data-stu-id="c7943-105">**MemberListType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="c7943-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="c7943-106">Attributes and elements</span></span>

<span data-ttu-id="c7943-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c7943-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c7943-108">属性</span><span class="sxs-lookup"><span data-stu-id="c7943-108">Attributes</span></span>

<span data-ttu-id="c7943-109">なし。</span><span class="sxs-lookup"><span data-stu-id="c7943-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c7943-110">子要素</span><span class="sxs-lookup"><span data-stu-id="c7943-110">Child elements</span></span>

|<span data-ttu-id="c7943-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="c7943-111">**Element**</span></span>|<span data-ttu-id="c7943-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="c7943-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c7943-113">メンバー</span><span class="sxs-lookup"><span data-stu-id="c7943-113">Member</span></span>](member-ex15websvcsotherref.md) <br/> |<span data-ttu-id="c7943-114">完全に解決された電子メールアドレスの識別子と、サーバー上のそのアドレスの状態を示します。</span><span class="sxs-lookup"><span data-stu-id="c7943-114">Provides an identifier for a fully resolved e-mail address, and the status of that address on the server.</span></span> <span data-ttu-id="c7943-115">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="c7943-115">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c7943-116">親要素</span><span class="sxs-lookup"><span data-stu-id="c7943-116">Parent elements</span></span>

|<span data-ttu-id="c7943-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="c7943-117">**Element**</span></span>|<span data-ttu-id="c7943-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="c7943-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c7943-119">DistributionList</span><span class="sxs-lookup"><span data-stu-id="c7943-119">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="c7943-120">配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="c7943-120">Represents a distribution list.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c7943-121">注釈</span><span class="sxs-lookup"><span data-stu-id="c7943-121">Remarks</span></span>

<span data-ttu-id="c7943-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="c7943-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c7943-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="c7943-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c7943-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="c7943-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c7943-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c7943-125">Schema Name</span></span>  <br/> |<span data-ttu-id="c7943-126">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="c7943-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="c7943-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c7943-127">Validation File</span></span>  <br/> |<span data-ttu-id="c7943-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="c7943-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c7943-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="c7943-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="c7943-130">正しくない</span><span class="sxs-lookup"><span data-stu-id="c7943-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c7943-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="c7943-131">See also</span></span>

- [<span data-ttu-id="c7943-132">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="c7943-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

