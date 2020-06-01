---
title: FindMessageTrackingReportResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindMessageTrackingReportResponse
api_type:
- schema
ms.assetid: ed4265dc-0e79-4b34-8bf4-88a94875629d
description: FindMessageTrackingReportResponse 要素には、単一の FindMessageTrackingReport 操作要求の状態と結果が含まれています。
ms.openlocfilehash: a72ae3b20f2cae3d37a90da36b816e6f3265c716
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462916"
---
# <a name="findmessagetrackingreportresponse"></a><span data-ttu-id="8e829-103">FindMessageTrackingReportResponse</span><span class="sxs-lookup"><span data-stu-id="8e829-103">FindMessageTrackingReportResponse</span></span>

<span data-ttu-id="8e829-104">**Findmessagetrackingreportresponse**要素には、単一の[Findmessagetrackingreport 操作](findmessagetrackingreport-operation.md)要求の状態と結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="8e829-104">The **FindMessageTrackingReportResponse** element contains the status and result of a single [FindMessageTrackingReport operation](findmessagetrackingreport-operation.md) request.</span></span> 
  
```xml
<FindMessageTrackingReportResponse ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Diagnostics/>
   <MessageTrackingSearchResults/>
   <Errors/>
   <Properties/>
</FindMessageTrackingReportResponse>
```

 <span data-ttu-id="8e829-105">**FindMessageTrackingReportResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="8e829-105">**FindMessageTrackingReportResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8e829-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="8e829-106">Attributes and elements</span></span>

<span data-ttu-id="8e829-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8e829-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8e829-108">属性</span><span class="sxs-lookup"><span data-stu-id="8e829-108">Attributes</span></span>

|<span data-ttu-id="8e829-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="8e829-109">**Attribute**</span></span>|<span data-ttu-id="8e829-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="8e829-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8e829-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="8e829-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="8e829-112">応答の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="8e829-112">Describes the status of the response.</span></span><br/><br/> <span data-ttu-id="8e829-113">この属性には、次の値が有効です。</span><span class="sxs-lookup"><span data-stu-id="8e829-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="8e829-114">-成功</span><span class="sxs-lookup"><span data-stu-id="8e829-114">-  Success</span></span>  <br/><span data-ttu-id="8e829-115">-Warning</span><span class="sxs-lookup"><span data-stu-id="8e829-115">-  Warning</span></span>  <br/><span data-ttu-id="8e829-116">-エラー</span><span class="sxs-lookup"><span data-stu-id="8e829-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="8e829-117">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="8e829-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="8e829-118">**値**</span><span class="sxs-lookup"><span data-stu-id="8e829-118">**Value**</span></span>|<span data-ttu-id="8e829-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="8e829-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8e829-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="8e829-120">**Success**</span></span> <br/> |<span data-ttu-id="8e829-121">満たされる要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="8e829-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="8e829-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="8e829-122">**Warning**</span></span> <br/> | <span data-ttu-id="8e829-123">処理されなかった要求を示します。</span><span class="sxs-lookup"><span data-stu-id="8e829-123">Describes a request that was not processed.</span></span> <span data-ttu-id="8e829-124">要求内のアイテムが処理され、その後のアイテムを処理できなかったときにエラーが発生した場合は、警告が返されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8e829-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="8e829-125">警告のソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8e829-125">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="8e829-126">-バッチ処理中に Exchange ストアがオフラインになります。</span><span class="sxs-lookup"><span data-stu-id="8e829-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="8e829-127">-Active Directory ドメインサービス (AD DS) がオフラインになっています。</span><span class="sxs-lookup"><span data-stu-id="8e829-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="8e829-128">-メールボックスが移動されました。</span><span class="sxs-lookup"><span data-stu-id="8e829-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="8e829-129">-メッセージデータベース (MDB) はオフラインです。</span><span class="sxs-lookup"><span data-stu-id="8e829-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="8e829-130">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="8e829-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="8e829-131">-クォータが限界を超えています。</span><span class="sxs-lookup"><span data-stu-id="8e829-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="8e829-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="8e829-132">**Error**</span></span> <br/> | <span data-ttu-id="8e829-133">満たされない要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="8e829-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="8e829-134">エラーのソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8e829-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="8e829-135">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="8e829-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="8e829-136">-範囲外の属性または要素</span><span class="sxs-lookup"><span data-stu-id="8e829-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="8e829-137">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="8e829-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="8e829-138">-コンテキスト内で有効ではない属性または要素</span><span class="sxs-lookup"><span data-stu-id="8e829-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="8e829-139">-クライアントによる権限のないアクセス試行</span><span class="sxs-lookup"><span data-stu-id="8e829-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="8e829-140">-有効なクライアント側の呼び出しに応答した場合のサーバー側障害</span><span class="sxs-lookup"><span data-stu-id="8e829-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="8e829-141">エラーに関する情報については、応答[secの](responsecode.md)要素と[messagetext](messagetext.md)要素を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8e829-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="8e829-142">子要素</span><span class="sxs-lookup"><span data-stu-id="8e829-142">Child elements</span></span>

|<span data-ttu-id="8e829-143">**Element**</span><span class="sxs-lookup"><span data-stu-id="8e829-143">**Element**</span></span>|<span data-ttu-id="8e829-144">**説明**</span><span class="sxs-lookup"><span data-stu-id="8e829-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8e829-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="8e829-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="8e829-146">応答の状態を説明するテキストを提供します。</span><span class="sxs-lookup"><span data-stu-id="8e829-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="8e829-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="8e829-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="8e829-148">要求で発生した特定のエラーを識別するエラーコードを提供します。</span><span class="sxs-lookup"><span data-stu-id="8e829-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="8e829-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="8e829-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="8e829-150">現在未使用で、今後の使用のために予約されています。</span><span class="sxs-lookup"><span data-stu-id="8e829-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="8e829-151">この要素には0の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="8e829-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="8e829-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="8e829-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="8e829-153">エラー応答に関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="8e829-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="8e829-154">Diagnostics</span><span class="sxs-lookup"><span data-stu-id="8e829-154">Diagnostics</span></span>](diagnostics.md) <br/> |<span data-ttu-id="8e829-155">データセンターの追跡機能に関するさまざまな統計レポートを生成するために使用される情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="8e829-155">Contains information that will be used to produce various statistical reports for the tracking feature in a DataCenter.</span></span>  <br/> |
|[<span data-ttu-id="8e829-156">MessageTrackingSearchResults</span><span class="sxs-lookup"><span data-stu-id="8e829-156">MessageTrackingSearchResults</span></span>](messagetrackingsearchresults.md) <br/> |<span data-ttu-id="8e829-157">検索要件に一致するメッセージの配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="8e829-157">Contains and array of messages that match the search requirements.</span></span>  <br/> |
|[<span data-ttu-id="8e829-158">ExecutedSearchScope</span><span class="sxs-lookup"><span data-stu-id="8e829-158">ExecutedSearchScope</span></span>](executedsearchscope.md) <br/> |<span data-ttu-id="8e829-159">検索結果を取得するために実行された検索の範囲を含みます。</span><span class="sxs-lookup"><span data-stu-id="8e829-159">Contains the scope of the search that was performed to get the search results.</span></span>  <br/> |
|[<span data-ttu-id="8e829-160">エラー</span><span class="sxs-lookup"><span data-stu-id="8e829-160">Errors</span></span>](errors-ex15websvcsotherref.md) <br/> |<span data-ttu-id="8e829-161">Web サービスによって返されたエラーを格納するためのプロパティバッグが格納されています。</span><span class="sxs-lookup"><span data-stu-id="8e829-161">Contains a property bag to store errors that are returned through the Web service.</span></span>  <br/> |
|[<span data-ttu-id="8e829-162">プロパティ (ArrayOfTrackingPropertiesType)</span><span class="sxs-lookup"><span data-stu-id="8e829-162">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md) <br/> |<span data-ttu-id="8e829-163">1つ以上の追跡プロパティの一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="8e829-163">Contains a list of one or more tracking properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8e829-164">親要素</span><span class="sxs-lookup"><span data-stu-id="8e829-164">Parent elements</span></span>

<span data-ttu-id="8e829-165">なし。</span><span class="sxs-lookup"><span data-stu-id="8e829-165">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="8e829-166">テキスト値</span><span class="sxs-lookup"><span data-stu-id="8e829-166">Text value</span></span>

<span data-ttu-id="8e829-167">なし。</span><span class="sxs-lookup"><span data-stu-id="8e829-167">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8e829-168">注釈</span><span class="sxs-lookup"><span data-stu-id="8e829-168">Remarks</span></span>

<span data-ttu-id="8e829-169">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="8e829-169">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8e829-170">要素の情報</span><span class="sxs-lookup"><span data-stu-id="8e829-170">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8e829-171">Namespace</span><span class="sxs-lookup"><span data-stu-id="8e829-171">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="8e829-172">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8e829-172">Schema Name</span></span>  <br/> |<span data-ttu-id="8e829-173">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="8e829-173">Messages schema</span></span>  <br/> |
|<span data-ttu-id="8e829-174">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8e829-174">Validation File</span></span>  <br/> |<span data-ttu-id="8e829-175">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="8e829-175">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8e829-176">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="8e829-176">Can be Empty</span></span>  <br/> |<span data-ttu-id="8e829-177">正しくない</span><span class="sxs-lookup"><span data-stu-id="8e829-177">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8e829-178">関連項目</span><span class="sxs-lookup"><span data-stu-id="8e829-178">See also</span></span>

- [<span data-ttu-id="8e829-179">FindMessageTrackingReport 操作</span><span class="sxs-lookup"><span data-stu-id="8e829-179">FindMessageTrackingReport operation</span></span>](findmessagetrackingreport-operation.md)
- [<span data-ttu-id="8e829-180">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="8e829-180">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

