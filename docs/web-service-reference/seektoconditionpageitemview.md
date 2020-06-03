---
title: SeekToConditionPageItemView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b3b86720-d086-47c3-94af-921fdd719edf
description: SeekToConditionPageItemView 要素は、検索の終了を識別するために使用される条件、検索の開始インデックス、返される最大エントリ、および FindItem または FindConversation 検索の検索方向を指定します。
ms.openlocfilehash: dbb073263740ccdf75367f85f672b7d5ec78f7a0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466837"
---
# <a name="seektoconditionpageitemview"></a><span data-ttu-id="a32fb-103">SeekToConditionPageItemView</span><span class="sxs-lookup"><span data-stu-id="a32fb-103">SeekToConditionPageItemView</span></span>

<span data-ttu-id="a32fb-104">**Seektoconditionpageitemview**要素は、検索の終了を識別するために使用される条件、検索の開始インデックス、返される最大エントリ、および**FindItem**または**findconversation**検索の検索方向を指定します。</span><span class="sxs-lookup"><span data-stu-id="a32fb-104">The **SeekToConditionPageItemView** element identifies the condition that is used to identify the end of a search, the starting index of a search, the maximum entries to return, and the search directions for a **FindItem** or **FindConversation** search.</span></span> 
  
```XML
<SeekToConditionPageItemView BasePoint="" MaxEntriesReturned="">
   <Condition/>
</SeekToConditionPageItemView>
```

 <span data-ttu-id="a32fb-105">**SeekToConditionPageViewType**</span><span class="sxs-lookup"><span data-stu-id="a32fb-105">**SeekToConditionPageViewType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a32fb-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="a32fb-106">Attributes and elements</span></span>

<span data-ttu-id="a32fb-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a32fb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a32fb-108">属性</span><span class="sxs-lookup"><span data-stu-id="a32fb-108">Attributes</span></span>

|<span data-ttu-id="a32fb-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="a32fb-109">**Attribute**</span></span>|<span data-ttu-id="a32fb-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="a32fb-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a32fb-111">BasePoint</span><span class="sxs-lookup"><span data-stu-id="a32fb-111">BasePoint</span></span>  <br/> |<span data-ttu-id="a32fb-112">**BasePoint**属性のテキスト値は、検索が開始されるベースポイントです。</span><span class="sxs-lookup"><span data-stu-id="a32fb-112">The text value of the **BasePoint** attribute is the base point from where the search will start.</span></span> <span data-ttu-id="a32fb-113">**先頭**のテキスト値は、検索が結果セットの先頭から開始されることを示します。</span><span class="sxs-lookup"><span data-stu-id="a32fb-113">A text value of **Beginning** indicates that the search will start at the beginning of the result set.</span></span> <span data-ttu-id="a32fb-114">テキスト値**End**は、検索が結果セットの末尾から開始されることを示します。</span><span class="sxs-lookup"><span data-stu-id="a32fb-114">A text value of **End** indicates that the search will start at the end of the result set.</span></span>  <br/> |
|<span data-ttu-id="a32fb-115">MaxEntriesReturned</span><span class="sxs-lookup"><span data-stu-id="a32fb-115">MaxEntriesReturned</span></span>  <br/> |<span data-ttu-id="a32fb-116">**Maxん返され**た属性のテキスト値は、結果セットで返すことができるアイテムの最大数です。</span><span class="sxs-lookup"><span data-stu-id="a32fb-116">The text value of the **MaxEntriesReturned** attribute is the maximum number of items that can be returned in a result set.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="a32fb-117">子要素</span><span class="sxs-lookup"><span data-stu-id="a32fb-117">Child elements</span></span>

[<span data-ttu-id="a32fb-118">条件 (RestrictionType)</span><span class="sxs-lookup"><span data-stu-id="a32fb-118">Condition (RestrictionType)</span></span>](condition-restrictiontype.md)
  
### <a name="parent-elements"></a><span data-ttu-id="a32fb-119">親要素</span><span class="sxs-lookup"><span data-stu-id="a32fb-119">Parent elements</span></span>

<span data-ttu-id="a32fb-120">[Findconversation](findconversation.md)  | [FindItem](finditem.md)</span><span class="sxs-lookup"><span data-stu-id="a32fb-120">[FindConversation](findconversation.md) | [FindItem](finditem.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a32fb-121">注釈</span><span class="sxs-lookup"><span data-stu-id="a32fb-121">Remarks</span></span>

<span data-ttu-id="a32fb-122">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="a32fb-122">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="a32fb-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="a32fb-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a32fb-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="a32fb-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a32fb-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="a32fb-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a32fb-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a32fb-126">Schema name</span></span>  <br/> |<span data-ttu-id="a32fb-127">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="a32fb-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a32fb-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a32fb-128">Validation file</span></span>  <br/> |<span data-ttu-id="a32fb-129">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="a32fb-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a32fb-130">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="a32fb-130">Can be empty</span></span>  <br/> |<span data-ttu-id="a32fb-131">false</span><span class="sxs-lookup"><span data-stu-id="a32fb-131">false</span></span>  <br/> |
   

