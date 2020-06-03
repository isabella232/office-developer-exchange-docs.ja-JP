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
ms.openlocfilehash: b969ac3f7bc2bbd3fc77bf753a15696c3b6d8216
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466403"
---
# <a name="findpeopleresponse"></a><span data-ttu-id="0cbea-103">FindPeopleResponse</span><span class="sxs-lookup"><span data-stu-id="0cbea-103">FindPeopleResponse</span></span>

<span data-ttu-id="0cbea-104">**FindPeopleResponse**要素は、 **findpeople**要求への応答を指定します。</span><span class="sxs-lookup"><span data-stu-id="0cbea-104">The **FindPeopleResponse** element specifies the response to a **FindPeople** request.</span></span> 
  
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

 <span data-ttu-id="0cbea-105">**FindPeopleResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="0cbea-105">**FindPeopleResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0cbea-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="0cbea-106">Attributes and elements</span></span>

<span data-ttu-id="0cbea-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0cbea-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0cbea-108">属性</span><span class="sxs-lookup"><span data-stu-id="0cbea-108">Attributes</span></span>

|<span data-ttu-id="0cbea-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="0cbea-109">**Attribute**</span></span>|<span data-ttu-id="0cbea-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="0cbea-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0cbea-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="0cbea-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="0cbea-112">Response クラスを指定します。</span><span class="sxs-lookup"><span data-stu-id="0cbea-112">Specifies the response class.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="0cbea-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="0cbea-113">ResponseClass</span></span>

|<span data-ttu-id="0cbea-114">**値**</span><span class="sxs-lookup"><span data-stu-id="0cbea-114">**Value**</span></span>|<span data-ttu-id="0cbea-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="0cbea-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0cbea-116">成功</span><span class="sxs-lookup"><span data-stu-id="0cbea-116">Success</span></span>  <br/> |<span data-ttu-id="0cbea-117">成功を示します。</span><span class="sxs-lookup"><span data-stu-id="0cbea-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="0cbea-118">警告</span><span class="sxs-lookup"><span data-stu-id="0cbea-118">Warning</span></span>  <br/> |<span data-ttu-id="0cbea-119">警告を示します。</span><span class="sxs-lookup"><span data-stu-id="0cbea-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="0cbea-120">Error</span><span class="sxs-lookup"><span data-stu-id="0cbea-120">Error</span></span>  <br/> |<span data-ttu-id="0cbea-121">エラーを示します。</span><span class="sxs-lookup"><span data-stu-id="0cbea-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="0cbea-122">子要素</span><span class="sxs-lookup"><span data-stu-id="0cbea-122">Child elements</span></span>

|<span data-ttu-id="0cbea-123">**Element**</span><span class="sxs-lookup"><span data-stu-id="0cbea-123">**Element**</span></span>|<span data-ttu-id="0cbea-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="0cbea-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0cbea-125">ユーザー</span><span class="sxs-lookup"><span data-stu-id="0cbea-125">People</span></span>](people.md) <br/> |<span data-ttu-id="0cbea-126">**Findpeople**要求の結果として返される persona data の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="0cbea-126">Specifies an array of persona data returned as the result of a **FindPeople** request.</span></span>  <br/> |
|[<span data-ttu-id="0cbea-127">TotalNumberOfPeopleInView</span><span class="sxs-lookup"><span data-stu-id="0cbea-127">TotalNumberOfPeopleInView</span></span>](totalnumberofpeopleinview.md) <br/> |<span data-ttu-id="0cbea-128">**Findpeople**要求によって返されたサーバーに格納されているペルソナの合計数を指定します。</span><span class="sxs-lookup"><span data-stu-id="0cbea-128">Specifies the total number of personas stored on a server that are returned by a **FindPeople** request.</span></span>  <br/> |
|[<span data-ttu-id="0cbea-129">MessageText</span><span class="sxs-lookup"><span data-stu-id="0cbea-129">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="0cbea-130">応答の状態を説明するテキストを提供します。</span><span class="sxs-lookup"><span data-stu-id="0cbea-130">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="0cbea-131">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="0cbea-131">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="0cbea-132">要求に関する状態情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="0cbea-132">Provides status information about the request.</span></span>  <br/> |
|[<span data-ttu-id="0cbea-133">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="0cbea-133">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="0cbea-134">現在未使用で、今後の使用のために予約されています。</span><span class="sxs-lookup"><span data-stu-id="0cbea-134">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="0cbea-135">MessageXml</span><span class="sxs-lookup"><span data-stu-id="0cbea-135">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="0cbea-136">エラー応答に関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="0cbea-136">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0cbea-137">親要素</span><span class="sxs-lookup"><span data-stu-id="0cbea-137">Parent elements</span></span>

|<span data-ttu-id="0cbea-138">**要素**</span><span class="sxs-lookup"><span data-stu-id="0cbea-138">**Element**</span></span>|<span data-ttu-id="0cbea-139">**説明**</span><span class="sxs-lookup"><span data-stu-id="0cbea-139">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0cbea-140">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="0cbea-140">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="0cbea-141">応答メッセージの配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="0cbea-141">Specifies an array of response messages.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0cbea-142">注釈</span><span class="sxs-lookup"><span data-stu-id="0cbea-142">Remarks</span></span>

<span data-ttu-id="0cbea-143">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="0cbea-143">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="0cbea-144">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="0cbea-144">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0cbea-145">要素の情報</span><span class="sxs-lookup"><span data-stu-id="0cbea-145">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0cbea-146">Namespace</span><span class="sxs-lookup"><span data-stu-id="0cbea-146">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0cbea-147">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0cbea-147">Schema Name</span></span>  <br/> |<span data-ttu-id="0cbea-148">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="0cbea-148">Message schema</span></span>  <br/> |
|<span data-ttu-id="0cbea-149">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0cbea-149">Validation File</span></span>  <br/> |<span data-ttu-id="0cbea-150">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="0cbea-150">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0cbea-151">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="0cbea-151">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="0cbea-152">関連項目</span><span class="sxs-lookup"><span data-stu-id="0cbea-152">See also</span></span>



- [<span data-ttu-id="0cbea-153">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="0cbea-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

