---
title: Emailuser.displayname
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: dc8133ff-c34e-4921-bb56-06e79aee0a8a
description: Emailuser.displayname 要素は、電子メールの受信者を指定します。
ms.openlocfilehash: c090106a536f4f40908d364cc3c9c43f6fe42beb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456536"
---
# <a name="emailuser"></a><span data-ttu-id="f0f87-103">Emailuser.displayname</span><span class="sxs-lookup"><span data-stu-id="f0f87-103">EmailUser</span></span>

<span data-ttu-id="f0f87-104">**Emailuser.displayname**要素は、電子メールの受信者を指定します。</span><span class="sxs-lookup"><span data-stu-id="f0f87-104">The **EmailUser** element specifies an email recipient.</span></span> 
  
```XML
<EmailUser>
    <Name/>
    <UserId/>
</EmailUser>
```

 <span data-ttu-id="f0f87-105">**EmailUserType**</span><span class="sxs-lookup"><span data-stu-id="f0f87-105">**EmailUserType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f0f87-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="f0f87-106">Attributes and elements</span></span>

<span data-ttu-id="f0f87-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f0f87-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f0f87-108">属性</span><span class="sxs-lookup"><span data-stu-id="f0f87-108">Attributes</span></span>

<span data-ttu-id="f0f87-109">なし。</span><span class="sxs-lookup"><span data-stu-id="f0f87-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f0f87-110">子要素</span><span class="sxs-lookup"><span data-stu-id="f0f87-110">Child elements</span></span>

|<span data-ttu-id="f0f87-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="f0f87-111">**Element**</span></span>|<span data-ttu-id="f0f87-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="f0f87-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f0f87-113">Name (string)</span><span class="sxs-lookup"><span data-stu-id="f0f87-113">Name (string)</span></span>](name-string.md) <br/> |<span data-ttu-id="f0f87-114">検索絞り込み条件の名前またはキーまたはメールユーザーの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="f0f87-114">Specifies a search refiner name or key or the name of an email user.</span></span>  <br/> |
|[<span data-ttu-id="f0f87-115">UserId (文字列)</span><span class="sxs-lookup"><span data-stu-id="f0f87-115">UserId (string)</span></span>](userid-string.md) <br/> |<span data-ttu-id="f0f87-116">電子メールユーザーのユーザー識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="f0f87-116">Specifies the user identifier of an email user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f0f87-117">親要素</span><span class="sxs-lookup"><span data-stu-id="f0f87-117">Parent elements</span></span>

|<span data-ttu-id="f0f87-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="f0f87-118">**Element**</span></span>|<span data-ttu-id="f0f87-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="f0f87-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f0f87-120">Attendees</span><span class="sxs-lookup"><span data-stu-id="f0f87-120">Attendees</span></span>](attendees.md) <br/> |<span data-ttu-id="f0f87-121">会議への招待の受信者を指定します。</span><span class="sxs-lookup"><span data-stu-id="f0f87-121">Specifies the recipients of an invitation to a meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f0f87-122">注釈</span><span class="sxs-lookup"><span data-stu-id="f0f87-122">Remarks</span></span>

<span data-ttu-id="f0f87-123">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="f0f87-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f0f87-124">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="f0f87-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f0f87-125">要素の情報</span><span class="sxs-lookup"><span data-stu-id="f0f87-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f0f87-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="f0f87-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f0f87-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f0f87-127">Schema Name</span></span>  <br/> |<span data-ttu-id="f0f87-128">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="f0f87-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="f0f87-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f0f87-129">Validation File</span></span>  <br/> |<span data-ttu-id="f0f87-130">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="f0f87-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="f0f87-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="f0f87-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="f0f87-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="f0f87-132">See also</span></span>



- [<span data-ttu-id="f0f87-133">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="f0f87-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

