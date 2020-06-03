---
title: TextBody
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bd0c0bce-3e7c-47c7-af7f-5ee5f5ad9820
description: TextBody 要素は、テキスト本文を指定します。
ms.openlocfilehash: c0002785fb990a251267218f7a5f232e521db41a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459484"
---
# <a name="textbody"></a><span data-ttu-id="ec488-103">TextBody</span><span class="sxs-lookup"><span data-stu-id="ec488-103">TextBody</span></span>

<span data-ttu-id="ec488-104">**Textbody**要素は、テキスト本文を指定します。</span><span class="sxs-lookup"><span data-stu-id="ec488-104">The **TextBody** element specifies the text body.</span></span> 
  
```XML
<TextBody BodyTypeType=" HTML | Text" IsTruncated=" true | false"></TextBody>
```

 <span data-ttu-id="ec488-105">**BodyType**</span><span class="sxs-lookup"><span data-stu-id="ec488-105">**BodyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ec488-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="ec488-106">Attributes and elements</span></span>

<span data-ttu-id="ec488-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ec488-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ec488-108">属性</span><span class="sxs-lookup"><span data-stu-id="ec488-108">Attributes</span></span>

|<span data-ttu-id="ec488-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="ec488-109">**Attribute**</span></span>|<span data-ttu-id="ec488-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="ec488-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ec488-111">BodyTypeType</span><span class="sxs-lookup"><span data-stu-id="ec488-111">BodyTypeType</span></span>  <br/> |<span data-ttu-id="ec488-112">本文の種類を示します。</span><span class="sxs-lookup"><span data-stu-id="ec488-112">Indicates the body type.</span></span> <span data-ttu-id="ec488-113">**Bodytypetype**属性の**テキスト**の値は、本文がプレーンテキスト形式であることを示します。</span><span class="sxs-lookup"><span data-stu-id="ec488-113">The value of **Text** for the **BodyTypeType** attribute indicates that the body is in plain text form.</span></span> <span data-ttu-id="ec488-114">**Bodytypetype**属性の**html**の値は、本文が HTML 形式であることを示します。</span><span class="sxs-lookup"><span data-stu-id="ec488-114">The value of **HTML** for the **BodyTypeType** attribute indicates that the body is in HTML form.</span></span> <span data-ttu-id="ec488-115">**Bodytypetype**属性は必須です。</span><span class="sxs-lookup"><span data-stu-id="ec488-115">The **BodyTypeType** attribute is required.</span></span>  <br/> |
|<span data-ttu-id="ec488-116">Istrがありません</span><span class="sxs-lookup"><span data-stu-id="ec488-116">IsTruncated</span></span>  <br/> |<span data-ttu-id="ec488-117">本文の内容が切り捨てられていることを示します。</span><span class="sxs-lookup"><span data-stu-id="ec488-117">Indicates that the body contents have been truncated.</span></span> <span data-ttu-id="ec488-118">**Istruncated** attribute のテキスト値が**false**の場合は、本文のコンテンツが切り捨てられていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="ec488-118">A text value of **false** for the **IsTruncated** attribute indicates that the body contents have not been truncated.</span></span> <span data-ttu-id="ec488-119">テキストの本文の長さが[Maximumbodysize](maximumbodysize.md)要素で設定された値よりも長い場合は、正規化された本文が切り捨てられます。</span><span class="sxs-lookup"><span data-stu-id="ec488-119">The normalized body will be truncated if the text body length is longer than the value set in the [MaximumBodySize](maximumbodysize.md) element.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="ec488-120">子要素</span><span class="sxs-lookup"><span data-stu-id="ec488-120">Child elements</span></span>

<span data-ttu-id="ec488-121">なし。</span><span class="sxs-lookup"><span data-stu-id="ec488-121">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ec488-122">親要素</span><span class="sxs-lookup"><span data-stu-id="ec488-122">Parent elements</span></span>

<span data-ttu-id="ec488-123">[アイテム](item.md)  | [連絡先](contact.md)  | [メッセージ](message-ex15websvcsotherref.md)  | [DistributionList](distributionlist.md)  | [Calendaritem](calendaritem.md)  | [Postitem](postitem.md)  | [タスク](task.md)</span><span class="sxs-lookup"><span data-stu-id="ec488-123">[Item](item.md) | [Contact](contact.md) | [Message](message-ex15websvcsotherref.md) | [DistributionList](distributionlist.md) | [CalendarItem](calendaritem.md) | [PostItem](postitem.md) | [Task](task.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="ec488-124">テキスト値</span><span class="sxs-lookup"><span data-stu-id="ec488-124">Text value</span></span>

<span data-ttu-id="ec488-125">**Textbody**要素のテキスト値は、アイテムの本文です。</span><span class="sxs-lookup"><span data-stu-id="ec488-125">The text value of the **TextBody** element is the text body of the item.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="ec488-126">注釈</span><span class="sxs-lookup"><span data-stu-id="ec488-126">Remarks</span></span>

<span data-ttu-id="ec488-127">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="ec488-127">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="ec488-128">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="ec488-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ec488-129">要素の情報</span><span class="sxs-lookup"><span data-stu-id="ec488-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ec488-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="ec488-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ec488-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ec488-131">Schema name</span></span>  <br/> |<span data-ttu-id="ec488-132">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="ec488-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="ec488-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ec488-133">Validation file</span></span>  <br/> |<span data-ttu-id="ec488-134">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="ec488-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ec488-135">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="ec488-135">Can be empty</span></span>  <br/> ||
   

