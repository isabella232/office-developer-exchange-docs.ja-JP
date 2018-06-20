---
title: AttachmentIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AttachmentIds
api_type:
- schema
ms.assetid: 46ce3ad7-4b20-43ae-8c63-39f1e3c2666b
description: AttachmentIds 要素には、添付ファイルの識別子の配列が含まれています。
ms.openlocfilehash: f205aefe6a7dc4ec208e8a96b8a6b47094aa741b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759454"
---
# <a name="attachmentids"></a><span data-ttu-id="21417-103">AttachmentIds</span><span class="sxs-lookup"><span data-stu-id="21417-103">AttachmentIds</span></span>

<span data-ttu-id="21417-104">**AttachmentIds**要素には、添付ファイルの識別子の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="21417-104">The **AttachmentIds** element contains an array of attachment identifiers.</span></span> 
  
```xml
<AttachmentIds>
   <AttachmentId Id=""/>
</AttachmentIds>
```

 <span data-ttu-id="21417-105">**NonEmptyArrayOfRequestAttachmentIdsType**</span><span class="sxs-lookup"><span data-stu-id="21417-105">**NonEmptyArrayOfRequestAttachmentIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="21417-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="21417-106">Attributes and elements</span></span>

<span data-ttu-id="21417-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="21417-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="21417-108">属性</span><span class="sxs-lookup"><span data-stu-id="21417-108">Attributes</span></span>

<span data-ttu-id="21417-109">なし。</span><span class="sxs-lookup"><span data-stu-id="21417-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="21417-110">子要素</span><span class="sxs-lookup"><span data-stu-id="21417-110">Child elements</span></span>

|<span data-ttu-id="21417-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="21417-111">**Element**</span></span>|<span data-ttu-id="21417-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="21417-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="21417-113">AttachmentId (GetAttachment と DeleteAttachment)</span><span class="sxs-lookup"><span data-stu-id="21417-113">AttachmentId (GetAttachment and DeleteAttachment)</span></span>](attachmentid-getattachment-and-deleteattachment.md) <br/> |<span data-ttu-id="21417-114">単一の添付ファイルを識別する要素です。</span><span class="sxs-lookup"><span data-stu-id="21417-114">The element that identifies a single attachment.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="21417-115">親要素</span><span class="sxs-lookup"><span data-stu-id="21417-115">Parent elements</span></span>

|<span data-ttu-id="21417-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="21417-116">**Element**</span></span>|<span data-ttu-id="21417-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="21417-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="21417-118">DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="21417-118">DeleteAttachment</span></span>](deleteattachment.md) <br/> |<span data-ttu-id="21417-119">Exchange ストアからの添付ファイルを削除する要求を定義する要素。</span><span class="sxs-lookup"><span data-stu-id="21417-119">The element that defines a request to delete an attachment from the Exchange store.</span></span>  <br/> <span data-ttu-id="21417-120">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="21417-120">The following is the XPath expression to this element:</span></span>  <br/>  `/DeleteAttachment` <br/> |
|[<span data-ttu-id="21417-121">GetAttachment</span><span class="sxs-lookup"><span data-stu-id="21417-121">GetAttachment</span></span>](getattachment.md) <br/> |<span data-ttu-id="21417-122">Exchange ストアからの添付ファイルを取得する要求を定義する要素。</span><span class="sxs-lookup"><span data-stu-id="21417-122">The element that defines a request to get an attachment from the Exchange store.</span></span>  <br/> <span data-ttu-id="21417-123">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="21417-123">The following is the XPath expression to this element:</span></span>  <br/>  `/GetAttachment` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="21417-124">備考</span><span class="sxs-lookup"><span data-stu-id="21417-124">Remarks</span></span>

<span data-ttu-id="21417-125">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="21417-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="21417-126">要素情報</span><span class="sxs-lookup"><span data-stu-id="21417-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="21417-127">名前空間</span><span class="sxs-lookup"><span data-stu-id="21417-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="21417-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="21417-128">Schema Name</span></span>  <br/> |<span data-ttu-id="21417-129">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="21417-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="21417-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="21417-130">Validation File</span></span>  <br/> |<span data-ttu-id="21417-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="21417-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="21417-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="21417-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="21417-133">False</span><span class="sxs-lookup"><span data-stu-id="21417-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="21417-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="21417-134">See also</span></span>

- [<span data-ttu-id="21417-135">DeleteAttachment 操作</span><span class="sxs-lookup"><span data-stu-id="21417-135">DeleteAttachment operation</span></span>](deleteattachment-operation.md)
- [<span data-ttu-id="21417-136">GetAttachment 操作</span><span class="sxs-lookup"><span data-stu-id="21417-136">GetAttachment operation</span></span>](getattachment-operation.md)

