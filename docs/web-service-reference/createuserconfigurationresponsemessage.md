---
title: CreateUserConfigurationResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateUserConfigurationResponseMessage
api_type:
- schema
ms.assetid: 9c11427c-74c9-4c6a-a0e7-7d5556670c1e
description: CreateUserConfigurationResponseMessage 要素には、1つの CreateUserConfiguration 要求の状態と結果が含まれています。
ms.openlocfilehash: 3217734f7451ad397c531cd9ff9ce7d44b13f6ba
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463735"
---
# <a name="createuserconfigurationresponsemessage"></a><span data-ttu-id="733c6-103">CreateUserConfigurationResponseMessage</span><span class="sxs-lookup"><span data-stu-id="733c6-103">CreateUserConfigurationResponseMessage</span></span>

<span data-ttu-id="733c6-104">**CreateUserConfigurationResponseMessage**要素には、1つの**CreateUserConfiguration**要求の状態と結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="733c6-104">The **CreateUserConfigurationResponseMessage** element contains the status and result of a single **CreateUserConfiguration** request.</span></span> 
  
```xml
<CreateUserConfigurationResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</CreateUserConfigurationResponseMessage>
```

<span data-ttu-id="733c6-105">**ResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="733c6-105">**ResponseMessageType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="733c6-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="733c6-106">Attributes and elements</span></span>

<span data-ttu-id="733c6-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="733c6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="733c6-108">属性</span><span class="sxs-lookup"><span data-stu-id="733c6-108">Attributes</span></span>

|<span data-ttu-id="733c6-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="733c6-109">**Attribute**</span></span>|<span data-ttu-id="733c6-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="733c6-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="733c6-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="733c6-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="733c6-112">応答の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="733c6-112">Describes the status of the response.</span></span><br/><br/><span data-ttu-id="733c6-113">この属性には、次の値が有効です。</span><span class="sxs-lookup"><span data-stu-id="733c6-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="733c6-114">-成功</span><span class="sxs-lookup"><span data-stu-id="733c6-114">-  Success</span></span>  <br/><span data-ttu-id="733c6-115">-Warning</span><span class="sxs-lookup"><span data-stu-id="733c6-115">-  Warning</span></span>  <br/><span data-ttu-id="733c6-116">-エラー</span><span class="sxs-lookup"><span data-stu-id="733c6-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="733c6-117">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="733c6-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="733c6-118">**値**</span><span class="sxs-lookup"><span data-stu-id="733c6-118">**Value**</span></span>|<span data-ttu-id="733c6-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="733c6-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="733c6-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="733c6-120">**Success**</span></span> <br/> |<span data-ttu-id="733c6-121">満たされる要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="733c6-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="733c6-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="733c6-122">**Warning**</span></span> <br/> | <span data-ttu-id="733c6-123">処理されなかった要求を示します。</span><span class="sxs-lookup"><span data-stu-id="733c6-123">Describes a request that was not processed.</span></span> <span data-ttu-id="733c6-124">要求内のアイテムが処理され、その後のアイテムを処理できなかったときにエラーが発生した場合は、警告が返されることがあります。</span><span class="sxs-lookup"><span data-stu-id="733c6-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="733c6-125">警告のソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="733c6-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="733c6-126">-バッチ処理中に Exchange ストアがオフラインになります。</span><span class="sxs-lookup"><span data-stu-id="733c6-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="733c6-127">-Active Directory ドメインサービス (AD DS) がオフラインになっています。</span><span class="sxs-lookup"><span data-stu-id="733c6-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="733c6-128">-メールボックスが移動されました。</span><span class="sxs-lookup"><span data-stu-id="733c6-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="733c6-129">-メッセージデータベース (MDB) はオフラインです。</span><span class="sxs-lookup"><span data-stu-id="733c6-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="733c6-130">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="733c6-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="733c6-131">-クォータが限界を超えています。</span><span class="sxs-lookup"><span data-stu-id="733c6-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="733c6-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="733c6-132">**Error**</span></span> <br/> | <span data-ttu-id="733c6-133">満たされない要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="733c6-133">Describes a request that cannot be fulfilled.</span></span><br/><br/> <span data-ttu-id="733c6-134">エラーのソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="733c6-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="733c6-135">-属性または要素が無効です。</span><span class="sxs-lookup"><span data-stu-id="733c6-135">-  Invalid attributes or elements.</span></span>  <br/><span data-ttu-id="733c6-136">-範囲外の属性または要素。</span><span class="sxs-lookup"><span data-stu-id="733c6-136">-  Attributes or elements that are out of range.</span></span>  <br/><span data-ttu-id="733c6-137">-不明なタグ。</span><span class="sxs-lookup"><span data-stu-id="733c6-137">-  An unknown tag.</span></span>  <br/><span data-ttu-id="733c6-138">-属性または要素がコンテキスト内で有効ではありません。</span><span class="sxs-lookup"><span data-stu-id="733c6-138">-  The attribute or element is not valid in the context.</span></span>  <br/><span data-ttu-id="733c6-139">-クライアントによる権限のないアクセス試行。</span><span class="sxs-lookup"><span data-stu-id="733c6-139">-  An unauthorized access attempt by any client.</span></span>  <br/><span data-ttu-id="733c6-140">-有効なクライアント側の呼び出しに応答して、サーバー側で障害が発生した。</span><span class="sxs-lookup"><span data-stu-id="733c6-140">-  A server-side failure in response to a valid client-side call.</span></span><br/><br/>  <span data-ttu-id="733c6-141">エラーに関する情報については、応答[secの](responsecode.md)要素と[messagetext](messagetext.md)要素を参照してください。</span><span class="sxs-lookup"><span data-stu-id="733c6-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="733c6-142">子要素</span><span class="sxs-lookup"><span data-stu-id="733c6-142">Child elements</span></span>

|<span data-ttu-id="733c6-143">**Element**</span><span class="sxs-lookup"><span data-stu-id="733c6-143">**Element**</span></span>|<span data-ttu-id="733c6-144">**説明**</span><span class="sxs-lookup"><span data-stu-id="733c6-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="733c6-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="733c6-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="733c6-146">応答の状態を説明するテキストを提供します。</span><span class="sxs-lookup"><span data-stu-id="733c6-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="733c6-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="733c6-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="733c6-148">要求で発生した特定のエラーを識別するエラーコードを提供します。</span><span class="sxs-lookup"><span data-stu-id="733c6-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="733c6-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="733c6-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="733c6-150">現在未使用で、今後の使用のために予約されています。</span><span class="sxs-lookup"><span data-stu-id="733c6-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="733c6-151">この要素には0の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="733c6-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="733c6-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="733c6-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="733c6-153">エラー応答に関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="733c6-153">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="733c6-154">親要素</span><span class="sxs-lookup"><span data-stu-id="733c6-154">Parent elements</span></span>

|<span data-ttu-id="733c6-155">**要素**</span><span class="sxs-lookup"><span data-stu-id="733c6-155">**Element**</span></span>|<span data-ttu-id="733c6-156">**説明**</span><span class="sxs-lookup"><span data-stu-id="733c6-156">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="733c6-157">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="733c6-157">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="733c6-158">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="733c6-158">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="733c6-159">テキスト値</span><span class="sxs-lookup"><span data-stu-id="733c6-159">Text value</span></span>

<span data-ttu-id="733c6-160">なし。</span><span class="sxs-lookup"><span data-stu-id="733c6-160">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="733c6-161">注釈</span><span class="sxs-lookup"><span data-stu-id="733c6-161">Remarks</span></span>

<span data-ttu-id="733c6-162">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="733c6-162">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="733c6-163">要素の情報</span><span class="sxs-lookup"><span data-stu-id="733c6-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="733c6-164">Namespace</span><span class="sxs-lookup"><span data-stu-id="733c6-164">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="733c6-165">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="733c6-165">Schema Name</span></span>  <br/> |<span data-ttu-id="733c6-166">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="733c6-166">Messages schema</span></span>  <br/> |
|<span data-ttu-id="733c6-167">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="733c6-167">Validation File</span></span>  <br/> |<span data-ttu-id="733c6-168">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="733c6-168">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="733c6-169">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="733c6-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="733c6-170">正しくない</span><span class="sxs-lookup"><span data-stu-id="733c6-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="733c6-171">関連項目</span><span class="sxs-lookup"><span data-stu-id="733c6-171">See also</span></span>

- [<span data-ttu-id="733c6-172">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="733c6-172">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

