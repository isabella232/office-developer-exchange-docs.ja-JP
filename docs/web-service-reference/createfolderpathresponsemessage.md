---
title: CreateFolderPathResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0f7b3507-713d-4ccf-8518-75fa6f967d6d
description: CreateFolderPathResponseMessage 要素は、CreateFolderPath 要求の応答メッセージを指定します。
ms.openlocfilehash: f8f85cc246bb5d5ecd5cb745267d9d373286cf7a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759820"
---
# <a name="createfolderpathresponsemessage"></a><span data-ttu-id="ae784-103">CreateFolderPathResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ae784-103">CreateFolderPathResponseMessage</span></span>

<span data-ttu-id="ae784-104">**CreateFolderPathResponseMessage**要素は、 **CreateFolderPath**要求の応答メッセージを指定します。</span><span class="sxs-lookup"><span data-stu-id="ae784-104">The **CreateFolderPathResponseMessage** element specifies the response message for a **CreateFolderPath** request.</span></span> 
  
```XML
<CreateFolderPathResponseMessage ResponseClass="">
    <Folders></Folders>
    <MessageText></MessageText>
    <ResponseCode></ResponseCode>
    <DescriptiveLinkKey></DescriptiveLinkKey>
    <MessageXml></MessageXml>
</CreateFolderPathResponseMessage>
```

 <span data-ttu-id="ae784-105">**FolderInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="ae784-105">**FolderInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ae784-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="ae784-106">Attributes and elements</span></span>

<span data-ttu-id="ae784-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ae784-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ae784-108">属性</span><span class="sxs-lookup"><span data-stu-id="ae784-108">Attributes</span></span>

|<span data-ttu-id="ae784-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="ae784-109">**Attribute**</span></span>|<span data-ttu-id="ae784-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="ae784-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ae784-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="ae784-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="ae784-112">応答のクラスを示します。</span><span class="sxs-lookup"><span data-stu-id="ae784-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="ae784-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="ae784-113">ResponseClass</span></span>

|<span data-ttu-id="ae784-114">**値**</span><span class="sxs-lookup"><span data-stu-id="ae784-114">**Value**</span></span>|<span data-ttu-id="ae784-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="ae784-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ae784-116">成功</span><span class="sxs-lookup"><span data-stu-id="ae784-116">Success</span></span>  <br/> |<span data-ttu-id="ae784-117">成功を示します。</span><span class="sxs-lookup"><span data-stu-id="ae784-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="ae784-118">警告</span><span class="sxs-lookup"><span data-stu-id="ae784-118">Warning</span></span>  <br/> |<span data-ttu-id="ae784-119">警告を示します。</span><span class="sxs-lookup"><span data-stu-id="ae784-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="ae784-120">エラー</span><span class="sxs-lookup"><span data-stu-id="ae784-120">Error</span></span>  <br/> |<span data-ttu-id="ae784-121">エラーを示します。</span><span class="sxs-lookup"><span data-stu-id="ae784-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="ae784-122">子要素</span><span class="sxs-lookup"><span data-stu-id="ae784-122">Child elements</span></span>

|<span data-ttu-id="ae784-123">**要素**</span><span class="sxs-lookup"><span data-stu-id="ae784-123">**Element**</span></span>|<span data-ttu-id="ae784-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="ae784-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ae784-125">フォルダー</span><span class="sxs-lookup"><span data-stu-id="ae784-125">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="ae784-126">フォルダーの操作で使用されているフォルダーの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ae784-126">Contains an array of folders that are used in folder operations.</span></span>  <br/> |
|[<span data-ttu-id="ae784-127">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="ae784-127">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="ae784-128">現在使用されていない、将来使用するために予約されています。</span><span class="sxs-lookup"><span data-stu-id="ae784-128">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="ae784-129">MessageText</span><span class="sxs-lookup"><span data-stu-id="ae784-129">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="ae784-130">応答のステータスの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="ae784-130">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="ae784-131">MessageXml</span><span class="sxs-lookup"><span data-stu-id="ae784-131">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="ae784-132">追加のエラー応答情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="ae784-132">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="ae784-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="ae784-133">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="ae784-134">要求に関するステータス情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="ae784-134">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ae784-135">親要素</span><span class="sxs-lookup"><span data-stu-id="ae784-135">Parent elements</span></span>

|<span data-ttu-id="ae784-136">**要素**</span><span class="sxs-lookup"><span data-stu-id="ae784-136">**Element**</span></span>|<span data-ttu-id="ae784-137">**説明**</span><span class="sxs-lookup"><span data-stu-id="ae784-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ae784-138">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="ae784-138">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="ae784-139">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="ae784-139">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ae784-140">備考</span><span class="sxs-lookup"><span data-stu-id="ae784-140">Remarks</span></span>

<span data-ttu-id="ae784-141">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="ae784-141">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="ae784-142">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="ae784-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ae784-143">要素情報</span><span class="sxs-lookup"><span data-stu-id="ae784-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ae784-144">名前空間</span><span class="sxs-lookup"><span data-stu-id="ae784-144">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ae784-145">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ae784-145">Schema Name</span></span>  <br/> |<span data-ttu-id="ae784-146">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="ae784-146">Message schema</span></span>  <br/> |
|<span data-ttu-id="ae784-147">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ae784-147">Validation File</span></span>  <br/> |<span data-ttu-id="ae784-148">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ae784-148">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ae784-149">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="ae784-149">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="ae784-150">関連項目</span><span class="sxs-lookup"><span data-stu-id="ae784-150">See also</span></span>

- [<span data-ttu-id="ae784-151">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="ae784-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

