---
title: AppStatus
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f3ab8bf1-abc5-45cf-a2e1-d7602f2c24ec
description: AppStatus 要素の値は、メールアプリの状態を示します。
ms.openlocfilehash: d833947fd62d500418f257829d241a2e0b3bca9c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464778"
---
# <a name="appstatus"></a><span data-ttu-id="0f1d4-103">AppStatus</span><span class="sxs-lookup"><span data-stu-id="0f1d4-103">AppStatus</span></span>

<span data-ttu-id="0f1d4-104">**Appstatus**要素の値は、メールアプリの状態を示します。</span><span class="sxs-lookup"><span data-stu-id="0f1d4-104">The **AppStatus** element value indicates the status of the mail app.</span></span> 
  
```XML
<AppStatus/>
```

 <span data-ttu-id="0f1d4-105">**string**</span><span class="sxs-lookup"><span data-stu-id="0f1d4-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0f1d4-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="0f1d4-106">Attributes and elements</span></span>

<span data-ttu-id="0f1d4-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0f1d4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0f1d4-108">属性</span><span class="sxs-lookup"><span data-stu-id="0f1d4-108">Attributes</span></span>

<span data-ttu-id="0f1d4-109">なし。</span><span class="sxs-lookup"><span data-stu-id="0f1d4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0f1d4-110">子要素</span><span class="sxs-lookup"><span data-stu-id="0f1d4-110">Child elements</span></span>

<span data-ttu-id="0f1d4-111">なし。</span><span class="sxs-lookup"><span data-stu-id="0f1d4-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0f1d4-112">親要素</span><span class="sxs-lookup"><span data-stu-id="0f1d4-112">Parent elements</span></span>

[<span data-ttu-id="0f1d4-113">メタデータ</span><span class="sxs-lookup"><span data-stu-id="0f1d4-113">Metadata</span></span>](metadata-ex15websvcsotherref.md)
  
## <a name="text-value"></a><span data-ttu-id="0f1d4-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="0f1d4-114">Text value</span></span>

<span data-ttu-id="0f1d4-115">**Appstatus**要素のテキスト値は、メールアプリの状態を示します。</span><span class="sxs-lookup"><span data-stu-id="0f1d4-115">The text value of the **AppStatus** element indicates the status of the mail app.</span></span> <span data-ttu-id="0f1d4-116">ユーザーがメールアプリの状態に関連する問題を修正できる場合、 [actionurl](actionurl.md)要素は修正を実行するための url を提供します。</span><span class="sxs-lookup"><span data-stu-id="0f1d4-116">If the user can fix an issue related to the status of the mail app, the [ActionUrl](actionurl.md) element provides the URL to perform the fix.</span></span> 
  
<span data-ttu-id="0f1d4-117">**表1AppStatus の値**</span><span class="sxs-lookup"><span data-stu-id="0f1d4-117">**Table 1. AppStatus values**</span></span>

|<span data-ttu-id="0f1d4-118">**値**</span><span class="sxs-lookup"><span data-stu-id="0f1d4-118">**Value**</span></span>|<span data-ttu-id="0f1d4-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="0f1d4-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0f1d4-120">Null または0</span><span class="sxs-lookup"><span data-stu-id="0f1d4-120">Null or 0</span></span>  <br/> |<span data-ttu-id="0f1d4-121">メールアプリの状態は正常です。</span><span class="sxs-lookup"><span data-stu-id="0f1d4-121">The mail app has a healthy status.</span></span>  <br/> |
|<span data-ttu-id="0f1d4-122">1.0</span><span class="sxs-lookup"><span data-stu-id="0f1d4-122">1.0</span></span>  <br/> |<span data-ttu-id="0f1d4-123">メールアプリを自動的に更新できませんでした。</span><span class="sxs-lookup"><span data-stu-id="0f1d4-123">The mail app could not be automatically updated.</span></span> <span data-ttu-id="0f1d4-124">メールアプリを Office ストアから再インストールする必要があります。</span><span class="sxs-lookup"><span data-stu-id="0f1d4-124">The mail app needs to be re-installed from the Office Store.</span></span>  <br/> |
|<span data-ttu-id="0f1d4-125">1.1</span><span class="sxs-lookup"><span data-stu-id="0f1d4-125">1.1</span></span>  <br/> |<span data-ttu-id="0f1d4-126">メールアプリを自動的に更新できませんでした。</span><span class="sxs-lookup"><span data-stu-id="0f1d4-126">The mail app could not be automatically updated.</span></span> <span data-ttu-id="0f1d4-127">メールアプリには、強化されたアクセス許可が必要です。そのためには、確認とインストールの確認が必要です。</span><span class="sxs-lookup"><span data-stu-id="0f1d4-127">The mail app requires increased permissions, and this requires your review and confirmation to install.</span></span>  <br/> |
|<span data-ttu-id="0f1d4-128">1.2</span><span class="sxs-lookup"><span data-stu-id="0f1d4-128">1.2</span></span>  <br/> |<span data-ttu-id="0f1d4-129">メールアプリを自動的に更新できませんでした。</span><span class="sxs-lookup"><span data-stu-id="0f1d4-129">The mail app couldn't be updated automatically.</span></span> <span data-ttu-id="0f1d4-130">現在のライセンスの有効期限が切れているか、無効です。</span><span class="sxs-lookup"><span data-stu-id="0f1d4-130">The current license has expired or is invalid.</span></span> <span data-ttu-id="0f1d4-131">Office ストアからメールアプリを更新してください。</span><span class="sxs-lookup"><span data-stu-id="0f1d4-131">Please update the mail app from the Office Store.</span></span>  <br/> |
|<span data-ttu-id="0f1d4-132">2.0</span><span class="sxs-lookup"><span data-stu-id="0f1d4-132">2.0</span></span>  <br/> |<span data-ttu-id="0f1d4-133">メールアプリのライセンスを自動的に更新できませんでした。</span><span class="sxs-lookup"><span data-stu-id="0f1d4-133">The mail app license could not be automatically updated.</span></span> <span data-ttu-id="0f1d4-134">メールアプリのライセンスは、Office ストアから回復する必要があります。</span><span class="sxs-lookup"><span data-stu-id="0f1d4-134">The license for the mail app needs to be recovered from the Office Store.</span></span>  <br/> |
|<span data-ttu-id="0f1d4-135">2.1</span><span class="sxs-lookup"><span data-stu-id="0f1d4-135">2.1</span></span>  <br/> |<span data-ttu-id="0f1d4-136">メールアプリのライセンスを自動的に更新できませんでした。</span><span class="sxs-lookup"><span data-stu-id="0f1d4-136">The mail app license could not be automatically updated.</span></span> <span data-ttu-id="0f1d4-137">現在のライセンスの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="0f1d4-137">The current license has expired.</span></span> <span data-ttu-id="0f1d4-138">このアプリの新しいライセンスを Office ストアからインストールする必要があります。</span><span class="sxs-lookup"><span data-stu-id="0f1d4-138">A new license for this app needs to be installed from the Office Store.</span></span>  <br/> |
|<span data-ttu-id="0f1d4-139">3.0</span><span class="sxs-lookup"><span data-stu-id="0f1d4-139">3.0</span></span>  <br/> |<span data-ttu-id="0f1d4-140">メールアプリの Office ストアの状態が変更されました。</span><span class="sxs-lookup"><span data-stu-id="0f1d4-140">The Office Store status for the mail app has changed.</span></span> <span data-ttu-id="0f1d4-141">これは、メールアプリに問題があることを示している可能性があります。</span><span class="sxs-lookup"><span data-stu-id="0f1d4-141">This may indicate that there is a problem with the mail app.</span></span> <span data-ttu-id="0f1d4-142">詳細については、「Office ストアのメールアプリ」ページにアクセスしてください。</span><span class="sxs-lookup"><span data-stu-id="0f1d4-142">Go to the mail app page in the Office Store for more information.</span></span>  <br/> |
|<span data-ttu-id="0f1d4-143">3.1</span><span class="sxs-lookup"><span data-stu-id="0f1d4-143">3.1</span></span>  <br/> |<span data-ttu-id="0f1d4-144">メールアプリが Office ストアから削除されました。</span><span class="sxs-lookup"><span data-stu-id="0f1d4-144">The mail app has been removed from the Office Store.</span></span>  <br/> |
|<span data-ttu-id="0f1d4-145">3.2</span><span class="sxs-lookup"><span data-stu-id="0f1d4-145">3.2</span></span>  <br/> |<span data-ttu-id="0f1d4-146">メールアプリで問題が検出され、一時的に Office ストアから引き出されています。</span><span class="sxs-lookup"><span data-stu-id="0f1d4-146">A problem has been discovered with the mail app and it has temporarily been withdrawn from the Office Store.</span></span>  <br/> |
|<span data-ttu-id="0f1d4-147">3.3</span><span class="sxs-lookup"><span data-stu-id="0f1d4-147">3.3</span></span>  <br/> |<span data-ttu-id="0f1d4-148">メールアプリは、30日以内に Office ストアから削除されます。</span><span class="sxs-lookup"><span data-stu-id="0f1d4-148">The mail app will be removed from the Office Store within 30 days.</span></span>  <br/> |
|<span data-ttu-id="0f1d4-149">4.0</span><span class="sxs-lookup"><span data-stu-id="0f1d4-149">4.0</span></span>  <br/> |<span data-ttu-id="0f1d4-150">メールアプリは、メールクライアントによって自動的に無効にされています。</span><span class="sxs-lookup"><span data-stu-id="0f1d4-150">The mail app has been automatically disabled by your mail client.</span></span>  <br/> |
|<span data-ttu-id="0f1d4-151">4.1</span><span class="sxs-lookup"><span data-stu-id="0f1d4-151">4.1</span></span>  <br/> |<span data-ttu-id="0f1d4-152">パフォーマンス上の理由から、メールアプリは Outlook によって無効にされています。</span><span class="sxs-lookup"><span data-stu-id="0f1d4-152">The mail app has been disabled by Outlook for performance reasons.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0f1d4-153">注釈</span><span class="sxs-lookup"><span data-stu-id="0f1d4-153">Remarks</span></span>

<span data-ttu-id="0f1d4-154">この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="0f1d4-154">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="0f1d4-155">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="0f1d4-155">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0f1d4-156">要素の情報</span><span class="sxs-lookup"><span data-stu-id="0f1d4-156">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0f1d4-157">Namespace</span><span class="sxs-lookup"><span data-stu-id="0f1d4-157">Namespace</span></span>  <br/> | https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0f1d4-158">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0f1d4-158">Schema Name</span></span>  <br/> |<span data-ttu-id="0f1d4-159">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="0f1d4-159">Types schema</span></span>  <br/> |
|<span data-ttu-id="0f1d4-160">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0f1d4-160">Validation File</span></span>  <br/> |<span data-ttu-id="0f1d4-161">該当なし</span><span class="sxs-lookup"><span data-stu-id="0f1d4-161">Not applicable</span></span>  <br/> |
|<span data-ttu-id="0f1d4-162">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="0f1d4-162">Can be Empty</span></span>  <br/> |<span data-ttu-id="0f1d4-163">正しくない</span><span class="sxs-lookup"><span data-stu-id="0f1d4-163">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0f1d4-164">関連項目</span><span class="sxs-lookup"><span data-stu-id="0f1d4-164">See also</span></span>

- [<span data-ttu-id="0f1d4-165">メタデータ</span><span class="sxs-lookup"><span data-stu-id="0f1d4-165">Metadata</span></span>](metadata-ex15websvcsotherref.md)
- [<span data-ttu-id="0f1d4-166">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="0f1d4-166">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

