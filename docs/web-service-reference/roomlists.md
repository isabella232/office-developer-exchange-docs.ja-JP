---
title: RoomLists
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RoomLists
api_type:
- schema
ms.assetid: 2b190823-b11e-4635-97e4-3aba5865fd05
description: RoomLists 要素は、会議室の一覧を表す 1 つまたは複数のアドレスの一覧です。
ms.openlocfilehash: eb03c34aeb5d80c4a9c6c92471e4094c63f04c87
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833252"
---
# <a name="roomlists"></a><span data-ttu-id="9bf0a-103">RoomLists</span><span class="sxs-lookup"><span data-stu-id="9bf0a-103">RoomLists</span></span>

<span data-ttu-id="9bf0a-104">**RoomLists**要素は、会議室の一覧を表す 1 つまたは複数のアドレスの一覧です。</span><span class="sxs-lookup"><span data-stu-id="9bf0a-104">The **RoomLists** element is a list of one or more addresses that represent a list of meeting rooms.</span></span> 
  
[<span data-ttu-id="9bf0a-105">GetRoomListsResponse</span><span class="sxs-lookup"><span data-stu-id="9bf0a-105">GetRoomListsResponse</span></span>](getroomlistsresponse.md)
  
[<span data-ttu-id="9bf0a-106">RoomLists</span><span class="sxs-lookup"><span data-stu-id="9bf0a-106">RoomLists</span></span>](roomlists.md)
  
```xml
<RoomLists>   <Address/></RoomLists>
```

 <span data-ttu-id="9bf0a-107">**ArrayOfEmailAddressesType**</span><span class="sxs-lookup"><span data-stu-id="9bf0a-107">**ArrayOfEmailAddressesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9bf0a-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="9bf0a-108">Attributes and elements</span></span>

<span data-ttu-id="9bf0a-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9bf0a-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9bf0a-110">属性</span><span class="sxs-lookup"><span data-stu-id="9bf0a-110">Attributes</span></span>

<span data-ttu-id="9bf0a-111">なし。</span><span class="sxs-lookup"><span data-stu-id="9bf0a-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9bf0a-112">子要素</span><span class="sxs-lookup"><span data-stu-id="9bf0a-112">Child elements</span></span>

|<span data-ttu-id="9bf0a-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="9bf0a-113">**Element**</span></span>|<span data-ttu-id="9bf0a-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="9bf0a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9bf0a-115">アドレス (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="9bf0a-115">Address (EmailAddressType)</span></span>](address-emailaddresstype.md) <br/> |<span data-ttu-id="9bf0a-116">ルームのリストを表す表示名と電子メール アドレスを定義します。</span><span class="sxs-lookup"><span data-stu-id="9bf0a-116">Defines the e-mail address and display name that represents the room list.</span></span> <span data-ttu-id="9bf0a-117">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="9bf0a-117">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9bf0a-118">親要素</span><span class="sxs-lookup"><span data-stu-id="9bf0a-118">Parent elements</span></span>

|<span data-ttu-id="9bf0a-119">**要素**</span><span class="sxs-lookup"><span data-stu-id="9bf0a-119">**Element**</span></span>|<span data-ttu-id="9bf0a-120">**説明**</span><span class="sxs-lookup"><span data-stu-id="9bf0a-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9bf0a-121">GetRoomListsResponse</span><span class="sxs-lookup"><span data-stu-id="9bf0a-121">GetRoomListsResponse</span></span>](getroomlistsresponse.md) <br/> |<span data-ttu-id="9bf0a-122">状態と[GetRoomLists の操作](getroomlists-operation.md)要求の結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9bf0a-122">Contains the status and result of a [GetRoomLists operation](getroomlists-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9bf0a-123">備考</span><span class="sxs-lookup"><span data-stu-id="9bf0a-123">Remarks</span></span>

<span data-ttu-id="9bf0a-124">この要素を記述するスキーマは、インストールされているクライアント アクセス サーバーの役割と Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="9bf0a-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9bf0a-125">要素情報</span><span class="sxs-lookup"><span data-stu-id="9bf0a-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9bf0a-126">名前空間</span><span class="sxs-lookup"><span data-stu-id="9bf0a-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9bf0a-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9bf0a-127">Schema Name</span></span>  <br/> |<span data-ttu-id="9bf0a-128">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="9bf0a-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9bf0a-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9bf0a-129">Validation File</span></span>  <br/> |<span data-ttu-id="9bf0a-130">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9bf0a-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9bf0a-131">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="9bf0a-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="9bf0a-132">False</span><span class="sxs-lookup"><span data-stu-id="9bf0a-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9bf0a-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="9bf0a-133">See also</span></span>



[<span data-ttu-id="9bf0a-134">GetRoomLists 操作</span><span class="sxs-lookup"><span data-stu-id="9bf0a-134">GetRoomLists operation</span></span>](getroomlists-operation.md)


- [<span data-ttu-id="9bf0a-135">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="9bf0a-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

