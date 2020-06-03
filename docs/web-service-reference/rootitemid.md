---
title: RootItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RootItemId
api_type:
- schema
ms.assetid: f613c705-17ce-48ce-aa64-4dc2cea25e31
description: RootItemId 要素は、削除された添付ファイルのルートアイテムを識別します。
ms.openlocfilehash: d8badd465fd5a93e1a6354d55ac5c4b080897152
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457096"
---
# <a name="rootitemid"></a><span data-ttu-id="c8084-103">RootItemId</span><span class="sxs-lookup"><span data-stu-id="c8084-103">RootItemId</span></span>

<span data-ttu-id="c8084-104">**RootItemId**要素は、削除された添付ファイルのルートアイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="c8084-104">The **RootItemId** element identifies the root item of a deleted attachment.</span></span> 
  
[<span data-ttu-id="c8084-105">DeleteAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="c8084-105">DeleteAttachmentResponse</span></span>](deleteattachmentresponse.md)
  
[<span data-ttu-id="c8084-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="c8084-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="c8084-107">DeleteAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="c8084-107">DeleteAttachmentResponseMessage</span></span>](deleteattachmentresponsemessage.md)
  
[<span data-ttu-id="c8084-108">RootItemId</span><span class="sxs-lookup"><span data-stu-id="c8084-108">RootItemId</span></span>](rootitemid.md)
  
```xml
<RootItemId RootItemId="" RootItemChangeKey="" />
```

 <span data-ttu-id="c8084-109">**RootItemIdType**</span><span class="sxs-lookup"><span data-stu-id="c8084-109">**RootItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c8084-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="c8084-110">Attributes and elements</span></span>

<span data-ttu-id="c8084-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c8084-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c8084-112">属性</span><span class="sxs-lookup"><span data-stu-id="c8084-112">Attributes</span></span>

|<span data-ttu-id="c8084-113">**属性**</span><span class="sxs-lookup"><span data-stu-id="c8084-113">**Attribute**</span></span>|<span data-ttu-id="c8084-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="c8084-114">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c8084-115">**RootItemId**</span><span class="sxs-lookup"><span data-stu-id="c8084-115">**RootItemId**</span></span> <br/> |<span data-ttu-id="c8084-116">削除された添付ファイルのルートアイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="c8084-116">Identifies the root item of a deleted attachment.</span></span>  <br/> |
|<span data-ttu-id="c8084-117">**RootItemChangeKey**</span><span class="sxs-lookup"><span data-stu-id="c8084-117">**RootItemChangeKey**</span></span> <br/> |<span data-ttu-id="c8084-118">削除された添付ファイルのルートアイテムの新しい変更キーを識別します。</span><span class="sxs-lookup"><span data-stu-id="c8084-118">Identifies the new change key of the root item of a deleted attachment.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="c8084-119">子要素</span><span class="sxs-lookup"><span data-stu-id="c8084-119">Child elements</span></span>

<span data-ttu-id="c8084-120">なし。</span><span class="sxs-lookup"><span data-stu-id="c8084-120">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c8084-121">親要素</span><span class="sxs-lookup"><span data-stu-id="c8084-121">Parent elements</span></span>

|<span data-ttu-id="c8084-122">**要素**</span><span class="sxs-lookup"><span data-stu-id="c8084-122">**Element**</span></span>|<span data-ttu-id="c8084-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="c8084-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c8084-124">DeleteAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="c8084-124">DeleteAttachmentResponseMessage</span></span>](deleteattachmentresponsemessage.md) <br/> |<span data-ttu-id="c8084-125">DeleteAttachment 要求の状態と結果を格納します。</span><span class="sxs-lookup"><span data-stu-id="c8084-125">Contains the status and result of a DeleteAttachment request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c8084-126">注釈</span><span class="sxs-lookup"><span data-stu-id="c8084-126">Remarks</span></span>

<span data-ttu-id="c8084-127">**RootItemId**要素は、deleteattachment 応答でのみ使用されます。</span><span class="sxs-lookup"><span data-stu-id="c8084-127">The **RootItemId** element is only used in DeleteAttachment responses.</span></span> <span data-ttu-id="c8084-128">これにより、ルートアイテム識別子が識別されます。さらに重要なのは、親アイテムに対する新しい変更キーです。</span><span class="sxs-lookup"><span data-stu-id="c8084-128">This identifies the root item identifier, and more importantly, the new change key to the parent item.</span></span> 
  
<span data-ttu-id="c8084-129">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="c8084-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c8084-130">要素の情報</span><span class="sxs-lookup"><span data-stu-id="c8084-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c8084-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="c8084-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c8084-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c8084-132">Schema name</span></span>  <br/> |<span data-ttu-id="c8084-133">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="c8084-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="c8084-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c8084-134">Validation file</span></span>  <br/> |<span data-ttu-id="c8084-135">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="c8084-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c8084-136">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="c8084-136">Can be empty</span></span>  <br/> |<span data-ttu-id="c8084-137">正しくない</span><span class="sxs-lookup"><span data-stu-id="c8084-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c8084-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="c8084-138">See also</span></span>



[<span data-ttu-id="c8084-139">DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="c8084-139">DeleteAttachment</span></span>](deleteattachment.md)
  
[<span data-ttu-id="c8084-140">DeleteAttachment 操作</span><span class="sxs-lookup"><span data-stu-id="c8084-140">DeleteAttachment operation</span></span>](deleteattachment-operation.md)


- [<span data-ttu-id="c8084-141">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="c8084-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

