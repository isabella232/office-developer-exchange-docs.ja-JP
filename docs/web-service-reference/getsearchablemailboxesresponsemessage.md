---
title: GetSearchableMailboxesResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f45865fd-4626-4d80-84f6-7989339fdd85
description: GetSearchableMailboxesResponseMessage 要素は、Getsearchablemailemailrequest 要求に対する応答メッセージを指定します。
ms.openlocfilehash: 69f45d87cfbd398013d021cdd39b55497d78ae04
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458258"
---
# <a name="getsearchablemailboxesresponsemessage"></a><span data-ttu-id="c9b3f-103">GetSearchableMailboxesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="c9b3f-103">GetSearchableMailboxesResponseMessage</span></span>

<span data-ttu-id="c9b3f-104">**GetSearchableMailboxesResponseMessage**要素は、 **Getsearchablemailemailrequest**要求に対する応答メッセージを指定します。</span><span class="sxs-lookup"><span data-stu-id="c9b3f-104">The **GetSearchableMailboxesResponseMessage** element specifies the response message for a **GetSearchableMailboxes** request.</span></span> 
  
```XML
<GetSearchableMailboxesResponseMessage ResponseClass=" Success | Warning | Error ">
    <SearchableMailboxes/>
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</GetSearchablemailboxesResponseMessage>
```

 <span data-ttu-id="c9b3f-105">**GetSearchableMailboxesResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="c9b3f-105">**GetSearchableMailboxesResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c9b3f-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="c9b3f-106">Attributes and elements</span></span>

<span data-ttu-id="c9b3f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c9b3f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c9b3f-108">属性</span><span class="sxs-lookup"><span data-stu-id="c9b3f-108">Attributes</span></span>

|<span data-ttu-id="c9b3f-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="c9b3f-109">**Attribute**</span></span>|<span data-ttu-id="c9b3f-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="c9b3f-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c9b3f-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="c9b3f-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="c9b3f-112">応答のクラスを示します。</span><span class="sxs-lookup"><span data-stu-id="c9b3f-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="c9b3f-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="c9b3f-113">ResponseClass</span></span>

|<span data-ttu-id="c9b3f-114">**値**</span><span class="sxs-lookup"><span data-stu-id="c9b3f-114">**Value**</span></span>|<span data-ttu-id="c9b3f-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="c9b3f-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c9b3f-116">Success</span><span class="sxs-lookup"><span data-stu-id="c9b3f-116">Success</span></span>  <br/> |<span data-ttu-id="c9b3f-117">成功を示します。</span><span class="sxs-lookup"><span data-stu-id="c9b3f-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="c9b3f-118">警告</span><span class="sxs-lookup"><span data-stu-id="c9b3f-118">Warning</span></span>  <br/> |<span data-ttu-id="c9b3f-119">警告を示します。</span><span class="sxs-lookup"><span data-stu-id="c9b3f-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="c9b3f-120">Error</span><span class="sxs-lookup"><span data-stu-id="c9b3f-120">Error</span></span>  <br/> |<span data-ttu-id="c9b3f-121">エラーを示します。</span><span class="sxs-lookup"><span data-stu-id="c9b3f-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="c9b3f-122">子要素</span><span class="sxs-lookup"><span data-stu-id="c9b3f-122">Child elements</span></span>

|<span data-ttu-id="c9b3f-123">**Element**</span><span class="sxs-lookup"><span data-stu-id="c9b3f-123">**Element**</span></span>|<span data-ttu-id="c9b3f-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="c9b3f-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c9b3f-125">SearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="c9b3f-125">SearchableMailboxes</span></span>](searchablemailboxes.md) <br/> |<span data-ttu-id="c9b3f-126">**Getsearchablemailaddressrequest**から返されるメールボックスの配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="c9b3f-126">Contains an array of the mailboxes returned from a **GetSearchableMailboxes** request.</span></span>  <br/> |
|[<span data-ttu-id="c9b3f-127">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="c9b3f-127">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="c9b3f-128">現在未使用で、今後の使用のために予約されています。</span><span class="sxs-lookup"><span data-stu-id="c9b3f-128">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="c9b3f-129">MessageText</span><span class="sxs-lookup"><span data-stu-id="c9b3f-129">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="c9b3f-130">応答の状態を説明するテキストを提供します。</span><span class="sxs-lookup"><span data-stu-id="c9b3f-130">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="c9b3f-131">MessageXml</span><span class="sxs-lookup"><span data-stu-id="c9b3f-131">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="c9b3f-132">エラー応答に関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="c9b3f-132">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="c9b3f-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="c9b3f-133">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="c9b3f-134">要求に関する状態情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="c9b3f-134">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c9b3f-135">親要素</span><span class="sxs-lookup"><span data-stu-id="c9b3f-135">Parent elements</span></span>

|<span data-ttu-id="c9b3f-136">**要素**</span><span class="sxs-lookup"><span data-stu-id="c9b3f-136">**Element**</span></span>|<span data-ttu-id="c9b3f-137">**説明**</span><span class="sxs-lookup"><span data-stu-id="c9b3f-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c9b3f-138">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="c9b3f-138">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="c9b3f-139">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="c9b3f-139">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c9b3f-140">注釈</span><span class="sxs-lookup"><span data-stu-id="c9b3f-140">Remarks</span></span>

<span data-ttu-id="c9b3f-141">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="c9b3f-141">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="c9b3f-142">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="c9b3f-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c9b3f-143">要素の情報</span><span class="sxs-lookup"><span data-stu-id="c9b3f-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c9b3f-144">Namespace</span><span class="sxs-lookup"><span data-stu-id="c9b3f-144">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c9b3f-145">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c9b3f-145">Schema Name</span></span>  <br/> |<span data-ttu-id="c9b3f-146">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="c9b3f-146">Message schema</span></span>  <br/> |
|<span data-ttu-id="c9b3f-147">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c9b3f-147">Validation File</span></span>  <br/> |<span data-ttu-id="c9b3f-148">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="c9b3f-148">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c9b3f-149">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="c9b3f-149">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="c9b3f-150">関連項目</span><span class="sxs-lookup"><span data-stu-id="c9b3f-150">See also</span></span>



- [<span data-ttu-id="c9b3f-151">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="c9b3f-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

