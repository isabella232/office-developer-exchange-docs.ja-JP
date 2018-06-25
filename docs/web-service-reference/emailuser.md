---
title: EmailUser
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: dc8133ff-c34e-4921-bb56-06e79aee0a8a
description: EmailUser 要素は、電子メールの受信者を指定します。
ms.openlocfilehash: e724b3996d37a42527ec1183cef9bb6b312b8c93
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760266"
---
# <a name="emailuser"></a><span data-ttu-id="931ba-103">EmailUser</span><span class="sxs-lookup"><span data-stu-id="931ba-103">EmailUser</span></span>

<span data-ttu-id="931ba-104">**EmailUser**要素は、電子メールの受信者を指定します。</span><span class="sxs-lookup"><span data-stu-id="931ba-104">The **EmailUser** element specifies an email recipient.</span></span> 
  
```XML
<EmailUser>
    <Name/>
    <UserId/>
</EmailUser>
```

 <span data-ttu-id="931ba-105">**EmailUserType**</span><span class="sxs-lookup"><span data-stu-id="931ba-105">**EmailUserType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="931ba-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="931ba-106">Attributes and elements</span></span>

<span data-ttu-id="931ba-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="931ba-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="931ba-108">属性</span><span class="sxs-lookup"><span data-stu-id="931ba-108">Attributes</span></span>

<span data-ttu-id="931ba-109">なし。</span><span class="sxs-lookup"><span data-stu-id="931ba-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="931ba-110">子要素</span><span class="sxs-lookup"><span data-stu-id="931ba-110">Child elements</span></span>

|<span data-ttu-id="931ba-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="931ba-111">**Element**</span></span>|<span data-ttu-id="931ba-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="931ba-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="931ba-113">名 (文字列)</span><span class="sxs-lookup"><span data-stu-id="931ba-113">Name (string)</span></span>](name-string.md) <br/> |<span data-ttu-id="931ba-114">検索の絞り込み条件の名前またはキー、または、電子メール ユーザーの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="931ba-114">Specifies a search refiner name or key or the name of an email user.</span></span>  <br/> |
|[<span data-ttu-id="931ba-115">ユーザー Id (文字列)</span><span class="sxs-lookup"><span data-stu-id="931ba-115">UserId (string)</span></span>](userid-string.md) <br/> |<span data-ttu-id="931ba-116">メール ユーザーのユーザー識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="931ba-116">Specifies the user identifier of an email user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="931ba-117">親要素</span><span class="sxs-lookup"><span data-stu-id="931ba-117">Parent elements</span></span>

|<span data-ttu-id="931ba-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="931ba-118">**Element**</span></span>|<span data-ttu-id="931ba-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="931ba-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="931ba-120">Attendees</span><span class="sxs-lookup"><span data-stu-id="931ba-120">Attendees</span></span>](attendees.md) <br/> |<span data-ttu-id="931ba-121">会議への招待の受信者を指定します。</span><span class="sxs-lookup"><span data-stu-id="931ba-121">Specifies the recipients of an invitation to a meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="931ba-122">備考</span><span class="sxs-lookup"><span data-stu-id="931ba-122">Remarks</span></span>

<span data-ttu-id="931ba-123">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="931ba-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="931ba-124">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="931ba-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="931ba-125">要素情報</span><span class="sxs-lookup"><span data-stu-id="931ba-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="931ba-126">名前空間</span><span class="sxs-lookup"><span data-stu-id="931ba-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="931ba-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="931ba-127">Schema Name</span></span>  <br/> |<span data-ttu-id="931ba-128">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="931ba-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="931ba-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="931ba-129">Validation File</span></span>  <br/> |<span data-ttu-id="931ba-130">types.xsd</span><span class="sxs-lookup"><span data-stu-id="931ba-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="931ba-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="931ba-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="931ba-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="931ba-132">See also</span></span>



- [<span data-ttu-id="931ba-133">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="931ba-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

