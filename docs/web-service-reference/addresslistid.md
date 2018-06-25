---
title: AddressListId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a3334bb2-90dc-4fe1-96d9-890b13d9ff30
description: AddressListId 要素は、アドレス一覧の id を指定します。
ms.openlocfilehash: d8a513559b7d127559537b43d7c6c0a4db121702
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759301"
---
# <a name="addresslistid"></a><span data-ttu-id="19be6-103">AddressListId</span><span class="sxs-lookup"><span data-stu-id="19be6-103">AddressListId</span></span>

<span data-ttu-id="19be6-104">**AddressListId**要素は、アドレス一覧の id を指定します。</span><span class="sxs-lookup"><span data-stu-id="19be6-104">The **AddressListId** element specifies the identifier of an address list.</span></span> 
  
```XML
<AddressListId Id="">
</AddressListId>
```

 <span data-ttu-id="19be6-105">**AddressListIdType**</span><span class="sxs-lookup"><span data-stu-id="19be6-105">**AddressListIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="19be6-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="19be6-106">Attributes and elements</span></span>

<span data-ttu-id="19be6-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="19be6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="19be6-108">属性</span><span class="sxs-lookup"><span data-stu-id="19be6-108">Attributes</span></span>

|<span data-ttu-id="19be6-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="19be6-109">**Attribute**</span></span>|<span data-ttu-id="19be6-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="19be6-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="19be6-111">**Id**</span><span class="sxs-lookup"><span data-stu-id="19be6-111">**Id**</span></span> <br/> |<span data-ttu-id="19be6-112">文字列アドレス] ボックスの一覧の識別子です。</span><span class="sxs-lookup"><span data-stu-id="19be6-112">A string address list identifier.</span></span> <span data-ttu-id="19be6-113">この属性は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="19be6-113">This attribute is required.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="19be6-114">子要素</span><span class="sxs-lookup"><span data-stu-id="19be6-114">Child elements</span></span>

<span data-ttu-id="19be6-115">なし。</span><span class="sxs-lookup"><span data-stu-id="19be6-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="19be6-116">親要素</span><span class="sxs-lookup"><span data-stu-id="19be6-116">Parent elements</span></span>

|<span data-ttu-id="19be6-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="19be6-117">**Element**</span></span>|<span data-ttu-id="19be6-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="19be6-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="19be6-119">ContextFolderId</span><span class="sxs-lookup"><span data-stu-id="19be6-119">ContextFolderId</span></span>](contextfolderid.md) <br/> |<span data-ttu-id="19be6-120">フォルダーを使用する操作を対象としているフォルダーを示します。</span><span class="sxs-lookup"><span data-stu-id="19be6-120">Indicates the folder that is targeted for actions that use folders.</span></span> <span data-ttu-id="19be6-121">この要素は、コピー、削除、移動、およびターゲット フォルダー内のアイテムの会話の読み取り状態を設定するときに存在する必要があります。</span><span class="sxs-lookup"><span data-stu-id="19be6-121">This element must be present when copying, deleting, moving, and setting read state on conversation items in a target folder.</span></span>  <br/> |
|[<span data-ttu-id="19be6-122">CopyToFolder</span><span class="sxs-lookup"><span data-stu-id="19be6-122">CopyToFolder</span></span>](copytofolder.md) <br/> |<span data-ttu-id="19be6-123">メール アイテムのコピー先となるフォルダーの識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="19be6-123">Specifies the identifier of the folder to which email items are copied.</span></span>  <br/> |
|[<span data-ttu-id="19be6-124">DestinationFolderId</span><span class="sxs-lookup"><span data-stu-id="19be6-124">DestinationFolderId</span></span>](destinationfolderid.md) <br/> |<span data-ttu-id="19be6-125">コピー先のフォルダーを指定し、アクションを移動します。</span><span class="sxs-lookup"><span data-stu-id="19be6-125">Indicates the destination folder for copy and move actions.</span></span>  <br/> |
|[<span data-ttu-id="19be6-126">MoveToFolder</span><span class="sxs-lookup"><span data-stu-id="19be6-126">MoveToFolder</span></span>](movetofolder.md) <br/> |<span data-ttu-id="19be6-127">電子メール アイテムの移動先となるフォルダーの識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="19be6-127">Specifies the identifier of the folder to which email items are moved</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="19be6-128">備考</span><span class="sxs-lookup"><span data-stu-id="19be6-128">Remarks</span></span>

<span data-ttu-id="19be6-129">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="19be6-129">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="19be6-130">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="19be6-130">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="19be6-131">要素情報</span><span class="sxs-lookup"><span data-stu-id="19be6-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="19be6-132">名前空間</span><span class="sxs-lookup"><span data-stu-id="19be6-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="19be6-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="19be6-133">Schema Name</span></span>  <br/> |<span data-ttu-id="19be6-134">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="19be6-134">Type schema</span></span>  <br/> |
|<span data-ttu-id="19be6-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="19be6-135">Validation File</span></span>  <br/> |<span data-ttu-id="19be6-136">types.xsd</span><span class="sxs-lookup"><span data-stu-id="19be6-136">types.xsd</span></span>  <br/> |
|<span data-ttu-id="19be6-137">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="19be6-137">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="19be6-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="19be6-138">See also</span></span>

- [<span data-ttu-id="19be6-139">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="19be6-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

