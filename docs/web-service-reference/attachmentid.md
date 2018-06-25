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
description: AttachmentId 要素は、アイテムまたはファイルの添付ファイルを識別します。 CreateAttachment の応答は、この要素を使用します。
ms.openlocfilehash: 2910503d1661ca3aaeeb4e319deb39f6b57c5c0a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759451"
---
# <a name="attachmentid"></a><span data-ttu-id="79018-104">AttachmentId</span><span class="sxs-lookup"><span data-stu-id="79018-104">AttachmentId</span></span>

<span data-ttu-id="79018-105">**AttachmentId**要素は、アイテムまたはファイルの添付ファイルを識別します。</span><span class="sxs-lookup"><span data-stu-id="79018-105">The **AttachmentId** element identifies an item or file attachment.</span></span> <span data-ttu-id="79018-106">CreateAttachment の応答は、この要素を使用します。</span><span class="sxs-lookup"><span data-stu-id="79018-106">This element is used in CreateAttachment responses.</span></span> 
  
```xml
<AttachmentId Id="" RootItemId="" RootItemChangeKey="" />
```

 <span data-ttu-id="79018-107">**AttachmentIdType**</span><span class="sxs-lookup"><span data-stu-id="79018-107">**AttachmentIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="79018-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="79018-108">Attributes and elements</span></span>

<span data-ttu-id="79018-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="79018-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="79018-110">属性</span><span class="sxs-lookup"><span data-stu-id="79018-110">Attributes</span></span>

|<span data-ttu-id="79018-111">**属性**</span><span class="sxs-lookup"><span data-stu-id="79018-111">**Attribute**</span></span>|<span data-ttu-id="79018-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="79018-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="79018-113">**Id**</span><span class="sxs-lookup"><span data-stu-id="79018-113">**Id**</span></span> <br/> |<span data-ttu-id="79018-114">添付ファイルの一意の識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="79018-114">Identifies the unique identifier of the attachment.</span></span>  <br/> |
|<span data-ttu-id="79018-115">**RootItemId**</span><span class="sxs-lookup"><span data-stu-id="79018-115">**RootItemId**</span></span> <br/> |<span data-ttu-id="79018-116">添付ファイルが関連付けられているルート ストア アイテムの一意の識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="79018-116">Identifies the unique identifier of the root store item to which the attachment is attached.</span></span>  <br/> |
|<span data-ttu-id="79018-117">**RootItemChangeKey**</span><span class="sxs-lookup"><span data-stu-id="79018-117">**RootItemChangeKey**</span></span> <br/> |<span data-ttu-id="79018-118">添付ファイルが関連付けられているルート ストアの項目のキーの変更を識別します。</span><span class="sxs-lookup"><span data-stu-id="79018-118">Identifies the change key of the root store item to which the attachment is attached.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="79018-119">子要素</span><span class="sxs-lookup"><span data-stu-id="79018-119">Child elements</span></span>

<span data-ttu-id="79018-120">なし。</span><span class="sxs-lookup"><span data-stu-id="79018-120">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="79018-121">親要素</span><span class="sxs-lookup"><span data-stu-id="79018-121">Parent elements</span></span>

|<span data-ttu-id="79018-122">**要素**</span><span class="sxs-lookup"><span data-stu-id="79018-122">**Element**</span></span>|<span data-ttu-id="79018-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="79018-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="79018-124">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="79018-124">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="79018-125">Exchange の他のアイテムに関連付けられている Exchange アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="79018-125">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="79018-126">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="79018-126">FileAttachment</span></span>](fileattachment.md) <br/> |<span data-ttu-id="79018-127">Exchange ストア内のアイテムに関連付けられているファイルを表します。</span><span class="sxs-lookup"><span data-stu-id="79018-127">Represents a file that is attached to an item in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="79018-128">備考</span><span class="sxs-lookup"><span data-stu-id="79018-128">Remarks</span></span>

<span data-ttu-id="79018-129">添付ファイルが作成されると、ルート アイテムの変更キーが変更されることに注意する必要があります。</span><span class="sxs-lookup"><span data-stu-id="79018-129">It is important to note that when an attachment is created, the change key of the root item is altered.</span></span>
  
<span data-ttu-id="79018-130">DeleteAttachment および GetAttachment 要求は、 [AttachmentId](attachmentid-getattachment-and-deleteattachment.md)要素を使用します。</span><span class="sxs-lookup"><span data-stu-id="79018-130">The [AttachmentId (GetAttachment and DeleteAttachment)](attachmentid-getattachment-and-deleteattachment.md) element is used in DeleteAttachment and GetAttachment requests.</span></span> 
  
<span data-ttu-id="79018-131">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="79018-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="79018-132">要素情報</span><span class="sxs-lookup"><span data-stu-id="79018-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="79018-133">名前空間</span><span class="sxs-lookup"><span data-stu-id="79018-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="79018-134">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="79018-134">Schema name</span></span>  <br/> |<span data-ttu-id="79018-135">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="79018-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="79018-136">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="79018-136">Validation file</span></span>  <br/> |<span data-ttu-id="79018-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="79018-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="79018-138">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="79018-138">Can be empty</span></span>  <br/> |<span data-ttu-id="79018-139">False</span><span class="sxs-lookup"><span data-stu-id="79018-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="79018-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="79018-140">See also</span></span>

- [<span data-ttu-id="79018-141">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="79018-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

