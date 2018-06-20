---
title: ParentItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ParentItemId
api_type:
- schema
ms.assetid: 72dc4391-72db-44d2-85d9-4718d59886a7
description: ParentItemId 要素は、関連付けられている添付ファイルへのリンクを親項目を識別します。
ms.openlocfilehash: 9bd875ee5ead8b87996288a640e1bb14e3a5e8b8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832703"
---
# <a name="parentitemid"></a><span data-ttu-id="595d3-103">ParentItemId</span><span class="sxs-lookup"><span data-stu-id="595d3-103">ParentItemId</span></span>

<span data-ttu-id="595d3-104">**ParentItemId**要素は、関連付けられている添付ファイルへのリンクを親項目を識別します。</span><span class="sxs-lookup"><span data-stu-id="595d3-104">The **ParentItemId** element identifies the parent item that links to an associated attachment.</span></span> 
  
- [<span data-ttu-id="595d3-105">CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="595d3-105">CreateAttachment</span></span>](createattachment.md)
  
- [<span data-ttu-id="595d3-106">ParentItemId</span><span class="sxs-lookup"><span data-stu-id="595d3-106">ParentItemId</span></span>](parentitemid.md)
  
```xml
<ParentItemId Id="" ChangeKey="" />
```

<span data-ttu-id="595d3-107">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="595d3-107">**ItemIdType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="595d3-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="595d3-108">Attributes and elements</span></span>

<span data-ttu-id="595d3-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="595d3-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="595d3-110">属性</span><span class="sxs-lookup"><span data-stu-id="595d3-110">Attributes</span></span>

|<span data-ttu-id="595d3-111">**属性**</span><span class="sxs-lookup"><span data-stu-id="595d3-111">**Attribute**</span></span>|<span data-ttu-id="595d3-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="595d3-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="595d3-113">**Id**</span><span class="sxs-lookup"><span data-stu-id="595d3-113">**Id**</span></span> <br/> |<span data-ttu-id="595d3-114">添付ファイルを関連付けるには Exchange ストア内の 1 つの項目を識別します。</span><span class="sxs-lookup"><span data-stu-id="595d3-114">Identifies a single item in the Exchange store to associate with an attachment.</span></span> <span data-ttu-id="595d3-115">この値は、文字列です。</span><span class="sxs-lookup"><span data-stu-id="595d3-115">This value is a string.</span></span> <span data-ttu-id="595d3-116">この属性は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="595d3-116">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="595d3-117">**変更キー**</span><span class="sxs-lookup"><span data-stu-id="595d3-117">**ChangeKey**</span></span> <br/> |<span data-ttu-id="595d3-118">Exchange ストア内の**Id**属性によって識別される項目の指定のバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="595d3-118">Identifies an unspecified version of an item that is identified by the **Id** attribute in the Exchange store.</span></span> <span data-ttu-id="595d3-119">これを使用して、添付ファイルを更新するときに現在の項目が使用されているかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="595d3-119">This is used to make sure that a current item is used when it is updated with an attachment.</span></span> <span data-ttu-id="595d3-120">この値は、文字列です。</span><span class="sxs-lookup"><span data-stu-id="595d3-120">This value is a string.</span></span> <span data-ttu-id="595d3-121">この属性は、省略可能です。</span><span class="sxs-lookup"><span data-stu-id="595d3-121">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="595d3-122">子要素</span><span class="sxs-lookup"><span data-stu-id="595d3-122">Child elements</span></span>

<span data-ttu-id="595d3-123">なし。</span><span class="sxs-lookup"><span data-stu-id="595d3-123">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="595d3-124">親要素</span><span class="sxs-lookup"><span data-stu-id="595d3-124">Parent elements</span></span>

|<span data-ttu-id="595d3-125">**要素**</span><span class="sxs-lookup"><span data-stu-id="595d3-125">**Element**</span></span>|<span data-ttu-id="595d3-126">**説明**</span><span class="sxs-lookup"><span data-stu-id="595d3-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="595d3-127">CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="595d3-127">CreateAttachment</span></span>](createattachment.md) <br/> |<span data-ttu-id="595d3-128">メールボックス内のアイテムに添付ファイルを作成する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="595d3-128">Defines a request to create an attachment to an item in a mailbox.</span></span>  <br/> <span data-ttu-id="595d3-129">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="595d3-129">The following is the XPath expression to this element:</span></span>  <br/>  `/CreateAttachment` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="595d3-130">備考</span><span class="sxs-lookup"><span data-stu-id="595d3-130">Remarks</span></span>

<span data-ttu-id="595d3-131">[CreateAttachment 操作](createattachment-operation.md)では、この要素が必要です。</span><span class="sxs-lookup"><span data-stu-id="595d3-131">This element is required in the [CreateAttachment operation](createattachment-operation.md).</span></span> <span data-ttu-id="595d3-132">この要素は、基本的に[アイテム Id](itemid.md)の要素と同じです。</span><span class="sxs-lookup"><span data-stu-id="595d3-132">This element is basically the same as the [ItemId](itemid.md) element.</span></span> 
  
<span data-ttu-id="595d3-133">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="595d3-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="595d3-134">要素情報</span><span class="sxs-lookup"><span data-stu-id="595d3-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="595d3-135">名前空間</span><span class="sxs-lookup"><span data-stu-id="595d3-135">Namespace</span></span>  <br/> |[http://schemas.microsoft.com/exchange/services/2006/messages](http://schemas.microsoft.com/exchange/services/2006/messages) <br/> |
|<span data-ttu-id="595d3-136">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="595d3-136">Schema Name</span></span>  <br/> |<span data-ttu-id="595d3-137">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="595d3-137">Messages schema</span></span>  <br/> |
|<span data-ttu-id="595d3-138">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="595d3-138">Validation File</span></span>  <br/> |<span data-ttu-id="595d3-139">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="595d3-139">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="595d3-140">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="595d3-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="595d3-141">False</span><span class="sxs-lookup"><span data-stu-id="595d3-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="595d3-142">関連項目</span><span class="sxs-lookup"><span data-stu-id="595d3-142">See also</span></span>

- [<span data-ttu-id="595d3-143">CreateAttachment 操作</span><span class="sxs-lookup"><span data-stu-id="595d3-143">CreateAttachment operation</span></span>](createattachment-operation.md)

