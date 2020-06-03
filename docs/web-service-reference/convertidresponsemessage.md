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
description: ConvertIdResponseMessage 要素には、収束 Tid 操作要求の状態と結果が含まれています。
ms.openlocfilehash: cd0154f87390be3516ced4be53f5371d4a348c49
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456221"
---
# <a name="convertidresponsemessage"></a><span data-ttu-id="c2b90-103">ConvertIdResponseMessage</span><span class="sxs-lookup"><span data-stu-id="c2b90-103">ConvertIdResponseMessage</span></span>

<span data-ttu-id="c2b90-104">**ConvertIdResponseMessage**要素には、[収束 tid 操作](convertid-operation.md)要求の状態と結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="c2b90-104">The **ConvertIdResponseMessage** element contains the status and result of a [ConvertId operation](convertid-operation.md) request.</span></span> 
  
- [<span data-ttu-id="c2b90-105">ConvertIdResponse</span><span class="sxs-lookup"><span data-stu-id="c2b90-105">ConvertIdResponse</span></span>](convertidresponse.md) 
- [<span data-ttu-id="c2b90-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="c2b90-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="c2b90-107">ConvertIdResponseMessage</span><span class="sxs-lookup"><span data-stu-id="c2b90-107">ConvertIdResponseMessage</span></span>](convertidresponsemessage.md)
  
```xml
<ConvertIdResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <AlternateId/>
</ConvertIdResponseMessage>
```

 <span data-ttu-id="c2b90-108">**ConvertIdResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="c2b90-108">**ConvertIdResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c2b90-109">属性と要素</span><span class="sxs-lookup"><span data-stu-id="c2b90-109">Attributes and elements</span></span>

<span data-ttu-id="c2b90-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c2b90-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c2b90-111">属性</span><span class="sxs-lookup"><span data-stu-id="c2b90-111">Attributes</span></span>

|<span data-ttu-id="c2b90-112">**属性**</span><span class="sxs-lookup"><span data-stu-id="c2b90-112">**Attribute**</span></span>|<span data-ttu-id="c2b90-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="c2b90-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c2b90-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="c2b90-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="c2b90-115">[[コンバーター tid 操作](convertid-operation.md)の応答の状態について説明します。</span><span class="sxs-lookup"><span data-stu-id="c2b90-115">Describes the status of a [ConvertId operation](convertid-operation.md) response.</span></span><br/><br/><span data-ttu-id="c2b90-116">この属性には、次の値が有効です。</span><span class="sxs-lookup"><span data-stu-id="c2b90-116">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="c2b90-117">-成功</span><span class="sxs-lookup"><span data-stu-id="c2b90-117">- Success</span></span>  <br/><span data-ttu-id="c2b90-118">-Warning</span><span class="sxs-lookup"><span data-stu-id="c2b90-118">-  Warning</span></span>  <br/><span data-ttu-id="c2b90-119">-エラー</span><span class="sxs-lookup"><span data-stu-id="c2b90-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="c2b90-120">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="c2b90-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="c2b90-121">**値**</span><span class="sxs-lookup"><span data-stu-id="c2b90-121">**Value**</span></span>|<span data-ttu-id="c2b90-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="c2b90-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c2b90-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="c2b90-123">**Success**</span></span> <br/> |<span data-ttu-id="c2b90-124">満たされる要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="c2b90-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="c2b90-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="c2b90-125">**Warning**</span></span> <br/> | <span data-ttu-id="c2b90-126">完全には処理されなかった、または予期しない結果が発生した要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="c2b90-126">Describes a request that was not fully processed or for which an unintended result occurred.</span></span>  <br/> |
|<span data-ttu-id="c2b90-127">**Error**</span><span class="sxs-lookup"><span data-stu-id="c2b90-127">**Error**</span></span> <br/> | <span data-ttu-id="c2b90-128">満たされない要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="c2b90-128">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="c2b90-129">エラーのソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c2b90-129">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="c2b90-130">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="c2b90-130">- Invalid attributes or elements</span></span>  <br/><span data-ttu-id="c2b90-131">-範囲外の属性または要素</span><span class="sxs-lookup"><span data-stu-id="c2b90-131">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="c2b90-132">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="c2b90-132">-  An unknown tag</span></span>  <br/><span data-ttu-id="c2b90-133">-コンテキスト内で有効ではない属性または要素</span><span class="sxs-lookup"><span data-stu-id="c2b90-133">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="c2b90-134">-クライアントによる権限のないアクセス試行</span><span class="sxs-lookup"><span data-stu-id="c2b90-134">- An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="c2b90-135">-有効なクライアント側の呼び出しに応答した場合のサーバー側障害</span><span class="sxs-lookup"><span data-stu-id="c2b90-135">-  A server-side failure in response to a valid client-side call</span></span><br/><br/><span data-ttu-id="c2b90-136">エラーに関する情報については、応答[secの](responsecode.md)要素と[messagetext](messagetext.md)要素を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c2b90-136">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="c2b90-137">子要素</span><span class="sxs-lookup"><span data-stu-id="c2b90-137">Child elements</span></span>

|<span data-ttu-id="c2b90-138">**Element**</span><span class="sxs-lookup"><span data-stu-id="c2b90-138">**Element**</span></span>|<span data-ttu-id="c2b90-139">**説明**</span><span class="sxs-lookup"><span data-stu-id="c2b90-139">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c2b90-140">MessageText</span><span class="sxs-lookup"><span data-stu-id="c2b90-140">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="c2b90-141">応答の状態を説明するテキストを提供します。</span><span class="sxs-lookup"><span data-stu-id="c2b90-141">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="c2b90-142">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="c2b90-142">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="c2b90-143">要求で発生した特定のエラーを識別するエラーコードを提供します。</span><span class="sxs-lookup"><span data-stu-id="c2b90-143">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="c2b90-144">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="c2b90-144">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="c2b90-145">現在未使用で、今後の使用のために予約されています。</span><span class="sxs-lookup"><span data-stu-id="c2b90-145">Currently unused and reserved for future use.</span></span> <span data-ttu-id="c2b90-146">この要素には0の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="c2b90-146">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="c2b90-147">MessageXml</span><span class="sxs-lookup"><span data-stu-id="c2b90-147">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="c2b90-148">エラー応答に関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="c2b90-148">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="c2b90-149">AlternateId</span><span class="sxs-lookup"><span data-stu-id="c2b90-149">AlternateId</span></span>](alternateid.md) <br/> |<span data-ttu-id="c2b90-150">応答で変換された id を記述します。</span><span class="sxs-lookup"><span data-stu-id="c2b90-150">Describes a converted identifier in the response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c2b90-151">親要素</span><span class="sxs-lookup"><span data-stu-id="c2b90-151">Parent elements</span></span>

|<span data-ttu-id="c2b90-152">**要素**</span><span class="sxs-lookup"><span data-stu-id="c2b90-152">**Element**</span></span>|<span data-ttu-id="c2b90-153">**説明**</span><span class="sxs-lookup"><span data-stu-id="c2b90-153">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c2b90-154">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="c2b90-154">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="c2b90-155">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="c2b90-155">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c2b90-156">注釈</span><span class="sxs-lookup"><span data-stu-id="c2b90-156">Remarks</span></span>

<span data-ttu-id="c2b90-157">変換された識別子ごとに1つの応答メッセージが返されます。</span><span class="sxs-lookup"><span data-stu-id="c2b90-157">One response message per converted identifier is returned.</span></span> <span data-ttu-id="c2b90-158">エラー応答コードが返された場合、 [Alternateid](alternateid.md)要素は応答から失われます。</span><span class="sxs-lookup"><span data-stu-id="c2b90-158">The [AlternateId](alternateid.md) element will be missing from the response if an error response code is returned,</span></span> 
  
<span data-ttu-id="c2b90-159">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Exchange 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="c2b90-159">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c2b90-160">要素の情報</span><span class="sxs-lookup"><span data-stu-id="c2b90-160">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c2b90-161">Namespace</span><span class="sxs-lookup"><span data-stu-id="c2b90-161">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c2b90-162">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c2b90-162">Schema Name</span></span>  <br/> |<span data-ttu-id="c2b90-163">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="c2b90-163">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c2b90-164">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c2b90-164">Validation File</span></span>  <br/> |<span data-ttu-id="c2b90-165">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="c2b90-165">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c2b90-166">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="c2b90-166">Can be Empty</span></span>  <br/> |<span data-ttu-id="c2b90-167">正しくない</span><span class="sxs-lookup"><span data-stu-id="c2b90-167">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c2b90-168">関連項目</span><span class="sxs-lookup"><span data-stu-id="c2b90-168">See also</span></span>

- [<span data-ttu-id="c2b90-169">ConvertId 操作</span><span class="sxs-lookup"><span data-stu-id="c2b90-169">ConvertId operation</span></span>](convertid-operation.md)
- [<span data-ttu-id="c2b90-170">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="c2b90-170">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

