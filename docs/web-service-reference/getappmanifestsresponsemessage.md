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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459533"
---
# <a name="getappmanifestsresponsemessage"></a><span data-ttu-id="fde31-103">GetAppManifestsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="fde31-103">GetAppManifestsResponseMessage</span></span>

<span data-ttu-id="fde31-104">**GetAppManifestsResponseMessage**要素は、 **getappmanifests**要求の応答メッセージを指定します。</span><span class="sxs-lookup"><span data-stu-id="fde31-104">The **GetAppManifestsResponseMessage** element specifies the response message for a **GetAppManifests** request.</span></span> 
  
```XML
<GetAppManifestsResponseMessage ResponseClass=" Success | Warning | Error ">
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</GetAppManifestsResponseMessage>
```

 <span data-ttu-id="fde31-105">**ResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="fde31-105">**ResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fde31-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="fde31-106">Attributes and elements</span></span>

<span data-ttu-id="fde31-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="fde31-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fde31-108">属性</span><span class="sxs-lookup"><span data-stu-id="fde31-108">Attributes</span></span>

|<span data-ttu-id="fde31-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="fde31-109">**Attribute**</span></span>|<span data-ttu-id="fde31-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="fde31-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="fde31-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="fde31-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="fde31-112">応答のクラスを示します。</span><span class="sxs-lookup"><span data-stu-id="fde31-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="fde31-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="fde31-113">ResponseClass</span></span>

|<span data-ttu-id="fde31-114">**値**</span><span class="sxs-lookup"><span data-stu-id="fde31-114">**Value**</span></span>|<span data-ttu-id="fde31-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="fde31-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="fde31-116">Success</span><span class="sxs-lookup"><span data-stu-id="fde31-116">Success</span></span>  <br/> |<span data-ttu-id="fde31-117">成功を示します。</span><span class="sxs-lookup"><span data-stu-id="fde31-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="fde31-118">警告</span><span class="sxs-lookup"><span data-stu-id="fde31-118">Warning</span></span>  <br/> |<span data-ttu-id="fde31-119">警告を示します。</span><span class="sxs-lookup"><span data-stu-id="fde31-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="fde31-120">Error</span><span class="sxs-lookup"><span data-stu-id="fde31-120">Error</span></span>  <br/> |<span data-ttu-id="fde31-121">エラーを示します。</span><span class="sxs-lookup"><span data-stu-id="fde31-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="fde31-122">子要素</span><span class="sxs-lookup"><span data-stu-id="fde31-122">Child elements</span></span>

|<span data-ttu-id="fde31-123">**Element**</span><span class="sxs-lookup"><span data-stu-id="fde31-123">**Element**</span></span>|<span data-ttu-id="fde31-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="fde31-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fde31-125">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="fde31-125">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="fde31-126">現在未使用で、今後の使用のために予約されています。</span><span class="sxs-lookup"><span data-stu-id="fde31-126">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="fde31-127">MessageText</span><span class="sxs-lookup"><span data-stu-id="fde31-127">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="fde31-128">応答の状態を説明するテキストを提供します。</span><span class="sxs-lookup"><span data-stu-id="fde31-128">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="fde31-129">MessageXml</span><span class="sxs-lookup"><span data-stu-id="fde31-129">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="fde31-130">エラー応答に関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="fde31-130">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="fde31-131">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="fde31-131">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="fde31-132">要求に関する状態情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="fde31-132">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fde31-133">親要素</span><span class="sxs-lookup"><span data-stu-id="fde31-133">Parent elements</span></span>

|<span data-ttu-id="fde31-134">**要素**</span><span class="sxs-lookup"><span data-stu-id="fde31-134">**Element**</span></span>|<span data-ttu-id="fde31-135">**説明**</span><span class="sxs-lookup"><span data-stu-id="fde31-135">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fde31-136">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="fde31-136">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="fde31-137">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="fde31-137">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="fde31-138">注釈</span><span class="sxs-lookup"><span data-stu-id="fde31-138">Remarks</span></span>

<span data-ttu-id="fde31-139">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="fde31-139">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="fde31-140">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="fde31-140">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fde31-141">要素の情報</span><span class="sxs-lookup"><span data-stu-id="fde31-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fde31-142">Namespace</span><span class="sxs-lookup"><span data-stu-id="fde31-142">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="fde31-143">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="fde31-143">Schema Name</span></span>  <br/> |<span data-ttu-id="fde31-144">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="fde31-144">Message schema</span></span>  <br/> |
|<span data-ttu-id="fde31-145">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="fde31-145">Validation File</span></span>  <br/> |<span data-ttu-id="fde31-146">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="fde31-146">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fde31-147">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="fde31-147">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="fde31-148">関連項目</span><span class="sxs-lookup"><span data-stu-id="fde31-148">See also</span></span>



- [<span data-ttu-id="fde31-149">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="fde31-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

