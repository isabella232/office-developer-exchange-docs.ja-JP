---
title: 自動検出のエラー メッセージを処理する
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: e5939ec2-1100-4174-8a88-5a6e09b60b23
description: 自動検出の各種エラーと、そのエラーの対処法について説明します。
ms.openlocfilehash: fcafc799f4d35e92159d2913845474ecf7bc5657
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758898"
---
# <a name="handling-autodiscover-error-messages"></a><span data-ttu-id="097f1-103">自動検出のエラー メッセージを処理する</span><span class="sxs-lookup"><span data-stu-id="097f1-103">Handling Autodiscover error messages</span></span>

<span data-ttu-id="097f1-104">自動検出の各種エラーと、そのエラーの対処法について説明します。</span><span class="sxs-lookup"><span data-stu-id="097f1-104">Learn about the different types of Autodiscover errors and what to do with them.</span></span>
  
<span data-ttu-id="097f1-p101">自動検出により、カスタムのアプリケーションは構成情報を自動的に取得できるようになり、最適に動作するようになります。ただし、物事は計画どおりに進まないこともあります。発生することがある一般的なエラーについて説明して、ユーザーに要求するクライアントの手動構成を最小限にするためのエラー処理の方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="097f1-p101">Autodiscover enables your applications to retrieve configuration information automatically, and it works great. However, things don't always go according to plan. Let's look at the common errors that might occur and how you can handle them to minimize the need to prompt your user to manually configure your client.</span></span>
  
## <a name="http-status-errors"></a><span data-ttu-id="097f1-108">HTTP 状態のエラー</span><span class="sxs-lookup"><span data-stu-id="097f1-108">HTTP status errors</span></span>
<span data-ttu-id="097f1-109"><a name="bk_HttpErrors"> </a></span><span class="sxs-lookup"><span data-stu-id="097f1-109"></span></span>

<span data-ttu-id="097f1-p102">最初の種類のエラーは、自動検出の要求を送信するときに発生することがある HTTP 状態です。応答に含まれる HTTP 状態が 200 (OK) 以外の場合、求めている自動検出の応答は応答のペイロードに含まれていません。わかりやすくするために、200 以外の状態コードを 3 つのカテゴリに分類します。</span><span class="sxs-lookup"><span data-stu-id="097f1-p102">The first type of error you might encounter when sending Autodiscover requests is the HTTP status. If the HTTP status in your response is anything other than 200 (OK), the response payload doesn't contain the Autodiscover response you were looking for. For simplicity, we can group non-200 status codes into three categories.</span></span>
  
<span data-ttu-id="097f1-113">**表 1. HTTP 状態コード**</span><span class="sxs-lookup"><span data-stu-id="097f1-113">**Table 1.  HTTP status codes**</span></span>

|<span data-ttu-id="097f1-114">**ステータス コード**</span><span class="sxs-lookup"><span data-stu-id="097f1-114">**Status code**</span></span>|<span data-ttu-id="097f1-115">**エラーの種類**</span><span class="sxs-lookup"><span data-stu-id="097f1-115">**Type of error**</span></span>|<span data-ttu-id="097f1-116">**処理方法**</span><span class="sxs-lookup"><span data-stu-id="097f1-116">**To handle…**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="097f1-117">301 または 302</span><span class="sxs-lookup"><span data-stu-id="097f1-117">301 or 302</span></span>  <br/> |<span data-ttu-id="097f1-118">リダイレクト エラー</span><span class="sxs-lookup"><span data-stu-id="097f1-118">Redirect error</span></span>  <br/> |<span data-ttu-id="097f1-119">HTTP 応答ヘッダーの "Location" に格納されている URI に向けて要求を再送信します。</span><span class="sxs-lookup"><span data-stu-id="097f1-119">Resend your request to the URI contained in the "Location" HTTP response header. For details, see Handling redirect errors.</span></span> <span data-ttu-id="097f1-120">詳細については、「[リダイレクト エラーの処理](#bk_HandlingRedirects)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="097f1-120">For details, see [Handling redirect errors](#bk_HandlingRedirects).</span></span>  <br/> |
|<span data-ttu-id="097f1-121">401</span><span class="sxs-lookup"><span data-stu-id="097f1-121">401</span></span>  <br/> |<span data-ttu-id="097f1-122">未認証エラー</span><span class="sxs-lookup"><span data-stu-id="097f1-122">Unauthorized error</span></span>  <br/> |<span data-ttu-id="097f1-123">[自動検出プロセス](autodiscover-for-exchange.md)では、複数の潜在的な URL を試してみることが必要になるため、このエラーはある URL のみで発生することがあります (その次の URL は資格情報を受け入れた状態になります)。</span><span class="sxs-lookup"><span data-stu-id="097f1-123">Because the [Autodiscover process](autodiscover-for-exchange.md) involves trying multiple potential URLs, you could get this on one URL only to have the next one accept your credentials.</span></span> <span data-ttu-id="097f1-124">このため、単一の 401 エラーで資格情報が無効だと見なしてはいけません。</span><span class="sxs-lookup"><span data-stu-id="097f1-124">For this reason, you shouldn't consider a single 401 error to indicate that the credentials are invalid.</span></span> <span data-ttu-id="097f1-125">ただし、複数の URL から 401 エラーを受け取る場合は、ユーザーにパスワードの再入力を求めるプロンプトを表示します (可能な場合)。</span><span class="sxs-lookup"><span data-stu-id="097f1-125">However, if you receive 401 errors from multiple URLs, you might want to prompt the user to reenter their password (if possible).</span></span>  <br/> |
|<span data-ttu-id="097f1-126">その他の 200 以外の状態</span><span class="sxs-lookup"><span data-stu-id="097f1-126">Any other non-200 status</span></span>  <br/> |<span data-ttu-id="097f1-127">無効な自動検出エンドポイントのエラー</span><span class="sxs-lookup"><span data-stu-id="097f1-127">Invalid Autodiscover endpoint error</span></span>  <br/> |<span data-ttu-id="097f1-128">200 以外の状態コードを返す URL は無効であると見なして、一覧内で次に当たる URL の試行を続行します。</span><span class="sxs-lookup"><span data-stu-id="097f1-128">Consider the URL that returns any other non-200 status code to be invalid, and continue trying the next URL in your list.</span></span>  <br/> |
   
## <a name="autodiscover-errors"></a><span data-ttu-id="097f1-129">自動検出のエラー</span><span class="sxs-lookup"><span data-stu-id="097f1-129">Autodiscover errors</span></span>
<span data-ttu-id="097f1-130"><a name="bk_AutodiscoverErrors"> </a></span><span class="sxs-lookup"><span data-stu-id="097f1-130"></span></span>

<span data-ttu-id="097f1-p105">自動検出要求の送信後に 200 (OK) の状態コードを得たとしても、必要としている情報がサーバーから送られたという意味にはなりません。200 の状態は自動検出の応答があったということだけを意味し、その応答のペイロードにはエラーが含まれていることもあります。SOAP 形式と POX 形式では、エラー情報の場所が異なります。</span><span class="sxs-lookup"><span data-stu-id="097f1-p105">Even if you get a 200 (OK) status code after sending an Autodiscover request, that doesn't mean that the server sent the information you need. The 200 status only means that you have an Autodiscover response, and that response might contain an error within the payload. The location of the error information differs depending on whether the format is SOAP or POX.</span></span>
  
### <a name="soap-autodiscover-errors"></a><span data-ttu-id="097f1-134">SOAP 自動検出のエラー</span><span class="sxs-lookup"><span data-stu-id="097f1-134">SOAP Autodiscover errors</span></span>

<span data-ttu-id="097f1-135">SOAP 自動検出の場合は、1 つ以上の [ErrorCode (SOAP)](http://msdn.microsoft.com/library/5e5ec861-0191-4ecb-a906-47ce8ed96381%28Office.15%29.aspx) 要素が応答の異なる場所に含まれていることがあります。</span><span class="sxs-lookup"><span data-stu-id="097f1-135">For SOAP Autodiscover, the response can contain one or more [ErrorCode (SOAP)](http://msdn.microsoft.com/library/5e5ec861-0191-4ecb-a906-47ce8ed96381%28Office.15%29.aspx) elements, in different places.</span></span> <span data-ttu-id="097f1-136">一般に、[Response (SOAP)](http://msdn.microsoft.com/library/4c2bcdeb-95ce-4ffa-bd83-118af53b534f%28Office.15%29.aspx) 要素の子要素として期待することや、応答内の各 [UserResponse (SOAP)](http://msdn.microsoft.com/library/5007b1ba-bfcc-40d7-b1cb-e32fbaf54ffd%28Office.15%29.aspx) 要素の子として期待することができます。</span><span class="sxs-lookup"><span data-stu-id="097f1-136">Typically you can expect one as a child element of the [Response (SOAP)](http://msdn.microsoft.com/library/4c2bcdeb-95ce-4ffa-bd83-118af53b534f%28Office.15%29.aspx) element, and one as a child of each [UserResponse (SOAP)](http://msdn.microsoft.com/library/5007b1ba-bfcc-40d7-b1cb-e32fbaf54ffd%28Office.15%29.aspx) element in the response.</span></span> <span data-ttu-id="097f1-137">また、[UserSettingError (SOAP)](http://msdn.microsoft.com/library/abb175c5-4f38-4dcc-81e3-b511686862eb%28Office.15%29.aspx) 要素の子として出現することもあります (存在する場合)。</span><span class="sxs-lookup"><span data-stu-id="097f1-137">You might also encounter one as a child of a [UserSettingError (SOAP)](http://msdn.microsoft.com/library/abb175c5-4f38-4dcc-81e3-b511686862eb%28Office.15%29.aspx) element, if one is present.</span></span> <span data-ttu-id="097f1-138">エラーのコンテキストは、次に示すように **ErrorCode** 要素の場所によって変化します。</span><span class="sxs-lookup"><span data-stu-id="097f1-138">The context of the error depends on where the **ErrorCode** element is located, as follows:</span></span> 
  
- <span data-ttu-id="097f1-139">**Response** 要素の子要素の場合、**ErrorCode** 要素は要求全体に当てはまるエラーを表します。</span><span class="sxs-lookup"><span data-stu-id="097f1-139">As a child element of the **Response** element, the **ErrorCode** element represents an error that applies to the entire request.</span></span> 
    
- <span data-ttu-id="097f1-140">**UserResponse** 要素の子の場合は、特定のユーザーにのみ当てはまるエラーを表します。</span><span class="sxs-lookup"><span data-stu-id="097f1-140">As a child of the **UserResponse** element, it represents an error that applies just to that specific user.</span></span> 
    
- <span data-ttu-id="097f1-141">**UserSettingError** 要素の子の場合は、要求された特定の設定に当てはまるエラーを表します。</span><span class="sxs-lookup"><span data-stu-id="097f1-141">As a child of a **UserSettingError** element, it represents an error that applies to a specific setting that was requested.</span></span> 
    
<span data-ttu-id="097f1-142">応答の例を調べてみましょう。</span><span class="sxs-lookup"><span data-stu-id="097f1-142">Let's take a look at an example of a response.</span></span> <span data-ttu-id="097f1-143">この例では、**Response** 要素の **ErrorCode** 要素に "NoError" という値が含まれています。この値は、全体的な成功を表します。</span><span class="sxs-lookup"><span data-stu-id="097f1-143">In this example, the **ErrorCode** element under the **Response** element has a value of "NoError", which indicates overall success.</span></span> <span data-ttu-id="097f1-144">ただし、**UserResponse** 要素の **ErrorCode** 要素には "RedirectAddress" という値が含まれています。この値は、その特定のユーザーにエラーが発生したことを表します。</span><span class="sxs-lookup"><span data-stu-id="097f1-144">Let's take a look at an example of a response. In this example, the **ErrorCode** element under the **Response** element has a value of "NoError", which indicates overall success. However, the ErrorCode element under the UserResponse element has a value of "RedirectAddress", which indicates that an error occurred for that particular user.</span></span> 
  
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

<span data-ttu-id="097f1-145">「[ErrorCode (SOAP)](http://msdn.microsoft.com/library/5e5ec861-0191-4ecb-a906-47ce8ed96381%28Office.15%29.aspx)」の記事に、発生することがあるすべてのエラーの一覧が記載されています。</span><span class="sxs-lookup"><span data-stu-id="097f1-145">The [ErrorCode (SOAP)](http://msdn.microsoft.com/library/5e5ec861-0191-4ecb-a906-47ce8ed96381%28Office.15%29.aspx) article contains a full list of possible errors. Most of these indicate an unrecoverable error, but a few warrant special handling.</span></span> <span data-ttu-id="097f1-146">これらのほとんどは、回復不可能なエラーを表しますが、いくつかは特別な処理を認めるものがあります。</span><span class="sxs-lookup"><span data-stu-id="097f1-146">The ErrorCode (SOAP) article contains a full list of possible errors. Most of these indicate an unrecoverable error, but a few warrant special handling.</span></span> 
  
<span data-ttu-id="097f1-147">**表 2. SOAP 自動検出の ErrorCode の値**</span><span class="sxs-lookup"><span data-stu-id="097f1-147">**Table 2.  SOAP Autodisover ErrorCode values**</span></span>

|<span data-ttu-id="097f1-148">**ErrorCode の値**</span><span class="sxs-lookup"><span data-stu-id="097f1-148">**ErrorCode value**</span></span>|<span data-ttu-id="097f1-149">**処理方法**</span><span class="sxs-lookup"><span data-stu-id="097f1-149">**To handle…**</span></span>|
|:-----|:-----|
|<span data-ttu-id="097f1-150">RedirectAddress</span><span class="sxs-lookup"><span data-stu-id="097f1-150">RedirectAddress</span></span>  <br/> |<span data-ttu-id="097f1-151">[RedirectTarget (SOAP)](http://msdn.microsoft.com/library/f8162724-cf9a-4543-a1ad-5846c8b10bfa%28Office.15%29.aspx) 要素の電子メール アドレスを使用して、[新しい電子メール アドレスで自動検出を再開](#bk_RestartAutodiscover)します。</span><span class="sxs-lookup"><span data-stu-id="097f1-151">[Restarting Autodiscover with a new email address](#bk_RestartAutodiscover) with the email address in the [RedirectTarget (SOAP)](http://msdn.microsoft.com/library/f8162724-cf9a-4543-a1ad-5846c8b10bfa%28Office.15%29.aspx) element.</span></span>  <br/> |
|<span data-ttu-id="097f1-152">RedirectUrl</span><span class="sxs-lookup"><span data-stu-id="097f1-152">RedirectUrl</span></span>  <br/> |<span data-ttu-id="097f1-153">**RedirectTarget** 要素の URL を[新しい URL として要求を再送信](#bk_ResendRequest)します。</span><span class="sxs-lookup"><span data-stu-id="097f1-153">[Resending your request to a new URL](#bk_ResendRequest) to the URL in the **RedirectTarget** element.</span></span>  <br/> |
|<span data-ttu-id="097f1-154">ServerBusy</span><span class="sxs-lookup"><span data-stu-id="097f1-154">ServerBusy</span></span>  <br/> |<span data-ttu-id="097f1-p109">少し間をおいて、この URL を再試行します。一定時間待機するか、この URL を単に試行する URL の一覧の最後に移動します。このエラーを 1 つの URL から複数回受け取る場合は、その URL が無効であると見なす必要があります。</span><span class="sxs-lookup"><span data-stu-id="097f1-p109">Retry this URL after a small delay. You might wait a set amount of time or simply move this URL to the end of your list of URLs to try. If you receive this error multiple times from a URL, you should consider the URL to be invalid.</span></span>  <br/> |
   
### <a name="pox-autodiscover-errors"></a><span data-ttu-id="097f1-158">POX 自動検出のエラー</span><span class="sxs-lookup"><span data-stu-id="097f1-158">POX Autodiscover errors</span></span>

<span data-ttu-id="097f1-159">POX 自動検出サービスは、少し異なる方法でエラーを報告します。</span><span class="sxs-lookup"><span data-stu-id="097f1-159">The POX Autodiscover service reports errors a little differently.</span></span> <span data-ttu-id="097f1-160">回復不可能なエラーは、[Error (POX)](http://msdn.microsoft.com/library/91c63b62-ab68-4c32-a2f7-5a87c188335b%28Office.15%29.aspx) 要素に含まれています。</span><span class="sxs-lookup"><span data-stu-id="097f1-160">Non-recoverable errors are contained in the [Error (POX)](http://msdn.microsoft.com/library/91c63b62-ab68-4c32-a2f7-5a87c188335b%28Office.15%29.aspx) element.</span></span> <span data-ttu-id="097f1-161">「[ErrorCode (POX)](http://msdn.microsoft.com/library/064d73e4-45b7-4797-828e-9df590830db8%28Office.15%29.aspx)」の記事に、発生することがあるすべてのエラーの一覧が記載されています。</span><span class="sxs-lookup"><span data-stu-id="097f1-161">The [ErrorCode (POX)](http://msdn.microsoft.com/library/064d73e4-45b7-4797-828e-9df590830db8%28Office.15%29.aspx) article contains a full list of possible error codes.</span></span> 
  
<span data-ttu-id="097f1-162">リダイレクトのエラーは、[Action (POX)](http://msdn.microsoft.com/library/a3462c6b-453c-462a-830d-f29ee4a2babb%28Office.15%29.aspx) 要素に含まれています。</span><span class="sxs-lookup"><span data-stu-id="097f1-162">Redirect errors are contained in the [Action (POX)](http://msdn.microsoft.com/library/a3462c6b-453c-462a-830d-f29ee4a2babb%28Office.15%29.aspx) element.</span></span> <span data-ttu-id="097f1-163">**Action** 要素の "settings" 以外の値は、どれもリダイレクト エラーを表します。</span><span class="sxs-lookup"><span data-stu-id="097f1-163">Redirect errors are contained in the Action element. Any value of the **Action** element other than "settings" indicates a redirect error.</span></span> 
  
<span data-ttu-id="097f1-164">**表 3. POX 自動検出の ErrorCode の値**</span><span class="sxs-lookup"><span data-stu-id="097f1-164">**Table 3.  POX Autodisover ErrorCode values**</span></span>

|<span data-ttu-id="097f1-165">**Action の値**</span><span class="sxs-lookup"><span data-stu-id="097f1-165">**Action value**</span></span>|<span data-ttu-id="097f1-166">**処理方法**</span><span class="sxs-lookup"><span data-stu-id="097f1-166">**To handle…**</span></span>|
|:-----|:-----|
|<span data-ttu-id="097f1-167">redirectAddr</span><span class="sxs-lookup"><span data-stu-id="097f1-167">redirectAddr</span></span>  <br/> |<span data-ttu-id="097f1-168">[RedirectAddr (POX)](http://msdn.microsoft.com/library/0e9fa6b6-7991-4dc1-a59a-48e5f8e041e4%28Office.15%29.aspx) 要素の電子メール アドレスを使用して、[新しい電子メール アドレスで自動検出を再開](#bk_RestartAutodiscover)します。</span><span class="sxs-lookup"><span data-stu-id="097f1-168">[Restarting Autodiscover with a new email address](#bk_RestartAutodiscover) with the email address in the [RedirectAddr (POX)](http://msdn.microsoft.com/library/0e9fa6b6-7991-4dc1-a59a-48e5f8e041e4%28Office.15%29.aspx) element.</span></span>  <br/> |
|<span data-ttu-id="097f1-169">redirectUrl</span><span class="sxs-lookup"><span data-stu-id="097f1-169">redirectUrl</span></span>  <br/> |<span data-ttu-id="097f1-170">[RedirectUrl (POX)](http://msdn.microsoft.com/library/c54f310f-8c99-4c37-8e73-ac87722b6229%28Office.15%29.aspx) 要素の URL を[新しい URL として要求を再送信](#bk_ResendRequest)します。</span><span class="sxs-lookup"><span data-stu-id="097f1-170">[Resending your request to a new URL](#bk_ResendRequest) to the URL in the [RedirectUrl (POX)](http://msdn.microsoft.com/library/c54f310f-8c99-4c37-8e73-ac87722b6229%28Office.15%29.aspx) element.</span></span>  <br/> |
   
<span data-ttu-id="097f1-171">この例では、**Action** 要素には "redirectAddr" という値が含まれています。この値は、**RedirectAddr** 要素に含まれた新しい電子メール アドレスで新しい要求を送信する必要があることを示しています。</span><span class="sxs-lookup"><span data-stu-id="097f1-171">In this example, the **Action** element has a value of "redirectAddr", which indicates that a new request should be sent with the new email address contained in the **RedirectAddr** element.</span></span> 
  
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

## <a name="handling-redirect-errors"></a><span data-ttu-id="097f1-172">リダイレクト エラーの処理</span><span class="sxs-lookup"><span data-stu-id="097f1-172">Handling redirect errors</span></span>
<span data-ttu-id="097f1-173"><a name="bk_HandlingRedirects"> </a></span><span class="sxs-lookup"><span data-stu-id="097f1-173"></span></span>

<span data-ttu-id="097f1-174">リダイレクト エラーのシナリオは 2 つの方法で処理できます。</span><span class="sxs-lookup"><span data-stu-id="097f1-174">You can handle redirect error scenarios in two ways:</span></span>
  
- <span data-ttu-id="097f1-175">新しい電子メール アドレスで自動検出を再開する。</span><span class="sxs-lookup"><span data-stu-id="097f1-175">By restarting Autodiscover with a new email address.</span></span>
    
- <span data-ttu-id="097f1-176">新しい URL に要求を再送信する。</span><span class="sxs-lookup"><span data-stu-id="097f1-176">By resending your request to a new URL.</span></span>
    
<span data-ttu-id="097f1-177">どちらのシナリオも続行する前に何らかの検証が必要になります。</span><span class="sxs-lookup"><span data-stu-id="097f1-177">Both scenarios require some validation before proceeding.</span></span>
  
### <a name="restarting-autodiscover-with-a-new-email-address"></a><span data-ttu-id="097f1-178">新しい電子メール アドレスで自動検出を再開する</span><span class="sxs-lookup"><span data-stu-id="097f1-178">Restarting Autodiscover with a new email address</span></span>
<span data-ttu-id="097f1-179"><a name="bk_RestartAutodiscover"> </a></span><span class="sxs-lookup"><span data-stu-id="097f1-179"></span></span>

<span data-ttu-id="097f1-p112">自動検出のリダイレクト応答で新しい電子メール アドレスを取得したときには、リダイレクト エラー応答で提示された新しい電子メール アドレスがエラーになった要求で送信されたアドレスと同じでないことを最初に確認します。同じになる場合は、自動検出を再開してはいけません。その代わりに、応答を生成した URL を無効と見なします。</span><span class="sxs-lookup"><span data-stu-id="097f1-p112">When you get a new email address in an Autodiscover redirect response, first verify that the new email address that was provided in the redirect error response is not the same address that you sent in the request that resulted in the error. If it is, you should not restart Autodiscover and instead consider the URL that generated the response to be invalid.</span></span>
  
<span data-ttu-id="097f1-182">新しい電子メール アドレスが異なる場合は、潜在的な自動検出エンドポイント URL の既存の一覧を破棄して、新しい電子メール アドレスに基づいた新しい一覧を生成します。</span><span class="sxs-lookup"><span data-stu-id="097f1-182">If the new email address is different, discard your existing list of potential Autodiscover endpoint URLs and generate a new list based on the new email address.</span></span>
  
### <a name="resending-your-request-to-a-new-url"></a><span data-ttu-id="097f1-183">新しい URL に要求を再送信する</span><span class="sxs-lookup"><span data-stu-id="097f1-183">Resending your request to a new URL</span></span>
<span data-ttu-id="097f1-184"><a name="bk_ResendRequest"> </a></span><span class="sxs-lookup"><span data-stu-id="097f1-184"></span></span>

<span data-ttu-id="097f1-185">自動検出リダイレクト応答で新しい URL を取得したときには、まず、その URL を次のようにして検証する必要があります。</span><span class="sxs-lookup"><span data-stu-id="097f1-185">When you get a new URL in an Autodiscover redirect response, you should first validate the URL as follows:</span></span>
  
- <span data-ttu-id="097f1-186">URL が HTTPS URL であることを確認します。</span><span class="sxs-lookup"><span data-stu-id="097f1-186">Verify that the URL is an HTTPS URL.</span></span>
    
- <span data-ttu-id="097f1-187">これまでに現在の電子メール アドレスで、この URL からエラーを受け取っていないことを確認します。</span><span class="sxs-lookup"><span data-stu-id="097f1-187">Verify that you have not received an error from this URL with the current email address before.</span></span>
    
- <span data-ttu-id="097f1-188">カスタム アプリケーションに適用可能な場合は、ユーザーにリダイレクトについて知らせて、リダイレクトに従う許可を取ります。</span><span class="sxs-lookup"><span data-stu-id="097f1-188">If applicable to your application, inform the user of the redirection and get their permission to follow the redirect.</span></span>
    
- <span data-ttu-id="097f1-189">URL に要求を送信して、[サーバーが提示した SSL 証明書が有効であることを確認します](how-to-validate-a-server-certificate-for-the-ews-managed-api.md)。</span><span class="sxs-lookup"><span data-stu-id="097f1-189">Send a request to the URL and [verify that the SSL certificate presented by the server is valid](how-to-validate-a-server-certificate-for-the-ews-managed-api.md).</span></span>
    
<span data-ttu-id="097f1-190">URL が検証に合格した場合は、この新しい URL に要求を再送信します。</span><span class="sxs-lookup"><span data-stu-id="097f1-190">If the URL passes validation, resend the request to this new URL.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="097f1-191">関連項目</span><span class="sxs-lookup"><span data-stu-id="097f1-191">See also</span></span>


- [<span data-ttu-id="097f1-192">Exchange の自動検出</span><span class="sxs-lookup"><span data-stu-id="097f1-192">Autodiscover for Exchange</span></span>](autodiscover-for-exchange.md)
    
- [<span data-ttu-id="097f1-193">Exchange の SCP 参照を使用して自動検出エンドポイントを見つける</span><span class="sxs-lookup"><span data-stu-id="097f1-193">How to: Find Autodiscover endpoints by using SCP lookup in Exchange</span></span>](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md)
    
- [<span data-ttu-id="097f1-194">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="097f1-194">ErrorCode (SOAP)</span></span>](http://msdn.microsoft.com/library/5e5ec861-0191-4ecb-a906-47ce8ed96381%28Office.15%29.aspx)
    
- [<span data-ttu-id="097f1-195">ErrorCode (POX)</span><span class="sxs-lookup"><span data-stu-id="097f1-195">ErrorCode (POX)</span></span>](http://msdn.microsoft.com/library/064d73e4-45b7-4797-828e-9df590830db8%28Office.15%29.aspx)
    

