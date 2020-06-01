---
title: ルーム
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Rooms
api_type:
- schema
ms.assetid: 57b6079a-3d83-4429-861e-c551e9e1a991
description: ルーム要素は、会議室を表す1つまたは複数の要素のリストです。
ms.openlocfilehash: f8b60a9680f6abba459ebecc96613abfdd93766d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466186"
---
# <a name="rooms"></a><span data-ttu-id="21fa7-103">ルーム</span><span class="sxs-lookup"><span data-stu-id="21fa7-103">Rooms</span></span>

<span data-ttu-id="21fa7-104">**ルーム**要素は、会議室を表す1つまたは複数の要素のリストです。</span><span class="sxs-lookup"><span data-stu-id="21fa7-104">The **Rooms** element is a list of one or more elements that represent meeting rooms.</span></span> 
  
[<span data-ttu-id="21fa7-105">た getroomsresponse</span><span class="sxs-lookup"><span data-stu-id="21fa7-105">GetRoomsResponse</span></span>](getroomsresponse.md)
  
[<span data-ttu-id="21fa7-106">ルーム</span><span class="sxs-lookup"><span data-stu-id="21fa7-106">Rooms</span></span>](rooms.md)
  
```xml
<Rooms>   <Room/></Rooms>
```

 <span data-ttu-id="21fa7-107">**ArrayOfRoomsType**</span><span class="sxs-lookup"><span data-stu-id="21fa7-107">**ArrayOfRoomsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="21fa7-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="21fa7-108">Attributes and elements</span></span>

<span data-ttu-id="21fa7-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="21fa7-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="21fa7-110">属性</span><span class="sxs-lookup"><span data-stu-id="21fa7-110">Attributes</span></span>

<span data-ttu-id="21fa7-111">なし。</span><span class="sxs-lookup"><span data-stu-id="21fa7-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="21fa7-112">子要素</span><span class="sxs-lookup"><span data-stu-id="21fa7-112">Child elements</span></span>

|<span data-ttu-id="21fa7-113">**Element**</span><span class="sxs-lookup"><span data-stu-id="21fa7-113">**Element**</span></span>|<span data-ttu-id="21fa7-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="21fa7-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="21fa7-115">作る</span><span class="sxs-lookup"><span data-stu-id="21fa7-115">Room</span></span>](room.md) <br/> |<span data-ttu-id="21fa7-116">会議室を表す電子メールアドレスと表示名を定義します。</span><span class="sxs-lookup"><span data-stu-id="21fa7-116">Defines an e-mail address and display name that represents a meeting room.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="21fa7-117">親要素</span><span class="sxs-lookup"><span data-stu-id="21fa7-117">Parent elements</span></span>

|<span data-ttu-id="21fa7-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="21fa7-118">**Element**</span></span>|<span data-ttu-id="21fa7-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="21fa7-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="21fa7-120">た getroomsresponse</span><span class="sxs-lookup"><span data-stu-id="21fa7-120">GetRoomsResponse</span></span>](getroomsresponse.md) <br/> ||
   
## <a name="remarks"></a><span data-ttu-id="21fa7-121">注釈</span><span class="sxs-lookup"><span data-stu-id="21fa7-121">Remarks</span></span>

<span data-ttu-id="21fa7-122">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="21fa7-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="21fa7-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="21fa7-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="21fa7-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="21fa7-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="21fa7-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="21fa7-125">Schema Name</span></span>  <br/> |<span data-ttu-id="21fa7-126">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="21fa7-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="21fa7-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="21fa7-127">Validation File</span></span>  <br/> |<span data-ttu-id="21fa7-128">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="21fa7-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="21fa7-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="21fa7-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="21fa7-130">正しくない</span><span class="sxs-lookup"><span data-stu-id="21fa7-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="21fa7-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="21fa7-131">See also</span></span>



[<span data-ttu-id="21fa7-132">GetRooms 操作</span><span class="sxs-lookup"><span data-stu-id="21fa7-132">GetRooms operation</span></span>](getrooms-operation.md)


- [<span data-ttu-id="21fa7-133">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="21fa7-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

