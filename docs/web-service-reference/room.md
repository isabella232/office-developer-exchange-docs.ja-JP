---
title: ルーム
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Room
api_type:
- schema
ms.assetid: a2cde8b8-2d31-4ebf-8171-f4dfd650d079
description: ルームの要素は、会議室を表します。
ms.openlocfilehash: e064a458b5a9265fc9dad63c87c641eaf47d7062
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833242"
---
# <a name="room"></a><span data-ttu-id="d9410-103">ルーム</span><span class="sxs-lookup"><span data-stu-id="d9410-103">Room</span></span>

<span data-ttu-id="d9410-104">**ルーム**の要素は、会議室を表します。</span><span class="sxs-lookup"><span data-stu-id="d9410-104">The **Room** element represents a meeting room.</span></span> 
  
[<span data-ttu-id="d9410-105">ルーム</span><span class="sxs-lookup"><span data-stu-id="d9410-105">Rooms</span></span>](rooms.md)
  
[<span data-ttu-id="d9410-106">ルーム</span><span class="sxs-lookup"><span data-stu-id="d9410-106">Room</span></span>](room.md)
  
```XML
<Room>
   <Id/>
</Room>
```

 <span data-ttu-id="d9410-107">**RoomType**</span><span class="sxs-lookup"><span data-stu-id="d9410-107">**RoomType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d9410-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="d9410-108">Attributes and elements</span></span>

<span data-ttu-id="d9410-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d9410-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d9410-110">属性</span><span class="sxs-lookup"><span data-stu-id="d9410-110">Attributes</span></span>

<span data-ttu-id="d9410-111">なし。</span><span class="sxs-lookup"><span data-stu-id="d9410-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d9410-112">子要素</span><span class="sxs-lookup"><span data-stu-id="d9410-112">Child elements</span></span>

|<span data-ttu-id="d9410-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="d9410-113">**Element**</span></span>|<span data-ttu-id="d9410-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="d9410-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d9410-115">Id (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="d9410-115">Id (EmailAddressType)</span></span>](id-emailaddresstype.md) <br/> |<span data-ttu-id="d9410-116">電子メール アドレスが含まれている id および表示名を会議室を表します。</span><span class="sxs-lookup"><span data-stu-id="d9410-116">An identifier that contains an email address and display name that represents the meeting room.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d9410-117">親要素</span><span class="sxs-lookup"><span data-stu-id="d9410-117">Parent elements</span></span>

|<span data-ttu-id="d9410-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="d9410-118">**Element**</span></span>|<span data-ttu-id="d9410-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="d9410-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d9410-120">ルーム</span><span class="sxs-lookup"><span data-stu-id="d9410-120">Rooms</span></span>](rooms.md) <br/> |<span data-ttu-id="d9410-121">会議室が同じ建物内に配置されているなど、共通の機能に関連付けられているのリストを定義します。</span><span class="sxs-lookup"><span data-stu-id="d9410-121">Defines a list of meeting rooms associated with a common feature, such as being located in the same building.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d9410-122">備考</span><span class="sxs-lookup"><span data-stu-id="d9410-122">Remarks</span></span>

<span data-ttu-id="d9410-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="d9410-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d9410-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="d9410-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d9410-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="d9410-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d9410-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d9410-126">Schema Name</span></span>  <br/> |<span data-ttu-id="d9410-127">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="d9410-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="d9410-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d9410-128">Validation File</span></span>  <br/> |<span data-ttu-id="d9410-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d9410-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d9410-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d9410-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="d9410-131">False</span><span class="sxs-lookup"><span data-stu-id="d9410-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d9410-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="d9410-132">See also</span></span>



[<span data-ttu-id="d9410-133">GetRooms 操作</span><span class="sxs-lookup"><span data-stu-id="d9410-133">GetRooms operation</span></span>](getrooms-operation.md)


- [<span data-ttu-id="d9410-134">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="d9410-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

