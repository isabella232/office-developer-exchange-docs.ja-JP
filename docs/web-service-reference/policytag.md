---
title: PolicyTag
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fa4b1447-dc7b-47ad-a677-78fcee443dc6
description: PolicyTag 要素は、アイテムまたはフォルダーの保存期間の識別子を指定します。
ms.openlocfilehash: d6cd5aab1145f6006912541c8f8c1d0a91d1e17e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832835"
---
# <a name="policytag"></a><span data-ttu-id="fb884-103">PolicyTag</span><span class="sxs-lookup"><span data-stu-id="fb884-103">PolicyTag</span></span>

<span data-ttu-id="fb884-104">**PolicyTag**要素は、アイテムまたはフォルダーの保存期間の識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="fb884-104">The **PolicyTag** element specifies the retention identifier on an item or folder.</span></span> 
  
```xml
<PolicyTag IsExplicit="true | false"></PolicyTag>
```

 <span data-ttu-id="fb884-105">**RetentionTagType**</span><span class="sxs-lookup"><span data-stu-id="fb884-105">**RetentionTagType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fb884-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="fb884-106">Attributes and elements</span></span>

<span data-ttu-id="fb884-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="fb884-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fb884-108">属性</span><span class="sxs-lookup"><span data-stu-id="fb884-108">Attributes</span></span>

|<span data-ttu-id="fb884-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="fb884-109">**Attribute**</span></span>|<span data-ttu-id="fb884-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="fb884-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="fb884-111">IsExplicit</span><span class="sxs-lookup"><span data-stu-id="fb884-111">IsExplicit</span></span>  <br/> |<span data-ttu-id="fb884-112">ポリシー タグがアイテムまたはフォルダーに明示的に設定するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="fb884-112">Indicates whether a policy tag was explicitly set on an item or folder.</span></span>  <br/> <span data-ttu-id="fb884-113">の**場合は true** 、 **IsExplicit**属性のテキスト値は、ポリシー タグがアイテムまたはフォルダーを明示的に設定されていることを示します。</span><span class="sxs-lookup"><span data-stu-id="fb884-113">A text value of **true** for the **IsExplicit** attribute indicates that the policy tag was explicitly set on the item or folder.</span></span> <span data-ttu-id="fb884-114">**False**のテキスト値は、ポリシー タグがアイテムまたはフォルダーの親フォルダーのポリシー タグに基づいて暗黙的に設定されていることを示します。</span><span class="sxs-lookup"><span data-stu-id="fb884-114">A text value of **false** indicates that the policy tag was implicitly set on the item or folder based on the parent folder policy tag.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="fb884-115">子要素</span><span class="sxs-lookup"><span data-stu-id="fb884-115">Child elements</span></span>

<span data-ttu-id="fb884-116">なし。</span><span class="sxs-lookup"><span data-stu-id="fb884-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fb884-117">親要素</span><span class="sxs-lookup"><span data-stu-id="fb884-117">Parent elements</span></span>

<span data-ttu-id="fb884-118">[SearchPreviewItem](searchpreviewitem.md) | [アイテム](item.md) | [連絡先](contact.md) | [メッセージ](message-ex15websvcsotherref.md) | [DistributionList](distributionlist.md) | [カレンダー項目](calendaritem.md) | [PostItem](postitem.md) | [タスク](task.md)</span><span class="sxs-lookup"><span data-stu-id="fb884-118">[SearchPreviewItem](searchpreviewitem.md) | [Item](item.md) | [Contact](contact.md) | [Message](message-ex15websvcsotherref.md) | [DistributionList](distributionlist.md) | [CalendarItem](calendaritem.md) | [PostItem](postitem.md) | [Task](task.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="fb884-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="fb884-119">Text value</span></span>

<span data-ttu-id="fb884-120">**PolicyTag**要素のテキスト値は、ポリシー タグ識別子です。</span><span class="sxs-lookup"><span data-stu-id="fb884-120">The text value of the **PolicyTag** element is the policy tag identifier.</span></span> <span data-ttu-id="fb884-121">ポリシーのタグ識別子は、GUID です。</span><span class="sxs-lookup"><span data-stu-id="fb884-121">The policy tag identifier is a GUID.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="fb884-122">備考</span><span class="sxs-lookup"><span data-stu-id="fb884-122">Remarks</span></span>

<span data-ttu-id="fb884-123">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="fb884-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="fb884-124">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="fb884-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fb884-125">要素情報</span><span class="sxs-lookup"><span data-stu-id="fb884-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fb884-126">名前空間</span><span class="sxs-lookup"><span data-stu-id="fb884-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fb884-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="fb884-127">Schema name</span></span>  <br/> |<span data-ttu-id="fb884-128">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="fb884-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="fb884-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="fb884-129">Validation file</span></span>  <br/> |<span data-ttu-id="fb884-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="fb884-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fb884-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="fb884-131">Can be empty</span></span>  <br/> ||
   

