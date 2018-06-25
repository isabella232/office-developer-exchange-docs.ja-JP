---
title: ConvertIdResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConvertIdResponseMessage
api_type:
- schema
ms.assetid: 7a439cae-0268-4328-9ded-af56ad642227
description: ConvertIdResponseMessage 要素には、ステータスおよび ConvertId 操作要求の結果が含まれています。
ms.openlocfilehash: 6668c0b3254191ca628413bae5ff957c3cb95b5e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759779"
---
# <a name="convertidresponsemessage"></a><span data-ttu-id="5dbca-103">ConvertIdResponseMessage</span><span class="sxs-lookup"><span data-stu-id="5dbca-103">ConvertIdResponseMessage</span></span>

<span data-ttu-id="5dbca-104">**ConvertIdResponseMessage**要素には、ステータスおよび[ConvertId 操作](convertid-operation.md)要求の結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5dbca-104">The **ConvertIdResponseMessage** element contains the status and result of a [ConvertId operation](convertid-operation.md) request.</span></span> 
  
- [<span data-ttu-id="5dbca-105">ConvertIdResponse</span><span class="sxs-lookup"><span data-stu-id="5dbca-105">ConvertIdResponse</span></span>](convertidresponse.md) 
- [<span data-ttu-id="5dbca-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="5dbca-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="5dbca-107">ConvertIdResponseMessage</span><span class="sxs-lookup"><span data-stu-id="5dbca-107">ConvertIdResponseMessage</span></span>](convertidresponsemessage.md)
  
```xml
<ConvertIdResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <AlternateId/>
</ConvertIdResponseMessage>
```

 <span data-ttu-id="5dbca-108">**ConvertIdResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="5dbca-108">**ConvertIdResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5dbca-109">属性および要素</span><span class="sxs-lookup"><span data-stu-id="5dbca-109">Attributes and elements</span></span>

<span data-ttu-id="5dbca-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5dbca-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5dbca-111">属性</span><span class="sxs-lookup"><span data-stu-id="5dbca-111">Attributes</span></span>

|<span data-ttu-id="5dbca-112">**属性**</span><span class="sxs-lookup"><span data-stu-id="5dbca-112">**Attribute**</span></span>|<span data-ttu-id="5dbca-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="5dbca-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5dbca-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="5dbca-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="5dbca-115">[ConvertId 操作](convertid-operation.md)の応答のステータスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="5dbca-115">Describes the status of a [ConvertId operation](convertid-operation.md) response.</span></span><br/><br/><span data-ttu-id="5dbca-116">次の値は、この属性の有効です。</span><span class="sxs-lookup"><span data-stu-id="5dbca-116">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="5dbca-117">-成功</span><span class="sxs-lookup"><span data-stu-id="5dbca-117">- Success</span></span>  <br/><span data-ttu-id="5dbca-118">-警告</span><span class="sxs-lookup"><span data-stu-id="5dbca-118">-  Warning</span></span>  <br/><span data-ttu-id="5dbca-119">-エラー</span><span class="sxs-lookup"><span data-stu-id="5dbca-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="5dbca-120">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="5dbca-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="5dbca-121">**値**</span><span class="sxs-lookup"><span data-stu-id="5dbca-121">**Value**</span></span>|<span data-ttu-id="5dbca-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="5dbca-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5dbca-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="5dbca-123">**Success**</span></span> <br/> |<span data-ttu-id="5dbca-124">満了する要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="5dbca-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="5dbca-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="5dbca-125">**Warning**</span></span> <br/> | <span data-ttu-id="5dbca-126">完全に処理されていないか、意図しない結果が発生する要求について説明します。</span><span class="sxs-lookup"><span data-stu-id="5dbca-126">Describes a request that was not fully processed or for which an unintended result occurred.</span></span>  <br/> |
|<span data-ttu-id="5dbca-127">**Error**</span><span class="sxs-lookup"><span data-stu-id="5dbca-127">**Error**</span></span> <br/> | <span data-ttu-id="5dbca-128">満たせない要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="5dbca-128">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="5dbca-129">次に、エラーのソースの例を示します。</span><span class="sxs-lookup"><span data-stu-id="5dbca-129">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="5dbca-130">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="5dbca-130">- Invalid attributes or elements</span></span>  <br/><span data-ttu-id="5dbca-131">属性または要素の範囲を超えています。</span><span class="sxs-lookup"><span data-stu-id="5dbca-131">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="5dbca-132">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="5dbca-132">-  An unknown tag</span></span>  <br/><span data-ttu-id="5dbca-133">属性または要素のコンテキストでは有効ではないです。</span><span class="sxs-lookup"><span data-stu-id="5dbca-133">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="5dbca-134">-任意のクライアントから不正なアクセス試行</span><span class="sxs-lookup"><span data-stu-id="5dbca-134">- An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="5dbca-135">-クライアント側の有効な呼び出しへの応答でサーバー側エラー</span><span class="sxs-lookup"><span data-stu-id="5dbca-135">-  A server-side failure in response to a valid client-side call</span></span><br/><br/><span data-ttu-id="5dbca-136">エラーに関する情報は、 [ResponseCode](responsecode.md)および[メッセージ テキスト](messagetext.md)の要素を参照しています。</span><span class="sxs-lookup"><span data-stu-id="5dbca-136">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="5dbca-137">子要素</span><span class="sxs-lookup"><span data-stu-id="5dbca-137">Child elements</span></span>

|<span data-ttu-id="5dbca-138">**要素**</span><span class="sxs-lookup"><span data-stu-id="5dbca-138">**Element**</span></span>|<span data-ttu-id="5dbca-139">**説明**</span><span class="sxs-lookup"><span data-stu-id="5dbca-139">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5dbca-140">MessageText</span><span class="sxs-lookup"><span data-stu-id="5dbca-140">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="5dbca-141">応答のステータスの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="5dbca-141">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="5dbca-142">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="5dbca-142">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="5dbca-143">要求で発生した特定のエラーを識別するエラー コードを提供します。</span><span class="sxs-lookup"><span data-stu-id="5dbca-143">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="5dbca-144">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="5dbca-144">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="5dbca-145">現在使用されていない、将来使用するために予約されています。</span><span class="sxs-lookup"><span data-stu-id="5dbca-145">Currently unused and reserved for future use.</span></span> <span data-ttu-id="5dbca-146">この要素には、0 の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5dbca-146">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="5dbca-147">MessageXml</span><span class="sxs-lookup"><span data-stu-id="5dbca-147">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="5dbca-148">追加のエラー応答情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="5dbca-148">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="5dbca-149">AlternateId</span><span class="sxs-lookup"><span data-stu-id="5dbca-149">AlternateId</span></span>](alternateid.md) <br/> |<span data-ttu-id="5dbca-150">応答に変換された識別子をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="5dbca-150">Describes a converted identifier in the response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5dbca-151">親要素</span><span class="sxs-lookup"><span data-stu-id="5dbca-151">Parent elements</span></span>

|<span data-ttu-id="5dbca-152">**要素**</span><span class="sxs-lookup"><span data-stu-id="5dbca-152">**Element**</span></span>|<span data-ttu-id="5dbca-153">**説明**</span><span class="sxs-lookup"><span data-stu-id="5dbca-153">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5dbca-154">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="5dbca-154">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="5dbca-155">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="5dbca-155">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5dbca-156">備考</span><span class="sxs-lookup"><span data-stu-id="5dbca-156">Remarks</span></span>

<span data-ttu-id="5dbca-157">変換後の id ごとに 1 つの応答メッセージが返されます。</span><span class="sxs-lookup"><span data-stu-id="5dbca-157">One response message per converted identifier is returned.</span></span> <span data-ttu-id="5dbca-158">エラー応答コードが返された場合に、 [AlternateId](alternateid.md)要素が応答から消失します。</span><span class="sxs-lookup"><span data-stu-id="5dbca-158">The [AlternateId](alternateid.md) element will be missing from the response if an error response code is returned,</span></span> 
  
<span data-ttu-id="5dbca-159">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Exchange 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="5dbca-159">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5dbca-160">要素情報</span><span class="sxs-lookup"><span data-stu-id="5dbca-160">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5dbca-161">名前空間</span><span class="sxs-lookup"><span data-stu-id="5dbca-161">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5dbca-162">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5dbca-162">Schema Name</span></span>  <br/> |<span data-ttu-id="5dbca-163">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="5dbca-163">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5dbca-164">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5dbca-164">Validation File</span></span>  <br/> |<span data-ttu-id="5dbca-165">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="5dbca-165">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5dbca-166">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="5dbca-166">Can be Empty</span></span>  <br/> |<span data-ttu-id="5dbca-167">False</span><span class="sxs-lookup"><span data-stu-id="5dbca-167">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5dbca-168">関連項目</span><span class="sxs-lookup"><span data-stu-id="5dbca-168">See also</span></span>

- [<span data-ttu-id="5dbca-169">ConvertId 操作</span><span class="sxs-lookup"><span data-stu-id="5dbca-169">ConvertId operation</span></span>](convertid-operation.md)
- [<span data-ttu-id="5dbca-170">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="5dbca-170">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

