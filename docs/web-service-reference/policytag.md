---
title: PolicyTag
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fa4b1447-dc7b-47ad-a677-78fcee443dc6
description: PolicyTag 要素は、アイテムまたはフォルダーの保持識別子を指定します。
ms.openlocfilehash: ddc4d890d1e514586ba5ea7f6a8b541b2e4786c7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460898"
---
# <a name="policytag"></a><span data-ttu-id="f7816-103">PolicyTag</span><span class="sxs-lookup"><span data-stu-id="f7816-103">PolicyTag</span></span>

<span data-ttu-id="f7816-104">**Policytag**要素は、アイテムまたはフォルダーの保持識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="f7816-104">The **PolicyTag** element specifies the retention identifier on an item or folder.</span></span> 
  
```xml
<PolicyTag IsExplicit="true | false"></PolicyTag>
```

 <span data-ttu-id="f7816-105">**RetentionTagType**</span><span class="sxs-lookup"><span data-stu-id="f7816-105">**RetentionTagType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f7816-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="f7816-106">Attributes and elements</span></span>

<span data-ttu-id="f7816-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f7816-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f7816-108">属性</span><span class="sxs-lookup"><span data-stu-id="f7816-108">Attributes</span></span>

|<span data-ttu-id="f7816-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="f7816-109">**Attribute**</span></span>|<span data-ttu-id="f7816-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="f7816-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f7816-111">IsExplicit</span><span class="sxs-lookup"><span data-stu-id="f7816-111">IsExplicit</span></span>  <br/> |<span data-ttu-id="f7816-112">アイテムまたはフォルダーにポリシータグが明示的に設定されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f7816-112">Indicates whether a policy tag was explicitly set on an item or folder.</span></span>  <br/> <span data-ttu-id="f7816-113">**IsExplicit**属性のテキスト値が**true の場合**は、ポリシータグがアイテムまたはフォルダーに明示的に設定されていることを示します。</span><span class="sxs-lookup"><span data-stu-id="f7816-113">A text value of **true** for the **IsExplicit** attribute indicates that the policy tag was explicitly set on the item or folder.</span></span> <span data-ttu-id="f7816-114">テキスト値が**false**の場合は、親フォルダーポリシータグに基づいてアイテムまたはフォルダーにポリシータグが暗黙的に設定されていることを示します。</span><span class="sxs-lookup"><span data-stu-id="f7816-114">A text value of **false** indicates that the policy tag was implicitly set on the item or folder based on the parent folder policy tag.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="f7816-115">子要素</span><span class="sxs-lookup"><span data-stu-id="f7816-115">Child elements</span></span>

<span data-ttu-id="f7816-116">なし。</span><span class="sxs-lookup"><span data-stu-id="f7816-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f7816-117">親要素</span><span class="sxs-lookup"><span data-stu-id="f7816-117">Parent elements</span></span>

<span data-ttu-id="f7816-118">[Searchプレビューアイテム](searchpreviewitem.md)  | [アイテム](item.md)  | [連絡先](contact.md)  | [メッセージ](message-ex15websvcsotherref.md)  | [DistributionList](distributionlist.md)  | [Calendaritem](calendaritem.md)  | [Postitem](postitem.md)  | [タスク](task.md)</span><span class="sxs-lookup"><span data-stu-id="f7816-118">[SearchPreviewItem](searchpreviewitem.md) | [Item](item.md) | [Contact](contact.md) | [Message](message-ex15websvcsotherref.md) | [DistributionList](distributionlist.md) | [CalendarItem](calendaritem.md) | [PostItem](postitem.md) | [Task](task.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="f7816-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="f7816-119">Text value</span></span>

<span data-ttu-id="f7816-120">**Policytag**要素のテキスト値は、ポリシータグ識別子です。</span><span class="sxs-lookup"><span data-stu-id="f7816-120">The text value of the **PolicyTag** element is the policy tag identifier.</span></span> <span data-ttu-id="f7816-121">ポリシータグ識別子は GUID です。</span><span class="sxs-lookup"><span data-stu-id="f7816-121">The policy tag identifier is a GUID.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="f7816-122">注釈</span><span class="sxs-lookup"><span data-stu-id="f7816-122">Remarks</span></span>

<span data-ttu-id="f7816-123">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="f7816-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f7816-124">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="f7816-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f7816-125">要素の情報</span><span class="sxs-lookup"><span data-stu-id="f7816-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f7816-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="f7816-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f7816-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f7816-127">Schema name</span></span>  <br/> |<span data-ttu-id="f7816-128">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="f7816-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="f7816-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f7816-129">Validation file</span></span>  <br/> |<span data-ttu-id="f7816-130">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="f7816-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f7816-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="f7816-131">Can be empty</span></span>  <br/> ||
   

