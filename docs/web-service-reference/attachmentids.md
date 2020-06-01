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
description: AttachmentIds 要素には、添付ファイル識別子の配列が含まれています。
ms.openlocfilehash: cff1cb5658690fd6dd2c6a7812e1f600a4c80e29
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464253"
---
# <a name="attachmentids"></a><span data-ttu-id="b349a-103">AttachmentIds</span><span class="sxs-lookup"><span data-stu-id="b349a-103">AttachmentIds</span></span>

<span data-ttu-id="b349a-104">**AttachmentIds**要素には、添付ファイル識別子の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b349a-104">The **AttachmentIds** element contains an array of attachment identifiers.</span></span> 
  
```xml
<AttachmentIds>
   <AttachmentId Id=""/>
</AttachmentIds>
```

 <span data-ttu-id="b349a-105">**NonEmptyArrayOfRequestAttachmentIdsType**</span><span class="sxs-lookup"><span data-stu-id="b349a-105">**NonEmptyArrayOfRequestAttachmentIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b349a-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="b349a-106">Attributes and elements</span></span>

<span data-ttu-id="b349a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b349a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b349a-108">属性</span><span class="sxs-lookup"><span data-stu-id="b349a-108">Attributes</span></span>

<span data-ttu-id="b349a-109">なし。</span><span class="sxs-lookup"><span data-stu-id="b349a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b349a-110">子要素</span><span class="sxs-lookup"><span data-stu-id="b349a-110">Child elements</span></span>

|<span data-ttu-id="b349a-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="b349a-111">**Element**</span></span>|<span data-ttu-id="b349a-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="b349a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b349a-113">AttachmentId (GetAttachment と DeleteAttachment)</span><span class="sxs-lookup"><span data-stu-id="b349a-113">AttachmentId (GetAttachment and DeleteAttachment)</span></span>](attachmentid-getattachment-and-deleteattachment.md) <br/> |<span data-ttu-id="b349a-114">単一の添付ファイルを識別する要素。</span><span class="sxs-lookup"><span data-stu-id="b349a-114">The element that identifies a single attachment.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b349a-115">親要素</span><span class="sxs-lookup"><span data-stu-id="b349a-115">Parent elements</span></span>

|<span data-ttu-id="b349a-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="b349a-116">**Element**</span></span>|<span data-ttu-id="b349a-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="b349a-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b349a-118">DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="b349a-118">DeleteAttachment</span></span>](deleteattachment.md) <br/> |<span data-ttu-id="b349a-119">Exchange ストアから添付ファイルを削除する要求を定義する要素。</span><span class="sxs-lookup"><span data-stu-id="b349a-119">The element that defines a request to delete an attachment from the Exchange store.</span></span>  <br/> <span data-ttu-id="b349a-120">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b349a-120">The following is the XPath expression to this element:</span></span>  <br/>  `/DeleteAttachment` <br/> |
|[<span data-ttu-id="b349a-121">GetAttachment</span><span class="sxs-lookup"><span data-stu-id="b349a-121">GetAttachment</span></span>](getattachment.md) <br/> |<span data-ttu-id="b349a-122">Exchange ストアから添付ファイルを取得するための要求を定義する要素。</span><span class="sxs-lookup"><span data-stu-id="b349a-122">The element that defines a request to get an attachment from the Exchange store.</span></span>  <br/> <span data-ttu-id="b349a-123">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b349a-123">The following is the XPath expression to this element:</span></span>  <br/>  `/GetAttachment` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b349a-124">注釈</span><span class="sxs-lookup"><span data-stu-id="b349a-124">Remarks</span></span>

<span data-ttu-id="b349a-125">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="b349a-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b349a-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="b349a-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b349a-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="b349a-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b349a-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b349a-128">Schema Name</span></span>  <br/> |<span data-ttu-id="b349a-129">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="b349a-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b349a-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b349a-130">Validation File</span></span>  <br/> |<span data-ttu-id="b349a-131">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="b349a-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b349a-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="b349a-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="b349a-133">正しくない</span><span class="sxs-lookup"><span data-stu-id="b349a-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b349a-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="b349a-134">See also</span></span>

- [<span data-ttu-id="b349a-135">DeleteAttachment 操作</span><span class="sxs-lookup"><span data-stu-id="b349a-135">DeleteAttachment operation</span></span>](deleteattachment-operation.md)
- [<span data-ttu-id="b349a-136">GetAttachment 操作</span><span class="sxs-lookup"><span data-stu-id="b349a-136">GetAttachment operation</span></span>](getattachment-operation.md)

