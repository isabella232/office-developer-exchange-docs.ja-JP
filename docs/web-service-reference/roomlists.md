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
description: RoomLists 要素は、会議室のリストを表す1つまたは複数のアドレスのリストです。
ms.openlocfilehash: 8f6393b617331e5878e48113c94ca3546cba095e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459049"
---
# <a name="roomlists"></a><span data-ttu-id="67388-103">RoomLists</span><span class="sxs-lookup"><span data-stu-id="67388-103">RoomLists</span></span>

<span data-ttu-id="67388-104">**RoomLists**要素は、会議室のリストを表す1つまたは複数のアドレスのリストです。</span><span class="sxs-lookup"><span data-stu-id="67388-104">The **RoomLists** element is a list of one or more addresses that represent a list of meeting rooms.</span></span> 
  
[<span data-ttu-id="67388-105">た getroomlistsresponse</span><span class="sxs-lookup"><span data-stu-id="67388-105">GetRoomListsResponse</span></span>](getroomlistsresponse.md)
  
[<span data-ttu-id="67388-106">RoomLists</span><span class="sxs-lookup"><span data-stu-id="67388-106">RoomLists</span></span>](roomlists.md)
  
```xml
<RoomLists>   <Address/></RoomLists>
```

 <span data-ttu-id="67388-107">**ArrayOfEmailAddressesType**</span><span class="sxs-lookup"><span data-stu-id="67388-107">**ArrayOfEmailAddressesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="67388-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="67388-108">Attributes and elements</span></span>

<span data-ttu-id="67388-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="67388-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="67388-110">属性</span><span class="sxs-lookup"><span data-stu-id="67388-110">Attributes</span></span>

<span data-ttu-id="67388-111">なし。</span><span class="sxs-lookup"><span data-stu-id="67388-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="67388-112">子要素</span><span class="sxs-lookup"><span data-stu-id="67388-112">Child elements</span></span>

|<span data-ttu-id="67388-113">**Element**</span><span class="sxs-lookup"><span data-stu-id="67388-113">**Element**</span></span>|<span data-ttu-id="67388-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="67388-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="67388-115">Address (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="67388-115">Address (EmailAddressType)</span></span>](address-emailaddresstype.md) <br/> |<span data-ttu-id="67388-116">会議室一覧を表す電子メールアドレスと表示名を定義します。</span><span class="sxs-lookup"><span data-stu-id="67388-116">Defines the e-mail address and display name that represents the room list.</span></span> <span data-ttu-id="67388-117">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="67388-117">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="67388-118">親要素</span><span class="sxs-lookup"><span data-stu-id="67388-118">Parent elements</span></span>

|<span data-ttu-id="67388-119">**要素**</span><span class="sxs-lookup"><span data-stu-id="67388-119">**Element**</span></span>|<span data-ttu-id="67388-120">**説明**</span><span class="sxs-lookup"><span data-stu-id="67388-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="67388-121">た getroomlistsresponse</span><span class="sxs-lookup"><span data-stu-id="67388-121">GetRoomListsResponse</span></span>](getroomlistsresponse.md) <br/> |<span data-ttu-id="67388-122">[GetRoomLists 操作](getroomlists-operation.md)要求の状態と結果を格納します。</span><span class="sxs-lookup"><span data-stu-id="67388-122">Contains the status and result of a [GetRoomLists operation](getroomlists-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="67388-123">注釈</span><span class="sxs-lookup"><span data-stu-id="67388-123">Remarks</span></span>

<span data-ttu-id="67388-124">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされた Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="67388-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="67388-125">要素の情報</span><span class="sxs-lookup"><span data-stu-id="67388-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="67388-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="67388-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="67388-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="67388-127">Schema Name</span></span>  <br/> |<span data-ttu-id="67388-128">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="67388-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="67388-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="67388-129">Validation File</span></span>  <br/> |<span data-ttu-id="67388-130">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="67388-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="67388-131">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="67388-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="67388-132">正しくない</span><span class="sxs-lookup"><span data-stu-id="67388-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="67388-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="67388-133">See also</span></span>



[<span data-ttu-id="67388-134">GetRoomLists 操作</span><span class="sxs-lookup"><span data-stu-id="67388-134">GetRoomLists operation</span></span>](getroomlists-operation.md)


- [<span data-ttu-id="67388-135">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="67388-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

