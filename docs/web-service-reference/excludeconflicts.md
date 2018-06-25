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
description: ExcludeConflicts 要素を指定する候補を返すかどうか、参加者の間で競合するカレンダーの時間の時間です。
ms.openlocfilehash: 66b69d57246942e551de2f683949870823e2e4e1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760360"
---
# <a name="excludeconflicts"></a><span data-ttu-id="0bd61-103">ExcludeConflicts</span><span class="sxs-lookup"><span data-stu-id="0bd61-103">ExcludeConflicts</span></span>

<span data-ttu-id="0bd61-104">**ExcludeConflicts**要素を指定する候補を返すかどうか、参加者の間で競合するカレンダーの時間の時間です。</span><span class="sxs-lookup"><span data-stu-id="0bd61-104">The **ExcludeConflicts** element specifies whether to return suggested times for calendar times that conflict among the attendees.</span></span> 
  
[<span data-ttu-id="0bd61-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="0bd61-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="0bd61-106">MailboxDataArray</span><span class="sxs-lookup"><span data-stu-id="0bd61-106">MailboxDataArray</span></span>](mailboxdataarray.md)
  
[<span data-ttu-id="0bd61-107">MailboxData</span><span class="sxs-lookup"><span data-stu-id="0bd61-107">MailboxData</span></span>](mailboxdata.md)
  
[<span data-ttu-id="0bd61-108">ExcludeConflicts</span><span class="sxs-lookup"><span data-stu-id="0bd61-108">ExcludeConflicts</span></span>](excludeconflicts.md)
  
```xml
<ExcludeConflicts>true or false</ExcludeConflicts>
```

 <span data-ttu-id="0bd61-109">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="0bd61-109">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0bd61-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="0bd61-110">Attributes and elements</span></span>

<span data-ttu-id="0bd61-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0bd61-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0bd61-112">属性</span><span class="sxs-lookup"><span data-stu-id="0bd61-112">Attributes</span></span>

<span data-ttu-id="0bd61-113">なし。</span><span class="sxs-lookup"><span data-stu-id="0bd61-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0bd61-114">子要素</span><span class="sxs-lookup"><span data-stu-id="0bd61-114">Child elements</span></span>

<span data-ttu-id="0bd61-115">なし。</span><span class="sxs-lookup"><span data-stu-id="0bd61-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0bd61-116">親要素</span><span class="sxs-lookup"><span data-stu-id="0bd61-116">Parent elements</span></span>

|<span data-ttu-id="0bd61-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="0bd61-117">**Element**</span></span>|<span data-ttu-id="0bd61-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="0bd61-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0bd61-119">MailboxData</span><span class="sxs-lookup"><span data-stu-id="0bd61-119">MailboxData</span></span>](mailboxdata.md) <br/> |<span data-ttu-id="0bd61-120">個々 のメールボックス ユーザーのメールボックスのユーザーに返されるデータの種類のオプションを表します。</span><span class="sxs-lookup"><span data-stu-id="0bd61-120">Represents an individual mailbox user and options for the type of data to be returned about the mailbox user.</span></span>  <br/> <span data-ttu-id="0bd61-121">以下は、この要素の XPath です。</span><span class="sxs-lookup"><span data-stu-id="0bd61-121">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/MailboxDataArray/MailboxData` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0bd61-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="0bd61-122">Text value</span></span>

<span data-ttu-id="0bd61-123">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="0bd61-123">A text value is required.</span></span> <span data-ttu-id="0bd61-124">可能な値は、ブール値**true**または**false を指定**します。</span><span class="sxs-lookup"><span data-stu-id="0bd61-124">The possible values are a Boolean **true** or **false**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0bd61-125">備考</span><span class="sxs-lookup"><span data-stu-id="0bd61-125">Remarks</span></span>

<span data-ttu-id="0bd61-126">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="0bd61-126">This element is required.</span></span>
  
> [!NOTE]
> <span data-ttu-id="0bd61-127">この要素を記述するスキーマは、インストールされているクライアント アクセス サーバーの役割を持つ MicrosoftExchange Server 2007 を実行しているコンピューターの/EWS/ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="0bd61-127">The schema that describes this element is located in the /EWS/ directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="0bd61-128">要素情報</span><span class="sxs-lookup"><span data-stu-id="0bd61-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0bd61-129">名前空間</span><span class="sxs-lookup"><span data-stu-id="0bd61-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0bd61-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0bd61-130">Schema Name</span></span>  <br/> |<span data-ttu-id="0bd61-131">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="0bd61-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="0bd61-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0bd61-132">Validation File</span></span>  <br/> |<span data-ttu-id="0bd61-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0bd61-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0bd61-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="0bd61-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="0bd61-135">False</span><span class="sxs-lookup"><span data-stu-id="0bd61-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0bd61-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="0bd61-136">See also</span></span>



[<span data-ttu-id="0bd61-137">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="0bd61-137">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="0bd61-138">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="0bd61-138">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)


[<span data-ttu-id="0bd61-139">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="0bd61-139">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

