---
title: MemberCorrelationKey
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 60cc7094-2e31-49d2-8598-181bcfb5f130
description: MemberCorrelationKey 要素は、インスタント メッセージング (IM) のグループの一部である取引先担当者の識別子を指定します。
ms.openlocfilehash: 4e45a86a5ead48576dcab7f3a53e1c3ad72ec173
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832445"
---
# <a name="membercorrelationkey"></a><span data-ttu-id="bc15c-103">MemberCorrelationKey</span><span class="sxs-lookup"><span data-stu-id="bc15c-103">MemberCorrelationKey</span></span>

<span data-ttu-id="bc15c-104">**MemberCorrelationKey**要素は、インスタント メッセージング (IM) のグループの一部である取引先担当者の識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="bc15c-104">The **MemberCorrelationKey** element specifies the identifiers of the contacts that are part of the instant messaging (IM) group.</span></span> 
  
```XML
<MemberCorrelationKey>
   <ItemId/>
</MemberCorrelationKey>
```

<span data-ttu-id="bc15c-105">**NonEmptyArrayOfItemIdsType**</span><span class="sxs-lookup"><span data-stu-id="bc15c-105">**NonEmptyArrayOfItemIdsType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="bc15c-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="bc15c-106">Attributes and elements</span></span>

<span data-ttu-id="bc15c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="bc15c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bc15c-108">属性</span><span class="sxs-lookup"><span data-stu-id="bc15c-108">Attributes</span></span>

<span data-ttu-id="bc15c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="bc15c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bc15c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="bc15c-110">Child elements</span></span>

[<span data-ttu-id="bc15c-111">ItemId</span><span class="sxs-lookup"><span data-stu-id="bc15c-111">ItemId</span></span>](itemid.md)
  
### <a name="parent-elements"></a><span data-ttu-id="bc15c-112">親要素</span><span class="sxs-lookup"><span data-stu-id="bc15c-112">Parent elements</span></span>

[<span data-ttu-id="bc15c-113">ImGroup</span><span class="sxs-lookup"><span data-stu-id="bc15c-113">ImGroup</span></span>](imgroup.md)
  
## <a name="remarks"></a><span data-ttu-id="bc15c-114">備考</span><span class="sxs-lookup"><span data-stu-id="bc15c-114">Remarks</span></span>

<span data-ttu-id="bc15c-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="bc15c-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="bc15c-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="bc15c-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bc15c-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="bc15c-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bc15c-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="bc15c-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bc15c-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="bc15c-119">Schema name</span></span>  <br/> |<span data-ttu-id="bc15c-120">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="bc15c-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="bc15c-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="bc15c-121">Validation file</span></span>  <br/> |<span data-ttu-id="bc15c-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="bc15c-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bc15c-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="bc15c-123">Can be empty</span></span>  <br/> ||
   

