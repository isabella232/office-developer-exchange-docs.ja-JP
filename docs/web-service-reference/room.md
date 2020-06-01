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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460534"
---
# <a name="room"></a><span data-ttu-id="ff7ab-103">Room</span><span class="sxs-lookup"><span data-stu-id="ff7ab-103">Room</span></span>

<span data-ttu-id="ff7ab-104">**Room**要素は、会議室を表します。</span><span class="sxs-lookup"><span data-stu-id="ff7ab-104">The **Room** element represents a meeting room.</span></span> 
  
[<span data-ttu-id="ff7ab-105">ルーム</span><span class="sxs-lookup"><span data-stu-id="ff7ab-105">Rooms</span></span>](rooms.md)
  
[<span data-ttu-id="ff7ab-106">作る</span><span class="sxs-lookup"><span data-stu-id="ff7ab-106">Room</span></span>](room.md)
  
```XML
<Room>
   <Id/>
</Room>
```

 <span data-ttu-id="ff7ab-107">**RoomType**</span><span class="sxs-lookup"><span data-stu-id="ff7ab-107">**RoomType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ff7ab-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="ff7ab-108">Attributes and elements</span></span>

<span data-ttu-id="ff7ab-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ff7ab-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ff7ab-110">属性</span><span class="sxs-lookup"><span data-stu-id="ff7ab-110">Attributes</span></span>

<span data-ttu-id="ff7ab-111">なし。</span><span class="sxs-lookup"><span data-stu-id="ff7ab-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ff7ab-112">子要素</span><span class="sxs-lookup"><span data-stu-id="ff7ab-112">Child elements</span></span>

|<span data-ttu-id="ff7ab-113">**Element**</span><span class="sxs-lookup"><span data-stu-id="ff7ab-113">**Element**</span></span>|<span data-ttu-id="ff7ab-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="ff7ab-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ff7ab-115">Id (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="ff7ab-115">Id (EmailAddressType)</span></span>](id-emailaddresstype.md) <br/> |<span data-ttu-id="ff7ab-116">会議室を表す電子メールアドレスと表示名を含む識別子。</span><span class="sxs-lookup"><span data-stu-id="ff7ab-116">An identifier that contains an email address and display name that represents the meeting room.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ff7ab-117">親要素</span><span class="sxs-lookup"><span data-stu-id="ff7ab-117">Parent elements</span></span>

|<span data-ttu-id="ff7ab-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="ff7ab-118">**Element**</span></span>|<span data-ttu-id="ff7ab-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="ff7ab-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ff7ab-120">ルーム</span><span class="sxs-lookup"><span data-stu-id="ff7ab-120">Rooms</span></span>](rooms.md) <br/> |<span data-ttu-id="ff7ab-121">同じ建物内にあるなど、共通の機能に関連付けられている会議室のリストを定義します。</span><span class="sxs-lookup"><span data-stu-id="ff7ab-121">Defines a list of meeting rooms associated with a common feature, such as being located in the same building.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ff7ab-122">注釈</span><span class="sxs-lookup"><span data-stu-id="ff7ab-122">Remarks</span></span>

<span data-ttu-id="ff7ab-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="ff7ab-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ff7ab-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="ff7ab-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ff7ab-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="ff7ab-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ff7ab-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ff7ab-126">Schema Name</span></span>  <br/> |<span data-ttu-id="ff7ab-127">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="ff7ab-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="ff7ab-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ff7ab-128">Validation File</span></span>  <br/> |<span data-ttu-id="ff7ab-129">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="ff7ab-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ff7ab-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="ff7ab-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="ff7ab-131">正しくない</span><span class="sxs-lookup"><span data-stu-id="ff7ab-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ff7ab-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="ff7ab-132">See also</span></span>



[<span data-ttu-id="ff7ab-133">GetRooms 操作</span><span class="sxs-lookup"><span data-stu-id="ff7ab-133">GetRooms operation</span></span>](getrooms-operation.md)


- [<span data-ttu-id="ff7ab-134">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="ff7ab-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

