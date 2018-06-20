---
title: SeekToConditionPageItemView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b3b86720-d086-47c3-94af-921fdd719edf
description: SeekToConditionPageItemView 要素は、検索の終了、検索、戻るには、最大のエントリと FindItem または FindConversation の検索に検索方向の開始インデックスを識別するために使用される条件を識別します。
ms.openlocfilehash: e95246079f8c6e7acffac1dabb278895265767d9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833328"
---
# <a name="seektoconditionpageitemview"></a><span data-ttu-id="8e78f-103">SeekToConditionPageItemView</span><span class="sxs-lookup"><span data-stu-id="8e78f-103">SeekToConditionPageItemView</span></span>

<span data-ttu-id="8e78f-104">**FindItem**または**FindConversation の最後の検索、検索、戻るには、最大のエントリ、および検索方向の開始インデックスを識別するために使用される条件を識別する**SeekToConditionPageItemView**要素**検索します。</span><span class="sxs-lookup"><span data-stu-id="8e78f-104">The **SeekToConditionPageItemView** element identifies the condition that is used to identify the end of a search, the starting index of a search, the maximum entries to return, and the search directions for a **FindItem** or **FindConversation** search.</span></span> 
  
```XML
<SeekToConditionPageItemView BasePoint="" MaxEntriesReturned="">
   <Condition/>
</SeekToConditionPageItemView>
```

 <span data-ttu-id="8e78f-105">**SeekToConditionPageViewType**</span><span class="sxs-lookup"><span data-stu-id="8e78f-105">**SeekToConditionPageViewType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8e78f-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="8e78f-106">Attributes and elements</span></span>

<span data-ttu-id="8e78f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8e78f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8e78f-108">属性</span><span class="sxs-lookup"><span data-stu-id="8e78f-108">Attributes</span></span>

|<span data-ttu-id="8e78f-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="8e78f-109">**Attribute**</span></span>|<span data-ttu-id="8e78f-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="8e78f-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8e78f-111">ベース ポイント</span><span class="sxs-lookup"><span data-stu-id="8e78f-111">BasePoint</span></span>  <br/> |<span data-ttu-id="8e78f-112">**ベース ポイント**属性のテキスト値は、検索の開始位置から基本のポイントです。</span><span class="sxs-lookup"><span data-stu-id="8e78f-112">The text value of the **BasePoint** attribute is the base point from where the search will start.</span></span> <span data-ttu-id="8e78f-113">**先頭**のテキスト値は、結果セットの先頭に、検索を開始することを示します。</span><span class="sxs-lookup"><span data-stu-id="8e78f-113">A text value of **Beginning** indicates that the search will start at the beginning of the result set.</span></span> <span data-ttu-id="8e78f-114">**最後**のテキスト値は、結果セットの最後に、検索を開始することを示します。</span><span class="sxs-lookup"><span data-stu-id="8e78f-114">A text value of **End** indicates that the search will start at the end of the result set.</span></span>  <br/> |
|<span data-ttu-id="8e78f-115">MaxEntriesReturned</span><span class="sxs-lookup"><span data-stu-id="8e78f-115">MaxEntriesReturned</span></span>  <br/> |<span data-ttu-id="8e78f-116">**MaxEntriesReturned**属性のテキスト値は、結果セットで返すことができるアイテムの最大数です。</span><span class="sxs-lookup"><span data-stu-id="8e78f-116">The text value of the **MaxEntriesReturned** attribute is the maximum number of items that can be returned in a result set.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="8e78f-117">子要素</span><span class="sxs-lookup"><span data-stu-id="8e78f-117">Child elements</span></span>

[<span data-ttu-id="8e78f-118">条件 (RestrictionType)</span><span class="sxs-lookup"><span data-stu-id="8e78f-118">Condition (RestrictionType)</span></span>](condition-restrictiontype.md)
  
### <a name="parent-elements"></a><span data-ttu-id="8e78f-119">親要素</span><span class="sxs-lookup"><span data-stu-id="8e78f-119">Parent elements</span></span>

<span data-ttu-id="8e78f-120">[FindConversation](findconversation.md) | [FindItem](finditem.md)</span><span class="sxs-lookup"><span data-stu-id="8e78f-120">[FindConversation](findconversation.md) | [FindItem](finditem.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8e78f-121">備考</span><span class="sxs-lookup"><span data-stu-id="8e78f-121">Remarks</span></span>

<span data-ttu-id="8e78f-122">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="8e78f-122">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="8e78f-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="8e78f-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8e78f-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="8e78f-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8e78f-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="8e78f-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="8e78f-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8e78f-126">Schema name</span></span>  <br/> |<span data-ttu-id="8e78f-127">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="8e78f-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="8e78f-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8e78f-128">Validation file</span></span>  <br/> |<span data-ttu-id="8e78f-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="8e78f-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8e78f-130">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="8e78f-130">Can be empty</span></span>  <br/> |<span data-ttu-id="8e78f-131">false</span><span class="sxs-lookup"><span data-stu-id="8e78f-131">false</span></span>  <br/> |
   

