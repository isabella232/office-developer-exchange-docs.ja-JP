---
title: UpdateFolderResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateFolderResponseMessage
api_type:
- schema
ms.assetid: 914bb683-49ee-44a2-b59d-ef560244dfb8
description: UpdateFolderResponseMessage 要素には、ステータスおよび UpdateFolder 操作要求の FolderChange 要素で定義されている更新プログラムの結果が含まれています。
ms.openlocfilehash: 4cd00232bcc233f6534d844418f523c248ce54bf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839852"
---
# <a name="updatefolderresponsemessage"></a><span data-ttu-id="7b00f-103">UpdateFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="7b00f-103">UpdateFolderResponseMessage</span></span>

<span data-ttu-id="7b00f-104">**UpdateFolderResponseMessage**要素には、ステータスおよび[UpdateFolder 操作](updatefolder-operation.md)要求の[FolderChange](folderchange.md)要素で定義されている更新プログラムの結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="7b00f-104">The **UpdateFolderResponseMessage** element contains the status and result of updates defined by the [FolderChange](folderchange.md) element of an [UpdateFolder operation](updatefolder-operation.md) request.</span></span> 
  
- [<span data-ttu-id="7b00f-105">UpdateFolderResponse</span><span class="sxs-lookup"><span data-stu-id="7b00f-105">UpdateFolderResponse</span></span>](updatefolderresponse.md) 
- [<span data-ttu-id="7b00f-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="7b00f-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="7b00f-107">UpdateFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="7b00f-107">UpdateFolderResponseMessage</span></span>](updatefolderresponsemessage.md)
  
```xml
<UpdateFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Folders/>
</UpdateFolderResponseMessage>
```

 <span data-ttu-id="7b00f-108">**FolderInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="7b00f-108">**FolderInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7b00f-109">属性および要素</span><span class="sxs-lookup"><span data-stu-id="7b00f-109">Attributes and elements</span></span>

<span data-ttu-id="7b00f-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7b00f-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7b00f-111">属性</span><span class="sxs-lookup"><span data-stu-id="7b00f-111">Attributes</span></span>

|<span data-ttu-id="7b00f-112">**属性**</span><span class="sxs-lookup"><span data-stu-id="7b00f-112">**Attribute**</span></span>|<span data-ttu-id="7b00f-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="7b00f-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7b00f-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="7b00f-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="7b00f-115">[UpdateFolder 操作](updatefolder-operation.md)応答のステータスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="7b00f-115">Describes the status of an [UpdateFolder operation](updatefolder-operation.md) response.</span></span> <br/><br/><span data-ttu-id="7b00f-116">次の値は、この属性の有効です。</span><span class="sxs-lookup"><span data-stu-id="7b00f-116">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="7b00f-117">-成功</span><span class="sxs-lookup"><span data-stu-id="7b00f-117">-  Success</span></span>  <br/><span data-ttu-id="7b00f-118">-警告</span><span class="sxs-lookup"><span data-stu-id="7b00f-118">-  Warning</span></span>  <br/><span data-ttu-id="7b00f-119">-エラー</span><span class="sxs-lookup"><span data-stu-id="7b00f-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="7b00f-120">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="7b00f-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="7b00f-121">**値**</span><span class="sxs-lookup"><span data-stu-id="7b00f-121">**Value**</span></span>|<span data-ttu-id="7b00f-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="7b00f-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7b00f-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="7b00f-123">**Success**</span></span> <br/> |<span data-ttu-id="7b00f-124">満了する要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="7b00f-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="7b00f-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="7b00f-125">**Warning**</span></span> <br/> | <span data-ttu-id="7b00f-126">処理されなかった要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="7b00f-126">Describes a request that was not processed.</span></span> <span data-ttu-id="7b00f-127">警告は、要求内のアイテムを処理し、それ以降の項目を処理できませんでした、エラーが発生した場合に返される場合があります。</span><span class="sxs-lookup"><span data-stu-id="7b00f-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="7b00f-128">警告の送信元の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7b00f-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="7b00f-129">-Exchange ストアでは、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="7b00f-129">-  The Exchange store is offline.</span></span>  <br/><span data-ttu-id="7b00f-130">-Active Directory ドメイン サービス (AD DS) では、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="7b00f-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="7b00f-131">-メールボックスを移動するとします。</span><span class="sxs-lookup"><span data-stu-id="7b00f-131">-  A mailbox is moved.</span></span>  <br/><span data-ttu-id="7b00f-132">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="7b00f-132">-  A password is expired.</span></span>  <br/><span data-ttu-id="7b00f-133">クォータを超えています。</span><span class="sxs-lookup"><span data-stu-id="7b00f-133">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="7b00f-134">**Error**</span><span class="sxs-lookup"><span data-stu-id="7b00f-134">**Error**</span></span> <br/> | <span data-ttu-id="7b00f-135">満たせない要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="7b00f-135">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="7b00f-136">次に、エラーのソースの例を示します。</span><span class="sxs-lookup"><span data-stu-id="7b00f-136">The following are examples of sources for errors:</span></span>  <br/><br/><span data-ttu-id="7b00f-137">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="7b00f-137">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="7b00f-138">属性または要素が範囲外です</span><span class="sxs-lookup"><span data-stu-id="7b00f-138">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="7b00f-139">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="7b00f-139">-  Unknown tag</span></span>  <br/><span data-ttu-id="7b00f-140">属性または要素のコンテキストでは無効です</span><span class="sxs-lookup"><span data-stu-id="7b00f-140">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="7b00f-141">の任意のクライアントから不正アクセスしようと</span><span class="sxs-lookup"><span data-stu-id="7b00f-141">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="7b00f-142">の有効なクライアント側の呼び出しに応答サーバー側の障害</span><span class="sxs-lookup"><span data-stu-id="7b00f-142">-  Server-side failure in response to a valid client-side call</span></span>  <br/> <br/> <span data-ttu-id="7b00f-143">エラーに関する情報は、 [ResponseCode](responsecode.md)および[メッセージ テキスト](messagetext.md)の要素を参照しています。</span><span class="sxs-lookup"><span data-stu-id="7b00f-143">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="7b00f-144">子要素</span><span class="sxs-lookup"><span data-stu-id="7b00f-144">Child elements</span></span>

|<span data-ttu-id="7b00f-145">**要素**</span><span class="sxs-lookup"><span data-stu-id="7b00f-145">**Element**</span></span>|<span data-ttu-id="7b00f-146">**説明**</span><span class="sxs-lookup"><span data-stu-id="7b00f-146">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7b00f-147">MessageText</span><span class="sxs-lookup"><span data-stu-id="7b00f-147">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="7b00f-148">応答のステータスの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="7b00f-148">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="7b00f-149">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="7b00f-149">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="7b00f-150">要求で発生した特定のエラーを識別するエラー コードを提供します。</span><span class="sxs-lookup"><span data-stu-id="7b00f-150">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="7b00f-151">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="7b00f-151">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="7b00f-152">現在使用されていない将来の使用に予約されているとします。</span><span class="sxs-lookup"><span data-stu-id="7b00f-152">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="7b00f-153">0 の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="7b00f-153">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="7b00f-154">MessageXml</span><span class="sxs-lookup"><span data-stu-id="7b00f-154">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="7b00f-155">追加のエラー応答情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="7b00f-155">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="7b00f-156">フォルダー</span><span class="sxs-lookup"><span data-stu-id="7b00f-156">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="7b00f-157">フォルダーの操作に使用するフォルダーの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="7b00f-157">Contains an array of folders used in folder operations.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7b00f-158">親要素</span><span class="sxs-lookup"><span data-stu-id="7b00f-158">Parent elements</span></span>

|<span data-ttu-id="7b00f-159">**要素**</span><span class="sxs-lookup"><span data-stu-id="7b00f-159">**Element**</span></span>|<span data-ttu-id="7b00f-160">**説明**</span><span class="sxs-lookup"><span data-stu-id="7b00f-160">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7b00f-161">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="7b00f-161">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="7b00f-162">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="7b00f-162">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7b00f-163">備考</span><span class="sxs-lookup"><span data-stu-id="7b00f-163">Remarks</span></span>

<span data-ttu-id="7b00f-164">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="7b00f-164">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7b00f-165">要素情報</span><span class="sxs-lookup"><span data-stu-id="7b00f-165">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7b00f-166">名前空間</span><span class="sxs-lookup"><span data-stu-id="7b00f-166">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7b00f-167">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7b00f-167">Schema Name</span></span>  <br/> |<span data-ttu-id="7b00f-168">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="7b00f-168">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7b00f-169">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7b00f-169">Validation File</span></span>  <br/> |<span data-ttu-id="7b00f-170">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="7b00f-170">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7b00f-171">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="7b00f-171">Can be Empty</span></span>  <br/> |<span data-ttu-id="7b00f-172">False</span><span class="sxs-lookup"><span data-stu-id="7b00f-172">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7b00f-173">関連項目</span><span class="sxs-lookup"><span data-stu-id="7b00f-173">See also</span></span>

- <span data-ttu-id="7b00f-174">
  [UpdateFolder 操作](updatefolder-operation.md)</span><span class="sxs-lookup"><span data-stu-id="7b00f-174">[UpdateFolder operation](updatefolder-operation.md)</span></span>

