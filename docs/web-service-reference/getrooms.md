---
title: GetRooms
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetRooms
api_type:
- schema
ms.assetid: 82a737c7-da41-4777-8ad8-89851a0b602b
description: GetRooms 要素は、特定の会議室一覧内の部屋の一覧を取得する要求のルート要素です。
ms.openlocfilehash: 77fde5980a03d4c0509344933b0901cb21ab7197
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458594"
---
# <a name="getrooms"></a><span data-ttu-id="5cfc7-103">GetRooms</span><span class="sxs-lookup"><span data-stu-id="5cfc7-103">GetRooms</span></span>

<span data-ttu-id="5cfc7-104">**Getrooms**要素は、特定の会議室一覧内の部屋の一覧を取得する要求のルート要素です。</span><span class="sxs-lookup"><span data-stu-id="5cfc7-104">The **GetRooms** element is the root element in a request to get a list of rooms within a particular room list.</span></span> 
  
```XML
<GetRooms>
   <RoomList/>
</GetRooms>
```

 <span data-ttu-id="5cfc7-105">**GetRoomsType**</span><span class="sxs-lookup"><span data-stu-id="5cfc7-105">**GetRoomsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5cfc7-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="5cfc7-106">Attributes and elements</span></span>

<span data-ttu-id="5cfc7-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5cfc7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5cfc7-108">属性</span><span class="sxs-lookup"><span data-stu-id="5cfc7-108">Attributes</span></span>

<span data-ttu-id="5cfc7-109">なし。</span><span class="sxs-lookup"><span data-stu-id="5cfc7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5cfc7-110">子要素</span><span class="sxs-lookup"><span data-stu-id="5cfc7-110">Child elements</span></span>

|<span data-ttu-id="5cfc7-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="5cfc7-111">**Element**</span></span>|<span data-ttu-id="5cfc7-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="5cfc7-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5cfc7-113">RoomList</span><span class="sxs-lookup"><span data-stu-id="5cfc7-113">RoomList</span></span>](roomlist.md) <br/> |<span data-ttu-id="5cfc7-114">会議室の一覧を識別する電子メールアドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="5cfc7-114">Represents an e-mail address that identifies a list of meeting rooms</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5cfc7-115">親要素</span><span class="sxs-lookup"><span data-stu-id="5cfc7-115">Parent elements</span></span>

<span data-ttu-id="5cfc7-116">なし。</span><span class="sxs-lookup"><span data-stu-id="5cfc7-116">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="5cfc7-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="5cfc7-117">Text value</span></span>

<span data-ttu-id="5cfc7-118">なし。</span><span class="sxs-lookup"><span data-stu-id="5cfc7-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5cfc7-119">注釈</span><span class="sxs-lookup"><span data-stu-id="5cfc7-119">Remarks</span></span>

<span data-ttu-id="5cfc7-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="5cfc7-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5cfc7-121">要素の情報</span><span class="sxs-lookup"><span data-stu-id="5cfc7-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5cfc7-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="5cfc7-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5cfc7-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5cfc7-123">Schema Name</span></span>  <br/> |<span data-ttu-id="5cfc7-124">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="5cfc7-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5cfc7-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5cfc7-125">Validation File</span></span>  <br/> |<span data-ttu-id="5cfc7-126">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="5cfc7-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5cfc7-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="5cfc7-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="5cfc7-128">正しくない</span><span class="sxs-lookup"><span data-stu-id="5cfc7-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5cfc7-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="5cfc7-129">See also</span></span>



- [<span data-ttu-id="5cfc7-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="5cfc7-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

