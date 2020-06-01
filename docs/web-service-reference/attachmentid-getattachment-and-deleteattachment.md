---
title: AttachmentId (GetAttachment と DeleteAttachment)
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
ms.assetid: 4bea1cb5-0a0f-4e14-9b09-f91af8cf9899
description: AttachmentId 要素は、1つの添付ファイルを識別します。
ms.openlocfilehash: 1096487490f6066f70d2da861b3015f0fbf5a68f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460856"
---
# <a name="attachmentid-getattachment-and-deleteattachment"></a><span data-ttu-id="fbb98-103">AttachmentId (GetAttachment と DeleteAttachment)</span><span class="sxs-lookup"><span data-stu-id="fbb98-103">AttachmentId (GetAttachment and DeleteAttachment)</span></span>

<span data-ttu-id="fbb98-104">**AttachmentId**要素は、1つの添付ファイルを識別します。</span><span class="sxs-lookup"><span data-stu-id="fbb98-104">The **AttachmentId** element identifies a single attachment.</span></span> 
  
```xml
<AttachmentId Id="" />
```

 <span data-ttu-id="fbb98-105">**RequestAttachmentIdType**</span><span class="sxs-lookup"><span data-stu-id="fbb98-105">**RequestAttachmentIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fbb98-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="fbb98-106">Attributes and elements</span></span>

<span data-ttu-id="fbb98-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="fbb98-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fbb98-108">属性</span><span class="sxs-lookup"><span data-stu-id="fbb98-108">Attributes</span></span>

|<span data-ttu-id="fbb98-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="fbb98-109">**Attribute**</span></span>|<span data-ttu-id="fbb98-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="fbb98-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="fbb98-111">**Id**</span><span class="sxs-lookup"><span data-stu-id="fbb98-111">**Id**</span></span> <br/> |<span data-ttu-id="fbb98-112">添付ファイル識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="fbb98-112">Specifies the attachment identifier.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="fbb98-113">子要素</span><span class="sxs-lookup"><span data-stu-id="fbb98-113">Child elements</span></span>

<span data-ttu-id="fbb98-114">なし。</span><span class="sxs-lookup"><span data-stu-id="fbb98-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fbb98-115">親要素</span><span class="sxs-lookup"><span data-stu-id="fbb98-115">Parent elements</span></span>

|<span data-ttu-id="fbb98-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="fbb98-116">**Element**</span></span>|<span data-ttu-id="fbb98-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="fbb98-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fbb98-118">AttachmentIds</span><span class="sxs-lookup"><span data-stu-id="fbb98-118">AttachmentIds</span></span>](attachmentids.md) <br/> | <span data-ttu-id="fbb98-119">添付ファイル識別子の配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="fbb98-119">Contains an array of attachment identifiers.</span></span><br/><br/>  <span data-ttu-id="fbb98-120">この要素の XPath 式は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="fbb98-120">The following are the XPath expressions to this element:</span></span><br/><br/>`/DeleteAttachment/AttachmentIds`<br/><br/>`/GetAttachment/AttachmentIds` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="fbb98-121">注釈</span><span class="sxs-lookup"><span data-stu-id="fbb98-121">Remarks</span></span>

<span data-ttu-id="fbb98-122">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="fbb98-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fbb98-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="fbb98-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fbb98-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="fbb98-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fbb98-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="fbb98-125">Schema Name</span></span>  <br/> |<span data-ttu-id="fbb98-126">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="fbb98-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="fbb98-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="fbb98-127">Validation File</span></span>  <br/> |<span data-ttu-id="fbb98-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="fbb98-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fbb98-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="fbb98-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="fbb98-130">正しくない</span><span class="sxs-lookup"><span data-stu-id="fbb98-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fbb98-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="fbb98-131">See also</span></span>

- [<span data-ttu-id="fbb98-132">DeleteAttachment 操作</span><span class="sxs-lookup"><span data-stu-id="fbb98-132">DeleteAttachment operation</span></span>](deleteattachment-operation.md)
- [<span data-ttu-id="fbb98-133">GetAttachment 操作</span><span class="sxs-lookup"><span data-stu-id="fbb98-133">GetAttachment operation</span></span>](getattachment-operation.md)

