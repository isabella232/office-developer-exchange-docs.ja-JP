---
title: SendItemResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SendItemResponseMessage
api_type:
- schema
ms.assetid: 264f6a2f-c8cc-4c96-86e1-1aabb6f9d8ab
description: SendItemResponseMessage 要素には、1つの SendItem 操作要求の状態と結果が含まれています。
ms.openlocfilehash: fc5d4f6dc77b242c3d3d517133c23ed56956c1ca
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462270"
---
# <a name="senditemresponsemessage"></a><span data-ttu-id="d888f-103">SendItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d888f-103">SendItemResponseMessage</span></span>

<span data-ttu-id="d888f-104">**SendItemResponseMessage**要素には、1つの[SendItem 操作](senditem-operation.md)要求の状態と結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="d888f-104">The **SendItemResponseMessage** element contains the status and result of a single [SendItem operation](senditem-operation.md) request.</span></span> 
  
```xml
<SendItemResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</SendItemResponseMessage>
```

 <span data-ttu-id="d888f-105">**ResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="d888f-105">**ResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d888f-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d888f-106">Attributes and elements</span></span>

<span data-ttu-id="d888f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d888f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d888f-108">属性</span><span class="sxs-lookup"><span data-stu-id="d888f-108">Attributes</span></span>

|<span data-ttu-id="d888f-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="d888f-109">**Attribute**</span></span>|<span data-ttu-id="d888f-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="d888f-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d888f-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="d888f-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="d888f-112">[SendItem 操作](senditem-operation.md)の応答の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="d888f-112">Describes the status of a [SendItem operation](senditem-operation.md) response.</span></span> <br/><br/><span data-ttu-id="d888f-113">この属性には、次の値が有効です。</span><span class="sxs-lookup"><span data-stu-id="d888f-113">The following values are valid for this attribute:</span></span> <br/> <br/><span data-ttu-id="d888f-114">-成功</span><span class="sxs-lookup"><span data-stu-id="d888f-114">-  Success</span></span>  <br/><span data-ttu-id="d888f-115">-Warning</span><span class="sxs-lookup"><span data-stu-id="d888f-115">-  Warning</span></span>  <br/><span data-ttu-id="d888f-116">-エラー</span><span class="sxs-lookup"><span data-stu-id="d888f-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="d888f-117">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="d888f-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="d888f-118">**値**</span><span class="sxs-lookup"><span data-stu-id="d888f-118">**Value**</span></span>|<span data-ttu-id="d888f-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="d888f-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d888f-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="d888f-120">**Success**</span></span> <br/> |<span data-ttu-id="d888f-121">満たされる要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="d888f-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="d888f-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="d888f-122">**Warning**</span></span> <br/> | <span data-ttu-id="d888f-123">処理されなかった要求を示します。</span><span class="sxs-lookup"><span data-stu-id="d888f-123">Describes a request that was not processed.</span></span> <span data-ttu-id="d888f-124">要求内のアイテムが処理され、その後のアイテムを処理できなかったときにエラーが発生した場合は、警告が返されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d888f-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="d888f-125">警告のソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d888f-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="d888f-126">-バッチ処理中に Exchange ストアがオフラインになります。</span><span class="sxs-lookup"><span data-stu-id="d888f-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="d888f-127">-Active Directory ドメインサービス (AD DS) がオフラインになっています。</span><span class="sxs-lookup"><span data-stu-id="d888f-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="d888f-128">-メールボックスは移動されます。</span><span class="sxs-lookup"><span data-stu-id="d888f-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="d888f-129">-メッセージデータベース (MDB) はオフラインです。</span><span class="sxs-lookup"><span data-stu-id="d888f-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="d888f-130">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="d888f-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="d888f-131">-クォータが上限を超えています。</span><span class="sxs-lookup"><span data-stu-id="d888f-131">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="d888f-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="d888f-132">**Error**</span></span> <br/> | <span data-ttu-id="d888f-133">満たされない要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="d888f-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="d888f-134">エラーのソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d888f-134">The following are examples of sources of errors:</span></span>  <br/> <br/><span data-ttu-id="d888f-135">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="d888f-135">- Invalid attributes or elements</span></span>  <br/><span data-ttu-id="d888f-136">-属性または要素が範囲外です</span><span class="sxs-lookup"><span data-stu-id="d888f-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="d888f-137">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="d888f-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="d888f-138">-属性または要素がコンテキスト内で有効ではありません</span><span class="sxs-lookup"><span data-stu-id="d888f-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="d888f-139">-クライアントによる権限のないアクセス試行</span><span class="sxs-lookup"><span data-stu-id="d888f-139">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="d888f-140">-有効なクライアント側の呼び出しに応答した場合のサーバー側エラー</span><span class="sxs-lookup"><span data-stu-id="d888f-140">-  Server-side failure in response to a valid client-side call</span></span>  <br/> <br/> <span data-ttu-id="d888f-141">エラーに関する情報については、応答[secの](responsecode.md)要素と[messagetext](messagetext.md)要素を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d888f-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d888f-142">子要素</span><span class="sxs-lookup"><span data-stu-id="d888f-142">Child elements</span></span>

|<span data-ttu-id="d888f-143">**Element**</span><span class="sxs-lookup"><span data-stu-id="d888f-143">**Element**</span></span>|<span data-ttu-id="d888f-144">**説明**</span><span class="sxs-lookup"><span data-stu-id="d888f-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d888f-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="d888f-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="d888f-146">応答の状態を説明するテキストを提供します。</span><span class="sxs-lookup"><span data-stu-id="d888f-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="d888f-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="d888f-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="d888f-148">要求で発生した特定のエラーを識別するエラーコードを提供します。</span><span class="sxs-lookup"><span data-stu-id="d888f-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="d888f-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="d888f-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="d888f-150">現在未使用で、今後の使用のために予約されています。</span><span class="sxs-lookup"><span data-stu-id="d888f-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="d888f-151">このプロパティには0の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="d888f-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="d888f-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="d888f-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="d888f-153">エラー応答に関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="d888f-153">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d888f-154">親要素</span><span class="sxs-lookup"><span data-stu-id="d888f-154">Parent elements</span></span>

|<span data-ttu-id="d888f-155">**要素**</span><span class="sxs-lookup"><span data-stu-id="d888f-155">**Element**</span></span>|<span data-ttu-id="d888f-156">**説明**</span><span class="sxs-lookup"><span data-stu-id="d888f-156">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d888f-157">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="d888f-157">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="d888f-158">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="d888f-158">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d888f-159">注釈</span><span class="sxs-lookup"><span data-stu-id="d888f-159">Remarks</span></span>

<span data-ttu-id="d888f-160">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされた Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="d888f-160">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d888f-161">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d888f-161">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d888f-162">Namespace</span><span class="sxs-lookup"><span data-stu-id="d888f-162">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d888f-163">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d888f-163">Schema Name</span></span>  <br/> |<span data-ttu-id="d888f-164">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="d888f-164">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d888f-165">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d888f-165">Validation File</span></span>  <br/> |<span data-ttu-id="d888f-166">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="d888f-166">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d888f-167">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d888f-167">Can be Empty</span></span>  <br/> |<span data-ttu-id="d888f-168">正しくない</span><span class="sxs-lookup"><span data-stu-id="d888f-168">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d888f-169">関連項目</span><span class="sxs-lookup"><span data-stu-id="d888f-169">See also</span></span>

- [<span data-ttu-id="d888f-170">SendItem 操作</span><span class="sxs-lookup"><span data-stu-id="d888f-170">SendItem operation</span></span>](senditem-operation.md)
- [<span data-ttu-id="d888f-171">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="d888f-171">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

