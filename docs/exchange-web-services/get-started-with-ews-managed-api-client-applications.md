---
title: EWS マネージ API クライアント アプリケーションの概要
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: c2267733-6f4f-49e5-9614-1e4a24c3af1a
description: EWS マネージ API を使用して、Exchange 用の単純な Hello World メール クライアント アプリケーションを開発します。
ms.openlocfilehash: dafc8cbbf172ad725ab83c93553464ba96ef33b8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19758910"
---
# <a name="get-started-with-ews-managed-api-client-applications"></a><span data-ttu-id="64784-103">EWS マネージ API クライアント アプリケーションの概要</span><span class="sxs-lookup"><span data-stu-id="64784-103">Get started with EWS Managed API client applications</span></span>

<span data-ttu-id="64784-104">EWS マネージ API を使用して、Exchange 用の単純な Hello World メール クライアント アプリケーションを開発します。</span><span class="sxs-lookup"><span data-stu-id="64784-104">Develop a simple Hello World email client application for Exchange by using the EWS Managed API.</span></span> 
  
<span data-ttu-id="64784-p101">[EWS マネージ API](http://aka.ms/ews-managed-api-readme) では、クライアント アプリケーション、ポータル アプリケーション、サービス アプリケーションから Web サービス メッセージを送受信するための、直観的で使いやすいオブジェクト モデルが用意されています。EWS マネージ API を使用して、Exchange Online、Office 365 の一部としての Exchange Online、Exchange サーバー メールボックスに格納されているほとんどすべての情報にアクセスすることができます。この記事にある情報は、初めて EWS マネージ API のクライアント アプリケーションを開発する場合に役立ちます。</span><span class="sxs-lookup"><span data-stu-id="64784-p101">The [EWS Managed API](http://aka.ms/ews-managed-api-readme) provides an intuitive, easy-to-use object model for sending and receiving web service messages from client applications, portal applications, and service applications. You can access almost all the information stored in an Exchange Online, Exchange Online as part of Office 365, or an Exchange server mailbox by using the EWS Managed API. You can use the information in this article to help you develop your first EWS Managed API client application.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="64784-p102">[!メモ]  EWS マネージ API が、 [GitHub](https://github.com/officedev/ews-managed-api) のオープン ソース プロジェクトとして利用できるようになりました。オープン ソース ライブラリを使用して、次のことができます。 >  バグ修正と API の機能強化に貢献します。 >  公式のリリースで利用可能になる前に、修正プログラムや拡張機能を取得できます。 >  API の最も包括的かつ最新の実装にアクセスして、参照として使用するか、新しいプラットフォームで新しいライブラリを作成します。 >  GitHub による [貢献](https://github.com/OfficeDev/ews-managed-api/blob/master/CONTRIBUTING.md)を歓迎いたします。</span><span class="sxs-lookup"><span data-stu-id="64784-p102">The EWS Managed API is now available as an open source project on [GitHub](https://github.com/officedev/ews-managed-api). You can use the open source library to: >  Contribute bug fixes and enhancements to the API. >  Get fixes and enhancements before they are available in an official release. >  Access the most comprehensive and up-to-date implementation of the API, to use as a reference or to create new libraries on new platforms. >  We welcome your [contributions](https://github.com/OfficeDev/ews-managed-api/blob/master/CONTRIBUTING.md) via GitHub.</span></span> 
  
## <a name="youll-need-an-exchange-server"></a><span data-ttu-id="64784-113">Exchange サーバーの準備</span><span class="sxs-lookup"><span data-stu-id="64784-113">You'll need an Exchange server</span></span>
<span data-ttu-id="64784-114"><a name="NeedExchange"> </a></span><span class="sxs-lookup"><span data-stu-id="64784-114"></span></span>

<span data-ttu-id="64784-p103">Exchange メールボックス アカウントを既に所有している場合は、このセクションを省略してもかまいません。それ以外の場合は、次のいずれかの方法で、初めての EWS クライアント アプリケーション用の Exchange メールボックスをセットアップします。</span><span class="sxs-lookup"><span data-stu-id="64784-p103">If you already have an Exchange mailbox account, you can skip this section. Otherwise, you have the following options for setting up an Exchange mailbox for your first EWS client application:</span></span>
  
- <span data-ttu-id="64784-p104">[Office 365 開発者向けサイト](http://msdn.microsoft.com/en-us/library/office/fp179924.aspx)を取得します (推奨)。これが最も簡単に Exchange メールボックスをセットアップする方法です。</span><span class="sxs-lookup"><span data-stu-id="64784-p104">Get an [Office 365 Developer Site](http://msdn.microsoft.com/en-us/library/office/fp179924.aspx) (recommended). This is the quickest way for you to set up an Exchange mailbox.</span></span> 
    
- <span data-ttu-id="64784-119">[Exchange Server](http://office.microsoft.com/en-us/exchange/microsoft-exchange-try-or-buy-exchange-we-can-help-you-decide-FX103746846.aspx?WT%2Eintid1=ODC%5FENUS%5FFX103472230%5FXT103965589) をダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="64784-119">Download [Exchange Server](http://office.microsoft.com/en-us/exchange/microsoft-exchange-try-or-buy-exchange-we-can-help-you-decide-FX103746846.aspx?WT%2Eintid1=ODC%5FENUS%5FFX103472230%5FXT103965589).</span></span>
    
<span data-ttu-id="64784-p105">Exchange からメールを送受信できることが確認できたら、開発環境をセットアップする準備ができています。Exchange Web クライアントの [Outlook Web App](http://technet.microsoft.com/en-us/library/jj657718%28v=exchg.150%29.aspx) を使用して、メールが送信できることを確認します。</span><span class="sxs-lookup"><span data-stu-id="64784-p105">After you have verified that you can send and receive email from Exchange, you are ready to set up your development environment. You can use the Exchange web client [Outlook Web App](http://technet.microsoft.com/en-us/library/jj657718%28v=exchg.150%29.aspx) to verify that you can send email.</span></span> 
  
## <a name="set-up-your-development-environment"></a><span data-ttu-id="64784-122">開発環境のセットアップ</span><span class="sxs-lookup"><span data-stu-id="64784-122">Set up your development environment</span></span>
<span data-ttu-id="64784-123"><a name="Setup"> </a></span><span class="sxs-lookup"><span data-stu-id="64784-123"></span></span>

<span data-ttu-id="64784-124">以下にアクセスできることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="64784-124">Make sure that you have access to the following:</span></span>
  
- <span data-ttu-id="64784-p106">.NET Framework 4 をサポートしているバージョンの [Visual Studio](http://www.visualstudio.com/en-us/downloads/download-visual-studio-vs.aspx)。技術的には、どの C# コンパイラでも使用できるため Visual Studio は必ず必要であるというわけではありませんが、Visual Studio を使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="64784-p106">Any version of [Visual Studio](http://www.visualstudio.com/en-us/downloads/download-visual-studio-vs.aspx) that supports the .NET Framework 4. Although technically, you don't need Visual Studio because you can use any C# compiler, we recommend that you use it.</span></span> 
    
- <span data-ttu-id="64784-p107">[EWS マネージ API](http://aka.ms/ews-managed-api-readme)。システムに応じて、64 ビット バージョンと 32 ビット バージョンのどちらかをインストールします。既定のインストール場所を使用します。</span><span class="sxs-lookup"><span data-stu-id="64784-p107">The [EWS Managed API](http://aka.ms/ews-managed-api-readme). You can use either the 64-bit or 32-bit version, depending on your system. Use the default installation location.</span></span> 
    
## <a name="create-your-first-ews-managed-api-application"></a><span data-ttu-id="64784-130">初めての EWS マネージ API アプリケーションの作成</span><span class="sxs-lookup"><span data-stu-id="64784-130">Create your first EWS Managed API application</span></span>
<span data-ttu-id="64784-131"><a name="Create"> </a></span><span class="sxs-lookup"><span data-stu-id="64784-131"></span></span>

<span data-ttu-id="64784-p108">次の手順は、Office 365 開発者向けサイトをセットアップすることを前提としています。Exchange をダウンロードしてインストールした場合、Exchange サーバーに[有効な証明書をインストール](http://technet.microsoft.com/en-us/library/bb310769%28v=exchg.141%29.aspx)するか、既定で提供されている自己署名証明書用に[証明書の検証コールバックを実装](how-to-validate-a-server-certificate-for-the-ews-managed-api.md)する必要があります。なお、これらの手順は、使用している Visual Studio のバージョンによって若干異なる場合がありますのでご注意ください。</span><span class="sxs-lookup"><span data-stu-id="64784-p108">These steps assume that you set up an Office 365 Developer Site. If you downloaded and installed Exchange, you will need to [install a valid certificate](http://technet.microsoft.com/en-us/library/bb310769%28v=exchg.141%29.aspx) on your Exchange server or [implement a certificate validation](how-to-validate-a-server-certificate-for-the-ews-managed-api.md) callback for a self-signed certificate that is provided by default. Also note that these steps might vary slightly depending on the version of Visual Studio that you are using.</span></span> 
  
### <a name="step-1-create-a-project-in-visual-studio"></a><span data-ttu-id="64784-135">手順 1: Visual Studio でプロジェクトを作成する</span><span class="sxs-lookup"><span data-stu-id="64784-135">Step 1: Create a project in Visual Studio</span></span>

1. <span data-ttu-id="64784-p109">Visual Studio の **[ファイル]** メニューで、 **[新規]** を選択してから、 **[プロジェクト]** を選択します。 **[新しいプロジェクト]** ダイアログ ボックスが表示されます。</span><span class="sxs-lookup"><span data-stu-id="64784-p109">In Visual Studio, on the **File** menu, choose **New**, and then choose **Project**. The **New Project** dialog box opens.</span></span> 
    
2. <span data-ttu-id="64784-p110">**C# コンソール アプリケーション** を作成します。 **[テンプレート]** ウィンドウで、 **[Visual C#]** を選択してから、 **[コンソール アプリケーション]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="64784-p110">Create a **C# Console Application**. From the **Templates** pane, choose **Visual C#**, and then choose **Console Application**.</span></span> 
    
3. <span data-ttu-id="64784-140">プロジェクトに「HelloWorld」という名前を付けて、 **[OK]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="64784-140">Name the project HelloWorld, and then choose **OK**.</span></span>
    
<span data-ttu-id="64784-141">Visual Studio は、プロジェクトを作成し、Program.cs コードのドキュメント ウィンドウを開きます。</span><span class="sxs-lookup"><span data-stu-id="64784-141">Visual Studio creates the project and opens the Program.cs code document window.</span></span>

### <a name="step-2-add-a-reference-to-the-ews-managed-api"></a><span data-ttu-id="64784-142">手順 2:EWS マネージ API の参照を追加する</span><span class="sxs-lookup"><span data-stu-id="64784-142">Step 2: Add a reference to the EWS Managed API</span></span>

1. <span data-ttu-id="64784-p111">**[ソリューション エクスプ ローラー]** ウィンドウが既に開いている場合、この手順を省略し、手順 2 に進みます。 **[ソリューション エクスプ ローラー]** ウィンドウを開くには、 **[ビュー]** メニューで **[ソリューション エクスプ ローラー]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="64784-p111">If the **Solution Explorer** window is already open, skip this step and proceed to step 2. To open the **Solution Explorer** window, on the **View** menu, choose **Solution Explorer**.</span></span> 
    
2. <span data-ttu-id="64784-p112">**[ソリューション エクスプ ローラー]** の **HelloWorld** プロジェクトで **[参照]** のショートカット メニュー (右クリック) を開き、コンテキスト メニューから **[参照の追加]** を選択します。プロジェクトの参照を管理するためのダイアログ ボックスが開きます。</span><span class="sxs-lookup"><span data-stu-id="64784-p112">In the **Solution Explorer** and the **HelloWorld** project, open the shortcut menu (right-click) for **References** and choose **Add Reference** from the context menu. A dialog box for managing project references will open.</span></span> 
    
3. <span data-ttu-id="64784-147">[**参照**] オプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="64784-147">Choose the **Browse** option.</span></span> <span data-ttu-id="64784-148">EWS マネージ API DLL がインストールされている場所を参照します。</span><span class="sxs-lookup"><span data-stu-id="64784-148">Browse to the location where you installed the EWS Managed API DLL.</span></span> <span data-ttu-id="64784-149">インストーラーにより設定の既定のパスは、次: C:\Program Files\Microsoft\Exchange\Web サービス\<バージョン >\.</span><span class="sxs-lookup"><span data-stu-id="64784-149">The default path set by the installer is the following: C:\Program Files\Microsoft\Exchange\Web Services\<version>\.</span></span> <span data-ttu-id="64784-150">パスは、32 ビットまたは 64 ビット バージョンの Microsoft.Exchange.WebServices.dll をダウンロードするかどうか異なります。</span><span class="sxs-lookup"><span data-stu-id="64784-150">The path can vary based on whether you download the 32 or 64 bit version of the Microsoft.Exchange.WebServices.dll.</span></span> <span data-ttu-id="64784-151">**Microsoft.Exchange.WebServices.dll**を選択し、 **[ok]** または [**追加**を選択します。</span><span class="sxs-lookup"><span data-stu-id="64784-151">Choose **Microsoft.Exchange.WebServices.dll** and select **OK** or **Add**.</span></span> <span data-ttu-id="64784-152">EWS のマネージ API の参照をプロジェクトに追加します。</span><span class="sxs-lookup"><span data-stu-id="64784-152">This adds the EWS Managed API reference to your project.</span></span> 
    
4. <span data-ttu-id="64784-p114">EWS Managed API 2.0 を使用している場合は, .NET Framework 4 を対象とするよう HelloWorld プロジェクトを変更します。EWS マネージ API の他のバージョンでは、別の .NET Framework のターゲット バージョンを使用する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="64784-p114">If you are using EWS Managed API 2.0, change the HelloWorld project to target the .NET Framework 4. Other versions of the EWS Managed API might use a different target version of the .NET Framework.</span></span>
    
5. <span data-ttu-id="64784-p115">正しい .NET Framework のターゲット バージョンを使用していることを確認します。 **[ソリューション エクスプ ローラー]** で、 **HelloWorld** プロジェクトのショートカット メニュー (右クリック) を開き、 **[プロパティ]** を選択します。 **[ターゲット フレームワーク]** ドロップダウン ボックスで、 **[.NET Framework 4]** が選択されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="64784-p115">Confirm that you are using the correct target version of the .NET Framework. Open the shortcut menu (right-click) for your **HelloWorld** project in the **Solution Explorer**, and choose **Properties**. Verify that the **.NET Framework 4** is selected in the **Target framework** drop-down box.</span></span> 
    
<span data-ttu-id="64784-158">プロジェクトをセットアップし、EWS マネージ API への参照を作成したので、最初のアプリケーションを作成する準備ができました。</span><span class="sxs-lookup"><span data-stu-id="64784-158">Now that you have your project set up and you created a reference to the EWS Managed API, you are ready to create your first application.</span></span> <span data-ttu-id="64784-159">簡潔にするために、Program.cs ファイルにコードを追加します。</span><span class="sxs-lookup"><span data-stu-id="64784-159">To keep things simple, add your code to the Program.cs file.</span></span> <span data-ttu-id="64784-160">EWS のマネージ API の参照の詳細については[、EWS のマネージ API のアセンブリの参照](how-to-reference-the-ews-managed-api-assembly.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="64784-160">Read [Reference the EWS Managed API assembly](how-to-reference-the-ews-managed-api-assembly.md) for more information about referencing the EWS Managed API.</span></span> <span data-ttu-id="64784-161">次の手順では、ほとんどの EWS マネージ API クライアント アプリケーションを作成するための基本的なコードを開発します。</span><span class="sxs-lookup"><span data-stu-id="64784-161">In the next step, you will develop the basic code to write most EWS Managed API client applications.</span></span> 
### <a name="step-3-set-up-url-redirection-validation-for-autodiscover"></a><span data-ttu-id="64784-162">手順 3:自動検出のための URL リダイレクト検証を設定します。</span><span class="sxs-lookup"><span data-stu-id="64784-162">Step 3: Set up URL redirection validation for Autodiscover</span></span>

- <span data-ttu-id="64784-p117">**Main(string[] args)** メソッドの後に、次のリダイレクト検証コールバック メソッドを追加します。これは、 [自動検出](autodiscover-for-exchange.md)によって返される、リダイレクトされた URL が HTTPS エンドポイントを表すかどうかを検証します。</span><span class="sxs-lookup"><span data-stu-id="64784-p117">Add the following redirection validation callback method after the **Main(string[] args)** method. This validates whether redirected URLs returned by [Autodiscover](autodiscover-for-exchange.md) represent an HTTPS endpoint.</span></span> 
    
  ```cs
  private static bool RedirectionUrlValidationCallback(string redirectionUrl)
  {
     // The default for the validation callback is to reject the URL.
     bool result = false;
     Uri redirectionUri = new Uri(redirectionUrl);
     // Validate the contents of the redirection URL. In this simple validation
     // callback, the redirection URL is considered valid if it is using HTTPS
     // to encrypt the authentication credentials. 
     if (redirectionUri.Scheme == "https")
     {
        result = true;
     }
     return result;
  }
  ```

<span data-ttu-id="64784-p118">この検証コールバックは、手順 4 で **ExchangeService** オブジェクトに渡されます。アプリケーションが自動検出リダイレクトを信頼してそれに従うようにするには、これが必要です。自動検出リダイレクトの結果は、アプリケーションの EWS エンドポイントを提供します。</span><span class="sxs-lookup"><span data-stu-id="64784-p118">This validation callback will be passed to the **ExchangeService** object in step 4. You need this so that your application will trust and follow Autodiscover redirects - the results of the Autodiscover redirect provides the EWS endpoint for our application.</span></span> 

### <a name="step-4-prepare-the-exchangeservice-object"></a><span data-ttu-id="64784-167">手順 4:ExchangeService オブジェクトを準備する</span><span class="sxs-lookup"><span data-stu-id="64784-167">Step 4: Prepare the ExchangeService object</span></span>

1. <span data-ttu-id="64784-p119">**using** ディレクティブ参照を EWS マネージ API に追加します。Program.cs の上部の最後の **using** ディレクティブに次のコードを追加します。</span><span class="sxs-lookup"><span data-stu-id="64784-p119">Add a **using** directive reference to the EWS Managed API. Add the following code after the last **using** directive at the top of Program.cs.</span></span> 
    
   ```cs
    using Microsoft.Exchange.WebServices.Data;
   ```

2. <span data-ttu-id="64784-p120">**Main** メソッドで、対象とするサービス バージョンの [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトをインスタン化します。この例では、EWS スキーマの初期のバージョンを対象とします。</span><span class="sxs-lookup"><span data-stu-id="64784-p120">In the **Main** method, instantiate the [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object with the service version you intend to target. This example targets the earliest version of the EWS schema.</span></span> 
    
   ```cs
    ExchangeService service = new ExchangeService(ExchangeVersion.Exchange2007_SP1);
   ```

3. <span data-ttu-id="64784-p121">Exchange オンプレミス サーバーを対象としており、クライアントがドメインに参加している場合は、手順 4 に進みます。クライアントが Exchange Online または Office 365 開発者向けサイトのメールボックスを対象としている場合、明示的な資格情報を渡す必要があります。 **ExchangeService** オブジェクトのインスタンス化の後ろに次のコードを追加し、メールボックス アカウントの資格情報を設定します。ユーザー名は、ユーザー プリンシパル名でなければなりません。手順 5 に進んでください。</span><span class="sxs-lookup"><span data-stu-id="64784-p121">If you are targeting an on-premises Exchange server and your client is domain joined, proceed to step 4. If you client is targeting an Exchange Online or Office 365 Developer Site mailbox, you have to pass explicit credentials. Add the following code after the instantiation of the **ExchangeService** object and set the credentials for your mailbox account. The user name should be the user principal name. Proceed to step 5.</span></span> 
    
   ```cs
    service.Credentials = new WebCredentials("user1@contoso.com", "password");
   ```

4. <span data-ttu-id="64784-p122">オンプレミス Exchange サーバーを対象とする、ドメインに参加しているクライアントは、ログオンしているユーザーの既定の資格情報を使用できます。ここでは、この資格情報がメールボックスに関連付けられていることを想定しています。 **ExchangeService** オブジェクトのインスタンス化の後ろに、次のコードを追加します。</span><span class="sxs-lookup"><span data-stu-id="64784-p122">Domain-joined clients that target an on-premises Exchange server can use the default credentials of the user who is logged on, assuming the credentials are associated with a mailbox. Add the following code after the instantiation of the **ExchangeService** object.</span></span> 
    
   ```cs
    service.UseDefaultCredentials = true;
   ```

   <span data-ttu-id="64784-p123">クライアントが Exchange Online または Office 365 開発者向けサイトのメールボックスを対象とする場合、[UseDefaultCredentials](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.usedefaultcredentials%28v=exchg.80%29.aspx) が既定値である **false** に設定されていることを確認します。クライアントは、EWS サービスを呼び出すサービス URL を取得するために自動検出サービスの最初の呼び出しを行う準備ができました。</span><span class="sxs-lookup"><span data-stu-id="64784-p123">If your client targets an Exchange Online or Office 365 Developer Site mailbox, verify that [UseDefaultCredentials](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.usedefaultcredentials%28v=exchg.80%29.aspx) is set to **false**, which is the default value. Your client is ready to make the first call to the Autodiscover service to get the service URL for calls to the EWS service.</span></span>
    
5. <span data-ttu-id="64784-p124">**ExchangeService** オブジェクトの **AutodiscoverUrl** メソッドは、自動検出サービスに対して一連の呼び出しを実行してサービス URL を取得します。このメソッドの呼び出しが成功した場合、 **ExchangeService** オブジェクトの URL プロパティがサービス URL を使用して設定されます。ユーザーのメール アドレスおよび **RedirectionUrlValidationCallback** を **AutodiscoverUrl** メソッドに渡します。手順 3 または 手順 4 で資格情報を指定したら、次のコードを追加します。  `user1@contoso.com` を使用するメール アドレスに変更し、自動検出サービスが EWS エンドポイントを検索できるようにします。</span><span class="sxs-lookup"><span data-stu-id="64784-p124">The **AutodiscoverUrl** method on the **ExchangeService** object performs a series of calls to the Autodiscover service to get the service URL. If this method call is successful, the URL property on the **ExchangeService** object will be set with the service URL. Pass the user's email address and the **RedirectionUrlValidationCallback** to the **AutodiscoverUrl** method. Add the following code after the credentials have been specified in step 3 or 4. Change  `user1@contoso.com` to your email address so that the Autodiscover service finds your EWS endpoint.</span></span> 
    
   ```cs
    service.AutodiscoverUrl("user1@contoso.com", RedirectionUrlValidationCallback);
   ```

<span data-ttu-id="64784-186">この時点で、EWS を呼び出してメールボックスのデータにアクセスできるようにクライアントが設定されています。</span><span class="sxs-lookup"><span data-stu-id="64784-186">At this point, your client is set up to make calls to EWS to access mailbox data.</span></span> <span data-ttu-id="64784-187">コードを今すぐ実行する場合は、**ExchangeService.Url** プロパティの内容を調べて、 [AutodiscoverUrl](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) メソッド呼び出しが動作することを確認してください。</span><span class="sxs-lookup"><span data-stu-id="64784-187">If you run your code now, you can verify that the **AutodiscoverUrl** method call worked by examining the contents of the [ExchangeService.Url](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) property.</span></span> <span data-ttu-id="64784-188">このプロパティに URL が含まれる場合、呼び出しは正常に行われています。</span><span class="sxs-lookup"><span data-stu-id="64784-188">If this property contains a URL, your call was a success!</span></span> <span data-ttu-id="64784-189">これは、アプリケーションが正常にサービスで認証され、メールボックスの EWS エンドポイントを検出したことを意味します。</span><span class="sxs-lookup"><span data-stu-id="64784-189">This means that your application successfully authenticated with the service and discovered the EWS endpoint for your mailbox.</span></span> <span data-ttu-id="64784-190">これで、初めての EWS の呼び出しを行う準備が整いました。</span><span class="sxs-lookup"><span data-stu-id="64784-190">Now you are ready to make your first calls to EWS.</span></span> <span data-ttu-id="64784-191">EWS の URL を設定の詳細については[、EWS のマネージ API を使用して、EWS のサービスの URL の設定](how-to-set-the-ews-service-url-by-using-the-ews-managed-api.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="64784-191">Read [Set the EWS service URL by using the EWS Managed API](how-to-set-the-ews-service-url-by-using-the-ews-managed-api.md) for more information about setting the EWS URL.</span></span> 

### <a name="step-6-create-your-first-hello-world-email-message"></a><span data-ttu-id="64784-192">手順 6:初めての Hello World メール メッセージを作成する</span><span class="sxs-lookup"><span data-stu-id="64784-192">Step 6: Create your first Hello World email message</span></span>

1. <span data-ttu-id="64784-193">**AutodiscoverUrl** メソッド呼び出しの後に、新しい **EmailMessage** オブジェクトをインスタンス化し、作成したサービス オブジェクトに渡します。</span><span class="sxs-lookup"><span data-stu-id="64784-193">After the **AutodiscoverUrl** method call, instantiate a new **EmailMessage** object and pass in the service object you created.</span></span> 
    
   ```cs
    EmailMessage email = new EmailMessage(service);
   ```

   <span data-ttu-id="64784-p126">これで、サービス バインドが設定されているメール メッセージが作成されます。 **EmailMessage** オブジェクトで開始されるすべての呼び出しは、サービスの対象となります。</span><span class="sxs-lookup"><span data-stu-id="64784-p126">You now have an email message on which the service binding is set. Any calls initiated on the **EmailMessage** object will be targeted at the service.</span></span> 
    
2. <span data-ttu-id="64784-p127">次に、メール メッセージの宛先行の受信者を設定します。これを行うには、 `user1@contoso.com` を変更して SMTP アドレスを使用します。</span><span class="sxs-lookup"><span data-stu-id="64784-p127">Now set the To: line recipient of the email message. To do this, change  `user1@contoso.com` to use your SMTP address.</span></span> 
    
   ```cs
    email.ToRecipients.Add("user1@contoso.com");
   ```

3. <span data-ttu-id="64784-198">メール メッセージの件名および本文を設定します。</span><span class="sxs-lookup"><span data-stu-id="64784-198">Set the subject and the body of the email message.</span></span>
    
   ```cs
    email.Subject = "HelloWorld";
    email.Body = new MessageBody("This is the first email I've sent by using the EWS Managed API.");
   ```

4. <span data-ttu-id="64784-199">EWS マネージ API を使用して、最初のメール メッセージを送信する準備が整いました。</span><span class="sxs-lookup"><span data-stu-id="64784-199">You are now ready to send your first email message by using the EWS Managed API.</span></span> <span data-ttu-id="64784-200">**Send** メソッドは、サービスを呼び出し、配信用にメール メッセージを送信します。</span><span class="sxs-lookup"><span data-stu-id="64784-200">The **Send** method will call the service and submit the email message for delivery.</span></span> <span data-ttu-id="64784-201">Exchange との通信に使用することが他のメソッドの詳細については、 [EWS のマネージ API を使用して、EWS を使ってコミュニケーション](how-to-communicate-with-ews-by-using-the-ews-managed-api.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="64784-201">Read [Communicate with EWS by using the EWS Managed API](how-to-communicate-with-ews-by-using-the-ews-managed-api.md) to learn about other methods you can use to communicate with Exchange.</span></span> 
    
   ```cs
    email.Send();
   ```

5. <span data-ttu-id="64784-p129">Hello World アプリケーションを実行する準備が整いました。Visual Studio で、 **[F5]** を選択します。空のコンソール ウィンドウが開きます。アプリケーションが認証を行い、自動検出リダイレクトに従い、自分自身に送信するメール メッセージを作成するための最初の呼び出しを行っている間、コンソール ウィンドウには何も表示されません。実行されている呼び出しを表示する場合は、 **AutodiscoverUrl** メソッドが呼び出される前のところに次の 2 行のコードを追加します。F5 キーを押します。これで、コンソール ウィンドウに [EWS 要求と応答のトレースが出力されます](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md)。</span><span class="sxs-lookup"><span data-stu-id="64784-p129">You are ready to run your Hello World application. In Visual Studio, select **F5**. A blank console window will open. You will not see anything in the console window while your application authenticates, follows Autodiscover redirections, and then makes its first call to create an email message that you send to yourself. If you want to see the calls being made, add the following two lines of code before the **AutodiscoverUrl** method is called. Then press F5. This will [trace out the EWS requests and responses](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md) to the console window.</span></span> 
    
   ```cs
    service.TraceEnabled = true;
    service.TraceFlags = TraceFlags.All;
   ```

<span data-ttu-id="64784-p130">EWS マネージ API クライアント アプリケーションが作動するようになりました。利便性を考慮して、次の使用例では、Hello World アプリケーションを作成するために Program.cs に追加したすべてのコードを示します。</span><span class="sxs-lookup"><span data-stu-id="64784-p130">You now have a working EWS Managed API client application. For your convenience, the following example shows all the code that you added to Program.cs to create your Hello World application.</span></span>

```cs
using System;
using Microsoft.Exchange.WebServices.Data;
namespace HelloWorld
{
  class Program
  {
    static void Main(string[] args)
    {
      ExchangeService service = new ExchangeService(ExchangeVersion.Exchange2007_SP1);
      service.Credentials = new WebCredentials("user1@contoso.com", "password");
      service.TraceEnabled = true;
      service.TraceFlags = TraceFlags.All;
      service.AutodiscoverUrl("user1@contoso.com", RedirectionUrlValidationCallback);
      EmailMessage email = new EmailMessage(service);
      email.ToRecipients.Add("user1@contoso.com");
      email.Subject = "HelloWorld";
      email.Body = new MessageBody("This is the first email I've sent by using the EWS Managed API");
      email.Send();
    }
    private static bool RedirectionUrlValidationCallback(string redirectionUrl)
    {
      // The default for the validation callback is to reject the URL.
      bool result = false;
      Uri redirectionUri = new Uri(redirectionUrl);
      // Validate the contents of the redirection URL. In this simple validation
      // callback, the redirection URL is considered valid if it is using HTTPS
      // to encrypt the authentication credentials. 
      if (redirectionUri.Scheme == "https")
      {
        result = true;
      }
      return result;
    }
  }
}
```

## <a name="next-steps"></a><span data-ttu-id="64784-211">次の手順</span><span class="sxs-lookup"><span data-stu-id="64784-211">Next steps</span></span>
<span data-ttu-id="64784-212"><a name="Next"> </a></span><span class="sxs-lookup"><span data-stu-id="64784-212"></span></span>

<span data-ttu-id="64784-213">最初の EWS マネージ API クライアント アプリケーションでより多くの作業を行う準備ができている場合、次のリソースを参照します。</span><span class="sxs-lookup"><span data-stu-id="64784-213">If you're ready to do more with your first EWS Managed API client application, explore the following resources:</span></span>
  
- [<span data-ttu-id="64784-214">Exchange 2013:101 コード サンプル</span><span class="sxs-lookup"><span data-stu-id="64784-214">Exchange 2013: 101 code samples</span></span>](http://code.msdn.microsoft.com/exchange/Exchange-2013-101-Code-3c38582c)
    
- [<span data-ttu-id="64784-215">フォルダーとアイテム</span><span class="sxs-lookup"><span data-stu-id="64784-215">Folders and items</span></span>](folders-and-items-in-ews-in-exchange.md)
    
- [<span data-ttu-id="64784-216">EWSEditor</span><span class="sxs-lookup"><span data-stu-id="64784-216">EWSEditor</span></span>](http://ewseditor.codeplex.com/)
    
<span data-ttu-id="64784-217">カスタム アプリケーションで問題が発生したときには、[質問やコメントをフォーラムに投稿してみてください](http://social.technet.microsoft.com/Forums/exchange/en-US/home?forum=exchangesvrdevelopment) (最初の投稿は忘れずにお読みください)。</span><span class="sxs-lookup"><span data-stu-id="64784-217">If you run into any issues with your application, [try posting a question or comment in the forum](http://social.technet.microsoft.com/Forums/exchange/en-US/home?forum=exchangesvrdevelopment) (and don't forget to read the top post).</span></span> 
  
## <a name="in-this-section"></a><span data-ttu-id="64784-218">このセクションの内容</span><span class="sxs-lookup"><span data-stu-id="64784-218">In this section</span></span>
<span data-ttu-id="64784-219"><a name="Next"> </a></span><span class="sxs-lookup"><span data-stu-id="64784-219"></span></span>

- [<span data-ttu-id="64784-220">EWS のマネージ API のアセンブリを参照します。</span><span class="sxs-lookup"><span data-stu-id="64784-220">Reference the EWS Managed API assembly</span></span>](how-to-reference-the-ews-managed-api-assembly.md)
    
- [<span data-ttu-id="64784-221">EWS のマネージ API を使用して、EWS のサービスの URL を設定します。</span><span class="sxs-lookup"><span data-stu-id="64784-221">Set the EWS service URL by using the EWS Managed API</span></span>](how-to-set-the-ews-service-url-by-using-the-ews-managed-api.md)
    
- [<span data-ttu-id="64784-222">EWS のマネージ API を使用して通信 EWS</span><span class="sxs-lookup"><span data-stu-id="64784-222">Communicate with EWS by using the EWS Managed API</span></span>](how-to-communicate-with-ews-by-using-the-ews-managed-api.md)
    
## <a name="see-also"></a><span data-ttu-id="64784-223">関連項目</span><span class="sxs-lookup"><span data-stu-id="64784-223">See also</span></span>

- [<span data-ttu-id="64784-224">Exchange で Web サービスの使用を開始する</span><span class="sxs-lookup"><span data-stu-id="64784-224">Start using web services in Exchange</span></span>](start-using-web-services-in-exchange.md)    
- [<span data-ttu-id="64784-225">Exchange の EWS クライアントの設計の概要</span><span class="sxs-lookup"><span data-stu-id="64784-225">EWS client design overview for Exchange</span></span>](ews-client-design-overview-for-exchange.md)    
- [<span data-ttu-id="64784-226">Exchange の Web サービス クライアントを開発する</span><span class="sxs-lookup"><span data-stu-id="64784-226">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)   
- [<span data-ttu-id="64784-227">EWS のマネージ API アプリケーションのトラブルシューティングを行うには、要求と応答をトレースします。</span><span class="sxs-lookup"><span data-stu-id="64784-227">Trace requests and responses to troubleshoot EWS Managed API applications</span></span>](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md)
    

