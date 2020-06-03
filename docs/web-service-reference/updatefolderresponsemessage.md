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
description: UpdateFolderResponseMessage 要素には、UpdateFolder 操作要求の FolderChange 要素によって定義された更新の状態と結果が含まれています。
ms.openlocfilehash: bbe01583072e6203e099d440f2a171012f51e7df
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466585"
---
# <a name="updatefolderresponsemessage"></a><span data-ttu-id="876a5-103">UpdateFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="876a5-103">UpdateFolderResponseMessage</span></span>

<span data-ttu-id="876a5-104">**UpdateFolderResponseMessage**要素には、 [updatefolder 操作](updatefolder-operation.md)要求の[folderchange](folderchange.md)要素によって定義された更新の状態と結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="876a5-104">The **UpdateFolderResponseMessage** element contains the status and result of updates defined by the [FolderChange](folderchange.md) element of an [UpdateFolder operation](updatefolder-operation.md) request.</span></span> 
  
- [<span data-ttu-id="876a5-105">UpdateFolderResponse</span><span class="sxs-lookup"><span data-stu-id="876a5-105">UpdateFolderResponse</span></span>](updatefolderresponse.md) 
- [<span data-ttu-id="876a5-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="876a5-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="876a5-107">UpdateFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="876a5-107">UpdateFolderResponseMessage</span></span>](updatefolderresponsemessage.md)
  
```xml
<UpdateFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Folders/>
</UpdateFolderResponseMessage>
```

 <span data-ttu-id="876a5-108">**FolderInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="876a5-108">**FolderInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="876a5-109">属性と要素</span><span class="sxs-lookup"><span data-stu-id="876a5-109">Attributes and elements</span></span>

<span data-ttu-id="876a5-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="876a5-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="876a5-111">属性</span><span class="sxs-lookup"><span data-stu-id="876a5-111">Attributes</span></span>

|<span data-ttu-id="876a5-112">**属性**</span><span class="sxs-lookup"><span data-stu-id="876a5-112">**Attribute**</span></span>|<span data-ttu-id="876a5-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="876a5-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="876a5-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="876a5-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="876a5-115">[Updatefolder 操作](updatefolder-operation.md)の応答の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="876a5-115">Describes the status of an [UpdateFolder operation](updatefolder-operation.md) response.</span></span> <br/><br/><span data-ttu-id="876a5-116">この属性には、次の値が有効です。</span><span class="sxs-lookup"><span data-stu-id="876a5-116">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="876a5-117">-成功</span><span class="sxs-lookup"><span data-stu-id="876a5-117">-  Success</span></span>  <br/><span data-ttu-id="876a5-118">-Warning</span><span class="sxs-lookup"><span data-stu-id="876a5-118">-  Warning</span></span>  <br/><span data-ttu-id="876a5-119">-エラー</span><span class="sxs-lookup"><span data-stu-id="876a5-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="876a5-120">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="876a5-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="876a5-121">**値**</span><span class="sxs-lookup"><span data-stu-id="876a5-121">**Value**</span></span>|<span data-ttu-id="876a5-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="876a5-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="876a5-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="876a5-123">**Success**</span></span> <br/> |<span data-ttu-id="876a5-124">満たされる要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="876a5-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="876a5-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="876a5-125">**Warning**</span></span> <br/> | <span data-ttu-id="876a5-126">処理されなかった要求を示します。</span><span class="sxs-lookup"><span data-stu-id="876a5-126">Describes a request that was not processed.</span></span> <span data-ttu-id="876a5-127">要求内のアイテムが処理され、その後のアイテムを処理できなかったときにエラーが発生した場合は、警告が返されることがあります。</span><span class="sxs-lookup"><span data-stu-id="876a5-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="876a5-128">警告のソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="876a5-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="876a5-129">-Exchange ストアがオフラインになっている。</span><span class="sxs-lookup"><span data-stu-id="876a5-129">-  The Exchange store is offline.</span></span>  <br/><span data-ttu-id="876a5-130">-Active Directory ドメインサービス (AD DS) がオフラインになっています。</span><span class="sxs-lookup"><span data-stu-id="876a5-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="876a5-131">-メールボックスは移動されます。</span><span class="sxs-lookup"><span data-stu-id="876a5-131">-  A mailbox is moved.</span></span>  <br/><span data-ttu-id="876a5-132">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="876a5-132">-  A password is expired.</span></span>  <br/><span data-ttu-id="876a5-133">-クォータが上限を超えています。</span><span class="sxs-lookup"><span data-stu-id="876a5-133">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="876a5-134">**Error**</span><span class="sxs-lookup"><span data-stu-id="876a5-134">**Error**</span></span> <br/> | <span data-ttu-id="876a5-135">満たされない要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="876a5-135">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="876a5-136">エラーのソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="876a5-136">The following are examples of sources for errors:</span></span>  <br/><br/><span data-ttu-id="876a5-137">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="876a5-137">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="876a5-138">-属性または要素が範囲外です</span><span class="sxs-lookup"><span data-stu-id="876a5-138">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="876a5-139">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="876a5-139">-  Unknown tag</span></span>  <br/><span data-ttu-id="876a5-140">-属性または要素がコンテキスト内で有効ではありません</span><span class="sxs-lookup"><span data-stu-id="876a5-140">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="876a5-141">-クライアントによる権限のないアクセス試行</span><span class="sxs-lookup"><span data-stu-id="876a5-141">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="876a5-142">-有効なクライアント側の呼び出しに応答した場合のサーバー側エラー</span><span class="sxs-lookup"><span data-stu-id="876a5-142">-  Server-side failure in response to a valid client-side call</span></span>  <br/> <br/> <span data-ttu-id="876a5-143">エラーに関する情報については、応答[secの](responsecode.md)要素と[messagetext](messagetext.md)要素を参照してください。</span><span class="sxs-lookup"><span data-stu-id="876a5-143">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="876a5-144">子要素</span><span class="sxs-lookup"><span data-stu-id="876a5-144">Child elements</span></span>

|<span data-ttu-id="876a5-145">**Element**</span><span class="sxs-lookup"><span data-stu-id="876a5-145">**Element**</span></span>|<span data-ttu-id="876a5-146">**説明**</span><span class="sxs-lookup"><span data-stu-id="876a5-146">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="876a5-147">MessageText</span><span class="sxs-lookup"><span data-stu-id="876a5-147">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="876a5-148">応答の状態を説明するテキストを提供します。</span><span class="sxs-lookup"><span data-stu-id="876a5-148">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="876a5-149">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="876a5-149">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="876a5-150">要求で発生した特定のエラーを識別するエラーコードを提供します。</span><span class="sxs-lookup"><span data-stu-id="876a5-150">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="876a5-151">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="876a5-151">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="876a5-152">現在未使用で、今後の使用のために予約されています。</span><span class="sxs-lookup"><span data-stu-id="876a5-152">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="876a5-153">このプロパティには0の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="876a5-153">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="876a5-154">MessageXml</span><span class="sxs-lookup"><span data-stu-id="876a5-154">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="876a5-155">エラー応答に関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="876a5-155">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="876a5-156">フォルダー</span><span class="sxs-lookup"><span data-stu-id="876a5-156">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="876a5-157">Folder 操作で使用されるフォルダーの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="876a5-157">Contains an array of folders used in folder operations.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="876a5-158">親要素</span><span class="sxs-lookup"><span data-stu-id="876a5-158">Parent elements</span></span>

|<span data-ttu-id="876a5-159">**要素**</span><span class="sxs-lookup"><span data-stu-id="876a5-159">**Element**</span></span>|<span data-ttu-id="876a5-160">**説明**</span><span class="sxs-lookup"><span data-stu-id="876a5-160">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="876a5-161">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="876a5-161">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="876a5-162">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="876a5-162">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="876a5-163">注釈</span><span class="sxs-lookup"><span data-stu-id="876a5-163">Remarks</span></span>

<span data-ttu-id="876a5-164">この要素を記述するスキーマは、Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="876a5-164">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="876a5-165">要素の情報</span><span class="sxs-lookup"><span data-stu-id="876a5-165">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="876a5-166">Namespace</span><span class="sxs-lookup"><span data-stu-id="876a5-166">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="876a5-167">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="876a5-167">Schema Name</span></span>  <br/> |<span data-ttu-id="876a5-168">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="876a5-168">Messages schema</span></span>  <br/> |
|<span data-ttu-id="876a5-169">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="876a5-169">Validation File</span></span>  <br/> |<span data-ttu-id="876a5-170">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="876a5-170">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="876a5-171">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="876a5-171">Can be Empty</span></span>  <br/> |<span data-ttu-id="876a5-172">正しくない</span><span class="sxs-lookup"><span data-stu-id="876a5-172">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="876a5-173">関連項目</span><span class="sxs-lookup"><span data-stu-id="876a5-173">See also</span></span>

- [<span data-ttu-id="876a5-174">UpdateFolder 操作</span><span class="sxs-lookup"><span data-stu-id="876a5-174">UpdateFolder operation</span></span>](updatefolder-operation.md)

