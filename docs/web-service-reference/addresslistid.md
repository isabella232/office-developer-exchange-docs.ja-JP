---
title: AddressListId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a3334bb2-90dc-4fe1-96d9-890b13d9ff30
description: AddressListId 要素は、アドレス一覧の識別子を指定します。
ms.openlocfilehash: c33944bf6e41903a5de596628e1ce7ba9f7421e1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463609"
---
# <a name="addresslistid"></a><span data-ttu-id="1f6a5-103">AddressListId</span><span class="sxs-lookup"><span data-stu-id="1f6a5-103">AddressListId</span></span>

<span data-ttu-id="1f6a5-104">**AddressListId**要素は、アドレス一覧の識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="1f6a5-104">The **AddressListId** element specifies the identifier of an address list.</span></span> 
  
```XML
<AddressListId Id="">
</AddressListId>
```

 <span data-ttu-id="1f6a5-105">**AddressListIdType**</span><span class="sxs-lookup"><span data-stu-id="1f6a5-105">**AddressListIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1f6a5-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="1f6a5-106">Attributes and elements</span></span>

<span data-ttu-id="1f6a5-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1f6a5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1f6a5-108">属性</span><span class="sxs-lookup"><span data-stu-id="1f6a5-108">Attributes</span></span>

|<span data-ttu-id="1f6a5-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="1f6a5-109">**Attribute**</span></span>|<span data-ttu-id="1f6a5-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="1f6a5-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1f6a5-111">**Id**</span><span class="sxs-lookup"><span data-stu-id="1f6a5-111">**Id**</span></span> <br/> |<span data-ttu-id="1f6a5-112">文字列アドレス一覧の識別子。</span><span class="sxs-lookup"><span data-stu-id="1f6a5-112">A string address list identifier.</span></span> <span data-ttu-id="1f6a5-113">この属性は必須です。</span><span class="sxs-lookup"><span data-stu-id="1f6a5-113">This attribute is required.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="1f6a5-114">子要素</span><span class="sxs-lookup"><span data-stu-id="1f6a5-114">Child elements</span></span>

<span data-ttu-id="1f6a5-115">なし。</span><span class="sxs-lookup"><span data-stu-id="1f6a5-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1f6a5-116">親要素</span><span class="sxs-lookup"><span data-stu-id="1f6a5-116">Parent elements</span></span>

|<span data-ttu-id="1f6a5-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="1f6a5-117">**Element**</span></span>|<span data-ttu-id="1f6a5-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="1f6a5-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1f6a5-119">ContextFolderId</span><span class="sxs-lookup"><span data-stu-id="1f6a5-119">ContextFolderId</span></span>](contextfolderid.md) <br/> |<span data-ttu-id="1f6a5-120">フォルダーを使用する操作を対象とするフォルダーを示します。</span><span class="sxs-lookup"><span data-stu-id="1f6a5-120">Indicates the folder that is targeted for actions that use folders.</span></span> <span data-ttu-id="1f6a5-121">この要素は、ターゲットフォルダー内の会話アイテムのコピー、削除、移動、および読み取り状態の設定時に存在する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1f6a5-121">This element must be present when copying, deleting, moving, and setting read state on conversation items in a target folder.</span></span>  <br/> |
|[<span data-ttu-id="1f6a5-122">CopyToFolder</span><span class="sxs-lookup"><span data-stu-id="1f6a5-122">CopyToFolder</span></span>](copytofolder.md) <br/> |<span data-ttu-id="1f6a5-123">電子メールアイテムのコピー先フォルダーの識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="1f6a5-123">Specifies the identifier of the folder to which email items are copied.</span></span>  <br/> |
|[<span data-ttu-id="1f6a5-124">DestinationFolderId</span><span class="sxs-lookup"><span data-stu-id="1f6a5-124">DestinationFolderId</span></span>](destinationfolderid.md) <br/> |<span data-ttu-id="1f6a5-125">コピー操作と移動操作の宛先フォルダーを指定します。</span><span class="sxs-lookup"><span data-stu-id="1f6a5-125">Indicates the destination folder for copy and move actions.</span></span>  <br/> |
|[<span data-ttu-id="1f6a5-126">MoveToFolder</span><span class="sxs-lookup"><span data-stu-id="1f6a5-126">MoveToFolder</span></span>](movetofolder.md) <br/> |<span data-ttu-id="1f6a5-127">電子メールアイテムの移動先フォルダーの識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="1f6a5-127">Specifies the identifier of the folder to which email items are moved</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1f6a5-128">注釈</span><span class="sxs-lookup"><span data-stu-id="1f6a5-128">Remarks</span></span>

<span data-ttu-id="1f6a5-129">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="1f6a5-129">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="1f6a5-130">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="1f6a5-130">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1f6a5-131">要素の情報</span><span class="sxs-lookup"><span data-stu-id="1f6a5-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1f6a5-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="1f6a5-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1f6a5-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1f6a5-133">Schema Name</span></span>  <br/> |<span data-ttu-id="1f6a5-134">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="1f6a5-134">Type schema</span></span>  <br/> |
|<span data-ttu-id="1f6a5-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1f6a5-135">Validation File</span></span>  <br/> |<span data-ttu-id="1f6a5-136">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="1f6a5-136">types.xsd</span></span>  <br/> |
|<span data-ttu-id="1f6a5-137">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="1f6a5-137">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="1f6a5-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="1f6a5-138">See also</span></span>

- [<span data-ttu-id="1f6a5-139">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="1f6a5-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

