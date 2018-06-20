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
description: FreeBusyResponseArray 要素には、要求されたユーザーの利用可能時間情報と応答のステータスが含まれています。
ms.openlocfilehash: cc6022c28213667c40dc00b5627ed88c4f78e2f2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760600"
---
# <a name="freebusyresponsearray"></a><span data-ttu-id="cad59-103">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="cad59-103">FreeBusyResponseArray</span></span>

<span data-ttu-id="cad59-104">**FreeBusyResponseArray**要素には、要求されたユーザーの利用可能時間情報と応答のステータスが含まれています。</span><span class="sxs-lookup"><span data-stu-id="cad59-104">The **FreeBusyResponseArray** element contains the requested users' availability information and the response status.</span></span> 
  
[<span data-ttu-id="cad59-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="cad59-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="cad59-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="cad59-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
```xml
<FreeBusyResponseArray>
   <FreeBusyResponse>...</FreeBusyResponse>
</FreeBusyResponseArray>
```

 <span data-ttu-id="cad59-107">**ArrayOfFreeBusyResponse**</span><span class="sxs-lookup"><span data-stu-id="cad59-107">**ArrayOfFreeBusyResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cad59-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="cad59-108">Attributes and elements</span></span>

<span data-ttu-id="cad59-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="cad59-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cad59-110">属性</span><span class="sxs-lookup"><span data-stu-id="cad59-110">Attributes</span></span>

<span data-ttu-id="cad59-111">なし。</span><span class="sxs-lookup"><span data-stu-id="cad59-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cad59-112">子要素</span><span class="sxs-lookup"><span data-stu-id="cad59-112">Child elements</span></span>

|<span data-ttu-id="cad59-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="cad59-113">**Element**</span></span>|<span data-ttu-id="cad59-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="cad59-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cad59-115">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="cad59-115">FreeBusyResponse</span></span>](freebusyresponse.md) <br/> |<span data-ttu-id="cad59-116">1 つのメールボックス ユーザーと応答の状態の空き時間情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="cad59-116">Contains the free/busy information for a single mailbox user and the response status.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cad59-117">親要素</span><span class="sxs-lookup"><span data-stu-id="cad59-117">Parent elements</span></span>

|<span data-ttu-id="cad59-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="cad59-118">**Element**</span></span>|<span data-ttu-id="cad59-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="cad59-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cad59-120">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="cad59-120">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md) <br/> |<span data-ttu-id="cad59-121">ユーザーの利用可能時間情報を定義するか、会議の時刻の情報を提示するためのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="cad59-121">Contains the properties that define user availability information or suggested meeting time information.</span></span>  <br/> <span data-ttu-id="cad59-122">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="cad59-122">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="cad59-123">備考</span><span class="sxs-lookup"><span data-stu-id="cad59-123">Remarks</span></span>

<span data-ttu-id="cad59-124">空き時間情報が要求されない場合、この要素は GetUserAvailability の応答に含まれません。</span><span class="sxs-lookup"><span data-stu-id="cad59-124">This element is not included in a GetUserAvailability response if free/busy information is not requested.</span></span>
  
<span data-ttu-id="cad59-125">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="cad59-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cad59-126">要素情報</span><span class="sxs-lookup"><span data-stu-id="cad59-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cad59-127">名前空間</span><span class="sxs-lookup"><span data-stu-id="cad59-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="cad59-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="cad59-128">Schema Name</span></span>  <br/> |<span data-ttu-id="cad59-129">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="cad59-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="cad59-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="cad59-130">Validation File</span></span>  <br/> |<span data-ttu-id="cad59-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="cad59-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="cad59-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="cad59-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="cad59-133">False</span><span class="sxs-lookup"><span data-stu-id="cad59-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cad59-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="cad59-134">See also</span></span>



[<span data-ttu-id="cad59-135">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="cad59-135">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="cad59-136">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="cad59-136">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="cad59-137">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="cad59-137">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

