---
title: CreateFolderResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateFolderResponseMessage
api_type:
- schema
ms.assetid: 1301dd15-b008-4fd9-8c89-b15a20b186e2
description: CreateFolderResponseMessage 要素には、状態および 1 つの CreateFolder 操作要求の結果が含まれています。
ms.openlocfilehash: c587cca1f935b295a0ed30ab2210de40af28d06d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759826"
---
# <a name="createfolderresponsemessage"></a><span data-ttu-id="76414-103">CreateFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="76414-103">CreateFolderResponseMessage</span></span>

<span data-ttu-id="76414-104">**CreateFolderResponseMessage**要素には、状態および 1 つの結果が含まれている[CreateFolder 操作](createfolder-operation.md)を要求します。</span><span class="sxs-lookup"><span data-stu-id="76414-104">The **CreateFolderResponseMessage** element contains the status and result of a single [CreateFolder operation](createfolder-operation.md) request.</span></span> 
  
```xml
<CreateFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Folders/>
</CreateFolderResponseMessage>
```

<span data-ttu-id="76414-105">**FolderInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="76414-105">**FolderInfoResponseMessageType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="76414-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="76414-106">Attributes and elements</span></span>

<span data-ttu-id="76414-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="76414-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="76414-108">属性</span><span class="sxs-lookup"><span data-stu-id="76414-108">Attributes</span></span>

|<span data-ttu-id="76414-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="76414-109">**Attribute**</span></span>|<span data-ttu-id="76414-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="76414-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="76414-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="76414-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="76414-112">[CreateFolder 操作](createfolder-operation.md)の応答のステータスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="76414-112">Describes the status of a [CreateFolder operation](createfolder-operation.md) response.</span></span><br/><br/><span data-ttu-id="76414-113">次の値は、この属性の有効です。</span><span class="sxs-lookup"><span data-stu-id="76414-113">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="76414-114">-成功</span><span class="sxs-lookup"><span data-stu-id="76414-114">-  Success</span></span>  <br/><span data-ttu-id="76414-115">-警告</span><span class="sxs-lookup"><span data-stu-id="76414-115">-  Warning</span></span>  <br/><span data-ttu-id="76414-116">-エラー</span><span class="sxs-lookup"><span data-stu-id="76414-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="76414-117">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="76414-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="76414-118">**値**</span><span class="sxs-lookup"><span data-stu-id="76414-118">**Value**</span></span>|<span data-ttu-id="76414-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="76414-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="76414-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="76414-120">**Success**</span></span> <br/> |<span data-ttu-id="76414-121">満了する要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="76414-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="76414-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="76414-122">**Warning**</span></span> <br/> | <span data-ttu-id="76414-123">処理されなかった要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="76414-123">Describes a request that was not processed.</span></span> <span data-ttu-id="76414-124">警告は、要求内のアイテムを処理し、それ以降の項目を処理できませんでした、エラーが発生した場合に返される場合があります。</span><span class="sxs-lookup"><span data-stu-id="76414-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="76414-125">警告の送信元の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="76414-125">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="76414-126">-Exchange ストアは、バッチの実行中にオフラインです。</span><span class="sxs-lookup"><span data-stu-id="76414-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="76414-127">-Active Directory ドメイン サービス (AD DS) では、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="76414-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="76414-128">-メールボックスを移動します。</span><span class="sxs-lookup"><span data-stu-id="76414-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="76414-129">-メッセージ データベース (MDB) は、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="76414-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="76414-130">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="76414-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="76414-131">クォータを超えています。</span><span class="sxs-lookup"><span data-stu-id="76414-131">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="76414-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="76414-132">**Error**</span></span> <br/> | <span data-ttu-id="76414-133">満たせない要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="76414-133">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="76414-134">次に、エラーのソースの例を示します。</span><span class="sxs-lookup"><span data-stu-id="76414-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="76414-135">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="76414-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="76414-136">属性または要素が範囲外です</span><span class="sxs-lookup"><span data-stu-id="76414-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="76414-137">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="76414-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="76414-138">属性または要素のコンテキストでは無効です</span><span class="sxs-lookup"><span data-stu-id="76414-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="76414-139">の任意のクライアントから不正アクセスしようと</span><span class="sxs-lookup"><span data-stu-id="76414-139">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="76414-140">の有効なクライアント側の呼び出しに応答サーバー側の障害</span><span class="sxs-lookup"><span data-stu-id="76414-140">-  Server-side failure in response to a valid client-side call</span></span><br/><br/>  <span data-ttu-id="76414-141">エラーに関する情報は、 [ResponseCode](responsecode.md)および[メッセージ テキスト](messagetext.md)の要素を参照しています。</span><span class="sxs-lookup"><span data-stu-id="76414-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="76414-142">子要素</span><span class="sxs-lookup"><span data-stu-id="76414-142">Child elements</span></span>

|<span data-ttu-id="76414-143">**要素**</span><span class="sxs-lookup"><span data-stu-id="76414-143">**Element**</span></span>|<span data-ttu-id="76414-144">**説明**</span><span class="sxs-lookup"><span data-stu-id="76414-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="76414-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="76414-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="76414-146">応答のステータスの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="76414-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="76414-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="76414-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="76414-148">要求で発生した特定のエラーを識別するエラー コードを提供します。</span><span class="sxs-lookup"><span data-stu-id="76414-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="76414-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="76414-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="76414-150">現在使用されていない将来の使用に予約されているとします。</span><span class="sxs-lookup"><span data-stu-id="76414-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="76414-151">0 の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="76414-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="76414-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="76414-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="76414-153">追加のエラー応答情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="76414-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="76414-154">フォルダー</span><span class="sxs-lookup"><span data-stu-id="76414-154">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="76414-155">作成したフォルダーの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="76414-155">Contains an array of created folders.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="76414-156">親要素</span><span class="sxs-lookup"><span data-stu-id="76414-156">Parent elements</span></span>

|<span data-ttu-id="76414-157">**要素**</span><span class="sxs-lookup"><span data-stu-id="76414-157">**Element**</span></span>|<span data-ttu-id="76414-158">**説明**</span><span class="sxs-lookup"><span data-stu-id="76414-158">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="76414-159">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="76414-159">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="76414-160">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="76414-160">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="76414-161">備考</span><span class="sxs-lookup"><span data-stu-id="76414-161">Remarks</span></span>

<span data-ttu-id="76414-162">この要素を記述するスキーマは、インストールされているクライアント アクセス サーバーの役割と Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="76414-162">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="76414-163">要素情報</span><span class="sxs-lookup"><span data-stu-id="76414-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="76414-164">名前空間</span><span class="sxs-lookup"><span data-stu-id="76414-164">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="76414-165">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="76414-165">Schema Name</span></span>  <br/> |<span data-ttu-id="76414-166">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="76414-166">Messages schema</span></span>  <br/> |
|<span data-ttu-id="76414-167">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="76414-167">Validation File</span></span>  <br/> |<span data-ttu-id="76414-168">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="76414-168">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="76414-169">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="76414-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="76414-170">False</span><span class="sxs-lookup"><span data-stu-id="76414-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="76414-171">関連項目</span><span class="sxs-lookup"><span data-stu-id="76414-171">See also</span></span>

- <span data-ttu-id="76414-172">
  [CreateFolder 操作](createfolder-operation.md)</span><span class="sxs-lookup"><span data-stu-id="76414-172">[CreateFolder operation](createfolder-operation.md)</span></span>
- <span data-ttu-id="76414-173">
  [Exchange 用 EWS リファレンス](ews-reference-for-exchange.md)</span><span class="sxs-lookup"><span data-stu-id="76414-173">[EWS reference for Exchange](ews-reference-for-exchange.md)</span></span> 
- [<span data-ttu-id="76414-174">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="76414-174">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

