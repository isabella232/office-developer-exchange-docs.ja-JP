---
title: GetConversationItemsResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2e930650-7848-4bf2-a975-026309b3ea02
description: GetConversationItemsResponseMessage 要素は、GetConversationItems 要求の応答メッセージを指定します。
ms.openlocfilehash: b38bca60bb51c24a7635391c4e23e5426366cd72
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461073"
---
# <a name="getconversationitemsresponsemessage"></a><span data-ttu-id="07436-103">GetConversationItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="07436-103">GetConversationItemsResponseMessage</span></span>

<span data-ttu-id="07436-104">**GetConversationItemsResponseMessage**要素は、 **GetConversationItems**要求の応答メッセージを指定します。</span><span class="sxs-lookup"><span data-stu-id="07436-104">The **GetConversationItemsResponseMessage** element specifies the response message for a **GetConversationItems** request.</span></span> 
  
```XML
<GetConversationItemsResponseMessage ResponseClass="Success | Warning | Error">
    <Conversation/>
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</GetConversationItemsResponseMessage>
```

 <span data-ttu-id="07436-105">**GetConversationItemsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="07436-105">**GetConversationItemsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="07436-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="07436-106">Attributes and elements</span></span>

<span data-ttu-id="07436-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="07436-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="07436-108">属性</span><span class="sxs-lookup"><span data-stu-id="07436-108">Attributes</span></span>

|<span data-ttu-id="07436-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="07436-109">**Attribute**</span></span>|<span data-ttu-id="07436-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="07436-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="07436-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="07436-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="07436-112">応答のクラスを示します。</span><span class="sxs-lookup"><span data-stu-id="07436-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="07436-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="07436-113">ResponseClass</span></span>

|<span data-ttu-id="07436-114">**値**</span><span class="sxs-lookup"><span data-stu-id="07436-114">**Value**</span></span>|<span data-ttu-id="07436-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="07436-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="07436-116">Success</span><span class="sxs-lookup"><span data-stu-id="07436-116">Success</span></span>  <br/> |<span data-ttu-id="07436-117">成功を示します。</span><span class="sxs-lookup"><span data-stu-id="07436-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="07436-118">警告</span><span class="sxs-lookup"><span data-stu-id="07436-118">Warning</span></span>  <br/> |<span data-ttu-id="07436-119">警告を示します。</span><span class="sxs-lookup"><span data-stu-id="07436-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="07436-120">Error</span><span class="sxs-lookup"><span data-stu-id="07436-120">Error</span></span>  <br/> |<span data-ttu-id="07436-121">エラーを示します。</span><span class="sxs-lookup"><span data-stu-id="07436-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="07436-122">子要素</span><span class="sxs-lookup"><span data-stu-id="07436-122">Child elements</span></span>

|<span data-ttu-id="07436-123">**Element**</span><span class="sxs-lookup"><span data-stu-id="07436-123">**Element**</span></span>|<span data-ttu-id="07436-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="07436-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="07436-125">会話 (ConversationResponseType)</span><span class="sxs-lookup"><span data-stu-id="07436-125">Conversation (ConversationResponseType)</span></span>](conversation-conversationresponsetype.md) <br/> |<span data-ttu-id="07436-126">**GetConversationItems**応答で返される1つの会話を表します。</span><span class="sxs-lookup"><span data-stu-id="07436-126">Represents a single conversation returned in a **GetConversationItems** response.</span></span>  <br/> |
|[<span data-ttu-id="07436-127">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="07436-127">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="07436-128">現在未使用で、今後の使用のために予約されています。</span><span class="sxs-lookup"><span data-stu-id="07436-128">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="07436-129">MessageText</span><span class="sxs-lookup"><span data-stu-id="07436-129">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="07436-130">応答の状態を説明するテキストを提供します。</span><span class="sxs-lookup"><span data-stu-id="07436-130">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="07436-131">MessageXml</span><span class="sxs-lookup"><span data-stu-id="07436-131">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="07436-132">エラー応答に関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="07436-132">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="07436-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="07436-133">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="07436-134">要求に関する状態情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="07436-134">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="07436-135">親要素</span><span class="sxs-lookup"><span data-stu-id="07436-135">Parent elements</span></span>

|<span data-ttu-id="07436-136">**要素**</span><span class="sxs-lookup"><span data-stu-id="07436-136">**Element**</span></span>|<span data-ttu-id="07436-137">**説明**</span><span class="sxs-lookup"><span data-stu-id="07436-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="07436-138">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="07436-138">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="07436-139">Exchange Web サービス (EWS) 要求に対する応答メッセージが保存されています。</span><span class="sxs-lookup"><span data-stu-id="07436-139">Contains the response messages for an Exchange Web Services (EWS) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="07436-140">注釈</span><span class="sxs-lookup"><span data-stu-id="07436-140">Remarks</span></span>

<span data-ttu-id="07436-141">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="07436-141">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="07436-142">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="07436-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="07436-143">要素の情報</span><span class="sxs-lookup"><span data-stu-id="07436-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="07436-144">Namespace</span><span class="sxs-lookup"><span data-stu-id="07436-144">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="07436-145">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="07436-145">Schema Name</span></span>  <br/> |<span data-ttu-id="07436-146">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="07436-146">Message schema</span></span>  <br/> |
|<span data-ttu-id="07436-147">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="07436-147">Validation File</span></span>  <br/> |<span data-ttu-id="07436-148">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="07436-148">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="07436-149">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="07436-149">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="07436-150">関連項目</span><span class="sxs-lookup"><span data-stu-id="07436-150">See also</span></span>



- [<span data-ttu-id="07436-151">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="07436-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

