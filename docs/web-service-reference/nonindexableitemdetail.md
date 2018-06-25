---
title: NonIndexableItemDetail
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a26d4c02-f1bd-40c4-9257-5db45e839f17
description: NonIndexableItemDetail 要素は、インデックスを作成できないアイテムに関する詳細情報を指定します。
ms.openlocfilehash: ef1bd072a44b42b501a3016c394b89fe6ab25bf0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832543"
---
# <a name="nonindexableitemdetail"></a><span data-ttu-id="4c313-103">NonIndexableItemDetail</span><span class="sxs-lookup"><span data-stu-id="4c313-103">NonIndexableItemDetail</span></span>

<span data-ttu-id="4c313-104">**NonIndexableItemDetail**要素は、インデックスを作成できないアイテムに関する詳細情報を指定します。</span><span class="sxs-lookup"><span data-stu-id="4c313-104">The **NonIndexableItemDetail** element specifies detail information about an item that cannot be indexed.</span></span> 
  
```XML
<NonIndexableItemDetail>
   <ItemId/>
   <ErrorCode/>
   <ErrorDescription/>
   <IsPartiallyIndexed/>
   <IsPermanentFailure/>
   <SortValue/>
   <AttemptCount/>
   <LastAttemptTime/>
   <AdditionalInfo/>
</NonIndexableItemDetail>
```

 <span data-ttu-id="4c313-105">**NonIndexableItemDetailType**</span><span class="sxs-lookup"><span data-stu-id="4c313-105">**NonIndexableItemDetailType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4c313-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="4c313-106">Attributes and elements</span></span>

<span data-ttu-id="4c313-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4c313-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4c313-108">属性</span><span class="sxs-lookup"><span data-stu-id="4c313-108">Attributes</span></span>

<span data-ttu-id="4c313-109">なし。</span><span class="sxs-lookup"><span data-stu-id="4c313-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4c313-110">子要素</span><span class="sxs-lookup"><span data-stu-id="4c313-110">Child elements</span></span>

<span data-ttu-id="4c313-111">[ItemId](itemid.md) | [エラー コード (ItemIndexErrorType)](errorcode-itemindexerrortype.md) | [ErrorDescription](errordescription.md) | [IsPartiallyIndexed](ispartiallyindexed.md) | [IsPermanentFailure](ispermanentfailure.md) | [SortValue](sortvalue.md) | [AttemptCount](attemptcount.md)  |  [LastAttemptTime](lastattempttime.md) | [AdditionalInfo](additionalinfo.md)</span><span class="sxs-lookup"><span data-stu-id="4c313-111">[ItemId](itemid.md) | [ErrorCode (ItemIndexErrorType)](errorcode-itemindexerrortype.md) | [ErrorDescription](errordescription.md) | [IsPartiallyIndexed](ispartiallyindexed.md) | [IsPermanentFailure](ispermanentfailure.md) | [SortValue](sortvalue.md) | [AttemptCount](attemptcount.md) | [LastAttemptTime](lastattempttime.md) | [AdditionalInfo](additionalinfo.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4c313-112">親要素</span><span class="sxs-lookup"><span data-stu-id="4c313-112">Parent elements</span></span>

[<span data-ttu-id="4c313-113">アイテム (ArrayOfNonIndexableItemDetailsType)</span><span class="sxs-lookup"><span data-stu-id="4c313-113">Items (ArrayOfNonIndexableItemDetailsType)</span></span>](items-arrayofnonindexableitemdetailstype.md)
  
## <a name="remarks"></a><span data-ttu-id="4c313-114">備考</span><span class="sxs-lookup"><span data-stu-id="4c313-114">Remarks</span></span>

<span data-ttu-id="4c313-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="4c313-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4c313-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="4c313-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4c313-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="4c313-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4c313-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="4c313-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4c313-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4c313-119">Schema name</span></span>  <br/> |<span data-ttu-id="4c313-120">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="4c313-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="4c313-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4c313-121">Validation file</span></span>  <br/> |<span data-ttu-id="4c313-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4c313-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4c313-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="4c313-123">Can be empty</span></span>  <br/> ||
   

