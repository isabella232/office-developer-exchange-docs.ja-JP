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
description: FreeBusyResponse 要素には、単一のメールボックスのユーザーの空き時間情報が含まれています。
ms.openlocfilehash: 73e3972bb53d6bf59e5156098bad06bcde5f0155
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760597"
---
# <a name="freebusyresponse"></a><span data-ttu-id="2303f-103">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="2303f-103">FreeBusyResponse</span></span>

<span data-ttu-id="2303f-104">**FreeBusyResponse**要素には、単一のメールボックスのユーザーの空き時間情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="2303f-104">The **FreeBusyResponse** element contains the free/busy information for a single mailbox user.</span></span> 
  
[<span data-ttu-id="2303f-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="2303f-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="2303f-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="2303f-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="2303f-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="2303f-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
```xml
<FreeBusyResponse>
   <ResponseMessage>...</ResponseMessage>
   <FreeBusyView>...</FreeBusyView>
</FreeBusyResponse>
```

 <span data-ttu-id="2303f-108">**FreeBusyResponseType**</span><span class="sxs-lookup"><span data-stu-id="2303f-108">**FreeBusyResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2303f-109">属性および要素</span><span class="sxs-lookup"><span data-stu-id="2303f-109">Attributes and elements</span></span>

<span data-ttu-id="2303f-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2303f-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2303f-111">属性</span><span class="sxs-lookup"><span data-stu-id="2303f-111">Attributes</span></span>

<span data-ttu-id="2303f-112">なし。</span><span class="sxs-lookup"><span data-stu-id="2303f-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2303f-113">子要素</span><span class="sxs-lookup"><span data-stu-id="2303f-113">Child elements</span></span>

|<span data-ttu-id="2303f-114">**要素**</span><span class="sxs-lookup"><span data-stu-id="2303f-114">**Element**</span></span>|<span data-ttu-id="2303f-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="2303f-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2303f-116">ResponseMessage</span><span class="sxs-lookup"><span data-stu-id="2303f-116">ResponseMessage</span></span>](responsemessage.md) <br/> |<span data-ttu-id="2303f-117">応答ステータスに関する説明情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="2303f-117">Provides descriptive information about the response status.</span></span>  <br/> |
|[<span data-ttu-id="2303f-118">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="2303f-118">FreeBusyView</span></span>](freebusyview.md) <br/> |<span data-ttu-id="2303f-119">特定のユーザーの利用可能時間情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="2303f-119">Contains availability information for a specific user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2303f-120">親要素</span><span class="sxs-lookup"><span data-stu-id="2303f-120">Parent elements</span></span>

|<span data-ttu-id="2303f-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="2303f-121">**Element**</span></span>|<span data-ttu-id="2303f-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="2303f-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2303f-123">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="2303f-123">FreeBusyResponseArray</span></span>](freebusyresponsearray.md) <br/> |<span data-ttu-id="2303f-124">要求されたユーザーの利用可能時間情報と応答のステータスが含まれています。</span><span class="sxs-lookup"><span data-stu-id="2303f-124">Contains the requested users' availability information and the response status.</span></span>  <br/> <span data-ttu-id="2303f-125">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="2303f-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2303f-126">備考</span><span class="sxs-lookup"><span data-stu-id="2303f-126">Remarks</span></span>

<span data-ttu-id="2303f-127">空き時間情報が要求されない場合、この要素は GetUserAvailability の応答に含まれません。</span><span class="sxs-lookup"><span data-stu-id="2303f-127">This element is not included in a GetUserAvailability response if free/busy information is not requested.</span></span>
  
<span data-ttu-id="2303f-128">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="2303f-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2303f-129">要素情報</span><span class="sxs-lookup"><span data-stu-id="2303f-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2303f-130">名前空間</span><span class="sxs-lookup"><span data-stu-id="2303f-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2303f-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2303f-131">Schema Name</span></span>  <br/> |<span data-ttu-id="2303f-132">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="2303f-132">Messages schema</span></span>  <br/> |
|<span data-ttu-id="2303f-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2303f-133">Validation File</span></span>  <br/> |<span data-ttu-id="2303f-134">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="2303f-134">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2303f-135">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="2303f-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="2303f-136">False</span><span class="sxs-lookup"><span data-stu-id="2303f-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2303f-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="2303f-137">See also</span></span>



[<span data-ttu-id="2303f-138">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="2303f-138">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="2303f-139">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="2303f-139">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="2303f-140">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="2303f-140">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

