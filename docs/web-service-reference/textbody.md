---
title: TextBody
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bd0c0bce-3e7c-47c7-af7f-5ee5f5ad9820
description: TextBody 要素は、テキストの本文を指定します。
ms.openlocfilehash: 78b18b27891d571605d2eeeeffb5c252cc790c11
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839664"
---
# <a name="textbody"></a><span data-ttu-id="01e0d-103">TextBody</span><span class="sxs-lookup"><span data-stu-id="01e0d-103">TextBody</span></span>

<span data-ttu-id="01e0d-104">**TextBody**要素は、テキストの本文を指定します。</span><span class="sxs-lookup"><span data-stu-id="01e0d-104">The **TextBody** element specifies the text body.</span></span> 
  
```XML
<TextBody BodyTypeType=" HTML | Text" IsTruncated=" true | false"></TextBody>
```

 <span data-ttu-id="01e0d-105">**BodyType**</span><span class="sxs-lookup"><span data-stu-id="01e0d-105">**BodyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="01e0d-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="01e0d-106">Attributes and elements</span></span>

<span data-ttu-id="01e0d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="01e0d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="01e0d-108">属性</span><span class="sxs-lookup"><span data-stu-id="01e0d-108">Attributes</span></span>

|<span data-ttu-id="01e0d-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="01e0d-109">**Attribute**</span></span>|<span data-ttu-id="01e0d-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="01e0d-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="01e0d-111">BodyTypeType</span><span class="sxs-lookup"><span data-stu-id="01e0d-111">BodyTypeType</span></span>  <br/> |<span data-ttu-id="01e0d-112">本文の種類を示します。</span><span class="sxs-lookup"><span data-stu-id="01e0d-112">Indicates the body type.</span></span> <span data-ttu-id="01e0d-113">**BodyTypeType**属性の**テキスト**の値は、プレーン テキスト形式の本文であることを示します。</span><span class="sxs-lookup"><span data-stu-id="01e0d-113">The value of **Text** for the **BodyTypeType** attribute indicates that the body is in plain text form.</span></span> <span data-ttu-id="01e0d-114">**BodyTypeType**属性の値を**HTML**の本文が HTML フォーム内でことを示します。</span><span class="sxs-lookup"><span data-stu-id="01e0d-114">The value of **HTML** for the **BodyTypeType** attribute indicates that the body is in HTML form.</span></span> <span data-ttu-id="01e0d-115">**BodyTypeType**属性が必要です。</span><span class="sxs-lookup"><span data-stu-id="01e0d-115">The **BodyTypeType** attribute is required.</span></span>  <br/> |
|<span data-ttu-id="01e0d-116">IsTruncated</span><span class="sxs-lookup"><span data-stu-id="01e0d-116">IsTruncated</span></span>  <br/> |<span data-ttu-id="01e0d-117">本文の内容が切り詰められたことを示します。</span><span class="sxs-lookup"><span data-stu-id="01e0d-117">Indicates that the body contents have been truncated.</span></span> <span data-ttu-id="01e0d-118">テキスト値が**false**の**IsTruncated**属性のでは、本文の内容は切り捨てられましたしないことを示します。</span><span class="sxs-lookup"><span data-stu-id="01e0d-118">A text value of **false** for the **IsTruncated** attribute indicates that the body contents have not been truncated.</span></span> <span data-ttu-id="01e0d-119">テキスト本文の長さは、 [MaximumBodySize](maximumbodysize.md)要素で設定された値より長い場合、正規化された本文は切り捨てられます。</span><span class="sxs-lookup"><span data-stu-id="01e0d-119">The normalized body will be truncated if the text body length is longer than the value set in the [MaximumBodySize](maximumbodysize.md) element.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="01e0d-120">子要素</span><span class="sxs-lookup"><span data-stu-id="01e0d-120">Child elements</span></span>

<span data-ttu-id="01e0d-121">なし。</span><span class="sxs-lookup"><span data-stu-id="01e0d-121">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="01e0d-122">親要素</span><span class="sxs-lookup"><span data-stu-id="01e0d-122">Parent elements</span></span>

<span data-ttu-id="01e0d-123">[項目](item.md) | [連絡先](contact.md) | [メッセージ](message-ex15websvcsotherref.md) | [DistributionList](distributionlist.md) | [カレンダー項目](calendaritem.md) | [PostItem](postitem.md) | [タスク](task.md)</span><span class="sxs-lookup"><span data-stu-id="01e0d-123">[Item](item.md) | [Contact](contact.md) | [Message](message-ex15websvcsotherref.md) | [DistributionList](distributionlist.md) | [CalendarItem](calendaritem.md) | [PostItem](postitem.md) | [Task](task.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="01e0d-124">テキスト値</span><span class="sxs-lookup"><span data-stu-id="01e0d-124">Text value</span></span>

<span data-ttu-id="01e0d-125">**TextBody**要素のテキスト値は、項目のテキストの本文です。</span><span class="sxs-lookup"><span data-stu-id="01e0d-125">The text value of the **TextBody** element is the text body of the item.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="01e0d-126">備考</span><span class="sxs-lookup"><span data-stu-id="01e0d-126">Remarks</span></span>

<span data-ttu-id="01e0d-127">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="01e0d-127">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="01e0d-128">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="01e0d-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="01e0d-129">要素情報</span><span class="sxs-lookup"><span data-stu-id="01e0d-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="01e0d-130">名前空間</span><span class="sxs-lookup"><span data-stu-id="01e0d-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="01e0d-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="01e0d-131">Schema name</span></span>  <br/> |<span data-ttu-id="01e0d-132">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="01e0d-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="01e0d-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="01e0d-133">Validation file</span></span>  <br/> |<span data-ttu-id="01e0d-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="01e0d-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="01e0d-135">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="01e0d-135">Can be empty</span></span>  <br/> ||
   

