---
title: GetMessageTrackingReportResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetMessageTrackingReportResponse
api_type:
- schema
ms.assetid: 41177894-2008-44a6-86f8-bc34c0a48e36
description: GetMessageTrackingReportResponse 要素には、GetMessageTrackingReport 操作に対する応答が含まれています。
ms.openlocfilehash: bdb8b97e57f92a32cbdc498d09297920366b58bd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760794"
---
# <a name="getmessagetrackingreportresponse"></a><span data-ttu-id="f0ac9-103">GetMessageTrackingReportResponse</span><span class="sxs-lookup"><span data-stu-id="f0ac9-103">GetMessageTrackingReportResponse</span></span>

<span data-ttu-id="f0ac9-104">**GetMessageTrackingReportResponse**要素には、 [GetMessageTrackingReport 操作](getmessagetrackingreport-operation.md)の応答が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f0ac9-104">The **GetMessageTrackingReportResponse** element contains the response for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>
  
```xml
<GetMessageTrackingReportResponse ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <MessageTrackingReport/>
   <Diagnostics/>
   <Errors/>
   <Properties/>
</GetMessageTrackingReportResponse>
```

 <span data-ttu-id="f0ac9-105">**GetMessageTrackingReportResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="f0ac9-105">**GetMessageTrackingReportResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f0ac9-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="f0ac9-106">Attributes and elements</span></span>

<span data-ttu-id="f0ac9-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f0ac9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f0ac9-108">属性</span><span class="sxs-lookup"><span data-stu-id="f0ac9-108">Attributes</span></span>

|<span data-ttu-id="f0ac9-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="f0ac9-109">**Attribute**</span></span>|<span data-ttu-id="f0ac9-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="f0ac9-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f0ac9-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="f0ac9-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="f0ac9-112">応答のステータスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="f0ac9-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="f0ac9-113">次の値は、この属性の有効です。</span><span class="sxs-lookup"><span data-stu-id="f0ac9-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="f0ac9-114">-成功</span><span class="sxs-lookup"><span data-stu-id="f0ac9-114">-  Success</span></span>  <br/><span data-ttu-id="f0ac9-115">-警告</span><span class="sxs-lookup"><span data-stu-id="f0ac9-115">-  Warning</span></span>  <br/><span data-ttu-id="f0ac9-116">-エラー</span><span class="sxs-lookup"><span data-stu-id="f0ac9-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="f0ac9-117">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="f0ac9-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="f0ac9-118">**値**</span><span class="sxs-lookup"><span data-stu-id="f0ac9-118">**Value**</span></span>|<span data-ttu-id="f0ac9-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="f0ac9-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f0ac9-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="f0ac9-120">**Success**</span></span> <br/> |<span data-ttu-id="f0ac9-121">満了する要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="f0ac9-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="f0ac9-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="f0ac9-122">**Warning**</span></span> <br/> | <span data-ttu-id="f0ac9-123">処理されなかった要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="f0ac9-123">Describes a request that was not processed.</span></span> <span data-ttu-id="f0ac9-124">警告は、要求内のアイテムを処理し、それ以降の項目を処理できませんでした、エラーが発生した場合に返される場合があります。</span><span class="sxs-lookup"><span data-stu-id="f0ac9-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="f0ac9-125">警告の送信元の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f0ac9-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="f0ac9-126">-Exchange ストアは、バッチの実行中にオフラインです。</span><span class="sxs-lookup"><span data-stu-id="f0ac9-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="f0ac9-127">-Active Directory ドメイン機能 (AD DS) は、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="f0ac9-127">-  Active Directory Domain Serves (AD DS) is offline.</span></span>  <br/><span data-ttu-id="f0ac9-128">-メールボックスは移動されました。</span><span class="sxs-lookup"><span data-stu-id="f0ac9-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="f0ac9-129">-メッセージ データベース (MDB) は、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="f0ac9-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="f0ac9-130">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="f0ac9-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="f0ac9-131">クォータを超えています。</span><span class="sxs-lookup"><span data-stu-id="f0ac9-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="f0ac9-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="f0ac9-132">**Error**</span></span> <br/> | <span data-ttu-id="f0ac9-133">満たせない要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="f0ac9-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="f0ac9-134">次に、エラーのソースの例を示します。</span><span class="sxs-lookup"><span data-stu-id="f0ac9-134">The following are examples of sources of errors:</span></span>  <br/>  <span data-ttu-id="f0ac9-135">無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="f0ac9-135">Invalid attributes or elements</span></span>  <br/><br/><span data-ttu-id="f0ac9-136">属性または要素の範囲を超えています。</span><span class="sxs-lookup"><span data-stu-id="f0ac9-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="f0ac9-137">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="f0ac9-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="f0ac9-138">属性または要素のコンテキストでは有効ではないです。</span><span class="sxs-lookup"><span data-stu-id="f0ac9-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="f0ac9-139">-任意のクライアントから不正なアクセス試行</span><span class="sxs-lookup"><span data-stu-id="f0ac9-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="f0ac9-140">-クライアント側の有効な呼び出しへの応答でサーバー側エラー</span><span class="sxs-lookup"><span data-stu-id="f0ac9-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="f0ac9-141">エラーに関する情報は、 [ResponseCode](responsecode.md)および[メッセージ テキスト](messagetext.md)の要素を参照しています。</span><span class="sxs-lookup"><span data-stu-id="f0ac9-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="f0ac9-142">子要素</span><span class="sxs-lookup"><span data-stu-id="f0ac9-142">Child elements</span></span>

|<span data-ttu-id="f0ac9-143">**要素**</span><span class="sxs-lookup"><span data-stu-id="f0ac9-143">**Element**</span></span>|<span data-ttu-id="f0ac9-144">**説明**</span><span class="sxs-lookup"><span data-stu-id="f0ac9-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f0ac9-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="f0ac9-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="f0ac9-146">応答のステータスの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="f0ac9-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="f0ac9-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="f0ac9-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="f0ac9-148">要求で発生した特定のエラーを識別するエラー コードを提供します。</span><span class="sxs-lookup"><span data-stu-id="f0ac9-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="f0ac9-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="f0ac9-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="f0ac9-150">現在使用されていない、将来使用するために予約されています。</span><span class="sxs-lookup"><span data-stu-id="f0ac9-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="f0ac9-151">この要素には、0 の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f0ac9-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="f0ac9-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="f0ac9-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="f0ac9-153">追加のエラー応答情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="f0ac9-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="f0ac9-154">MessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="f0ac9-154">MessageTrackingReport</span></span>](messagetrackingreport.md) <br/> |<span data-ttu-id="f0ac9-155">[GetMessageTrackingReport 操作](getmessagetrackingreport-operation.md)で返される 1 つのメッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="f0ac9-155">Contains a single message that is returned in a [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="f0ac9-156">診断</span><span class="sxs-lookup"><span data-stu-id="f0ac9-156">Diagnostics</span></span>](diagnostics.md) <br/> |<span data-ttu-id="f0ac9-157">データ センターに報告するために使用されるタイミングとパフォーマンスの情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="f0ac9-157">Provides timing and performance information that is used for reporting in a DataCenter.</span></span>  <br/> |
|[<span data-ttu-id="f0ac9-158">エラー</span><span class="sxs-lookup"><span data-stu-id="f0ac9-158">Errors</span></span>](errors-ex15websvcsotherref.md) <br/> |<span data-ttu-id="f0ac9-159">Web サービスから返されるエラーを格納するプロパティ バッグに含まれています。</span><span class="sxs-lookup"><span data-stu-id="f0ac9-159">Contains a property bag to store errors that are returned through the Web service.</span></span>  <br/> |
|[<span data-ttu-id="f0ac9-160">プロパティ (ArrayOfTrackingPropertiesType)</span><span class="sxs-lookup"><span data-stu-id="f0ac9-160">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md) <br/> |<span data-ttu-id="f0ac9-161">1 つまたは複数の追跡のプロパティの一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f0ac9-161">Contains a list of one or more tracking properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f0ac9-162">親要素</span><span class="sxs-lookup"><span data-stu-id="f0ac9-162">Parent elements</span></span>

<span data-ttu-id="f0ac9-163">なし。</span><span class="sxs-lookup"><span data-stu-id="f0ac9-163">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="f0ac9-164">テキスト値</span><span class="sxs-lookup"><span data-stu-id="f0ac9-164">Text value</span></span>

<span data-ttu-id="f0ac9-165">なし。</span><span class="sxs-lookup"><span data-stu-id="f0ac9-165">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f0ac9-166">備考</span><span class="sxs-lookup"><span data-stu-id="f0ac9-166">Remarks</span></span>

<span data-ttu-id="f0ac9-167">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="f0ac9-167">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f0ac9-168">要素情報</span><span class="sxs-lookup"><span data-stu-id="f0ac9-168">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f0ac9-169">名前空間</span><span class="sxs-lookup"><span data-stu-id="f0ac9-169">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f0ac9-170">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f0ac9-170">Schema Name</span></span>  <br/> |<span data-ttu-id="f0ac9-171">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="f0ac9-171">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f0ac9-172">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f0ac9-172">Validation File</span></span>  <br/> |<span data-ttu-id="f0ac9-173">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f0ac9-173">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f0ac9-174">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="f0ac9-174">Can be Empty</span></span>  <br/> |<span data-ttu-id="f0ac9-175">False</span><span class="sxs-lookup"><span data-stu-id="f0ac9-175">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f0ac9-176">関連項目</span><span class="sxs-lookup"><span data-stu-id="f0ac9-176">See also</span></span>

- [<span data-ttu-id="f0ac9-177">GetMessageTrackingReport 操作</span><span class="sxs-lookup"><span data-stu-id="f0ac9-177">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)
- [<span data-ttu-id="f0ac9-178">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="f0ac9-178">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

