---
title: AttachmentId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AttachmentId
api_type:
- schema
ms.assetid: 55a5fd77-60d1-40fa-8144-770600cedc6a
description: AttachmentId 要素は、アイテムまたは添付ファイルを識別します。 この要素は、CreateAttachment の応答で使用されます。
ms.openlocfilehash: b5dc9299b615f0fc01b8afcbaabf0ec7996e53d1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459112"
---
# <a name="attachmentid"></a><span data-ttu-id="0e9d7-104">AttachmentId</span><span class="sxs-lookup"><span data-stu-id="0e9d7-104">AttachmentId</span></span>

<span data-ttu-id="0e9d7-105">**AttachmentId**要素は、アイテムまたは添付ファイルを識別します。</span><span class="sxs-lookup"><span data-stu-id="0e9d7-105">The **AttachmentId** element identifies an item or file attachment.</span></span> <span data-ttu-id="0e9d7-106">この要素は、CreateAttachment の応答で使用されます。</span><span class="sxs-lookup"><span data-stu-id="0e9d7-106">This element is used in CreateAttachment responses.</span></span> 
  
```xml
<AttachmentId Id="" RootItemId="" RootItemChangeKey="" />
```

 <span data-ttu-id="0e9d7-107">**AttachmentIdType**</span><span class="sxs-lookup"><span data-stu-id="0e9d7-107">**AttachmentIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0e9d7-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="0e9d7-108">Attributes and elements</span></span>

<span data-ttu-id="0e9d7-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0e9d7-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0e9d7-110">属性</span><span class="sxs-lookup"><span data-stu-id="0e9d7-110">Attributes</span></span>

|<span data-ttu-id="0e9d7-111">**属性**</span><span class="sxs-lookup"><span data-stu-id="0e9d7-111">**Attribute**</span></span>|<span data-ttu-id="0e9d7-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="0e9d7-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0e9d7-113">**Id**</span><span class="sxs-lookup"><span data-stu-id="0e9d7-113">**Id**</span></span> <br/> |<span data-ttu-id="0e9d7-114">添付ファイルの一意識別子を識別します。</span><span class="sxs-lookup"><span data-stu-id="0e9d7-114">Identifies the unique identifier of the attachment.</span></span>  <br/> |
|<span data-ttu-id="0e9d7-115">**RootItemId**</span><span class="sxs-lookup"><span data-stu-id="0e9d7-115">**RootItemId**</span></span> <br/> |<span data-ttu-id="0e9d7-116">添付ファイルが添付されているルートストアアイテムの一意識別子を識別します。</span><span class="sxs-lookup"><span data-stu-id="0e9d7-116">Identifies the unique identifier of the root store item to which the attachment is attached.</span></span>  <br/> |
|<span data-ttu-id="0e9d7-117">**RootItemChangeKey**</span><span class="sxs-lookup"><span data-stu-id="0e9d7-117">**RootItemChangeKey**</span></span> <br/> |<span data-ttu-id="0e9d7-118">添付ファイルが添付されているルートストアアイテムの変更キーを識別します。</span><span class="sxs-lookup"><span data-stu-id="0e9d7-118">Identifies the change key of the root store item to which the attachment is attached.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="0e9d7-119">子要素</span><span class="sxs-lookup"><span data-stu-id="0e9d7-119">Child elements</span></span>

<span data-ttu-id="0e9d7-120">なし。</span><span class="sxs-lookup"><span data-stu-id="0e9d7-120">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0e9d7-121">親要素</span><span class="sxs-lookup"><span data-stu-id="0e9d7-121">Parent elements</span></span>

|<span data-ttu-id="0e9d7-122">**要素**</span><span class="sxs-lookup"><span data-stu-id="0e9d7-122">**Element**</span></span>|<span data-ttu-id="0e9d7-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="0e9d7-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0e9d7-124">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="0e9d7-124">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="0e9d7-125">別の Exchange アイテムに関連付けられている Exchange アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="0e9d7-125">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="0e9d7-126">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="0e9d7-126">FileAttachment</span></span>](fileattachment.md) <br/> |<span data-ttu-id="0e9d7-127">Exchange ストア内のアイテムに添付されているファイルを表します。</span><span class="sxs-lookup"><span data-stu-id="0e9d7-127">Represents a file that is attached to an item in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0e9d7-128">注釈</span><span class="sxs-lookup"><span data-stu-id="0e9d7-128">Remarks</span></span>

<span data-ttu-id="0e9d7-129">添付ファイルを作成すると、ルートアイテムの変更キーが変更されることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="0e9d7-129">It is important to note that when an attachment is created, the change key of the root item is altered.</span></span>
  
<span data-ttu-id="0e9d7-130">[AttachmentId (getattachment と deleteattachment)](attachmentid-getattachment-and-deleteattachment.md)要素は、deleteattachment 要求と getattachment 要求で使用されます。</span><span class="sxs-lookup"><span data-stu-id="0e9d7-130">The [AttachmentId (GetAttachment and DeleteAttachment)](attachmentid-getattachment-and-deleteattachment.md) element is used in DeleteAttachment and GetAttachment requests.</span></span> 
  
<span data-ttu-id="0e9d7-131">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="0e9d7-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0e9d7-132">要素の情報</span><span class="sxs-lookup"><span data-stu-id="0e9d7-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0e9d7-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="0e9d7-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0e9d7-134">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0e9d7-134">Schema name</span></span>  <br/> |<span data-ttu-id="0e9d7-135">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="0e9d7-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="0e9d7-136">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0e9d7-136">Validation file</span></span>  <br/> |<span data-ttu-id="0e9d7-137">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="0e9d7-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0e9d7-138">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="0e9d7-138">Can be empty</span></span>  <br/> |<span data-ttu-id="0e9d7-139">正しくない</span><span class="sxs-lookup"><span data-stu-id="0e9d7-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0e9d7-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="0e9d7-140">See also</span></span>

- [<span data-ttu-id="0e9d7-141">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="0e9d7-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

