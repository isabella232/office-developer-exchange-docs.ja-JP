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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462431"
---
# <a name="members-memberlisttype"></a><span data-ttu-id="0b986-103">Members (MemberListType)</span><span class="sxs-lookup"><span data-stu-id="0b986-103">Members (MemberListType)</span></span>

<span data-ttu-id="0b986-104">**Members**要素は、配布リストのメンバーの一覧を提供します。</span><span class="sxs-lookup"><span data-stu-id="0b986-104">The **Members** element provides the list of members for a distribution list.</span></span> 
  
```xml
<Members>
   <Member/>
</Members>
```

<span data-ttu-id="0b986-105">**MemberListType**</span><span class="sxs-lookup"><span data-stu-id="0b986-105">**MemberListType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="0b986-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="0b986-106">Attributes and elements</span></span>

<span data-ttu-id="0b986-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0b986-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0b986-108">属性</span><span class="sxs-lookup"><span data-stu-id="0b986-108">Attributes</span></span>

<span data-ttu-id="0b986-109">なし。</span><span class="sxs-lookup"><span data-stu-id="0b986-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0b986-110">子要素</span><span class="sxs-lookup"><span data-stu-id="0b986-110">Child elements</span></span>

|<span data-ttu-id="0b986-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="0b986-111">**Element**</span></span>|<span data-ttu-id="0b986-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="0b986-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0b986-113">メンバー</span><span class="sxs-lookup"><span data-stu-id="0b986-113">Member</span></span>](member-ex15websvcsotherref.md) <br/> |<span data-ttu-id="0b986-114">完全に解決された電子メールアドレスの識別子と、サーバー上のそのアドレスの状態を示します。</span><span class="sxs-lookup"><span data-stu-id="0b986-114">Provides an identifier for a fully resolved e-mail address, and the status of that address on the server.</span></span> <span data-ttu-id="0b986-115">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="0b986-115">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0b986-116">親要素</span><span class="sxs-lookup"><span data-stu-id="0b986-116">Parent elements</span></span>

|<span data-ttu-id="0b986-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="0b986-117">**Element**</span></span>|<span data-ttu-id="0b986-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="0b986-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0b986-119">DistributionList</span><span class="sxs-lookup"><span data-stu-id="0b986-119">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="0b986-120">配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="0b986-120">Represents a distribution list.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0b986-121">注釈</span><span class="sxs-lookup"><span data-stu-id="0b986-121">Remarks</span></span>

<span data-ttu-id="0b986-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="0b986-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0b986-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="0b986-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0b986-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="0b986-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0b986-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0b986-125">Schema Name</span></span>  <br/> |<span data-ttu-id="0b986-126">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="0b986-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="0b986-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0b986-127">Validation File</span></span>  <br/> |<span data-ttu-id="0b986-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="0b986-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0b986-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="0b986-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="0b986-130">正しくない</span><span class="sxs-lookup"><span data-stu-id="0b986-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0b986-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="0b986-131">See also</span></span>

- [<span data-ttu-id="0b986-132">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="0b986-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

