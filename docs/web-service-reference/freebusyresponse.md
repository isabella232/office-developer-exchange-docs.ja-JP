---
title: FreeBusyResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FreeBusyResponse
api_type:
- schema
ms.assetid: 3038d106-9ac9-4ac7-bb43-96c783edbef5
description: FreeBusyResponse 要素には、1つのメールボックスユーザーの空き時間情報が含まれています。
ms.openlocfilehash: 45a3e12756f3cbf29b76b442f7103abc5fb9a833
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461927"
---
# <a name="freebusyresponse"></a><span data-ttu-id="a5122-103">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="a5122-103">FreeBusyResponse</span></span>

<span data-ttu-id="a5122-104">**FreeBusyResponse**要素には、1つのメールボックスユーザーの空き時間情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a5122-104">The **FreeBusyResponse** element contains the free/busy information for a single mailbox user.</span></span> 
  
[<span data-ttu-id="a5122-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="a5122-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="a5122-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="a5122-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="a5122-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="a5122-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
```xml
<FreeBusyResponse>
   <ResponseMessage>...</ResponseMessage>
   <FreeBusyView>...</FreeBusyView>
</FreeBusyResponse>
```

 <span data-ttu-id="a5122-108">**FreeBusyResponseType**</span><span class="sxs-lookup"><span data-stu-id="a5122-108">**FreeBusyResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a5122-109">属性と要素</span><span class="sxs-lookup"><span data-stu-id="a5122-109">Attributes and elements</span></span>

<span data-ttu-id="a5122-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a5122-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a5122-111">属性</span><span class="sxs-lookup"><span data-stu-id="a5122-111">Attributes</span></span>

<span data-ttu-id="a5122-112">なし。</span><span class="sxs-lookup"><span data-stu-id="a5122-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a5122-113">子要素</span><span class="sxs-lookup"><span data-stu-id="a5122-113">Child elements</span></span>

|<span data-ttu-id="a5122-114">**Element**</span><span class="sxs-lookup"><span data-stu-id="a5122-114">**Element**</span></span>|<span data-ttu-id="a5122-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="a5122-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a5122-116">ResponseMessage</span><span class="sxs-lookup"><span data-stu-id="a5122-116">ResponseMessage</span></span>](responsemessage.md) <br/> |<span data-ttu-id="a5122-117">応答状態に関する説明情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="a5122-117">Provides descriptive information about the response status.</span></span>  <br/> |
|[<span data-ttu-id="a5122-118">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="a5122-118">FreeBusyView</span></span>](freebusyview.md) <br/> |<span data-ttu-id="a5122-119">特定のユーザーの空き時間情報が保存されています。</span><span class="sxs-lookup"><span data-stu-id="a5122-119">Contains availability information for a specific user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a5122-120">親要素</span><span class="sxs-lookup"><span data-stu-id="a5122-120">Parent elements</span></span>

|<span data-ttu-id="a5122-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="a5122-121">**Element**</span></span>|<span data-ttu-id="a5122-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="a5122-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a5122-123">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="a5122-123">FreeBusyResponseArray</span></span>](freebusyresponsearray.md) <br/> |<span data-ttu-id="a5122-124">要求されたユーザーの空き時間情報と応答の状態を含みます。</span><span class="sxs-lookup"><span data-stu-id="a5122-124">Contains the requested users' availability information and the response status.</span></span>  <br/> <span data-ttu-id="a5122-125">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a5122-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a5122-126">注釈</span><span class="sxs-lookup"><span data-stu-id="a5122-126">Remarks</span></span>

<span data-ttu-id="a5122-127">この要素は、空き時間情報が要求されない場合、GetUserAvailability 応答には含まれません。</span><span class="sxs-lookup"><span data-stu-id="a5122-127">This element is not included in a GetUserAvailability response if free/busy information is not requested.</span></span>
  
<span data-ttu-id="a5122-128">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="a5122-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a5122-129">要素の情報</span><span class="sxs-lookup"><span data-stu-id="a5122-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a5122-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="a5122-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a5122-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a5122-131">Schema Name</span></span>  <br/> |<span data-ttu-id="a5122-132">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="a5122-132">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a5122-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a5122-133">Validation File</span></span>  <br/> |<span data-ttu-id="a5122-134">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="a5122-134">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a5122-135">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="a5122-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="a5122-136">正しくない</span><span class="sxs-lookup"><span data-stu-id="a5122-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a5122-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="a5122-137">See also</span></span>



[<span data-ttu-id="a5122-138">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="a5122-138">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="a5122-139">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="a5122-139">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="a5122-140">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="a5122-140">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

