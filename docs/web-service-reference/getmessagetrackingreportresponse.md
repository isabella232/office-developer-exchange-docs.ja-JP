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
ms.openlocfilehash: 15e1f5c91c07dbaad224fb0cd3bc89f444a18087
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460569"
---
# <a name="getmessagetrackingreportresponse"></a><span data-ttu-id="94c1f-103">GetMessageTrackingReportResponse</span><span class="sxs-lookup"><span data-stu-id="94c1f-103">GetMessageTrackingReportResponse</span></span>

<span data-ttu-id="94c1f-104">**Getmessagetrackingreportresponse**要素には、 [Getmessagetrackingreport 操作](getmessagetrackingreport-operation.md)に対する応答が含まれています。</span><span class="sxs-lookup"><span data-stu-id="94c1f-104">The **GetMessageTrackingReportResponse** element contains the response for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>
  
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

 <span data-ttu-id="94c1f-105">**GetMessageTrackingReportResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="94c1f-105">**GetMessageTrackingReportResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="94c1f-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="94c1f-106">Attributes and elements</span></span>

<span data-ttu-id="94c1f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="94c1f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="94c1f-108">属性</span><span class="sxs-lookup"><span data-stu-id="94c1f-108">Attributes</span></span>

|<span data-ttu-id="94c1f-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="94c1f-109">**Attribute**</span></span>|<span data-ttu-id="94c1f-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="94c1f-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="94c1f-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="94c1f-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="94c1f-112">応答の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="94c1f-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="94c1f-113">この属性には、次の値が有効です。</span><span class="sxs-lookup"><span data-stu-id="94c1f-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="94c1f-114">-成功</span><span class="sxs-lookup"><span data-stu-id="94c1f-114">-  Success</span></span>  <br/><span data-ttu-id="94c1f-115">-Warning</span><span class="sxs-lookup"><span data-stu-id="94c1f-115">-  Warning</span></span>  <br/><span data-ttu-id="94c1f-116">-エラー</span><span class="sxs-lookup"><span data-stu-id="94c1f-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="94c1f-117">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="94c1f-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="94c1f-118">**値**</span><span class="sxs-lookup"><span data-stu-id="94c1f-118">**Value**</span></span>|<span data-ttu-id="94c1f-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="94c1f-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="94c1f-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="94c1f-120">**Success**</span></span> <br/> |<span data-ttu-id="94c1f-121">満たされる要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="94c1f-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="94c1f-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="94c1f-122">**Warning**</span></span> <br/> | <span data-ttu-id="94c1f-123">処理されなかった要求を示します。</span><span class="sxs-lookup"><span data-stu-id="94c1f-123">Describes a request that was not processed.</span></span> <span data-ttu-id="94c1f-124">要求内のアイテムが処理され、その後のアイテムを処理できなかったときにエラーが発生した場合は、警告が返されることがあります。</span><span class="sxs-lookup"><span data-stu-id="94c1f-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="94c1f-125">警告のソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="94c1f-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="94c1f-126">-バッチ処理中に Exchange ストアがオフラインになります。</span><span class="sxs-lookup"><span data-stu-id="94c1f-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="94c1f-127">-Active Directory ドメインの機能 (AD DS) がオフラインになっています。</span><span class="sxs-lookup"><span data-stu-id="94c1f-127">-  Active Directory Domain Serves (AD DS) is offline.</span></span>  <br/><span data-ttu-id="94c1f-128">-メールボックスが移動されました。</span><span class="sxs-lookup"><span data-stu-id="94c1f-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="94c1f-129">-メッセージデータベース (MDB) はオフラインです。</span><span class="sxs-lookup"><span data-stu-id="94c1f-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="94c1f-130">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="94c1f-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="94c1f-131">-クォータが限界を超えています。</span><span class="sxs-lookup"><span data-stu-id="94c1f-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="94c1f-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="94c1f-132">**Error**</span></span> <br/> | <span data-ttu-id="94c1f-133">満たされない要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="94c1f-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="94c1f-134">エラーのソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="94c1f-134">The following are examples of sources of errors:</span></span>  <br/>  <span data-ttu-id="94c1f-135">無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="94c1f-135">Invalid attributes or elements</span></span>  <br/><br/><span data-ttu-id="94c1f-136">-範囲外の属性または要素</span><span class="sxs-lookup"><span data-stu-id="94c1f-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="94c1f-137">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="94c1f-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="94c1f-138">-コンテキスト内で有効ではない属性または要素</span><span class="sxs-lookup"><span data-stu-id="94c1f-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="94c1f-139">-クライアントによる権限のないアクセス試行</span><span class="sxs-lookup"><span data-stu-id="94c1f-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="94c1f-140">-有効なクライアント側の呼び出しに応答した場合のサーバー側障害</span><span class="sxs-lookup"><span data-stu-id="94c1f-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="94c1f-141">エラーに関する情報については、応答[secの](responsecode.md)要素と[messagetext](messagetext.md)要素を参照してください。</span><span class="sxs-lookup"><span data-stu-id="94c1f-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="94c1f-142">子要素</span><span class="sxs-lookup"><span data-stu-id="94c1f-142">Child elements</span></span>

|<span data-ttu-id="94c1f-143">**Element**</span><span class="sxs-lookup"><span data-stu-id="94c1f-143">**Element**</span></span>|<span data-ttu-id="94c1f-144">**説明**</span><span class="sxs-lookup"><span data-stu-id="94c1f-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="94c1f-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="94c1f-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="94c1f-146">応答の状態を説明するテキストを提供します。</span><span class="sxs-lookup"><span data-stu-id="94c1f-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="94c1f-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="94c1f-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="94c1f-148">要求で発生した特定のエラーを識別するエラーコードを提供します。</span><span class="sxs-lookup"><span data-stu-id="94c1f-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="94c1f-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="94c1f-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="94c1f-150">現在未使用で、今後の使用のために予約されています。</span><span class="sxs-lookup"><span data-stu-id="94c1f-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="94c1f-151">この要素には0の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="94c1f-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="94c1f-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="94c1f-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="94c1f-153">エラー応答に関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="94c1f-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="94c1f-154">および search-messagetrackingreport</span><span class="sxs-lookup"><span data-stu-id="94c1f-154">MessageTrackingReport</span></span>](messagetrackingreport.md) <br/> |<span data-ttu-id="94c1f-155">[Getmessagetrackingreport 操作](getmessagetrackingreport-operation.md)で返される1つのメッセージを格納します。</span><span class="sxs-lookup"><span data-stu-id="94c1f-155">Contains a single message that is returned in a [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="94c1f-156">Diagnostics</span><span class="sxs-lookup"><span data-stu-id="94c1f-156">Diagnostics</span></span>](diagnostics.md) <br/> |<span data-ttu-id="94c1f-157">データセンターでのレポート作成に使用されるタイミングとパフォーマンスに関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="94c1f-157">Provides timing and performance information that is used for reporting in a DataCenter.</span></span>  <br/> |
|[<span data-ttu-id="94c1f-158">エラー</span><span class="sxs-lookup"><span data-stu-id="94c1f-158">Errors</span></span>](errors-ex15websvcsotherref.md) <br/> |<span data-ttu-id="94c1f-159">Web サービスによって返されたエラーを格納するためのプロパティバッグが格納されています。</span><span class="sxs-lookup"><span data-stu-id="94c1f-159">Contains a property bag to store errors that are returned through the Web service.</span></span>  <br/> |
|[<span data-ttu-id="94c1f-160">プロパティ (ArrayOfTrackingPropertiesType)</span><span class="sxs-lookup"><span data-stu-id="94c1f-160">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md) <br/> |<span data-ttu-id="94c1f-161">1つ以上の追跡プロパティの一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="94c1f-161">Contains a list of one or more tracking properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="94c1f-162">親要素</span><span class="sxs-lookup"><span data-stu-id="94c1f-162">Parent elements</span></span>

<span data-ttu-id="94c1f-163">なし。</span><span class="sxs-lookup"><span data-stu-id="94c1f-163">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="94c1f-164">テキスト値</span><span class="sxs-lookup"><span data-stu-id="94c1f-164">Text value</span></span>

<span data-ttu-id="94c1f-165">なし。</span><span class="sxs-lookup"><span data-stu-id="94c1f-165">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="94c1f-166">注釈</span><span class="sxs-lookup"><span data-stu-id="94c1f-166">Remarks</span></span>

<span data-ttu-id="94c1f-167">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="94c1f-167">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="94c1f-168">要素の情報</span><span class="sxs-lookup"><span data-stu-id="94c1f-168">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="94c1f-169">Namespace</span><span class="sxs-lookup"><span data-stu-id="94c1f-169">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="94c1f-170">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="94c1f-170">Schema Name</span></span>  <br/> |<span data-ttu-id="94c1f-171">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="94c1f-171">Messages schema</span></span>  <br/> |
|<span data-ttu-id="94c1f-172">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="94c1f-172">Validation File</span></span>  <br/> |<span data-ttu-id="94c1f-173">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="94c1f-173">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="94c1f-174">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="94c1f-174">Can be Empty</span></span>  <br/> |<span data-ttu-id="94c1f-175">正しくない</span><span class="sxs-lookup"><span data-stu-id="94c1f-175">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="94c1f-176">関連項目</span><span class="sxs-lookup"><span data-stu-id="94c1f-176">See also</span></span>

- [<span data-ttu-id="94c1f-177">GetMessageTrackingReport 操作</span><span class="sxs-lookup"><span data-stu-id="94c1f-177">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)
- [<span data-ttu-id="94c1f-178">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="94c1f-178">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

