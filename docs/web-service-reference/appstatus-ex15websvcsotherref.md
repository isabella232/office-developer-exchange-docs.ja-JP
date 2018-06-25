---
title: AppStatus
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f3ab8bf1-abc5-45cf-a2e1-d7602f2c24ec
description: AppStatus 要素の値は、メール アプリケーションのステータスを示します。
ms.openlocfilehash: cf213fc3d7be02c411e9c2e83a4ff153dbefe098
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759427"
---
# <a name="appstatus"></a><span data-ttu-id="b37fb-103">AppStatus</span><span class="sxs-lookup"><span data-stu-id="b37fb-103">AppStatus</span></span>

<span data-ttu-id="b37fb-104">**AppStatus**要素の値は、メール アプリケーションのステータスを示します。</span><span class="sxs-lookup"><span data-stu-id="b37fb-104">The **AppStatus** element value indicates the status of the mail app.</span></span> 
  
```XML
<AppStatus/>
```

 <span data-ttu-id="b37fb-105">**string**</span><span class="sxs-lookup"><span data-stu-id="b37fb-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b37fb-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="b37fb-106">Attributes and elements</span></span>

<span data-ttu-id="b37fb-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b37fb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b37fb-108">属性</span><span class="sxs-lookup"><span data-stu-id="b37fb-108">Attributes</span></span>

<span data-ttu-id="b37fb-109">なし。</span><span class="sxs-lookup"><span data-stu-id="b37fb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b37fb-110">子要素</span><span class="sxs-lookup"><span data-stu-id="b37fb-110">Child elements</span></span>

<span data-ttu-id="b37fb-111">なし。</span><span class="sxs-lookup"><span data-stu-id="b37fb-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b37fb-112">親要素</span><span class="sxs-lookup"><span data-stu-id="b37fb-112">Parent elements</span></span>

[<span data-ttu-id="b37fb-113">メタデータ</span><span class="sxs-lookup"><span data-stu-id="b37fb-113">Metadata</span></span>](metadata-ex15websvcsotherref.md)
  
## <a name="text-value"></a><span data-ttu-id="b37fb-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="b37fb-114">Text value</span></span>

<span data-ttu-id="b37fb-115">**AppStatus**要素のテキスト値は、メール アプリケーションのステータスを示します。</span><span class="sxs-lookup"><span data-stu-id="b37fb-115">The text value of the **AppStatus** element indicates the status of the mail app.</span></span> <span data-ttu-id="b37fb-116">ユーザーは、メール アプリケーションの状態に関連する問題を修正することができます、 [ActionUrl](actionurl.md)要素は、この修正プログラムを実行する URL を提供します。</span><span class="sxs-lookup"><span data-stu-id="b37fb-116">If the user can fix an issue related to the status of the mail app, the [ActionUrl](actionurl.md) element provides the URL to perform the fix.</span></span> 
  
<span data-ttu-id="b37fb-117">**表 1 です。AppStatus 値**</span><span class="sxs-lookup"><span data-stu-id="b37fb-117">**Table 1. AppStatus values**</span></span>

|<span data-ttu-id="b37fb-118">**値**</span><span class="sxs-lookup"><span data-stu-id="b37fb-118">**Value**</span></span>|<span data-ttu-id="b37fb-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="b37fb-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b37fb-120">Null または 0</span><span class="sxs-lookup"><span data-stu-id="b37fb-120">Null or 0</span></span>  <br/> |<span data-ttu-id="b37fb-121">メール アプリケーションでは、正常な状態があります。</span><span class="sxs-lookup"><span data-stu-id="b37fb-121">The mail app has a healthy status.</span></span>  <br/> |
|<span data-ttu-id="b37fb-122">1.0</span><span class="sxs-lookup"><span data-stu-id="b37fb-122">1.0</span></span>  <br/> |<span data-ttu-id="b37fb-123">メール アプリケーションが自動的に更新できませんでした。</span><span class="sxs-lookup"><span data-stu-id="b37fb-123">The mail app could not be automatically updated.</span></span> <span data-ttu-id="b37fb-124">メール アプリケーションでは、Office ストアから再インストールする必要があります。</span><span class="sxs-lookup"><span data-stu-id="b37fb-124">The mail app needs to be re-installed from the Office Store.</span></span>  <br/> |
|<span data-ttu-id="b37fb-125">1.1</span><span class="sxs-lookup"><span data-stu-id="b37fb-125">1.1</span></span>  <br/> |<span data-ttu-id="b37fb-126">メール アプリケーションが自動的に更新できませんでした。</span><span class="sxs-lookup"><span data-stu-id="b37fb-126">The mail app could not be automatically updated.</span></span> <span data-ttu-id="b37fb-127">メール アプリケーションは、拡張されたアクセス許可を必要とし、確認とインストールを確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b37fb-127">The mail app requires increased permissions, and this requires your review and confirmation to install.</span></span>  <br/> |
|<span data-ttu-id="b37fb-128">1.2</span><span class="sxs-lookup"><span data-stu-id="b37fb-128">1.2</span></span>  <br/> |<span data-ttu-id="b37fb-129">メール アプリケーションを自動的に更新することができませんでした。</span><span class="sxs-lookup"><span data-stu-id="b37fb-129">The mail app couldn't be updated automatically.</span></span> <span data-ttu-id="b37fb-130">現在のライセンスは期限が切れているか、無効です。</span><span class="sxs-lookup"><span data-stu-id="b37fb-130">The current license has expired or is invalid.</span></span> <span data-ttu-id="b37fb-131">Office ストアからのメール アプリケーションを更新してください。</span><span class="sxs-lookup"><span data-stu-id="b37fb-131">Please update the mail app from the Office Store.</span></span>  <br/> |
|<span data-ttu-id="b37fb-132">2.0</span><span class="sxs-lookup"><span data-stu-id="b37fb-132">2.0</span></span>  <br/> |<span data-ttu-id="b37fb-133">メール アプリケーションのライセンスを自動的に更新できませんでした。</span><span class="sxs-lookup"><span data-stu-id="b37fb-133">The mail app license could not be automatically updated.</span></span> <span data-ttu-id="b37fb-134">メール アプリケーションのライセンスは、Office ストアから回復する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b37fb-134">The license for the mail app needs to be recovered from the Office Store.</span></span>  <br/> |
|<span data-ttu-id="b37fb-135">2.1</span><span class="sxs-lookup"><span data-stu-id="b37fb-135">2.1</span></span>  <br/> |<span data-ttu-id="b37fb-136">メール アプリケーションのライセンスを自動的に更新できませんでした。</span><span class="sxs-lookup"><span data-stu-id="b37fb-136">The mail app license could not be automatically updated.</span></span> <span data-ttu-id="b37fb-137">現在のライセンスの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="b37fb-137">The current license has expired.</span></span> <span data-ttu-id="b37fb-138">このアプリケーション用の新しいライセンスは、Office ストアからインストールする必要があります。</span><span class="sxs-lookup"><span data-stu-id="b37fb-138">A new license for this app needs to be installed from the Office Store.</span></span>  <br/> |
|<span data-ttu-id="b37fb-139">3.0</span><span class="sxs-lookup"><span data-stu-id="b37fb-139">3.0</span></span>  <br/> |<span data-ttu-id="b37fb-140">メール アプリケーションの Office のストアの状態が変更されました。</span><span class="sxs-lookup"><span data-stu-id="b37fb-140">The Office Store status for the mail app has changed.</span></span> <span data-ttu-id="b37fb-141">メール アプリケーションに関連した問題がある可能性があります。</span><span class="sxs-lookup"><span data-stu-id="b37fb-141">This may indicate that there is a problem with the mail app.</span></span> <span data-ttu-id="b37fb-142">詳細については Office ストアにメール アプリケーションのページに移動します。</span><span class="sxs-lookup"><span data-stu-id="b37fb-142">Go to the mail app page in the Office Store for more information.</span></span>  <br/> |
|<span data-ttu-id="b37fb-143">3.1</span><span class="sxs-lookup"><span data-stu-id="b37fb-143">3.1</span></span>  <br/> |<span data-ttu-id="b37fb-144">メール アプリが Office ストアから削除されました。</span><span class="sxs-lookup"><span data-stu-id="b37fb-144">The mail app has been removed from the Office Store.</span></span>  <br/> |
|<span data-ttu-id="b37fb-145">3.2</span><span class="sxs-lookup"><span data-stu-id="b37fb-145">3.2</span></span>  <br/> |<span data-ttu-id="b37fb-146">メール アプリケーションで問題が検出され、が一時的に Office ストアから引き出されています。</span><span class="sxs-lookup"><span data-stu-id="b37fb-146">A problem has been discovered with the mail app and it has temporarily been withdrawn from the Office Store.</span></span>  <br/> |
|<span data-ttu-id="b37fb-147">3.3</span><span class="sxs-lookup"><span data-stu-id="b37fb-147">3.3</span></span>  <br/> |<span data-ttu-id="b37fb-148">30 日以内、メール アプリを Office ストアから削除されます。</span><span class="sxs-lookup"><span data-stu-id="b37fb-148">The mail app will be removed from the Office Store within 30 days.</span></span>  <br/> |
|<span data-ttu-id="b37fb-149">4.0</span><span class="sxs-lookup"><span data-stu-id="b37fb-149">4.0</span></span>  <br/> |<span data-ttu-id="b37fb-150">メール アプリケーションは、メール クライアントによって自動的に無効にされています。</span><span class="sxs-lookup"><span data-stu-id="b37fb-150">The mail app has been automatically disabled by your mail client.</span></span>  <br/> |
|<span data-ttu-id="b37fb-151">4.1</span><span class="sxs-lookup"><span data-stu-id="b37fb-151">4.1</span></span>  <br/> |<span data-ttu-id="b37fb-152">パフォーマンス上の理由から、Outlook によってメール アプリケーションを無効にされています。</span><span class="sxs-lookup"><span data-stu-id="b37fb-152">The mail app has been disabled by Outlook for performance reasons.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b37fb-153">備考</span><span class="sxs-lookup"><span data-stu-id="b37fb-153">Remarks</span></span>

<span data-ttu-id="b37fb-154">この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="b37fb-154">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="b37fb-155">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="b37fb-155">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b37fb-156">要素情報</span><span class="sxs-lookup"><span data-stu-id="b37fb-156">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b37fb-157">名前空間</span><span class="sxs-lookup"><span data-stu-id="b37fb-157">Namespace</span></span>  <br/> | http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b37fb-158">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b37fb-158">Schema Name</span></span>  <br/> |<span data-ttu-id="b37fb-159">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="b37fb-159">Types schema</span></span>  <br/> |
|<span data-ttu-id="b37fb-160">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b37fb-160">Validation File</span></span>  <br/> |<span data-ttu-id="b37fb-161">該当しない</span><span class="sxs-lookup"><span data-stu-id="b37fb-161">Not applicable</span></span>  <br/> |
|<span data-ttu-id="b37fb-162">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="b37fb-162">Can be Empty</span></span>  <br/> |<span data-ttu-id="b37fb-163">False</span><span class="sxs-lookup"><span data-stu-id="b37fb-163">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b37fb-164">関連項目</span><span class="sxs-lookup"><span data-stu-id="b37fb-164">See also</span></span>

- [<span data-ttu-id="b37fb-165">メタデータ</span><span class="sxs-lookup"><span data-stu-id="b37fb-165">Metadata</span></span>](metadata-ex15websvcsotherref.md)
- [<span data-ttu-id="b37fb-166">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="b37fb-166">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

