---
title: 出席者
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 837bb372-39eb-48ae-9c09-0d2552511f93
description: 出席者要素は、会議への招待の受信者を指定します。
ms.openlocfilehash: 3a63bdf7e49309697ac503be5f4c95eb805b9635
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460331"
---
# <a name="attendees"></a><span data-ttu-id="4bb0d-103">出席者</span><span class="sxs-lookup"><span data-stu-id="4bb0d-103">Attendees</span></span>

<span data-ttu-id="4bb0d-104">**出席者**要素は、会議への招待の受信者を指定します。</span><span class="sxs-lookup"><span data-stu-id="4bb0d-104">The **Attendees** element specifies the recipients of an invitation to a meeting.</span></span> 
  
```XML
<Attendees>
    <EmailUser></EmailUser>
</Attendees>
```

 <span data-ttu-id="4bb0d-105">**ArrayOfEmailUsersType**</span><span class="sxs-lookup"><span data-stu-id="4bb0d-105">**ArrayOfEmailUsersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4bb0d-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="4bb0d-106">Attributes and elements</span></span>

<span data-ttu-id="4bb0d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4bb0d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4bb0d-108">属性</span><span class="sxs-lookup"><span data-stu-id="4bb0d-108">Attributes</span></span>

<span data-ttu-id="4bb0d-109">なし。</span><span class="sxs-lookup"><span data-stu-id="4bb0d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4bb0d-110">子要素</span><span class="sxs-lookup"><span data-stu-id="4bb0d-110">Child elements</span></span>

|<span data-ttu-id="4bb0d-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="4bb0d-111">**Element**</span></span>|<span data-ttu-id="4bb0d-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="4bb0d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4bb0d-113">Emailuser.displayname</span><span class="sxs-lookup"><span data-stu-id="4bb0d-113">EmailUser</span></span>](emailuser.md) <br/> |<span data-ttu-id="4bb0d-114">電子メール受信者または Active Directory の連絡先を指定します。</span><span class="sxs-lookup"><span data-stu-id="4bb0d-114">Specifies an email recipient or Active Directory contact.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4bb0d-115">親要素</span><span class="sxs-lookup"><span data-stu-id="4bb0d-115">Parent elements</span></span>

|<span data-ttu-id="4bb0d-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="4bb0d-116">**Element**</span></span>|<span data-ttu-id="4bb0d-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="4bb0d-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4bb0d-118">MeetingSuggestion</span><span class="sxs-lookup"><span data-stu-id="4bb0d-118">MeetingSuggestion</span></span>](meetingsuggestion.md) <br/> |<span data-ttu-id="4bb0d-119">提案された会議を指定します。</span><span class="sxs-lookup"><span data-stu-id="4bb0d-119">Specifies a proposed meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4bb0d-120">注釈</span><span class="sxs-lookup"><span data-stu-id="4bb0d-120">Remarks</span></span>

<span data-ttu-id="4bb0d-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="4bb0d-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4bb0d-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="4bb0d-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4bb0d-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="4bb0d-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4bb0d-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="4bb0d-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4bb0d-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4bb0d-125">Schema Name</span></span>  <br/> |<span data-ttu-id="4bb0d-126">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="4bb0d-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="4bb0d-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4bb0d-127">Validation File</span></span>  <br/> |<span data-ttu-id="4bb0d-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="4bb0d-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="4bb0d-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="4bb0d-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="4bb0d-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="4bb0d-130">See also</span></span>

- [<span data-ttu-id="4bb0d-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="4bb0d-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

