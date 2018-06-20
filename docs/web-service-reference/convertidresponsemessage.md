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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759779"
---
# <a name="convertidresponsemessage"></a><span data-ttu-id="852e5-103">ConvertIdResponseMessage</span><span class="sxs-lookup"><span data-stu-id="852e5-103">ConvertIdResponseMessage</span></span>

<span data-ttu-id="852e5-104">**ConvertIdResponseMessage**要素には、ステータスおよび[ConvertId 操作](convertid-operation.md)要求の結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="852e5-104">The **ConvertIdResponseMessage** element contains the status and result of a [ConvertId operation](convertid-operation.md) request.</span></span> 
  
- [<span data-ttu-id="852e5-105">ConvertIdResponse</span><span class="sxs-lookup"><span data-stu-id="852e5-105">ConvertIdResponse</span></span>](convertidresponse.md) 
- [<span data-ttu-id="852e5-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="852e5-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="852e5-107">ConvertIdResponseMessage</span><span class="sxs-lookup"><span data-stu-id="852e5-107">ConvertIdResponseMessage</span></span>](convertidresponsemessage.md)
  
```xml
<ConvertIdResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <AlternateId/>
</ConvertIdResponseMessage>
```

 <span data-ttu-id="852e5-108">**ConvertIdResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="852e5-108">**ConvertIdResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="852e5-109">属性および要素</span><span class="sxs-lookup"><span data-stu-id="852e5-109">Attributes and elements</span></span>

<span data-ttu-id="852e5-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="852e5-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="852e5-111">属性</span><span class="sxs-lookup"><span data-stu-id="852e5-111">Attributes</span></span>

|<span data-ttu-id="852e5-112">**属性**</span><span class="sxs-lookup"><span data-stu-id="852e5-112">**Attribute**</span></span>|<span data-ttu-id="852e5-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="852e5-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="852e5-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="852e5-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="852e5-115">[ConvertId 操作](convertid-operation.md)の応答のステータスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="852e5-115">Describes the status of a [ConvertId operation](convertid-operation.md) response.</span></span><br/><br/><span data-ttu-id="852e5-116">次の値は、この属性の有効です。</span><span class="sxs-lookup"><span data-stu-id="852e5-116">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="852e5-117">-成功</span><span class="sxs-lookup"><span data-stu-id="852e5-117">- Success</span></span>  <br/><span data-ttu-id="852e5-118">-警告</span><span class="sxs-lookup"><span data-stu-id="852e5-118">-  Warning</span></span>  <br/><span data-ttu-id="852e5-119">-エラー</span><span class="sxs-lookup"><span data-stu-id="852e5-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="852e5-120">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="852e5-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="852e5-121">**値**</span><span class="sxs-lookup"><span data-stu-id="852e5-121">**Value**</span></span>|<span data-ttu-id="852e5-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="852e5-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="852e5-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="852e5-123">**Success**</span></span> <br/> |<span data-ttu-id="852e5-124">満了する要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="852e5-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="852e5-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="852e5-125">**Warning**</span></span> <br/> | <span data-ttu-id="852e5-126">完全に処理されていないか、意図しない結果が発生する要求について説明します。</span><span class="sxs-lookup"><span data-stu-id="852e5-126">Describes a request that was not fully processed or for which an unintended result occurred.</span></span>  <br/> |
|<span data-ttu-id="852e5-127">**Error**</span><span class="sxs-lookup"><span data-stu-id="852e5-127">**Error**</span></span> <br/> | <span data-ttu-id="852e5-128">満たせない要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="852e5-128">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="852e5-129">次に、エラーのソースの例を示します。</span><span class="sxs-lookup"><span data-stu-id="852e5-129">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="852e5-130">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="852e5-130">- Invalid attributes or elements</span></span>  <br/><span data-ttu-id="852e5-131">属性または要素の範囲を超えています。</span><span class="sxs-lookup"><span data-stu-id="852e5-131">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="852e5-132">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="852e5-132">-  An unknown tag</span></span>  <br/><span data-ttu-id="852e5-133">属性または要素のコンテキストでは有効ではないです。</span><span class="sxs-lookup"><span data-stu-id="852e5-133">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="852e5-134">-任意のクライアントから不正なアクセス試行</span><span class="sxs-lookup"><span data-stu-id="852e5-134">- An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="852e5-135">-クライアント側の有効な呼び出しへの応答でサーバー側エラー</span><span class="sxs-lookup"><span data-stu-id="852e5-135">-  A server-side failure in response to a valid client-side call</span></span><br/><br/><span data-ttu-id="852e5-136">エラーに関する情報は、 [ResponseCode](responsecode.md)および[メッセージ テキスト](messagetext.md)の要素を参照しています。</span><span class="sxs-lookup"><span data-stu-id="852e5-136">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="852e5-137">子要素</span><span class="sxs-lookup"><span data-stu-id="852e5-137">Child elements</span></span>

|<span data-ttu-id="852e5-138">**要素**</span><span class="sxs-lookup"><span data-stu-id="852e5-138">**Element**</span></span>|<span data-ttu-id="852e5-139">**説明**</span><span class="sxs-lookup"><span data-stu-id="852e5-139">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="852e5-140">MessageText</span><span class="sxs-lookup"><span data-stu-id="852e5-140">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="852e5-141">応答のステータスの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="852e5-141">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="852e5-142">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="852e5-142">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="852e5-143">要求で発生した特定のエラーを識別するエラー コードを提供します。</span><span class="sxs-lookup"><span data-stu-id="852e5-143">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="852e5-144">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="852e5-144">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="852e5-145">現在使用されていない、将来使用するために予約されています。</span><span class="sxs-lookup"><span data-stu-id="852e5-145">Currently unused and reserved for future use.</span></span> <span data-ttu-id="852e5-146">この要素には、0 の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="852e5-146">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="852e5-147">MessageXml</span><span class="sxs-lookup"><span data-stu-id="852e5-147">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="852e5-148">追加のエラー応答情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="852e5-148">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="852e5-149">AlternateId</span><span class="sxs-lookup"><span data-stu-id="852e5-149">AlternateId</span></span>](alternateid.md) <br/> |<span data-ttu-id="852e5-150">応答に変換された識別子をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="852e5-150">Describes a converted identifier in the response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="852e5-151">親要素</span><span class="sxs-lookup"><span data-stu-id="852e5-151">Parent elements</span></span>

|<span data-ttu-id="852e5-152">**要素**</span><span class="sxs-lookup"><span data-stu-id="852e5-152">**Element**</span></span>|<span data-ttu-id="852e5-153">**説明**</span><span class="sxs-lookup"><span data-stu-id="852e5-153">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="852e5-154">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="852e5-154">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="852e5-155">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="852e5-155">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="852e5-156">備考</span><span class="sxs-lookup"><span data-stu-id="852e5-156">Remarks</span></span>

<span data-ttu-id="852e5-157">変換後の id ごとに 1 つの応答メッセージが返されます。</span><span class="sxs-lookup"><span data-stu-id="852e5-157">One response message per converted identifier is returned.</span></span> <span data-ttu-id="852e5-158">エラー応答コードが返された場合に、 [AlternateId](alternateid.md)要素が応答から消失します。</span><span class="sxs-lookup"><span data-stu-id="852e5-158">The [AlternateId](alternateid.md) element will be missing from the response if an error response code is returned,</span></span> 
  
<span data-ttu-id="852e5-159">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Exchange 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="852e5-159">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="852e5-160">要素情報</span><span class="sxs-lookup"><span data-stu-id="852e5-160">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="852e5-161">名前空間</span><span class="sxs-lookup"><span data-stu-id="852e5-161">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="852e5-162">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="852e5-162">Schema Name</span></span>  <br/> |<span data-ttu-id="852e5-163">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="852e5-163">Messages schema</span></span>  <br/> |
|<span data-ttu-id="852e5-164">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="852e5-164">Validation File</span></span>  <br/> |<span data-ttu-id="852e5-165">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="852e5-165">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="852e5-166">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="852e5-166">Can be Empty</span></span>  <br/> |<span data-ttu-id="852e5-167">False</span><span class="sxs-lookup"><span data-stu-id="852e5-167">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="852e5-168">関連項目</span><span class="sxs-lookup"><span data-stu-id="852e5-168">See also</span></span>

- [<span data-ttu-id="852e5-169">ConvertId 操作</span><span class="sxs-lookup"><span data-stu-id="852e5-169">ConvertId operation</span></span>](convertid-operation.md)
- [<span data-ttu-id="852e5-170">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="852e5-170">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

