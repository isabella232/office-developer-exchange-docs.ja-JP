---
title: ClientExtension
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3445ef2b-1bb1-43ea-bc93-85c72401e5b6
description: ClientExtension 要素には、アプリケーションのユーザーおよび構成情報が含まれています。
ms.openlocfilehash: 5051248a2c8e664d82666bd7b42ee3c3046f43fe
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759626"
---
# <a name="clientextension"></a><span data-ttu-id="832c8-103">ClientExtension</span><span class="sxs-lookup"><span data-stu-id="832c8-103">ClientExtension</span></span>

<span data-ttu-id="832c8-104">**ClientExtension**要素には、アプリケーションのユーザーおよび構成情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="832c8-104">The **ClientExtension** element contains user and configuration information about an app.</span></span> 
  
```XML
<ClientExtension IsAvailable=" true | false " IsMandatory=" true | false " IsEnabledByDefault=" true | false " Type="" Scope="" MarketplaceAssetId="" MarketplaceContentMarket="" AppStatus="" Etoken="">
    <SpecificUsers></SpecificUsers>
    <Manifest></Manifest>
</ClientExtension>
```

 <span data-ttu-id="832c8-105">**ClientExtensionType**</span><span class="sxs-lookup"><span data-stu-id="832c8-105">**ClientExtensionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="832c8-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="832c8-106">Attributes and elements</span></span>

<span data-ttu-id="832c8-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="832c8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="832c8-108">属性</span><span class="sxs-lookup"><span data-stu-id="832c8-108">Attributes</span></span>

|<span data-ttu-id="832c8-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="832c8-109">**Attribute**</span></span>|<span data-ttu-id="832c8-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="832c8-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="832c8-111">提供</span><span class="sxs-lookup"><span data-stu-id="832c8-111">IsAvailable</span></span>  <br/> |<span data-ttu-id="832c8-112">アプリケーションが使用できるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="832c8-112">Specifies whether the app is available.</span></span> <span data-ttu-id="832c8-113">テキストの値**は true**属性で**提供**は、アプリケーションが利用できることを示します。</span><span class="sxs-lookup"><span data-stu-id="832c8-113">A text value of **true** for the **IsAvailable** attribute indicates that the app is available.</span></span> <span data-ttu-id="832c8-114">**False**の値は、アプリケーションが使用できないことを示します。</span><span class="sxs-lookup"><span data-stu-id="832c8-114">A value of **false** indicates that the app is not available.</span></span> <span data-ttu-id="832c8-115">この属性は、省略可能です。</span><span class="sxs-lookup"><span data-stu-id="832c8-115">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="832c8-116">IsMandatory</span><span class="sxs-lookup"><span data-stu-id="832c8-116">IsMandatory</span></span>  <br/> |<span data-ttu-id="832c8-117">アプリケーションが必須かどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="832c8-117">Specifies whether the app is mandatory.</span></span> <span data-ttu-id="832c8-118">の**場合は true** 、 **IsMandatory**属性のテキスト値は、アプリケーションがメールボックスの必須であることを示します。</span><span class="sxs-lookup"><span data-stu-id="832c8-118">A text value of **true** for the **IsMandatory** attribute indicates that the app is mandatory for the mailbox.</span></span> <span data-ttu-id="832c8-119">**False**の値は、アプリケーションが必須ではないことを示します。</span><span class="sxs-lookup"><span data-stu-id="832c8-119">A value of **false** indicates that the app is not mandatory.</span></span> <span data-ttu-id="832c8-120">この属性は、省略可能です。</span><span class="sxs-lookup"><span data-stu-id="832c8-120">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="832c8-121">IsEnabledByDefault</span><span class="sxs-lookup"><span data-stu-id="832c8-121">IsEnabledByDefault</span></span>  <br/> |<span data-ttu-id="832c8-122">アプリケーションが既定で有効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="832c8-122">Specifies whether the app is enabled by default.</span></span> <span data-ttu-id="832c8-123">の**場合は true** 、 **IsEnabledByDefault**属性のテキスト値は、アプリケーションが既定で有効になっていることを示します。</span><span class="sxs-lookup"><span data-stu-id="832c8-123">A text value of **true** for the **IsEnabledByDefault** attribute indicates that the app is enabled by default.</span></span> <span data-ttu-id="832c8-124">**False**の値は、アプリケーションが既定で無効になっていることを示します。</span><span class="sxs-lookup"><span data-stu-id="832c8-124">A value of **false** indicates that the app is not enabled by default.</span></span> <span data-ttu-id="832c8-125">この属性は、省略可能です。</span><span class="sxs-lookup"><span data-stu-id="832c8-125">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="832c8-126">受ける</span><span class="sxs-lookup"><span data-stu-id="832c8-126">ProvidedTo</span></span>  <br/> |<span data-ttu-id="832c8-127">アプリケーションの提供先を指定します。</span><span class="sxs-lookup"><span data-stu-id="832c8-127">Specifies to whom the app is provided.</span></span> <span data-ttu-id="832c8-128">この属性は、省略可能です。</span><span class="sxs-lookup"><span data-stu-id="832c8-128">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="832c8-129">型</span><span class="sxs-lookup"><span data-stu-id="832c8-129">Type</span></span>  <br/> |<span data-ttu-id="832c8-130">アプリケーションの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="832c8-130">Specifies the type of the app.</span></span>  <br/> |
|<span data-ttu-id="832c8-131">スコープ</span><span class="sxs-lookup"><span data-stu-id="832c8-131">Scope</span></span>  <br/> |<span data-ttu-id="832c8-132">アプリケーションのスコープを指定します。</span><span class="sxs-lookup"><span data-stu-id="832c8-132">Specifies the scope of the app.</span></span>  <br/> |
|<span data-ttu-id="832c8-133">MarketplaceAssetId</span><span class="sxs-lookup"><span data-stu-id="832c8-133">MarketplaceAssetId</span></span>  <br/> |<span data-ttu-id="832c8-134">アプリケーションの市場の資産の id を指定します。</span><span class="sxs-lookup"><span data-stu-id="832c8-134">Specifies the marketplace asset identifier of the app.</span></span>  <br/> |
|<span data-ttu-id="832c8-135">MarketplaceContentMarket</span><span class="sxs-lookup"><span data-stu-id="832c8-135">MarketplaceContentMarket</span></span>  <br/> |<span data-ttu-id="832c8-136">マーケットプ レース コンテンツをユーザーの詳細情報の表示し、アプリのレビューを指定します。</span><span class="sxs-lookup"><span data-stu-id="832c8-136">Specifies the marketplace content that a user sees for details and reviews about an app.</span></span>  <br/> |
|<span data-ttu-id="832c8-137">AppStatus</span><span class="sxs-lookup"><span data-stu-id="832c8-137">AppStatus</span></span>  <br/> |<span data-ttu-id="832c8-138">予期しない状態では、メール アプリケーションのステータス コードを指定します。</span><span class="sxs-lookup"><span data-stu-id="832c8-138">Specifies the status code of a mail app in an unexpected state.</span></span>  <br/> |
|<span data-ttu-id="832c8-139">Etoken</span><span class="sxs-lookup"><span data-stu-id="832c8-139">Etoken</span></span>  <br/> |<span data-ttu-id="832c8-140">メールまたは有料の試用版のアプリのライセンス トークンを指定します。</span><span class="sxs-lookup"><span data-stu-id="832c8-140">Specifies the license token for paid or trial mail apps.</span></span>  <br/> |
   
#### <a name="type"></a><span data-ttu-id="832c8-141">型</span><span class="sxs-lookup"><span data-stu-id="832c8-141">Type</span></span>

|<span data-ttu-id="832c8-142">**値**</span><span class="sxs-lookup"><span data-stu-id="832c8-142">**Value**</span></span>|<span data-ttu-id="832c8-143">**説明**</span><span class="sxs-lookup"><span data-stu-id="832c8-143">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="832c8-144">Default</span><span class="sxs-lookup"><span data-stu-id="832c8-144">Default</span></span>  <br/> |<span data-ttu-id="832c8-145">アプリケーションが既定で使用できることを示します。</span><span class="sxs-lookup"><span data-stu-id="832c8-145">Indicates that the app is available by default.</span></span>  <br/> |
|<span data-ttu-id="832c8-146">非公開</span><span class="sxs-lookup"><span data-stu-id="832c8-146">Private</span></span>  <br/> |<span data-ttu-id="832c8-147">アプリケーションがプライベートであることを示します。</span><span class="sxs-lookup"><span data-stu-id="832c8-147">Indicates that the app is private.</span></span>  <br/> |
|<span data-ttu-id="832c8-148">マーケットプ レース</span><span class="sxs-lookup"><span data-stu-id="832c8-148">MarketPlace</span></span>  <br/> |<span data-ttu-id="832c8-149">アプリケーションが市場のアプリケーションであることを示します。</span><span class="sxs-lookup"><span data-stu-id="832c8-149">Indicates that the app is a marketplace app.</span></span>  <br/> |
   
#### <a name="scope"></a><span data-ttu-id="832c8-150">スコープ</span><span class="sxs-lookup"><span data-stu-id="832c8-150">Scope</span></span>

|<span data-ttu-id="832c8-151">**値**</span><span class="sxs-lookup"><span data-stu-id="832c8-151">**Value**</span></span>|<span data-ttu-id="832c8-152">**説明**</span><span class="sxs-lookup"><span data-stu-id="832c8-152">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="832c8-153">なし</span><span class="sxs-lookup"><span data-stu-id="832c8-153">None</span></span>  <br/> |<span data-ttu-id="832c8-154">アプリケーションにスコープが含まれていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="832c8-154">Indicates that the app has no scope.</span></span>  <br/> |
|<span data-ttu-id="832c8-155">ユーザー</span><span class="sxs-lookup"><span data-stu-id="832c8-155">User</span></span>  <br/> |<span data-ttu-id="832c8-156">ユーザーごとのアプリケーションであることを示します。</span><span class="sxs-lookup"><span data-stu-id="832c8-156">Indicates that the app is per user.</span></span>  <br/> |
|<span data-ttu-id="832c8-157">組織</span><span class="sxs-lookup"><span data-stu-id="832c8-157">Organization</span></span>  <br/> |<span data-ttu-id="832c8-158">アプリケーションが組織であることを示します。</span><span class="sxs-lookup"><span data-stu-id="832c8-158">Indicates that the app is for an organization.</span></span>  <br/> |
|<span data-ttu-id="832c8-159">Default</span><span class="sxs-lookup"><span data-stu-id="832c8-159">Default</span></span>  <br/> |<span data-ttu-id="832c8-160">アプリケーションが既定のアプリケーションであることを示します。</span><span class="sxs-lookup"><span data-stu-id="832c8-160">Indicates that the app is a default app.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="832c8-161">子要素</span><span class="sxs-lookup"><span data-stu-id="832c8-161">Child elements</span></span>

|<span data-ttu-id="832c8-162">**要素**</span><span class="sxs-lookup"><span data-stu-id="832c8-162">**Element**</span></span>|<span data-ttu-id="832c8-163">**説明**</span><span class="sxs-lookup"><span data-stu-id="832c8-163">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="832c8-164">SpecificUsers</span><span class="sxs-lookup"><span data-stu-id="832c8-164">SpecificUsers</span></span>](specificusers.md) <br/> |<span data-ttu-id="832c8-165">アプリケーションにアクセスできる電子メール アカウントを指定します。</span><span class="sxs-lookup"><span data-stu-id="832c8-165">Specifies the email accounts that can access the app.</span></span>  <br/> |
|[<span data-ttu-id="832c8-166">Manifest</span><span class="sxs-lookup"><span data-stu-id="832c8-166">Manifest</span></span>](manifest.md) <br/> |<span data-ttu-id="832c8-167">Base 64 エンコードされたアプリケーション マニフェスト ファイルが含まれています。</span><span class="sxs-lookup"><span data-stu-id="832c8-167">Contains the base-64 encoded app manifest file.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="832c8-168">親要素</span><span class="sxs-lookup"><span data-stu-id="832c8-168">Parent elements</span></span>

|<span data-ttu-id="832c8-169">**要素**</span><span class="sxs-lookup"><span data-stu-id="832c8-169">**Element**</span></span>|<span data-ttu-id="832c8-170">**説明**</span><span class="sxs-lookup"><span data-stu-id="832c8-170">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="832c8-171">ClientExtensions</span><span class="sxs-lookup"><span data-stu-id="832c8-171">ClientExtensions</span></span>](clientextensions.md) <br/> |<span data-ttu-id="832c8-172">**ClientExtension**要素の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="832c8-172">Specifies an array of **ClientExtension** elements.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="832c8-173">備考</span><span class="sxs-lookup"><span data-stu-id="832c8-173">Remarks</span></span>

<span data-ttu-id="832c8-174">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="832c8-174">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="832c8-175">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="832c8-175">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="832c8-176">要素情報</span><span class="sxs-lookup"><span data-stu-id="832c8-176">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="832c8-177">名前空間</span><span class="sxs-lookup"><span data-stu-id="832c8-177">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="832c8-178">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="832c8-178">Schema Name</span></span>  <br/> |<span data-ttu-id="832c8-179">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="832c8-179">Type schema</span></span>  <br/> |
|<span data-ttu-id="832c8-180">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="832c8-180">Validation File</span></span>  <br/> |<span data-ttu-id="832c8-181">types.xsd</span><span class="sxs-lookup"><span data-stu-id="832c8-181">types.xsd</span></span>  <br/> |
|<span data-ttu-id="832c8-182">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="832c8-182">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="832c8-183">関連項目</span><span class="sxs-lookup"><span data-stu-id="832c8-183">See also</span></span>



- [<span data-ttu-id="832c8-184">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="832c8-184">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

