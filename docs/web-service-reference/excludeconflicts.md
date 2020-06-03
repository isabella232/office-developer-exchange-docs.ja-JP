---
title: ExcludeConflicts
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExcludeConflicts
api_type:
- schema
ms.assetid: ec33ef23-8537-41eb-8d89-7eb906a1fad7
description: ExcludeConflicts 要素は、出席者間での予定表の時間について提案された時間を返すかどうかを指定します。
ms.openlocfilehash: d20c594ae600abf110681ea678b2d95a23bf7809
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456977"
---
# <a name="excludeconflicts"></a><span data-ttu-id="06b16-103">ExcludeConflicts</span><span class="sxs-lookup"><span data-stu-id="06b16-103">ExcludeConflicts</span></span>

<span data-ttu-id="06b16-104">**ExcludeConflicts**要素は、出席者間での予定表の時間について提案された時間を返すかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="06b16-104">The **ExcludeConflicts** element specifies whether to return suggested times for calendar times that conflict among the attendees.</span></span> 
  
[<span data-ttu-id="06b16-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="06b16-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="06b16-106">MailboxDataArray</span><span class="sxs-lookup"><span data-stu-id="06b16-106">MailboxDataArray</span></span>](mailboxdataarray.md)
  
[<span data-ttu-id="06b16-107">MailboxData</span><span class="sxs-lookup"><span data-stu-id="06b16-107">MailboxData</span></span>](mailboxdata.md)
  
[<span data-ttu-id="06b16-108">ExcludeConflicts</span><span class="sxs-lookup"><span data-stu-id="06b16-108">ExcludeConflicts</span></span>](excludeconflicts.md)
  
```xml
<ExcludeConflicts>true or false</ExcludeConflicts>
```

 <span data-ttu-id="06b16-109">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="06b16-109">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="06b16-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="06b16-110">Attributes and elements</span></span>

<span data-ttu-id="06b16-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="06b16-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="06b16-112">属性</span><span class="sxs-lookup"><span data-stu-id="06b16-112">Attributes</span></span>

<span data-ttu-id="06b16-113">なし。</span><span class="sxs-lookup"><span data-stu-id="06b16-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="06b16-114">子要素</span><span class="sxs-lookup"><span data-stu-id="06b16-114">Child elements</span></span>

<span data-ttu-id="06b16-115">なし。</span><span class="sxs-lookup"><span data-stu-id="06b16-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="06b16-116">親要素</span><span class="sxs-lookup"><span data-stu-id="06b16-116">Parent elements</span></span>

|<span data-ttu-id="06b16-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="06b16-117">**Element**</span></span>|<span data-ttu-id="06b16-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="06b16-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="06b16-119">MailboxData</span><span class="sxs-lookup"><span data-stu-id="06b16-119">MailboxData</span></span>](mailboxdata.md) <br/> |<span data-ttu-id="06b16-120">個々のメールボックスユーザー、およびメールボックスユーザーに関して返されるデータの種類のオプションを表します。</span><span class="sxs-lookup"><span data-stu-id="06b16-120">Represents an individual mailbox user and options for the type of data to be returned about the mailbox user.</span></span>  <br/> <span data-ttu-id="06b16-121">この要素の XPath を次に示します。</span><span class="sxs-lookup"><span data-stu-id="06b16-121">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/MailboxDataArray/MailboxData` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="06b16-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="06b16-122">Text value</span></span>

<span data-ttu-id="06b16-123">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="06b16-123">A text value is required.</span></span> <span data-ttu-id="06b16-124">指定できる値は、ブール値**true**または**false**です。</span><span class="sxs-lookup"><span data-stu-id="06b16-124">The possible values are a Boolean **true** or **false**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="06b16-125">注釈</span><span class="sxs-lookup"><span data-stu-id="06b16-125">Remarks</span></span>

<span data-ttu-id="06b16-126">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="06b16-126">This element is required.</span></span>
  
> [!NOTE]
> <span data-ttu-id="06b16-127">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの/EWS/ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="06b16-127">The schema that describes this element is located in the /EWS/ directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="06b16-128">要素の情報</span><span class="sxs-lookup"><span data-stu-id="06b16-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="06b16-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="06b16-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="06b16-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="06b16-130">Schema Name</span></span>  <br/> |<span data-ttu-id="06b16-131">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="06b16-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="06b16-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="06b16-132">Validation File</span></span>  <br/> |<span data-ttu-id="06b16-133">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="06b16-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="06b16-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="06b16-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="06b16-135">正しくない</span><span class="sxs-lookup"><span data-stu-id="06b16-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="06b16-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="06b16-136">See also</span></span>



[<span data-ttu-id="06b16-137">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="06b16-137">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="06b16-138">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="06b16-138">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)


[<span data-ttu-id="06b16-139">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="06b16-139">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

