---
title: Attendees
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 837bb372-39eb-48ae-9c09-0d2552511f93
description: 出席者の要素は、会議への招待の受信者を指定します。
ms.openlocfilehash: 22d88bb092b416c553144496e133680b53f5d30e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759461"
---
# <a name="attendees"></a><span data-ttu-id="57b31-103">Attendees</span><span class="sxs-lookup"><span data-stu-id="57b31-103">Attendees</span></span>

<span data-ttu-id="57b31-104">**出席者**の要素は、会議への招待の受信者を指定します。</span><span class="sxs-lookup"><span data-stu-id="57b31-104">The **Attendees** element specifies the recipients of an invitation to a meeting.</span></span> 
  
```XML
<Attendees>
    <EmailUser></EmailUser>
</Attendees>
```

 <span data-ttu-id="57b31-105">**ArrayOfEmailUsersType**</span><span class="sxs-lookup"><span data-stu-id="57b31-105">**ArrayOfEmailUsersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="57b31-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="57b31-106">Attributes and elements</span></span>

<span data-ttu-id="57b31-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="57b31-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="57b31-108">属性</span><span class="sxs-lookup"><span data-stu-id="57b31-108">Attributes</span></span>

<span data-ttu-id="57b31-109">なし。</span><span class="sxs-lookup"><span data-stu-id="57b31-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="57b31-110">子要素</span><span class="sxs-lookup"><span data-stu-id="57b31-110">Child elements</span></span>

|<span data-ttu-id="57b31-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="57b31-111">**Element**</span></span>|<span data-ttu-id="57b31-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="57b31-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="57b31-113">EmailUser</span><span class="sxs-lookup"><span data-stu-id="57b31-113">EmailUser</span></span>](emailuser.md) <br/> |<span data-ttu-id="57b31-114">電子メールの受信者または Active Directory の連絡先を指定します。</span><span class="sxs-lookup"><span data-stu-id="57b31-114">Specifies an email recipient or Active Directory contact.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="57b31-115">親要素</span><span class="sxs-lookup"><span data-stu-id="57b31-115">Parent elements</span></span>

|<span data-ttu-id="57b31-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="57b31-116">**Element**</span></span>|<span data-ttu-id="57b31-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="57b31-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="57b31-118">MeetingSuggestion</span><span class="sxs-lookup"><span data-stu-id="57b31-118">MeetingSuggestion</span></span>](meetingsuggestion.md) <br/> |<span data-ttu-id="57b31-119">提案された会議を指定します。</span><span class="sxs-lookup"><span data-stu-id="57b31-119">Specifies a proposed meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="57b31-120">備考</span><span class="sxs-lookup"><span data-stu-id="57b31-120">Remarks</span></span>

<span data-ttu-id="57b31-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="57b31-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="57b31-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="57b31-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="57b31-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="57b31-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="57b31-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="57b31-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="57b31-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="57b31-125">Schema Name</span></span>  <br/> |<span data-ttu-id="57b31-126">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="57b31-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="57b31-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="57b31-127">Validation File</span></span>  <br/> |<span data-ttu-id="57b31-128">types.xsd</span><span class="sxs-lookup"><span data-stu-id="57b31-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="57b31-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="57b31-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="57b31-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="57b31-130">See also</span></span>

- [<span data-ttu-id="57b31-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="57b31-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

