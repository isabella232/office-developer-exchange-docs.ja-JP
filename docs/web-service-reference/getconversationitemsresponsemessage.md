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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461073"
---
# <a name="getconversationitemsresponsemessage"></a><span data-ttu-id="40922-103">GetConversationItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="40922-103">GetConversationItemsResponseMessage</span></span>

<span data-ttu-id="40922-104">**GetConversationItemsResponseMessage**要素は、 **GetConversationItems**要求の応答メッセージを指定します。</span><span class="sxs-lookup"><span data-stu-id="40922-104">The **GetConversationItemsResponseMessage** element specifies the response message for a **GetConversationItems** request.</span></span> 
  
```XML
<GetConversationItemsResponseMessage ResponseClass="Success | Warning | Error">
    <Conversation/>
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</GetConversationItemsResponseMessage>
```

 <span data-ttu-id="40922-105">**GetConversationItemsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="40922-105">**GetConversationItemsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="40922-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="40922-106">Attributes and elements</span></span>

<span data-ttu-id="40922-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="40922-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="40922-108">属性</span><span class="sxs-lookup"><span data-stu-id="40922-108">Attributes</span></span>

|<span data-ttu-id="40922-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="40922-109">**Attribute**</span></span>|<span data-ttu-id="40922-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="40922-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="40922-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="40922-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="40922-112">応答のクラスを示します。</span><span class="sxs-lookup"><span data-stu-id="40922-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="40922-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="40922-113">ResponseClass</span></span>

|<span data-ttu-id="40922-114">**値**</span><span class="sxs-lookup"><span data-stu-id="40922-114">**Value**</span></span>|<span data-ttu-id="40922-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="40922-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="40922-116">成功</span><span class="sxs-lookup"><span data-stu-id="40922-116">Success</span></span>  <br/> |<span data-ttu-id="40922-117">成功を示します。</span><span class="sxs-lookup"><span data-stu-id="40922-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="40922-118">警告</span><span class="sxs-lookup"><span data-stu-id="40922-118">Warning</span></span>  <br/> |<span data-ttu-id="40922-119">警告を示します。</span><span class="sxs-lookup"><span data-stu-id="40922-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="40922-120">Error</span><span class="sxs-lookup"><span data-stu-id="40922-120">Error</span></span>  <br/> |<span data-ttu-id="40922-121">エラーを示します。</span><span class="sxs-lookup"><span data-stu-id="40922-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="40922-122">子要素</span><span class="sxs-lookup"><span data-stu-id="40922-122">Child elements</span></span>

|<span data-ttu-id="40922-123">**Element**</span><span class="sxs-lookup"><span data-stu-id="40922-123">**Element**</span></span>|<span data-ttu-id="40922-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="40922-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="40922-125">会話 (ConversationResponseType)</span><span class="sxs-lookup"><span data-stu-id="40922-125">Conversation (ConversationResponseType)</span></span>](conversation-conversationresponsetype.md) <br/> |<span data-ttu-id="40922-126">**GetConversationItems**応答で返される1つの会話を表します。</span><span class="sxs-lookup"><span data-stu-id="40922-126">Represents a single conversation returned in a **GetConversationItems** response.</span></span>  <br/> |
|[<span data-ttu-id="40922-127">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="40922-127">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="40922-128">現在未使用で、今後の使用のために予約されています。</span><span class="sxs-lookup"><span data-stu-id="40922-128">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="40922-129">MessageText</span><span class="sxs-lookup"><span data-stu-id="40922-129">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="40922-130">応答の状態を説明するテキストを提供します。</span><span class="sxs-lookup"><span data-stu-id="40922-130">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="40922-131">MessageXml</span><span class="sxs-lookup"><span data-stu-id="40922-131">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="40922-132">エラー応答に関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="40922-132">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="40922-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="40922-133">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="40922-134">要求に関する状態情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="40922-134">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="40922-135">親要素</span><span class="sxs-lookup"><span data-stu-id="40922-135">Parent elements</span></span>

|<span data-ttu-id="40922-136">**要素**</span><span class="sxs-lookup"><span data-stu-id="40922-136">**Element**</span></span>|<span data-ttu-id="40922-137">**説明**</span><span class="sxs-lookup"><span data-stu-id="40922-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="40922-138">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="40922-138">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="40922-139">Exchange Web サービス (EWS) 要求に対する応答メッセージが保存されています。</span><span class="sxs-lookup"><span data-stu-id="40922-139">Contains the response messages for an Exchange Web Services (EWS) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="40922-140">注釈</span><span class="sxs-lookup"><span data-stu-id="40922-140">Remarks</span></span>

<span data-ttu-id="40922-141">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="40922-141">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="40922-142">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="40922-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="40922-143">要素の情報</span><span class="sxs-lookup"><span data-stu-id="40922-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="40922-144">Namespace</span><span class="sxs-lookup"><span data-stu-id="40922-144">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="40922-145">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="40922-145">Schema Name</span></span>  <br/> |<span data-ttu-id="40922-146">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="40922-146">Message schema</span></span>  <br/> |
|<span data-ttu-id="40922-147">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="40922-147">Validation File</span></span>  <br/> |<span data-ttu-id="40922-148">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="40922-148">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="40922-149">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="40922-149">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="40922-150">関連項目</span><span class="sxs-lookup"><span data-stu-id="40922-150">See also</span></span>



- [<span data-ttu-id="40922-151">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="40922-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

