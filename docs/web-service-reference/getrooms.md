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
description: GetRooms 要素は、特定の会議室の一覧内の会議室の一覧を取得する要求のルート要素です。
ms.openlocfilehash: a787097752cfeee9489e5f118549c2d939ba4c9a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760851"
---
# <a name="getrooms"></a><span data-ttu-id="aaa25-103">GetRooms</span><span class="sxs-lookup"><span data-stu-id="aaa25-103">GetRooms</span></span>

<span data-ttu-id="aaa25-104">**GetRooms**要素は、特定の会議室の一覧内の会議室の一覧を取得する要求のルート要素です。</span><span class="sxs-lookup"><span data-stu-id="aaa25-104">The **GetRooms** element is the root element in a request to get a list of rooms within a particular room list.</span></span> 
  
```XML
<GetRooms>
   <RoomList/>
</GetRooms>
```

 <span data-ttu-id="aaa25-105">**GetRoomsType**</span><span class="sxs-lookup"><span data-stu-id="aaa25-105">**GetRoomsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="aaa25-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="aaa25-106">Attributes and elements</span></span>

<span data-ttu-id="aaa25-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="aaa25-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="aaa25-108">属性</span><span class="sxs-lookup"><span data-stu-id="aaa25-108">Attributes</span></span>

<span data-ttu-id="aaa25-109">なし。</span><span class="sxs-lookup"><span data-stu-id="aaa25-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="aaa25-110">子要素</span><span class="sxs-lookup"><span data-stu-id="aaa25-110">Child elements</span></span>

|<span data-ttu-id="aaa25-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="aaa25-111">**Element**</span></span>|<span data-ttu-id="aaa25-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="aaa25-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aaa25-113">RoomList</span><span class="sxs-lookup"><span data-stu-id="aaa25-113">RoomList</span></span>](roomlist.md) <br/> |<span data-ttu-id="aaa25-114">会議室の一覧を識別する電子メール アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="aaa25-114">Represents an e-mail address that identifies a list of meeting rooms</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="aaa25-115">親要素</span><span class="sxs-lookup"><span data-stu-id="aaa25-115">Parent elements</span></span>

<span data-ttu-id="aaa25-116">なし。</span><span class="sxs-lookup"><span data-stu-id="aaa25-116">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="aaa25-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="aaa25-117">Text value</span></span>

<span data-ttu-id="aaa25-118">なし。</span><span class="sxs-lookup"><span data-stu-id="aaa25-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="aaa25-119">備考</span><span class="sxs-lookup"><span data-stu-id="aaa25-119">Remarks</span></span>

<span data-ttu-id="aaa25-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="aaa25-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="aaa25-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="aaa25-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="aaa25-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="aaa25-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="aaa25-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="aaa25-123">Schema Name</span></span>  <br/> |<span data-ttu-id="aaa25-124">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="aaa25-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="aaa25-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="aaa25-125">Validation File</span></span>  <br/> |<span data-ttu-id="aaa25-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="aaa25-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="aaa25-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="aaa25-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="aaa25-128">False</span><span class="sxs-lookup"><span data-stu-id="aaa25-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="aaa25-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="aaa25-129">See also</span></span>



- [<span data-ttu-id="aaa25-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="aaa25-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

