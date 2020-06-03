---
title: GetAppManifestsResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 815908f1-4223-42d8-92dc-f8bdfc6b5df8
description: GetAppManifestsResponseMessage 要素は、GetAppManifests 要求の応答メッセージを指定します。
ms.openlocfilehash: 26a521d8647a010fe956596eaf63d4df4756edb2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459533"
---
# <a name="getappmanifestsresponsemessage"></a><span data-ttu-id="a2a36-103">GetAppManifestsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="a2a36-103">GetAppManifestsResponseMessage</span></span>

<span data-ttu-id="a2a36-104">**GetAppManifestsResponseMessage**要素は、 **getappmanifests**要求の応答メッセージを指定します。</span><span class="sxs-lookup"><span data-stu-id="a2a36-104">The **GetAppManifestsResponseMessage** element specifies the response message for a **GetAppManifests** request.</span></span> 
  
```XML
<GetAppManifestsResponseMessage ResponseClass=" Success | Warning | Error ">
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</GetAppManifestsResponseMessage>
```

 <span data-ttu-id="a2a36-105">**ResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="a2a36-105">**ResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a2a36-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="a2a36-106">Attributes and elements</span></span>

<span data-ttu-id="a2a36-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a2a36-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a2a36-108">属性</span><span class="sxs-lookup"><span data-stu-id="a2a36-108">Attributes</span></span>

|<span data-ttu-id="a2a36-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="a2a36-109">**Attribute**</span></span>|<span data-ttu-id="a2a36-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="a2a36-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a2a36-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="a2a36-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="a2a36-112">応答のクラスを示します。</span><span class="sxs-lookup"><span data-stu-id="a2a36-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="a2a36-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="a2a36-113">ResponseClass</span></span>

|<span data-ttu-id="a2a36-114">**値**</span><span class="sxs-lookup"><span data-stu-id="a2a36-114">**Value**</span></span>|<span data-ttu-id="a2a36-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="a2a36-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a2a36-116">成功</span><span class="sxs-lookup"><span data-stu-id="a2a36-116">Success</span></span>  <br/> |<span data-ttu-id="a2a36-117">成功を示します。</span><span class="sxs-lookup"><span data-stu-id="a2a36-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="a2a36-118">警告</span><span class="sxs-lookup"><span data-stu-id="a2a36-118">Warning</span></span>  <br/> |<span data-ttu-id="a2a36-119">警告を示します。</span><span class="sxs-lookup"><span data-stu-id="a2a36-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="a2a36-120">Error</span><span class="sxs-lookup"><span data-stu-id="a2a36-120">Error</span></span>  <br/> |<span data-ttu-id="a2a36-121">エラーを示します。</span><span class="sxs-lookup"><span data-stu-id="a2a36-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="a2a36-122">子要素</span><span class="sxs-lookup"><span data-stu-id="a2a36-122">Child elements</span></span>

|<span data-ttu-id="a2a36-123">**Element**</span><span class="sxs-lookup"><span data-stu-id="a2a36-123">**Element**</span></span>|<span data-ttu-id="a2a36-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="a2a36-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a2a36-125">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="a2a36-125">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="a2a36-126">現在未使用で、今後の使用のために予約されています。</span><span class="sxs-lookup"><span data-stu-id="a2a36-126">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="a2a36-127">MessageText</span><span class="sxs-lookup"><span data-stu-id="a2a36-127">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="a2a36-128">応答の状態を説明するテキストを提供します。</span><span class="sxs-lookup"><span data-stu-id="a2a36-128">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="a2a36-129">MessageXml</span><span class="sxs-lookup"><span data-stu-id="a2a36-129">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="a2a36-130">エラー応答に関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="a2a36-130">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="a2a36-131">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="a2a36-131">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="a2a36-132">要求に関する状態情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="a2a36-132">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a2a36-133">親要素</span><span class="sxs-lookup"><span data-stu-id="a2a36-133">Parent elements</span></span>

|<span data-ttu-id="a2a36-134">**要素**</span><span class="sxs-lookup"><span data-stu-id="a2a36-134">**Element**</span></span>|<span data-ttu-id="a2a36-135">**説明**</span><span class="sxs-lookup"><span data-stu-id="a2a36-135">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a2a36-136">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="a2a36-136">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="a2a36-137">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="a2a36-137">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a2a36-138">注釈</span><span class="sxs-lookup"><span data-stu-id="a2a36-138">Remarks</span></span>

<span data-ttu-id="a2a36-139">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="a2a36-139">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="a2a36-140">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="a2a36-140">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a2a36-141">要素の情報</span><span class="sxs-lookup"><span data-stu-id="a2a36-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a2a36-142">Namespace</span><span class="sxs-lookup"><span data-stu-id="a2a36-142">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a2a36-143">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a2a36-143">Schema Name</span></span>  <br/> |<span data-ttu-id="a2a36-144">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="a2a36-144">Message schema</span></span>  <br/> |
|<span data-ttu-id="a2a36-145">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a2a36-145">Validation File</span></span>  <br/> |<span data-ttu-id="a2a36-146">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="a2a36-146">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a2a36-147">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="a2a36-147">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="a2a36-148">関連項目</span><span class="sxs-lookup"><span data-stu-id="a2a36-148">See also</span></span>



- [<span data-ttu-id="a2a36-149">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="a2a36-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

