---
title: ClientExtension
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3445ef2b-1bb1-43ea-bc93-85c72401e5b6
description: ClientExtension 要素には、アプリに関するユーザーおよび構成情報が含まれています。
ms.openlocfilehash: d3d9ce1d242a63f28da3464f0faff86abde502c9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460198"
---
# <a name="clientextension"></a><span data-ttu-id="061bf-103">ClientExtension</span><span class="sxs-lookup"><span data-stu-id="061bf-103">ClientExtension</span></span>

<span data-ttu-id="061bf-104">**Clientextension**要素には、アプリに関するユーザーおよび構成情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="061bf-104">The **ClientExtension** element contains user and configuration information about an app.</span></span> 
  
```XML
<ClientExtension IsAvailable=" true | false " IsMandatory=" true | false " IsEnabledByDefault=" true | false " Type="" Scope="" MarketplaceAssetId="" MarketplaceContentMarket="" AppStatus="" Etoken="">
    <SpecificUsers></SpecificUsers>
    <Manifest></Manifest>
</ClientExtension>
```

 <span data-ttu-id="061bf-105">**ClientExtensionType**</span><span class="sxs-lookup"><span data-stu-id="061bf-105">**ClientExtensionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="061bf-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="061bf-106">Attributes and elements</span></span>

<span data-ttu-id="061bf-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="061bf-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="061bf-108">属性</span><span class="sxs-lookup"><span data-stu-id="061bf-108">Attributes</span></span>

|<span data-ttu-id="061bf-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="061bf-109">**Attribute**</span></span>|<span data-ttu-id="061bf-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="061bf-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="061bf-111">IsAvailable</span><span class="sxs-lookup"><span data-stu-id="061bf-111">IsAvailable</span></span>  <br/> |<span data-ttu-id="061bf-112">アプリが利用可能かどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="061bf-112">Specifies whether the app is available.</span></span> <span data-ttu-id="061bf-113">**IsAvailable**属性のテキスト値が**true**の場合は、アプリが利用可能であることを示します。</span><span class="sxs-lookup"><span data-stu-id="061bf-113">A text value of **true** for the **IsAvailable** attribute indicates that the app is available.</span></span> <span data-ttu-id="061bf-114">値が**false**の場合は、アプリが使用できないことを示します。</span><span class="sxs-lookup"><span data-stu-id="061bf-114">A value of **false** indicates that the app is not available.</span></span> <span data-ttu-id="061bf-115">この属性は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="061bf-115">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="061bf-116">IsMandatory</span><span class="sxs-lookup"><span data-stu-id="061bf-116">IsMandatory</span></span>  <br/> |<span data-ttu-id="061bf-117">アプリが必須であるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="061bf-117">Specifies whether the app is mandatory.</span></span> <span data-ttu-id="061bf-118">**Ismandatory**属性のテキスト値が**true の場合**は、そのアプリがメールボックスに対して必須であることを示します。</span><span class="sxs-lookup"><span data-stu-id="061bf-118">A text value of **true** for the **IsMandatory** attribute indicates that the app is mandatory for the mailbox.</span></span> <span data-ttu-id="061bf-119">値が**false**の場合、アプリは必須ではないことを示します。</span><span class="sxs-lookup"><span data-stu-id="061bf-119">A value of **false** indicates that the app is not mandatory.</span></span> <span data-ttu-id="061bf-120">この属性は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="061bf-120">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="061bf-121">IsEnabledByDefault デフォルト)</span><span class="sxs-lookup"><span data-stu-id="061bf-121">IsEnabledByDefault</span></span>  <br/> |<span data-ttu-id="061bf-122">アプリが既定で有効になっているかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="061bf-122">Specifies whether the app is enabled by default.</span></span> <span data-ttu-id="061bf-123">**Isenabledbydefault**属性のテキスト値が**true の場合**は、アプリが既定で有効になっていることを示します。</span><span class="sxs-lookup"><span data-stu-id="061bf-123">A text value of **true** for the **IsEnabledByDefault** attribute indicates that the app is enabled by default.</span></span> <span data-ttu-id="061bf-124">値が**false**の場合、アプリが既定で有効になっていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="061bf-124">A value of **false** indicates that the app is not enabled by default.</span></span> <span data-ttu-id="061bf-125">この属性は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="061bf-125">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="061bf-126">ProvidedTo</span><span class="sxs-lookup"><span data-stu-id="061bf-126">ProvidedTo</span></span>  <br/> |<span data-ttu-id="061bf-127">アプリが提供されるユーザーを指定します。</span><span class="sxs-lookup"><span data-stu-id="061bf-127">Specifies to whom the app is provided.</span></span> <span data-ttu-id="061bf-128">この属性は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="061bf-128">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="061bf-129">種類</span><span class="sxs-lookup"><span data-stu-id="061bf-129">Type</span></span>  <br/> |<span data-ttu-id="061bf-130">アプリの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="061bf-130">Specifies the type of the app.</span></span>  <br/> |
|<span data-ttu-id="061bf-131">範囲</span><span class="sxs-lookup"><span data-stu-id="061bf-131">Scope</span></span>  <br/> |<span data-ttu-id="061bf-132">アプリのスコープを指定します。</span><span class="sxs-lookup"><span data-stu-id="061bf-132">Specifies the scope of the app.</span></span>  <br/> |
|<span data-ttu-id="061bf-133">MarketplaceAssetId</span><span class="sxs-lookup"><span data-stu-id="061bf-133">MarketplaceAssetId</span></span>  <br/> |<span data-ttu-id="061bf-134">アプリの marketplace アセット識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="061bf-134">Specifies the marketplace asset identifier of the app.</span></span>  <br/> |
|<span data-ttu-id="061bf-135">MarketplaceContentMarket</span><span class="sxs-lookup"><span data-stu-id="061bf-135">MarketplaceContentMarket</span></span>  <br/> |<span data-ttu-id="061bf-136">ユーザーがアプリに関する詳細およびレビューのために表示する marketplace コンテンツを指定します。</span><span class="sxs-lookup"><span data-stu-id="061bf-136">Specifies the marketplace content that a user sees for details and reviews about an app.</span></span>  <br/> |
|<span data-ttu-id="061bf-137">AppStatus</span><span class="sxs-lookup"><span data-stu-id="061bf-137">AppStatus</span></span>  <br/> |<span data-ttu-id="061bf-138">予期しない状態にあるメールアプリの状態コードを指定します。</span><span class="sxs-lookup"><span data-stu-id="061bf-138">Specifies the status code of a mail app in an unexpected state.</span></span>  <br/> |
|<span data-ttu-id="061bf-139">Etoken</span><span class="sxs-lookup"><span data-stu-id="061bf-139">Etoken</span></span>  <br/> |<span data-ttu-id="061bf-140">有料または試用版のメールアプリのライセンストークンを指定します。</span><span class="sxs-lookup"><span data-stu-id="061bf-140">Specifies the license token for paid or trial mail apps.</span></span>  <br/> |
   
#### <a name="type"></a><span data-ttu-id="061bf-141">種類</span><span class="sxs-lookup"><span data-stu-id="061bf-141">Type</span></span>

|<span data-ttu-id="061bf-142">**値**</span><span class="sxs-lookup"><span data-stu-id="061bf-142">**Value**</span></span>|<span data-ttu-id="061bf-143">**説明**</span><span class="sxs-lookup"><span data-stu-id="061bf-143">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="061bf-144">既定値</span><span class="sxs-lookup"><span data-stu-id="061bf-144">Default</span></span>  <br/> |<span data-ttu-id="061bf-145">アプリが既定で利用できることを示します。</span><span class="sxs-lookup"><span data-stu-id="061bf-145">Indicates that the app is available by default.</span></span>  <br/> |
|<span data-ttu-id="061bf-146">Kirkland</span><span class="sxs-lookup"><span data-stu-id="061bf-146">Private</span></span>  <br/> |<span data-ttu-id="061bf-147">アプリがプライベートであることを示します。</span><span class="sxs-lookup"><span data-stu-id="061bf-147">Indicates that the app is private.</span></span>  <br/> |
|<span data-ttu-id="061bf-148">プレース</span><span class="sxs-lookup"><span data-stu-id="061bf-148">MarketPlace</span></span>  <br/> |<span data-ttu-id="061bf-149">アプリが marketplace アプリであることを示します。</span><span class="sxs-lookup"><span data-stu-id="061bf-149">Indicates that the app is a marketplace app.</span></span>  <br/> |
   
#### <a name="scope"></a><span data-ttu-id="061bf-150">範囲</span><span class="sxs-lookup"><span data-stu-id="061bf-150">Scope</span></span>

|<span data-ttu-id="061bf-151">**値**</span><span class="sxs-lookup"><span data-stu-id="061bf-151">**Value**</span></span>|<span data-ttu-id="061bf-152">**説明**</span><span class="sxs-lookup"><span data-stu-id="061bf-152">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="061bf-153">なし</span><span class="sxs-lookup"><span data-stu-id="061bf-153">None</span></span>  <br/> |<span data-ttu-id="061bf-154">アプリにスコープがないことを示します。</span><span class="sxs-lookup"><span data-stu-id="061bf-154">Indicates that the app has no scope.</span></span>  <br/> |
|<span data-ttu-id="061bf-155">User</span><span class="sxs-lookup"><span data-stu-id="061bf-155">User</span></span>  <br/> |<span data-ttu-id="061bf-156">アプリがユーザーごとにあることを示します。</span><span class="sxs-lookup"><span data-stu-id="061bf-156">Indicates that the app is per user.</span></span>  <br/> |
|<span data-ttu-id="061bf-157">組織</span><span class="sxs-lookup"><span data-stu-id="061bf-157">Organization</span></span>  <br/> |<span data-ttu-id="061bf-158">アプリが組織用であることを示します。</span><span class="sxs-lookup"><span data-stu-id="061bf-158">Indicates that the app is for an organization.</span></span>  <br/> |
|<span data-ttu-id="061bf-159">既定値</span><span class="sxs-lookup"><span data-stu-id="061bf-159">Default</span></span>  <br/> |<span data-ttu-id="061bf-160">アプリが既定のアプリであることを示します。</span><span class="sxs-lookup"><span data-stu-id="061bf-160">Indicates that the app is a default app.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="061bf-161">子要素</span><span class="sxs-lookup"><span data-stu-id="061bf-161">Child elements</span></span>

|<span data-ttu-id="061bf-162">**Element**</span><span class="sxs-lookup"><span data-stu-id="061bf-162">**Element**</span></span>|<span data-ttu-id="061bf-163">**説明**</span><span class="sxs-lookup"><span data-stu-id="061bf-163">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="061bf-164">固有のユーザー</span><span class="sxs-lookup"><span data-stu-id="061bf-164">SpecificUsers</span></span>](specificusers.md) <br/> |<span data-ttu-id="061bf-165">アプリにアクセスできる電子メールアカウントを指定します。</span><span class="sxs-lookup"><span data-stu-id="061bf-165">Specifies the email accounts that can access the app.</span></span>  <br/> |
|[<span data-ttu-id="061bf-166">マニフェスト</span><span class="sxs-lookup"><span data-stu-id="061bf-166">Manifest</span></span>](manifest.md) <br/> |<span data-ttu-id="061bf-167">64でエンコードされたアプリケーションマニフェストファイルが保存されています。</span><span class="sxs-lookup"><span data-stu-id="061bf-167">Contains the base-64 encoded app manifest file.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="061bf-168">親要素</span><span class="sxs-lookup"><span data-stu-id="061bf-168">Parent elements</span></span>

|<span data-ttu-id="061bf-169">**要素**</span><span class="sxs-lookup"><span data-stu-id="061bf-169">**Element**</span></span>|<span data-ttu-id="061bf-170">**説明**</span><span class="sxs-lookup"><span data-stu-id="061bf-170">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="061bf-171">ClientExtensions</span><span class="sxs-lookup"><span data-stu-id="061bf-171">ClientExtensions</span></span>](clientextensions.md) <br/> |<span data-ttu-id="061bf-172">**Clientextension**要素の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="061bf-172">Specifies an array of **ClientExtension** elements.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="061bf-173">注釈</span><span class="sxs-lookup"><span data-stu-id="061bf-173">Remarks</span></span>

<span data-ttu-id="061bf-174">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="061bf-174">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="061bf-175">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="061bf-175">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="061bf-176">要素の情報</span><span class="sxs-lookup"><span data-stu-id="061bf-176">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="061bf-177">Namespace</span><span class="sxs-lookup"><span data-stu-id="061bf-177">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="061bf-178">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="061bf-178">Schema Name</span></span>  <br/> |<span data-ttu-id="061bf-179">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="061bf-179">Type schema</span></span>  <br/> |
|<span data-ttu-id="061bf-180">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="061bf-180">Validation File</span></span>  <br/> |<span data-ttu-id="061bf-181">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="061bf-181">types.xsd</span></span>  <br/> |
|<span data-ttu-id="061bf-182">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="061bf-182">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="061bf-183">関連項目</span><span class="sxs-lookup"><span data-stu-id="061bf-183">See also</span></span>



- [<span data-ttu-id="061bf-184">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="061bf-184">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

