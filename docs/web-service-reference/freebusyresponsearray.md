---
title: FreeBusyResponseArray
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FreeBusyResponseArray
api_type:
- schema
ms.assetid: 5592a37e-cf4b-4643-8a2a-fa58c40345b9
description: FreeBusyResponseArray 要素には、要求されたユーザーの空き時間情報と応答の状態が含まれています。
ms.openlocfilehash: b45938c19b76a377fca125fb6a19f9d712718db6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457810"
---
# <a name="freebusyresponsearray"></a><span data-ttu-id="1f710-103">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="1f710-103">FreeBusyResponseArray</span></span>

<span data-ttu-id="1f710-104">**FreeBusyResponseArray**要素には、要求されたユーザーの空き時間情報と応答の状態が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1f710-104">The **FreeBusyResponseArray** element contains the requested users' availability information and the response status.</span></span> 
  
[<span data-ttu-id="1f710-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="1f710-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="1f710-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="1f710-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
```xml
<FreeBusyResponseArray>
   <FreeBusyResponse>...</FreeBusyResponse>
</FreeBusyResponseArray>
```

 <span data-ttu-id="1f710-107">**ArrayOfFreeBusyResponse**</span><span class="sxs-lookup"><span data-stu-id="1f710-107">**ArrayOfFreeBusyResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1f710-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="1f710-108">Attributes and elements</span></span>

<span data-ttu-id="1f710-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1f710-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1f710-110">属性</span><span class="sxs-lookup"><span data-stu-id="1f710-110">Attributes</span></span>

<span data-ttu-id="1f710-111">なし。</span><span class="sxs-lookup"><span data-stu-id="1f710-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1f710-112">子要素</span><span class="sxs-lookup"><span data-stu-id="1f710-112">Child elements</span></span>

|<span data-ttu-id="1f710-113">**Element**</span><span class="sxs-lookup"><span data-stu-id="1f710-113">**Element**</span></span>|<span data-ttu-id="1f710-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="1f710-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1f710-115">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="1f710-115">FreeBusyResponse</span></span>](freebusyresponse.md) <br/> |<span data-ttu-id="1f710-116">1つのメールボックスユーザーの空き時間情報と、応答の状態を格納します。</span><span class="sxs-lookup"><span data-stu-id="1f710-116">Contains the free/busy information for a single mailbox user and the response status.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1f710-117">親要素</span><span class="sxs-lookup"><span data-stu-id="1f710-117">Parent elements</span></span>

|<span data-ttu-id="1f710-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="1f710-118">**Element**</span></span>|<span data-ttu-id="1f710-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="1f710-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1f710-120">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="1f710-120">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md) <br/> |<span data-ttu-id="1f710-121">ユーザーの空き時間情報または推奨される会議時刻情報を定義するプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="1f710-121">Contains the properties that define user availability information or suggested meeting time information.</span></span>  <br/> <span data-ttu-id="1f710-122">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1f710-122">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1f710-123">注釈</span><span class="sxs-lookup"><span data-stu-id="1f710-123">Remarks</span></span>

<span data-ttu-id="1f710-124">この要素は、空き時間情報が要求されない場合、GetUserAvailability 応答には含まれません。</span><span class="sxs-lookup"><span data-stu-id="1f710-124">This element is not included in a GetUserAvailability response if free/busy information is not requested.</span></span>
  
<span data-ttu-id="1f710-125">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="1f710-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1f710-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="1f710-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1f710-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="1f710-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1f710-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1f710-128">Schema Name</span></span>  <br/> |<span data-ttu-id="1f710-129">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="1f710-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1f710-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1f710-130">Validation File</span></span>  <br/> |<span data-ttu-id="1f710-131">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="1f710-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1f710-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="1f710-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="1f710-133">正しくない</span><span class="sxs-lookup"><span data-stu-id="1f710-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1f710-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="1f710-134">See also</span></span>



[<span data-ttu-id="1f710-135">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="1f710-135">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="1f710-136">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="1f710-136">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="1f710-137">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="1f710-137">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

