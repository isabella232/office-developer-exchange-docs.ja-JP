---
title: FindPeopleResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 95f016a9-002f-4be3-abd6-f5e3528afd44
description: FindPeopleResponse 要素は、FindPeople 要求への応答を指定します。
ms.openlocfilehash: 4f2c2f6069a515d5153ea488b35182d8b35f029f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760533"
---
# <a name="findpeopleresponse"></a><span data-ttu-id="588ae-103">FindPeopleResponse</span><span class="sxs-lookup"><span data-stu-id="588ae-103">FindPeopleResponse</span></span>

<span data-ttu-id="588ae-104">**FindPeopleResponse**要素は、 **FindPeople**要求への応答を指定します。</span><span class="sxs-lookup"><span data-stu-id="588ae-104">The **FindPeopleResponse** element specifies the response to a **FindPeople** request.</span></span> 
  
```XML
<FindPeopleResponse ResponseClass=" Success | Warning | Error ">
    <People/>
    <TotalNumberOfPeopleInView/>
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</FindPeopleResponse>
```

 <span data-ttu-id="588ae-105">**FindPeopleResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="588ae-105">**FindPeopleResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="588ae-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="588ae-106">Attributes and elements</span></span>

<span data-ttu-id="588ae-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="588ae-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="588ae-108">属性</span><span class="sxs-lookup"><span data-stu-id="588ae-108">Attributes</span></span>

|<span data-ttu-id="588ae-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="588ae-109">**Attribute**</span></span>|<span data-ttu-id="588ae-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="588ae-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="588ae-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="588ae-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="588ae-112">応答クラスを指定します。</span><span class="sxs-lookup"><span data-stu-id="588ae-112">Specifies the response class.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="588ae-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="588ae-113">ResponseClass</span></span>

|<span data-ttu-id="588ae-114">**値**</span><span class="sxs-lookup"><span data-stu-id="588ae-114">**Value**</span></span>|<span data-ttu-id="588ae-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="588ae-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="588ae-116">成功</span><span class="sxs-lookup"><span data-stu-id="588ae-116">Success</span></span>  <br/> |<span data-ttu-id="588ae-117">成功を示します。</span><span class="sxs-lookup"><span data-stu-id="588ae-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="588ae-118">警告</span><span class="sxs-lookup"><span data-stu-id="588ae-118">Warning</span></span>  <br/> |<span data-ttu-id="588ae-119">警告を示します。</span><span class="sxs-lookup"><span data-stu-id="588ae-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="588ae-120">エラー</span><span class="sxs-lookup"><span data-stu-id="588ae-120">Error</span></span>  <br/> |<span data-ttu-id="588ae-121">エラーを示します。</span><span class="sxs-lookup"><span data-stu-id="588ae-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="588ae-122">子要素</span><span class="sxs-lookup"><span data-stu-id="588ae-122">Child elements</span></span>

|<span data-ttu-id="588ae-123">**要素**</span><span class="sxs-lookup"><span data-stu-id="588ae-123">**Element**</span></span>|<span data-ttu-id="588ae-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="588ae-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="588ae-125">連絡先</span><span class="sxs-lookup"><span data-stu-id="588ae-125">People</span></span>](people.md) <br/> |<span data-ttu-id="588ae-126">**FindPeople**要求の結果として返されるペルソナ データの配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="588ae-126">Specifies an array of persona data returned as the result of a **FindPeople** request.</span></span>  <br/> |
|[<span data-ttu-id="588ae-127">TotalNumberOfPeopleInView</span><span class="sxs-lookup"><span data-stu-id="588ae-127">TotalNumberOfPeopleInView</span></span>](totalnumberofpeopleinview.md) <br/> |<span data-ttu-id="588ae-128">**FindPeople**の要求によって返されるサーバーに格納されているペルソナの合計数を指定します。</span><span class="sxs-lookup"><span data-stu-id="588ae-128">Specifies the total number of personas stored on a server that are returned by a **FindPeople** request.</span></span>  <br/> |
|[<span data-ttu-id="588ae-129">MessageText</span><span class="sxs-lookup"><span data-stu-id="588ae-129">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="588ae-130">応答のステータスの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="588ae-130">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="588ae-131">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="588ae-131">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="588ae-132">要求に関するステータス情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="588ae-132">Provides status information about the request.</span></span>  <br/> |
|[<span data-ttu-id="588ae-133">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="588ae-133">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="588ae-134">現在使用されていない、将来使用するために予約されています。</span><span class="sxs-lookup"><span data-stu-id="588ae-134">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="588ae-135">MessageXml</span><span class="sxs-lookup"><span data-stu-id="588ae-135">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="588ae-136">追加のエラー応答情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="588ae-136">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="588ae-137">親要素</span><span class="sxs-lookup"><span data-stu-id="588ae-137">Parent elements</span></span>

|<span data-ttu-id="588ae-138">**要素**</span><span class="sxs-lookup"><span data-stu-id="588ae-138">**Element**</span></span>|<span data-ttu-id="588ae-139">**説明**</span><span class="sxs-lookup"><span data-stu-id="588ae-139">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="588ae-140">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="588ae-140">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="588ae-141">応答メッセージの配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="588ae-141">Specifies an array of response messages.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="588ae-142">備考</span><span class="sxs-lookup"><span data-stu-id="588ae-142">Remarks</span></span>

<span data-ttu-id="588ae-143">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="588ae-143">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="588ae-144">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="588ae-144">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="588ae-145">要素情報</span><span class="sxs-lookup"><span data-stu-id="588ae-145">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="588ae-146">名前空間</span><span class="sxs-lookup"><span data-stu-id="588ae-146">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="588ae-147">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="588ae-147">Schema Name</span></span>  <br/> |<span data-ttu-id="588ae-148">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="588ae-148">Message schema</span></span>  <br/> |
|<span data-ttu-id="588ae-149">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="588ae-149">Validation File</span></span>  <br/> |<span data-ttu-id="588ae-150">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="588ae-150">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="588ae-151">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="588ae-151">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="588ae-152">関連項目</span><span class="sxs-lookup"><span data-stu-id="588ae-152">See also</span></span>



- [<span data-ttu-id="588ae-153">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="588ae-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

