---
title: 自動検出のエラー メッセージの処理
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: e5939ec2-1100-4174-8a88-5a6e09b60b23
description: 自動検出の各種エラーと、そのエラーの対処法について説明します。
ms.openlocfilehash: fcafc799f4d35e92159d2913845474ecf7bc5657
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19758898"
---
# <a name="handling-autodiscover-error-messages"></a><span data-ttu-id="000e3-103">自動検出のエラー メッセージの処理</span><span class="sxs-lookup"><span data-stu-id="000e3-103">Handling Autodiscover error messages</span></span>

<span data-ttu-id="000e3-104">自動検出の各種エラーと、そのエラーの対処法について説明します。</span><span class="sxs-lookup"><span data-stu-id="000e3-104">Learn about the different types of Autodiscover errors and what to do with them.</span></span>
  
<span data-ttu-id="000e3-p101">自動検出により、カスタムのアプリケーションは構成情報を自動的に取得できるようになり、最適に動作するようになります。ただし、物事は計画どおりに進まないこともあります。発生することがある一般的なエラーについて説明して、ユーザーに要求するクライアントの手動構成を最小限にするためのエラー処理の方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="000e3-p101">Autodiscover enables your applications to retrieve configuration information automatically, and it works great. However, things don't always go according to plan. Let's look at the common errors that might occur and how you can handle them to minimize the need to prompt your user to manually configure your client.</span></span>
  
## <a name="http-status-errors"></a><span data-ttu-id="000e3-108">HTTP 状態のエラー</span><span class="sxs-lookup"><span data-stu-id="000e3-108">HTTP status errors</span></span>
<span data-ttu-id="000e3-109"><a name="bk_HttpErrors"> </a></span><span class="sxs-lookup"><span data-stu-id="000e3-109"></span></span>

<span data-ttu-id="000e3-p102">最初の種類のエラーは、自動検出の要求を送信するときに発生することがある HTTP 状態です。応答に含まれる HTTP 状態が 200 (OK) 以外の場合、求めている自動検出の応答は応答のペイロードに含まれていません。わかりやすくするために、200 以外の状態コードを 3 つのカテゴリに分類します。</span><span class="sxs-lookup"><span data-stu-id="000e3-p102">The first type of error you might encounter when sending Autodiscover requests is the HTTP status. If the HTTP status in your response is anything other than 200 (OK), the response payload doesn't contain the Autodiscover response you were looking for. For simplicity, we can group non-200 status codes into three categories.</span></span>
  
<span data-ttu-id="000e3-113">**表 1 です。HTTP ステータス ・ コード**</span><span class="sxs-lookup"><span data-stu-id="000e3-113">**Table 1. HTTP status codes**</span></span>

|<span data-ttu-id="000e3-114">**ステータス コード**</span><span class="sxs-lookup"><span data-stu-id="000e3-114">**Status code**</span></span>|<span data-ttu-id="000e3-115">**エラーの種類**</span><span class="sxs-lookup"><span data-stu-id="000e3-115">**Type of error**</span></span>|<span data-ttu-id="000e3-116">**処理しています.**</span><span class="sxs-lookup"><span data-stu-id="000e3-116">**To handle…**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="000e3-117">301 または 302</span><span class="sxs-lookup"><span data-stu-id="000e3-117">301 or 302</span></span>  <br/> |<span data-ttu-id="000e3-118">リダイレクト エラー</span><span class="sxs-lookup"><span data-stu-id="000e3-118">Redirect error</span></span>  <br/> |<span data-ttu-id="000e3-119">「場所」HTTP 応答ヘッダーに含まれている URI への要求を再送信します。</span><span class="sxs-lookup"><span data-stu-id="000e3-119">Resend your request to the URI contained in the "Location" HTTP response header.</span></span> <span data-ttu-id="000e3-120">詳細については、[処理エラーをリダイレクトする](#bk_HandlingRedirects)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="000e3-120">For details, see [Handling redirect errors](#bk_HandlingRedirects).</span></span>  <br/> |
|<span data-ttu-id="000e3-121">401</span><span class="sxs-lookup"><span data-stu-id="000e3-121">401</span></span>  <br/> |<span data-ttu-id="000e3-122">未認証エラー</span><span class="sxs-lookup"><span data-stu-id="000e3-122">Unauthorized error</span></span>  <br/> |<span data-ttu-id="000e3-123">[自動検出プロセス](autodiscover-for-exchange.md)では、複数の潜在的な Url をしようとして、これを次のいずれかの資格情報をそのまま使用するだけの 1 つの URL の取得でした。</span><span class="sxs-lookup"><span data-stu-id="000e3-123">Because the [Autodiscover process](autodiscover-for-exchange.md) involves trying multiple potential URLs, you could get this on one URL only to have the next one accept your credentials.</span></span> <span data-ttu-id="000e3-124">このため、資格情報が有効ではないことを示すために 401 エラーが 1 つを考慮するべきではありません。</span><span class="sxs-lookup"><span data-stu-id="000e3-124">For this reason, you shouldn't consider a single 401 error to indicate that the credentials are invalid.</span></span> <span data-ttu-id="000e3-125">ただし、複数の Url から 401 エラーが発生した場合は (可能な場合)、パスワードを再入力するユーザーに確認します。</span><span class="sxs-lookup"><span data-stu-id="000e3-125">However, if you receive 401 errors from multiple URLs, you might want to prompt the user to reenter their password (if possible).</span></span>  <br/> |
|<span data-ttu-id="000e3-126">その他の 200 以外の状態</span><span class="sxs-lookup"><span data-stu-id="000e3-126">Any other non-200 status</span></span>  <br/> |<span data-ttu-id="000e3-127">無効な自動検出エンドポイントのエラー</span><span class="sxs-lookup"><span data-stu-id="000e3-127">Invalid Autodiscover endpoint error</span></span>  <br/> |<span data-ttu-id="000e3-128">200 以外の状態コードを返す URL は無効であると見なして、一覧内で次に当たる URL の試行を続行します。</span><span class="sxs-lookup"><span data-stu-id="000e3-128">Consider the URL that returns any other non-200 status code to be invalid, and continue trying the next URL in your list.</span></span>  <br/> |
   
## <a name="autodiscover-errors"></a><span data-ttu-id="000e3-129">自動検出のエラー</span><span class="sxs-lookup"><span data-stu-id="000e3-129">Autodiscover errors</span></span>
<span data-ttu-id="000e3-130"><a name="bk_AutodiscoverErrors"> </a></span><span class="sxs-lookup"><span data-stu-id="000e3-130"></span></span>

<span data-ttu-id="000e3-p105">自動検出要求の送信後に 200 (OK) の状態コードを得たとしても、必要としている情報がサーバーから送られたという意味にはなりません。200 の状態は自動検出の応答があったということだけを意味し、その応答のペイロードにはエラーが含まれていることもあります。SOAP 形式と POX 形式では、エラー情報の場所が異なります。</span><span class="sxs-lookup"><span data-stu-id="000e3-p105">Even if you get a 200 (OK) status code after sending an Autodiscover request, that doesn't mean that the server sent the information you need. The 200 status only means that you have an Autodiscover response, and that response might contain an error within the payload. The location of the error information differs depending on whether the format is SOAP or POX.</span></span>
  
### <a name="soap-autodiscover-errors"></a><span data-ttu-id="000e3-134">SOAP 自動検出のエラー</span><span class="sxs-lookup"><span data-stu-id="000e3-134">SOAP Autodiscover errors</span></span>

<span data-ttu-id="000e3-135">SOAP の自動検出の応答は、別の場所で、1 つまたは複数の[エラー コード (SOAP)](http://msdn.microsoft.com/library/5e5ec861-0191-4ecb-a906-47ce8ed96381%28Office.15%29.aspx)要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="000e3-135">For SOAP Autodiscover, the response can contain one or more [ErrorCode (SOAP)](http://msdn.microsoft.com/library/5e5ec861-0191-4ecb-a906-47ce8ed96381%28Office.15%29.aspx) elements, in different places.</span></span> <span data-ttu-id="000e3-136">通常の応答では、[応答 (SOAP)](http://msdn.microsoft.com/library/4c2bcdeb-95ce-4ffa-bd83-118af53b534f%28Office.15%29.aspx)の要素の子要素として 1 つは、 [UserResponse (SOAP)](http://msdn.microsoft.com/library/5007b1ba-bfcc-40d7-b1cb-e32fbaf54ffd%28Office.15%29.aspx)の各要素の子として 1 つを期待できます。</span><span class="sxs-lookup"><span data-stu-id="000e3-136">Typically you can expect one as a child element of the [Response (SOAP)](http://msdn.microsoft.com/library/4c2bcdeb-95ce-4ffa-bd83-118af53b534f%28Office.15%29.aspx) element, and one as a child of each [UserResponse (SOAP)](http://msdn.microsoft.com/library/5007b1ba-bfcc-40d7-b1cb-e32fbaf54ffd%28Office.15%29.aspx) element in the response.</span></span> <span data-ttu-id="000e3-137">発生する可能性も、 [UserSettingError (SOAP)](http://msdn.microsoft.com/library/abb175c5-4f38-4dcc-81e3-b511686862eb%28Office.15%29.aspx)要素の子として 1 つが存在する場合。</span><span class="sxs-lookup"><span data-stu-id="000e3-137">You might also encounter one as a child of a [UserSettingError (SOAP)](http://msdn.microsoft.com/library/abb175c5-4f38-4dcc-81e3-b511686862eb%28Office.15%29.aspx) element, if one is present.</span></span> <span data-ttu-id="000e3-138">エラーのコンテキストは、**エラー コード**要素が存在、次のようにによって異なります。</span><span class="sxs-lookup"><span data-stu-id="000e3-138">The context of the error depends on where the **ErrorCode** element is located, as follows:</span></span> 
  
- <span data-ttu-id="000e3-139">**応答**要素の子要素とは、**エラー コード**要素は、要求全体に適用されるエラーを表します。</span><span class="sxs-lookup"><span data-stu-id="000e3-139">As a child element of the **Response** element, the **ErrorCode** element represents an error that applies to the entire request.</span></span> 
    
- <span data-ttu-id="000e3-140">**UserResponse**要素の子として、その特定のユーザーにだけ適用されるエラーを表します。</span><span class="sxs-lookup"><span data-stu-id="000e3-140">As a child of the **UserResponse** element, it represents an error that applies just to that specific user.</span></span> 
    
- <span data-ttu-id="000e3-141">**UserSettingError**要素の子として、要求された特定の設定に適用されるエラーを表します。</span><span class="sxs-lookup"><span data-stu-id="000e3-141">As a child of a **UserSettingError** element, it represents an error that applies to a specific setting that was requested.</span></span> 
    
<span data-ttu-id="000e3-142">応答の例を見てみましょう。</span><span class="sxs-lookup"><span data-stu-id="000e3-142">Let's take a look at an example of a response.</span></span> <span data-ttu-id="000e3-143">**応答**要素の下で**エラー コード**要素では、この例では、"NoError"は、全体的な成功を示す値があります。</span><span class="sxs-lookup"><span data-stu-id="000e3-143">In this example, the **ErrorCode** element under the **Response** element has a value of "NoError", which indicates overall success.</span></span> <span data-ttu-id="000e3-144">ただし、 **UserResponse**要素の下で**エラー コード**要素には、"RedirectAddress"は、その特定のユーザーのエラーが発生したことを示す値があります。</span><span class="sxs-lookup"><span data-stu-id="000e3-144">However, the **ErrorCode** element under the **UserResponse** element has a value of "RedirectAddress", which indicates that an error occurred for that particular user.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/" 
    xmlns:a="http://www.w3.org/2005/08/addressing">
  <s:Header>
    <a:Action s:mustUnderstand="1">http://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetUserSettingsResponse</a:Action>
    <h:ServerVersionInfo xmlns:h="http://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
      <h:MajorVersion>14</h:MajorVersion>
      <h:MinorVersion>3</h:MinorVersion>
      <h:MajorBuildNumber>136</h:MajorBuildNumber>
      <h:MinorBuildNumber>1</h:MinorBuildNumber>
      <h:Version>Exchange2010_SP2</h:Version>
    </h:ServerVersionInfo>
  </s:Header>
  <s:Body>
    <GetUserSettingsResponseMessage xmlns="http://schemas.microsoft.com/exchange/2010/Autodiscover">
      <Response xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
        <ErrorCode>NoError</ErrorCode>
        <ErrorMessage />
        <UserResponses>
          <UserResponse>
            <ErrorCode>RedirectAddress</ErrorCode>
            <ErrorMessage>Redirection address.</ErrorMessage>
            <RedirectTarget>elvin@mail.contoso.com</RedirectTarget>
            <UserSettingErrors />
            <UserSettings />
          </UserResponse>
        </UserResponses>
      </Response>
    </GetUserSettingsResponseMessage>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="000e3-145">[エラー コード (SOAP)](http://msdn.microsoft.com/library/5e5ec861-0191-4ecb-a906-47ce8ed96381%28Office.15%29.aspx)の資料には、可能性のあるエラーの完全なリストが含まれています。</span><span class="sxs-lookup"><span data-stu-id="000e3-145">The [ErrorCode (SOAP)](http://msdn.microsoft.com/library/5e5ec861-0191-4ecb-a906-47ce8ed96381%28Office.15%29.aspx) article contains a full list of possible errors.</span></span> <span data-ttu-id="000e3-146">これらのほとんどは、回復不能なエラーを示すが、いくつかは、特別な処理を保証するものです。</span><span class="sxs-lookup"><span data-stu-id="000e3-146">Most of these indicate an unrecoverable error, but a few warrant special handling.</span></span> 
  
<span data-ttu-id="000e3-147">**表 2 になります。SOAP Autodisover のエラー コードの値**</span><span class="sxs-lookup"><span data-stu-id="000e3-147">**Table 2. SOAP Autodisover ErrorCode values**</span></span>

|<span data-ttu-id="000e3-148">**エラー コードの値**</span><span class="sxs-lookup"><span data-stu-id="000e3-148">**ErrorCode value**</span></span>|<span data-ttu-id="000e3-149">**処理しています.**</span><span class="sxs-lookup"><span data-stu-id="000e3-149">**To handle…**</span></span>|
|:-----|:-----|
|<span data-ttu-id="000e3-150">RedirectAddress</span><span class="sxs-lookup"><span data-stu-id="000e3-150">RedirectAddress</span></span>  <br/> |<span data-ttu-id="000e3-151">[RedirectTarget (SOAP)](http://msdn.microsoft.com/library/f8162724-cf9a-4543-a1ad-5846c8b10bfa%28Office.15%29.aspx)の要素で電子メール アドレスを持つ[新しい電子メール アドレスを使用して自動検出を再起動すること](#bk_RestartAutodiscover)にします。</span><span class="sxs-lookup"><span data-stu-id="000e3-151">[Restarting Autodiscover with a new email address](#bk_RestartAutodiscover) with the email address in the [RedirectTarget (SOAP)](http://msdn.microsoft.com/library/f8162724-cf9a-4543-a1ad-5846c8b10bfa%28Office.15%29.aspx) element.</span></span>  <br/> |
|<span data-ttu-id="000e3-152">RedirectUrl</span><span class="sxs-lookup"><span data-stu-id="000e3-152">RedirectUrl</span></span>  <br/> |<span data-ttu-id="000e3-153">**RedirectTarget**要素内の URL を[新しい URL に要求を再送信](#bk_ResendRequest)をします。</span><span class="sxs-lookup"><span data-stu-id="000e3-153">[Resending your request to a new URL](#bk_ResendRequest) to the URL in the **RedirectTarget** element.</span></span>  <br/> |
|<span data-ttu-id="000e3-154">ServerBusy</span><span class="sxs-lookup"><span data-stu-id="000e3-154">ServerBusy</span></span>  <br/> |<span data-ttu-id="000e3-p109">少し間をおいて、この URL を再試行します。一定時間待機するか、この URL を単に試行する URL の一覧の最後に移動します。このエラーを 1 つの URL から複数回受け取る場合は、その URL が無効であると見なす必要があります。</span><span class="sxs-lookup"><span data-stu-id="000e3-p109">Retry this URL after a small delay. You might wait a set amount of time or simply move this URL to the end of your list of URLs to try. If you receive this error multiple times from a URL, you should consider the URL to be invalid.</span></span>  <br/> |
   
### <a name="pox-autodiscover-errors"></a><span data-ttu-id="000e3-158">POX 自動検出のエラー</span><span class="sxs-lookup"><span data-stu-id="000e3-158">POX Autodiscover errors</span></span>

<span data-ttu-id="000e3-159">POX の自動検出サービスは、少し異なる方法でエラーを報告します。</span><span class="sxs-lookup"><span data-stu-id="000e3-159">The POX Autodiscover service reports errors a little differently.</span></span> <span data-ttu-id="000e3-160">不可能なエラーは、[エラー (POX)](http://msdn.microsoft.com/library/91c63b62-ab68-4c32-a2f7-5a87c188335b%28Office.15%29.aspx)要素に含まれます。</span><span class="sxs-lookup"><span data-stu-id="000e3-160">Non-recoverable errors are contained in the [Error (POX)](http://msdn.microsoft.com/library/91c63b62-ab68-4c32-a2f7-5a87c188335b%28Office.15%29.aspx) element.</span></span> <span data-ttu-id="000e3-161">[エラー コード (POX)](http://msdn.microsoft.com/library/064d73e4-45b7-4797-828e-9df590830db8%28Office.15%29.aspx)の資料には、可能性のあるエラー コードの完全なリストが含まれています。</span><span class="sxs-lookup"><span data-stu-id="000e3-161">The [ErrorCode (POX)](http://msdn.microsoft.com/library/064d73e4-45b7-4797-828e-9df590830db8%28Office.15%29.aspx) article contains a full list of possible error codes.</span></span> 
  
<span data-ttu-id="000e3-162">[アクション (POX)](http://msdn.microsoft.com/library/a3462c6b-453c-462a-830d-f29ee4a2babb%28Office.15%29.aspx)要素には、リダイレクト エラーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="000e3-162">Redirect errors are contained in the [Action (POX)](http://msdn.microsoft.com/library/a3462c6b-453c-462a-830d-f29ee4a2babb%28Office.15%29.aspx) element.</span></span> <span data-ttu-id="000e3-163">[設定] 以外の**アクション**要素のすべての値は、リダイレクト エラーを示します。</span><span class="sxs-lookup"><span data-stu-id="000e3-163">Any value of the **Action** element other than "settings" indicates a redirect error.</span></span> 
  
<span data-ttu-id="000e3-164">**表 3。POX Autodisover のエラー コードの値**</span><span class="sxs-lookup"><span data-stu-id="000e3-164">**Table 3. POX Autodisover ErrorCode values**</span></span>

|<span data-ttu-id="000e3-165">**アクションの値**</span><span class="sxs-lookup"><span data-stu-id="000e3-165">**Action value**</span></span>|<span data-ttu-id="000e3-166">**処理しています.**</span><span class="sxs-lookup"><span data-stu-id="000e3-166">**To handle…**</span></span>|
|:-----|:-----|
|<span data-ttu-id="000e3-167">redirectAddr</span><span class="sxs-lookup"><span data-stu-id="000e3-167">redirectAddr</span></span>  <br/> |<span data-ttu-id="000e3-168">[RedirectAddr (POX)](http://msdn.microsoft.com/library/0e9fa6b6-7991-4dc1-a59a-48e5f8e041e4%28Office.15%29.aspx)要素内の電子メール アドレスと[新しい電子メール アドレスを使用して自動検出を再起動すること](#bk_RestartAutodiscover)をします。</span><span class="sxs-lookup"><span data-stu-id="000e3-168">[Restarting Autodiscover with a new email address](#bk_RestartAutodiscover) with the email address in the [RedirectAddr (POX)](http://msdn.microsoft.com/library/0e9fa6b6-7991-4dc1-a59a-48e5f8e041e4%28Office.15%29.aspx) element.</span></span>  <br/> |
|<span data-ttu-id="000e3-169">redirectUrl</span><span class="sxs-lookup"><span data-stu-id="000e3-169">redirectUrl</span></span>  <br/> |<span data-ttu-id="000e3-170">[RedirectUrl (POX)](http://msdn.microsoft.com/library/c54f310f-8c99-4c37-8e73-ac87722b6229%28Office.15%29.aspx)要素内の URL を[新しい URL に要求を再送信](#bk_ResendRequest)をします。</span><span class="sxs-lookup"><span data-stu-id="000e3-170">[Resending your request to a new URL](#bk_ResendRequest) to the URL in the [RedirectUrl (POX)](http://msdn.microsoft.com/library/c54f310f-8c99-4c37-8e73-ac87722b6229%28Office.15%29.aspx) element.</span></span>  <br/> |
   
<span data-ttu-id="000e3-171">この例では、**アクション**要素は、"redirectAddr"は、 **RedirectAddr**要素に格納されている新しい電子メール アドレスを持つ新しい要求を送信する必要があることを示しますの値を持ちます。</span><span class="sxs-lookup"><span data-stu-id="000e3-171">In this example, the **Action** element has a value of "redirectAddr", which indicates that a new request should be sent with the new email address contained in the **RedirectAddr** element.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<Autodiscover xmlns="http://schemas.microsoft.com/exchange/autodiscover/responseschema/2006">
  <Response xmlns="http://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a">
    <Account>
      <Action>redirectAddr</Action>
      <RedirectAddr>elvin@mail.contoso.com</RedirectAddr>
    </Account>
  </Response>
</Autodiscover>
```

## <a name="handling-redirect-errors"></a><span data-ttu-id="000e3-172">リダイレクト エラーの処理</span><span class="sxs-lookup"><span data-stu-id="000e3-172">Handling redirect errors</span></span>
<span data-ttu-id="000e3-173"><a name="bk_HandlingRedirects"> </a></span><span class="sxs-lookup"><span data-stu-id="000e3-173"></span></span>

<span data-ttu-id="000e3-174">リダイレクト エラーのシナリオは 2 つの方法で処理できます。</span><span class="sxs-lookup"><span data-stu-id="000e3-174">You can handle redirect error scenarios in two ways:</span></span>
  
- <span data-ttu-id="000e3-175">新しい電子メール アドレスで自動検出を再開する。</span><span class="sxs-lookup"><span data-stu-id="000e3-175">By restarting Autodiscover with a new email address.</span></span>
    
- <span data-ttu-id="000e3-176">新しい URL に要求を再送信する。</span><span class="sxs-lookup"><span data-stu-id="000e3-176">By resending your request to a new URL.</span></span>
    
<span data-ttu-id="000e3-177">どちらのシナリオも続行する前に何らかの検証が必要になります。</span><span class="sxs-lookup"><span data-stu-id="000e3-177">Both scenarios require some validation before proceeding.</span></span>
  
### <a name="restarting-autodiscover-with-a-new-email-address"></a><span data-ttu-id="000e3-178">新しい電子メール アドレスで自動検出を再開する</span><span class="sxs-lookup"><span data-stu-id="000e3-178">Restarting Autodiscover with a new email address</span></span>
<span data-ttu-id="000e3-179"><a name="bk_RestartAutodiscover"> </a></span><span class="sxs-lookup"><span data-stu-id="000e3-179"></span></span>

<span data-ttu-id="000e3-p112">自動検出のリダイレクト応答で新しい電子メール アドレスを取得したときには、リダイレクト エラー応答で提示された新しい電子メール アドレスがエラーになった要求で送信されたアドレスと同じでないことを最初に確認します。同じになる場合は、自動検出を再開してはいけません。その代わりに、応答を生成した URL を無効と見なします。</span><span class="sxs-lookup"><span data-stu-id="000e3-p112">When you get a new email address in an Autodiscover redirect response, first verify that the new email address that was provided in the redirect error response is not the same address that you sent in the request that resulted in the error. If it is, you should not restart Autodiscover and instead consider the URL that generated the response to be invalid.</span></span>
  
<span data-ttu-id="000e3-182">新しい電子メール アドレスが異なる場合は、潜在的な自動検出エンドポイント URL の既存の一覧を破棄して、新しい電子メール アドレスに基づいた新しい一覧を生成します。</span><span class="sxs-lookup"><span data-stu-id="000e3-182">If the new email address is different, discard your existing list of potential Autodiscover endpoint URLs and generate a new list based on the new email address.</span></span>
  
### <a name="resending-your-request-to-a-new-url"></a><span data-ttu-id="000e3-183">新しい URL に要求を再送信する</span><span class="sxs-lookup"><span data-stu-id="000e3-183">Resending your request to a new URL</span></span>
<span data-ttu-id="000e3-184"><a name="bk_ResendRequest"> </a></span><span class="sxs-lookup"><span data-stu-id="000e3-184"></span></span>

<span data-ttu-id="000e3-185">自動検出リダイレクト応答で新しい URL を取得したときには、まず、その URL を次のようにして検証する必要があります。</span><span class="sxs-lookup"><span data-stu-id="000e3-185">When you get a new URL in an Autodiscover redirect response, you should first validate the URL as follows:</span></span>
  
- <span data-ttu-id="000e3-186">URL が HTTPS URL であることを確認します。</span><span class="sxs-lookup"><span data-stu-id="000e3-186">Verify that the URL is an HTTPS URL.</span></span>
    
- <span data-ttu-id="000e3-187">これまでに現在の電子メール アドレスで、この URL からエラーを受け取っていないことを確認します。</span><span class="sxs-lookup"><span data-stu-id="000e3-187">Verify that you have not received an error from this URL with the current email address before.</span></span>
    
- <span data-ttu-id="000e3-188">カスタム アプリケーションに適用可能な場合は、ユーザーにリダイレクトについて知らせて、リダイレクトに従う許可を取ります。</span><span class="sxs-lookup"><span data-stu-id="000e3-188">If applicable to your application, inform the user of the redirection and get their permission to follow the redirect.</span></span>
    
- <span data-ttu-id="000e3-189">URL と[、サーバーから提示された SSL 証明書が有効であることを確認](how-to-validate-a-server-certificate-for-the-ews-managed-api.md)するには、要求を送信します。</span><span class="sxs-lookup"><span data-stu-id="000e3-189">Send a request to the URL and [verify that the SSL certificate presented by the server is valid](how-to-validate-a-server-certificate-for-the-ews-managed-api.md).</span></span>
    
<span data-ttu-id="000e3-190">URL が検証に合格した場合は、この新しい URL に要求を再送信します。</span><span class="sxs-lookup"><span data-stu-id="000e3-190">If the URL passes validation, resend the request to this new URL.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="000e3-191">関連項目</span><span class="sxs-lookup"><span data-stu-id="000e3-191">See also</span></span>


- [<span data-ttu-id="000e3-192">Exchange の自動検出</span><span class="sxs-lookup"><span data-stu-id="000e3-192">Autodiscover for Exchange</span></span>](autodiscover-for-exchange.md)
    
- [<span data-ttu-id="000e3-193">Exchange SCP のルックアップを使用して自動検出エンドポイントを検索します。</span><span class="sxs-lookup"><span data-stu-id="000e3-193">Find Autodiscover endpoints by using SCP lookup in Exchange</span></span>](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md)
    
- [<span data-ttu-id="000e3-194">エラー コード (SOAP)</span><span class="sxs-lookup"><span data-stu-id="000e3-194">ErrorCode (SOAP)</span></span>](http://msdn.microsoft.com/library/5e5ec861-0191-4ecb-a906-47ce8ed96381%28Office.15%29.aspx)
    
- [<span data-ttu-id="000e3-195">エラー コード (POX)</span><span class="sxs-lookup"><span data-stu-id="000e3-195">ErrorCode (POX)</span></span>](http://msdn.microsoft.com/library/064d73e4-45b7-4797-828e-9df590830db8%28Office.15%29.aspx)
    

