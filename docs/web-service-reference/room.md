---
title: Room
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
description: Room 要素は、会議室を表します。
ms.openlocfilehash: 3d5d587853e435016fdff6b9d268892a35fea825
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460534"
---
# <a name="room"></a><span data-ttu-id="5a7f2-103">Room</span><span class="sxs-lookup"><span data-stu-id="5a7f2-103">Room</span></span>

<span data-ttu-id="5a7f2-104">**Room**要素は、会議室を表します。</span><span class="sxs-lookup"><span data-stu-id="5a7f2-104">The **Room** element represents a meeting room.</span></span> 
  
[<span data-ttu-id="5a7f2-105">ルーム</span><span class="sxs-lookup"><span data-stu-id="5a7f2-105">Rooms</span></span>](rooms.md)
  
[<span data-ttu-id="5a7f2-106">作る</span><span class="sxs-lookup"><span data-stu-id="5a7f2-106">Room</span></span>](room.md)
  
```XML
<Room>
   <Id/>
</Room>
```

 <span data-ttu-id="5a7f2-107">**RoomType**</span><span class="sxs-lookup"><span data-stu-id="5a7f2-107">**RoomType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5a7f2-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="5a7f2-108">Attributes and elements</span></span>

<span data-ttu-id="5a7f2-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5a7f2-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5a7f2-110">属性</span><span class="sxs-lookup"><span data-stu-id="5a7f2-110">Attributes</span></span>

<span data-ttu-id="5a7f2-111">なし。</span><span class="sxs-lookup"><span data-stu-id="5a7f2-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5a7f2-112">子要素</span><span class="sxs-lookup"><span data-stu-id="5a7f2-112">Child elements</span></span>

|<span data-ttu-id="5a7f2-113">**Element**</span><span class="sxs-lookup"><span data-stu-id="5a7f2-113">**Element**</span></span>|<span data-ttu-id="5a7f2-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="5a7f2-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5a7f2-115">Id (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="5a7f2-115">Id (EmailAddressType)</span></span>](id-emailaddresstype.md) <br/> |<span data-ttu-id="5a7f2-116">会議室を表す電子メールアドレスと表示名を含む識別子。</span><span class="sxs-lookup"><span data-stu-id="5a7f2-116">An identifier that contains an email address and display name that represents the meeting room.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5a7f2-117">親要素</span><span class="sxs-lookup"><span data-stu-id="5a7f2-117">Parent elements</span></span>

|<span data-ttu-id="5a7f2-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="5a7f2-118">**Element**</span></span>|<span data-ttu-id="5a7f2-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="5a7f2-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5a7f2-120">ルーム</span><span class="sxs-lookup"><span data-stu-id="5a7f2-120">Rooms</span></span>](rooms.md) <br/> |<span data-ttu-id="5a7f2-121">同じ建物内にあるなど、共通の機能に関連付けられている会議室のリストを定義します。</span><span class="sxs-lookup"><span data-stu-id="5a7f2-121">Defines a list of meeting rooms associated with a common feature, such as being located in the same building.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5a7f2-122">注釈</span><span class="sxs-lookup"><span data-stu-id="5a7f2-122">Remarks</span></span>

<span data-ttu-id="5a7f2-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="5a7f2-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5a7f2-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="5a7f2-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5a7f2-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="5a7f2-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5a7f2-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5a7f2-126">Schema Name</span></span>  <br/> |<span data-ttu-id="5a7f2-127">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="5a7f2-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="5a7f2-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5a7f2-128">Validation File</span></span>  <br/> |<span data-ttu-id="5a7f2-129">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="5a7f2-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5a7f2-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="5a7f2-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="5a7f2-131">正しくない</span><span class="sxs-lookup"><span data-stu-id="5a7f2-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5a7f2-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="5a7f2-132">See also</span></span>



[<span data-ttu-id="5a7f2-133">GetRooms 操作</span><span class="sxs-lookup"><span data-stu-id="5a7f2-133">GetRooms operation</span></span>](getrooms-operation.md)


- [<span data-ttu-id="5a7f2-134">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="5a7f2-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

