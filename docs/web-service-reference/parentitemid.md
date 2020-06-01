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
description: ParentItemId 要素は、関連付けられた添付ファイルにリンクする親アイテムを識別します。
ms.openlocfilehash: 4f3e33da0af2438948313f0e335cd03e076d135a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465745"
---
# <a name="parentitemid"></a><span data-ttu-id="1f16c-103">ParentItemId</span><span class="sxs-lookup"><span data-stu-id="1f16c-103">ParentItemId</span></span>

<span data-ttu-id="1f16c-104">**Parentitemid**要素は、関連付けられた添付ファイルにリンクする親アイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="1f16c-104">The **ParentItemId** element identifies the parent item that links to an associated attachment.</span></span> 
  
- [<span data-ttu-id="1f16c-105">CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="1f16c-105">CreateAttachment</span></span>](createattachment.md)
  
- [<span data-ttu-id="1f16c-106">ParentItemId</span><span class="sxs-lookup"><span data-stu-id="1f16c-106">ParentItemId</span></span>](parentitemid.md)
  
```xml
<ParentItemId Id="" ChangeKey="" />
```

<span data-ttu-id="1f16c-107">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="1f16c-107">**ItemIdType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="1f16c-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="1f16c-108">Attributes and elements</span></span>

<span data-ttu-id="1f16c-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1f16c-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1f16c-110">属性</span><span class="sxs-lookup"><span data-stu-id="1f16c-110">Attributes</span></span>

|<span data-ttu-id="1f16c-111">**属性**</span><span class="sxs-lookup"><span data-stu-id="1f16c-111">**Attribute**</span></span>|<span data-ttu-id="1f16c-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="1f16c-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1f16c-113">**Id**</span><span class="sxs-lookup"><span data-stu-id="1f16c-113">**Id**</span></span> <br/> |<span data-ttu-id="1f16c-114">添付ファイルに関連付ける Exchange ストア内の1つのアイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="1f16c-114">Identifies a single item in the Exchange store to associate with an attachment.</span></span> <span data-ttu-id="1f16c-115">この値は文字列です。</span><span class="sxs-lookup"><span data-stu-id="1f16c-115">This value is a string.</span></span> <span data-ttu-id="1f16c-116">この属性は必須です。</span><span class="sxs-lookup"><span data-stu-id="1f16c-116">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="1f16c-117">**ChangeKey**</span><span class="sxs-lookup"><span data-stu-id="1f16c-117">**ChangeKey**</span></span> <br/> |<span data-ttu-id="1f16c-118">Exchange ストアの**Id**属性によって識別されるアイテムの指定されていないバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="1f16c-118">Identifies an unspecified version of an item that is identified by the **Id** attribute in the Exchange store.</span></span> <span data-ttu-id="1f16c-119">これは、添付ファイルによって更新されるときに、現在のアイテムが使用されるようにするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="1f16c-119">This is used to make sure that a current item is used when it is updated with an attachment.</span></span> <span data-ttu-id="1f16c-120">この値は文字列です。</span><span class="sxs-lookup"><span data-stu-id="1f16c-120">This value is a string.</span></span> <span data-ttu-id="1f16c-121">この属性は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="1f16c-121">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="1f16c-122">子要素</span><span class="sxs-lookup"><span data-stu-id="1f16c-122">Child elements</span></span>

<span data-ttu-id="1f16c-123">なし。</span><span class="sxs-lookup"><span data-stu-id="1f16c-123">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1f16c-124">親要素</span><span class="sxs-lookup"><span data-stu-id="1f16c-124">Parent elements</span></span>

|<span data-ttu-id="1f16c-125">**要素**</span><span class="sxs-lookup"><span data-stu-id="1f16c-125">**Element**</span></span>|<span data-ttu-id="1f16c-126">**説明**</span><span class="sxs-lookup"><span data-stu-id="1f16c-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1f16c-127">CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="1f16c-127">CreateAttachment</span></span>](createattachment.md) <br/> |<span data-ttu-id="1f16c-128">メールボックス内のアイテムの添付ファイルを作成するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="1f16c-128">Defines a request to create an attachment to an item in a mailbox.</span></span>  <br/> <span data-ttu-id="1f16c-129">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1f16c-129">The following is the XPath expression to this element:</span></span>  <br/>  `/CreateAttachment` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1f16c-130">注釈</span><span class="sxs-lookup"><span data-stu-id="1f16c-130">Remarks</span></span>

<span data-ttu-id="1f16c-131">この要素は、 [Createattachment 操作](createattachment-operation.md)で必要です。</span><span class="sxs-lookup"><span data-stu-id="1f16c-131">This element is required in the [CreateAttachment operation](createattachment-operation.md).</span></span> <span data-ttu-id="1f16c-132">この要素は、基本的に[ItemId](itemid.md)要素と同じです。</span><span class="sxs-lookup"><span data-stu-id="1f16c-132">This element is basically the same as the [ItemId](itemid.md) element.</span></span> 
  
<span data-ttu-id="1f16c-133">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="1f16c-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1f16c-134">要素の情報</span><span class="sxs-lookup"><span data-stu-id="1f16c-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1f16c-135">Namespace</span><span class="sxs-lookup"><span data-stu-id="1f16c-135">Namespace</span></span>  <br/> |[https://schemas.microsoft.com/exchange/services/2006/messages](https://schemas.microsoft.com/exchange/services/2006/messages) <br/> |
|<span data-ttu-id="1f16c-136">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1f16c-136">Schema Name</span></span>  <br/> |<span data-ttu-id="1f16c-137">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="1f16c-137">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1f16c-138">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1f16c-138">Validation File</span></span>  <br/> |<span data-ttu-id="1f16c-139">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="1f16c-139">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1f16c-140">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="1f16c-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="1f16c-141">正しくない</span><span class="sxs-lookup"><span data-stu-id="1f16c-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1f16c-142">関連項目</span><span class="sxs-lookup"><span data-stu-id="1f16c-142">See also</span></span>

- [<span data-ttu-id="1f16c-143">CreateAttachment 操作</span><span class="sxs-lookup"><span data-stu-id="1f16c-143">CreateAttachment operation</span></span>](createattachment-operation.md)

