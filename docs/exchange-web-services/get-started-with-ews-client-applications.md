---
title: EWS クライアント アプリケーションの概要
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.assetid: e6fd5c23-0ba5-4a7b-bdde-4a553447069f
description: Exchange Web サービス (EWS) を使用して、Exchange の初めてのアプリケーションを作成します。
localization_priority: Priority
ms.openlocfilehash: fd02c46777dabd04b492ba3c4420a0737640c5eb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528399"
---
# <a name="get-started-with-ews-client-applications"></a><span data-ttu-id="dc73a-103">EWS クライアント アプリケーションの概要</span><span class="sxs-lookup"><span data-stu-id="dc73a-103">Get started with EWS client applications</span></span>

<span data-ttu-id="dc73a-104">Exchange Web サービス (EWS) を使用して、Exchange の初めてのアプリケーションを作成します。</span><span class="sxs-lookup"><span data-stu-id="dc73a-104">Create your first application by using Exchange Web Services (EWS) in Exchange.</span></span>
  
<span data-ttu-id="dc73a-p101">EWS とは、包括的なサービスです。これを使用すると、カスタムのアプリケーションは Exchange Online、Office 365 の一部としての Exchange Online、または Exchange オンプレミスのメールボックスに保存されている情報のほとんどすべてにアクセスできるようになります。EWS は標準の Web プロトコルを使用して、Exchange サーバーへのアクセスを提供します。[EWS マネージ API](get-started-with-ews-managed-api-client-applications.md) などのライブラリは、EWS の操作をラップして、オブジェクト指向のインターフェイス提供します。この記事の例の実行を完了する頃には、EWS によって実行できることについて、基本的な知識が身についていることでしょう。</span><span class="sxs-lookup"><span data-stu-id="dc73a-p101">EWS is a comprehensive service that your applications can use to access almost all the information stored in an Exchange Online, Exchange Online as part of Office 365, or Exchange on-premises mailbox. EWS uses standard web protocols to provide access to an Exchange server; libraries like the [EWS Managed API](get-started-with-ews-managed-api-client-applications.md) wrap the EWS operations to provide an object-oriented interface. After you've run the examples in this article, you will have a basic understanding of what you can do with EWS.</span></span> 
  
<span data-ttu-id="dc73a-p102">EWS 操作は、あらゆるオペレーティング システムまたは言語から呼び出すことができます。これは、EWS の要求と応答には SOAP プロトコルが使用されているためです。この記事の例は C# で記述されていて, .NET Framework の [HttpWebRequest](https://msdn.microsoft.com/library/System.Net.HttpWebRequest.aspx) オブジェクトと [HttpWebResponse](https://msdn.microsoft.com/library/System.Net.HttpWebResponse.aspx) オブジェクトを使用していますが、コードで重要なのは、EWS 要求の作成に使用される XML と、サーバーから返された XML 応答の部分です。コード例では、XML の処理ではなく、XML トランザクションの部分を目立たせています。</span><span class="sxs-lookup"><span data-stu-id="dc73a-p102">You can call EWS operations from any operating system or language, because the EWS requests and responses use the SOAP protocol. The examples in this article are written using C# and make use of the .NET Framework [HttpWebRequest](https://msdn.microsoft.com/library/System.Net.HttpWebRequest.aspx) and [HttpWebResponse](https://msdn.microsoft.com/library/System.Net.HttpWebResponse.aspx) objects; however, the important part of the code is the XML used to make the EWS request and the XML response returned from the server. The code examples emphasize the XML transactions and not processing the XML.</span></span> 
  
## <a name="youll-need-an-exchange-server"></a><span data-ttu-id="dc73a-111">Exchange サーバーの準備</span><span class="sxs-lookup"><span data-stu-id="dc73a-111">You'll need an Exchange server</span></span>

<span data-ttu-id="dc73a-p103">Exchange メールボックス アカウントを既に所有している場合は、この手順を省略してもかまいません。それ以外の場合は、次のいずれかの方法で、初めての EWS アプリケーション用の Exchange メールボックスをセットアップします。</span><span class="sxs-lookup"><span data-stu-id="dc73a-p103">If you already have an Exchange mailbox account, you can skip this step. Otherwise, you have the following options for setting up an Exchange mailbox for your first EWS application:</span></span>
  
- <span data-ttu-id="dc73a-p104">[Office 365 の開発者向けサイトを取得する](https://msdn.microsoft.com/library/office/fp179924.aspx) (推奨)。最も簡単に Exchange メールボックスを入手する方法です。</span><span class="sxs-lookup"><span data-stu-id="dc73a-p104">[Get an Office 365 Developer Site ](https://msdn.microsoft.com/library/office/fp179924.aspx)(recommended). This is the quickest way for you to get an Exchange mailbox.</span></span>
    
- <span data-ttu-id="dc73a-116">[Exchange Server](https://office.microsoft.com/exchange/microsoft-exchange-try-or-buy-exchange-we-can-help-you-decide-FX103746846.aspx?WT%2Eintid1=ODC%5FENUS%5FFX103472230%5FXT103965589) をダウンロードする。</span><span class="sxs-lookup"><span data-stu-id="dc73a-116">Download [Exchange Server](https://office.microsoft.com/exchange/microsoft-exchange-try-or-buy-exchange-we-can-help-you-decide-FX103746846.aspx?WT%2Eintid1=ODC%5FENUS%5FFX103472230%5FXT103965589).</span></span>

    
<span data-ttu-id="dc73a-p105">Exchange サーバーから電子メールを送受信できることを確認したら、開発環境をセットアップするための準備が完了します。Outlook Web App を使用して、電子メールが送信できることを確認します。</span><span class="sxs-lookup"><span data-stu-id="dc73a-p105">After you've verified that you can send and receive email from your Exchange server you are ready to set up your development environment. You can use Outlook Web App to verify that you can send email.</span></span>
  
<span data-ttu-id="dc73a-p106">また、サーバーの EWS エンドポイントの URL を確認することも必要になります。実稼働アプリケーションでは、[自動検出](autodiscover-for-exchange.md)を使用して EWS の URL を判断します。この記事の例では、Office 365 EWS エンドポイント の URL `https://outlook.office365.com/EWS/Exchange.asmx` を使用します。「[次の手順](#bk_next)」のセクションには、自動検出に関する詳細へのリンクが掲載されています (必要になったら参照してください)。</span><span class="sxs-lookup"><span data-stu-id="dc73a-p106">You'll also need to know the URL of the EWS endpoint for your server. In a production application, you'd use [Autodiscover](autodiscover-for-exchange.md) to determine the EWS URL. The examples in this article use the Office 365 EWS endpoint URL, `https://outlook.office365.com/EWS/Exchange.asmx`. The [Next steps](#bk_next) section has links to more information about Autodiscover when you're ready.</span></span> 
  
<span data-ttu-id="dc73a-123">アプリケーションのテストに、既定の自己署名証明書がある Exchange サーバーを使用する場合は、自分の組織のセキュリティ要件に適合する[証明書の検証メソッド](how-to-validate-a-server-certificate-for-the-ews-managed-api.md)を作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="dc73a-123">If you are testing your application using an Exchange server that has the default self-signed certificate, you'll need to create a [certificate validation method](how-to-validate-a-server-certificate-for-the-ews-managed-api.md) that meets the security requirements of your organization.</span></span> 
  
## <a name="set-up-your-development-environment"></a><span data-ttu-id="dc73a-124">開発環境のセットアップ</span><span class="sxs-lookup"><span data-stu-id="dc73a-124">Set up your development environment</span></span>

<span data-ttu-id="dc73a-p107">初めての EWS アプリケーションの作成に使用するツールは、どのオペレーティング システムと言語を使用するかによって決まりますが、大部分は好みの問題になります。この記事の C# の例に沿って進めようとしている場合は、次のものが必要になります。</span><span class="sxs-lookup"><span data-stu-id="dc73a-p107">The tools that you use to create your first EWS application depend on the operating system and language that you use, and are mostly a matter of taste. If you want to follow along with the C# examples in this article, you'll need:</span></span> 
  
- <span data-ttu-id="dc73a-127">.NET Framework 4.0 をサポートしているバージョンの Visual Studio。</span><span class="sxs-lookup"><span data-stu-id="dc73a-127">Any version of Visual Studio that supports the .NET Framework 4.0.</span></span> 
    
- <span data-ttu-id="dc73a-p108">開発マシンから Exchange サーバーへの接続に使用できるインターネット接続。IP アドレスではなく DNS 名で Exchange サーバーに接続する Outlook Web App を使用できる場合は、セットアップが完了しています。</span><span class="sxs-lookup"><span data-stu-id="dc73a-p108">An Internet connection that your development machine can use to contact your Exchange server. If you can use Outlook Web App with a DNS name rather than an IP address to connect to your Exchange server, you are set up.</span></span>
    
## <a name="create-your-first-ews-application"></a><span data-ttu-id="dc73a-130">初めての EWS アプリケーションの作成</span><span class="sxs-lookup"><span data-stu-id="dc73a-130">Create your first EWS application</span></span>

<span data-ttu-id="dc73a-131">これから作成する EWS アプリケーションでは、EWS を使用する際の一般的な 2 つのシナリオについて示します。</span><span class="sxs-lookup"><span data-stu-id="dc73a-131">The EWS application that you will create shows two typical scenarios for using EWS:</span></span>
  
1. <span data-ttu-id="dc73a-132">Exchange メールボックスから情報を取得して、その情報をユーザーに表示する。</span><span class="sxs-lookup"><span data-stu-id="dc73a-132">Get information from an Exchange mailbox and display that information to the user.</span></span>
    
2. <span data-ttu-id="dc73a-133">電子メールの送信などのアクションを実行して、そのアクションが成功したかどうかを確認するために応答を調べる。</span><span class="sxs-lookup"><span data-stu-id="dc73a-133">Perform an action, such as sending an email, and check the response to see if the action succeeded.</span></span>
    
<span data-ttu-id="dc73a-134">それでは始めましょう。</span><span class="sxs-lookup"><span data-stu-id="dc73a-134">Let's get started.</span></span>
  
### <a name="set-up-the-solution"></a><span data-ttu-id="dc73a-135">ソリューションのセットアップ</span><span class="sxs-lookup"><span data-stu-id="dc73a-135">Set up the solution</span></span>

<span data-ttu-id="dc73a-p109">まず、Visual Studio を使用して、新しいコンソール アプリケーション ソリューションを作成します。ソリューションの準備ができたら、Tracing.cs という名前の新しいオブジェクトを作成します。このオブジェクトを使用して、コンソールとログ ファイルの両方に情報を書き込み、コードの実行後に結果を確認できるようにします。Tracing.cs ファイルに、次のコードを貼り付けます。</span><span class="sxs-lookup"><span data-stu-id="dc73a-p109">First, create a new console application solution using Visual Studio. When the solution is ready, create a new object called Tracing.cs. Use this object to write information to both the console and a log file so that you can review the results after you run your code. Paste the following code into the Tracing.cs file.</span></span>
  
```cs
using System;
using System.IO;
namespace Microsoft.Exchange.Samples.EWS
{
  class Tracing
  {
    private static TextWriter logFileWriter = null;
    public static void OpenLog(string fileName)
    {
      logFileWriter = new StreamWriter(fileName);
    }
    public static void Write(string format, params object[] args)
    {
      Console.Write(format, args);
      if (logFileWriter != null)
      {
        logFileWriter.Write(format, args);
      }
    }
    public static void WriteLine(string format, params object[] args)
    {
      Console.WriteLine(format, args);
      if (logFileWriter != null)
      {
        logFileWriter.WriteLine(format, args);
      }
    }
    public static void CloseLog()
    {
      logFileWriter.Flush();
      logFileWriter.Close();
    }
  }
}
```

<span data-ttu-id="dc73a-p110">次に、Program.cs ファイルを開きます。この例のコードの残りの部分は、このファイルに記述することになります。</span><span class="sxs-lookup"><span data-stu-id="dc73a-p110">Next, open the Program.cs file. You will put the rest of the code for the example in this file.</span></span>
  
<span data-ttu-id="dc73a-p111">まず、プログラムの外郭をセットアップします。プログラムでは、次を実行します。</span><span class="sxs-lookup"><span data-stu-id="dc73a-p111">First, set up the shell of the program. The program will:</span></span> 
  
1. <span data-ttu-id="dc73a-144">ログ ファイルを作成して、後からの調査のために要求と応答をディスクに書き込めるようにします。</span><span class="sxs-lookup"><span data-stu-id="dc73a-144">Create a log file so that the request and response can be written to disk for later study.</span></span>
    
2. <span data-ttu-id="dc73a-145">アクセスするアカウントの電子メール アドレスとパスワードを取得します。</span><span class="sxs-lookup"><span data-stu-id="dc73a-145">Get the email address and password of the account that you'll access.</span></span>
    
3. <span data-ttu-id="dc73a-146">簡単なメソッドを呼び出します。</span><span class="sxs-lookup"><span data-stu-id="dc73a-146">Call the sample methods.</span></span>
    
<span data-ttu-id="dc73a-147">Program.cs の  `Main` メソッドを次のコードに置き換えます。</span><span class="sxs-lookup"><span data-stu-id="dc73a-147">Replace the  `Main` method in the Program.cs with the following code.</span></span> 
  
```cs
    static void Main(string[] args)
    {
      // Start tracing to console and a log file.
      Tracing.OpenLog("./GetStartedWithEWS.log");
      Tracing.WriteLine("EWS sample application started.");
      var isValidEmailAddress = false;
      Console.Write("Enter an email address: ");
      var emailAddress = Console.ReadLine();
      
        isValidEmailAddress = (emailAddress.Contains("@") &amp;&amp; emailAddress.Contains("."));
      if (!isValidEmailAddress)
      {
        Tracing.WriteLine("Email address " + emailAddress + " is not a valid SMTP address. Closing program.");
        return;
      }
      SecureString password = GetPasswordFromConsole();
      if (password.Length == 0)
      {
        Tracing.WriteLine("Password empty, closing program.");
      }
      NetworkCredential userCredentials = new NetworkCredential(emailAddress, password);
      // These are the sample methods that demonstrate using EWS.
      // ShowNumberOfMessagesInInbox(userCredentials);
      // SendTestEmail(userCredentials);
     
      Tracing.WriteLine("EWS sample application ends.");
      Tracing.CloseLog();
      Console.WriteLine("Press enter to exit: ");
      Console.ReadLine();
    }
    // These method stubs will be filled in later.
    private static void ShowNumberOfMessagesInInbox(NetworkCredential userCredentials)
    {
    }
    private static void SendTestEmail(NetworkCredential userCredentials)
    {
    }
```

<span data-ttu-id="dc73a-p112">最後にもう 1 つ必要なことがあります。 `GetPasswordFromConsole` 静的メソッドの追加です。このメソッドは、コンソールで入力したパスワードを格納する [SecureString](https://msdn.microsoft.com/library/System.Security.SecureString.aspx) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="dc73a-p112">The last thing that you need to do is add the  `GetPasswordFromConsole` static method. This method returns a [SecureString](https://msdn.microsoft.com/library/System.Security.SecureString.aspx) object that contains a password typed at the console.</span></span> 
  
```cs
    private static SecureString GetPasswordFromConsole()
    {
      SecureString password = new SecureString();
      bool readingPassword = true;
      Console.Write("Enter password: ");
      while (readingPassword)
      {
        ConsoleKeyInfo userInput = Console.ReadKey(true);
        switch (userInput.Key)
        {
          case (ConsoleKey.Enter):
            readingPassword = false;
            break;
          case (ConsoleKey.Escape):
            password.Clear();
            readingPassword = false;
            break;
          case (ConsoleKey.Backspace):
            if (password.Length > 0)
            {
              password.RemoveAt(password.Length - 1);
              Console.SetCursorPosition(Console.CursorLeft - 1, Console.CursorTop);
              Console.Write(" ");
              Console.SetCursorPosition(Console.CursorLeft - 1, Console.CursorTop);
            }
            break;
          default:
            if (userInput.KeyChar != 0)
            {
              password.AppendChar(userInput.KeyChar);
              Console.Write("*");
            }
            break;
        }
      }
      Console.WriteLine();
      password.MakeReadOnly();
      return password;
    }
```

### <a name="get-the-number-of-new-messages-in-an-inbox"></a><span data-ttu-id="dc73a-150">受信トレイにある新しいメッセージ数の取得</span><span class="sxs-lookup"><span data-stu-id="dc73a-150">Get the number of new messages in an Inbox</span></span>

<span data-ttu-id="dc73a-p113">EWS アプリケーションの一般的な操作とは、電子メール メッセージ、予定、会議、およびそれらを格納するフォルダーに関する情報を取得することです。この例では、アカウントの受信トレイ内にあるメッセージ数を取得して、合計メッセージ数と未読メッセージ数を表示します。ここでは、EWS アプリケーションにとって一般的な次のアクションについて示します</span><span class="sxs-lookup"><span data-stu-id="dc73a-p113">A common operation in an EWS application is to get information about email messages, appointments, meetings, and the folders that store them. This example gets the number of messages in an account's Inbox and displays the total number of messages and the number of unread messages. It demonstrates the following common actions for EWS applications:</span></span>
  
- <span data-ttu-id="dc73a-154">Exchange サーバーへの EWS の要求。</span><span class="sxs-lookup"><span data-stu-id="dc73a-154">Making an EWS request to the Exchange server.</span></span>
    
- <span data-ttu-id="dc73a-155">要求した情報に対して返される XML 応答の解析。</span><span class="sxs-lookup"><span data-stu-id="dc73a-155">Parsing the returned XML response for the requested information.</span></span>
    
- <span data-ttu-id="dc73a-156">一般的な例外とエラー メッセージの処理。</span><span class="sxs-lookup"><span data-stu-id="dc73a-156">Handling common exceptions and error messages.</span></span>
    
<span data-ttu-id="dc73a-p114">main メソッドの後でスタブ アウトされていた  `ShowNumberOfMessagesInInbox` メソッドに、次のコードを追加します。アプリケーションを実行すると、アカウントの受信トレイ内にあるメッセージの数と、受信トレイ内で未読のメッセージ数が出力されます。アプリケーションの実行後に、GetStartedWithEWS.log ファイルを開くと、Exchange サーバーに送信された XML 要求と、サーバーから返された応答を確認できます</span><span class="sxs-lookup"><span data-stu-id="dc73a-p114">Add the following code to the  `ShowNumberOfMessagesInInbox` method that was stubbed out after the main method. When you run the application, it will print the number of messages in the account's Inbox and the number of unread messages in the Inbox. After you run the application, you can open the GetStartedWithEWS.log file to see the XML request that was sent to the Exchange server and the response that the server returned.</span></span> 
  
```cs
      /// This is the XML request that is sent to the Exchange server.
      var getFolderSOAPRequest =
"<?xml version=\"1.0\" encoding=\"utf-8\"?>\n" +
"<soap:Envelope xmlns:soap=\"https://schemas.xmlsoap.org/soap/envelope/\"\n" +
"   xmlns:t=\"https://schemas.microsoft.com/exchange/services/2006/types\">\n" +
"<soap:Header>\n" +
"    <t:RequestServerVersion Version=\"Exchange2007_SP1\" />\n" +
"  </soap:Header>\n" +
"  <soap:Body>\n" +
"    <GetFolder xmlns=\"https://schemas.microsoft.com/exchange/services/2006/messages\"\n" +
"               xmlns:t=\"https://schemas.microsoft.com/exchange/services/2006/types\">\n" +
"      <FolderShape>\n" +
"        <t:BaseShape>Default</t:BaseShape>\n" +
"      </FolderShape>\n" +
"      <FolderIds>\n" +
"        <t:DistinguishedFolderId Id=\"inbox\"/>\n" +
"      </FolderIds>\n" +
"    </GetFolder>\n" +
"  </soap:Body>\n" +
"</soap:Envelope>\n";
      // Write the get folder operation request to the console and log file.
      Tracing.WriteLine("Get folder operation request:");
      Tracing.WriteLine(getFolderSOAPRequest);
      var getFolderRequest = WebRequest.CreateHttp(Office365WebServicesURL);
      getFolderRequest.AllowAutoRedirect = false;
      getFolderRequest.Credentials = userCredentials;
      getFolderRequest.Method = "POST";
      getFolderRequest.ContentType = "text/xml";
      var requestWriter = new StreamWriter(getFolderRequest.GetRequestStream());
      requestWriter.Write(getFolderSOAPRequest);
      requestWriter.Close();
      try
      {
        var getFolderResponse = (HttpWebResponse)(getFolderRequest.GetResponse());
        if (getFolderResponse.StatusCode == HttpStatusCode.OK)
        {
          var responseStream = getFolderResponse.GetResponseStream();
          XElement responseEnvelope = XElement.Load(responseStream);
          if (responseEnvelope != null)
          {
            // Write the response to the console and log file.
            Tracing.WriteLine("Response:");
            StringBuilder stringBuilder = new StringBuilder();
            XmlWriterSettings settings = new XmlWriterSettings();
            settings.Indent = true;
            XmlWriter writer = XmlWriter.Create(stringBuilder, settings);
            responseEnvelope.Save(writer);
            writer.Close();
            Tracing.WriteLine(stringBuilder.ToString());
            // Check the response for error codes. If there is an error, throw an application exception.
            IEnumerable<XElement> errorCodes = from errorCode in responseEnvelope.Descendants
                                               ("{https://schemas.microsoft.com/exchange/services/2006/messages}ResponseCode")
                                               select errorCode;
            foreach (var errorCode in errorCodes)
            {
              if (errorCode.Value != "NoError")
              {
                switch (errorCode.Parent.Name.LocalName.ToString())
                {
                  case "Response":
                    string responseError = "Response-level error getting inbox information:\n" + errorCode.Value;
                    throw new ApplicationException(responseError);
                  case "UserResponse":
                    string userError = "User-level error getting inbox information:\n" + errorCode.Value;
                    throw new ApplicationException(userError);
                }
              }
            }
            // Process the response.
            IEnumerable<XElement> folders = from folderElement in
                                              responseEnvelope.Descendants
                                              ("{https://schemas.microsoft.com/exchange/services/2006/messages}Folders")
                                            select folderElement;
            foreach (var folder in folders)
            {
              Tracing.Write("Folder name:     ");
              var folderName = from folderElement in
                                 folder.Descendants
                                 ("{https://schemas.microsoft.com/exchange/services/2006/types}DisplayName")
                               select folderElement.Value;
              Tracing.WriteLine(folderName.ElementAt(0));
              Tracing.Write("Total messages:  ");
              var totalCount = from folderElement in
                                 folder.Descendants
                                   ("{https://schemas.microsoft.com/exchange/services/2006/types}TotalCount")
                               select folderElement.Value;
              Tracing.WriteLine(totalCount.ElementAt(0));
              Tracing.Write("Unread messages: ");
              var unreadCount = from folderElement in
                                 folder.Descendants
                                   ("{https://schemas.microsoft.com/exchange/services/2006/types}UnreadCount")
                               select folderElement.Value;
              Tracing.WriteLine(unreadCount.ElementAt(0));
            }
          }
        }
      }
      catch (WebException ex)
      {
        Tracing.WriteLine("Caught Web exception:");
        Tracing.WriteLine(ex.Message);
      }
      catch (ApplicationException ex)
      {
        Tracing.WriteLine("Caught application exception:");
        Tracing.WriteLine(ex.Message);
      }

```

### <a name="send-an-email-message"></a><span data-ttu-id="dc73a-160">電子メール メッセージの送信</span><span class="sxs-lookup"><span data-stu-id="dc73a-160">Send an email message</span></span>

<span data-ttu-id="dc73a-p115">もう 1 つの EWS アプリケーションの一般的な操作は、電子メール メッセージや会議出席依頼の送信です。この例では、電子メール メッセージを作成して、以前に入力されたユーザーの資格情報を使用して送信します。ここでは、一般的な EWS アプリケーションの 3 つのタスクを例示しています。</span><span class="sxs-lookup"><span data-stu-id="dc73a-p115">Another common operation for an EWS application is to send email messages or meeting requests. This example creates and sends an email message using the user credentials that were entered earlier. It demonstrates these common EWS application tasks:</span></span>
  
- <span data-ttu-id="dc73a-164">電子メールの作成と送信。</span><span class="sxs-lookup"><span data-stu-id="dc73a-164">Creating and sending an email.</span></span>
    
- <span data-ttu-id="dc73a-165">返された XML 応答の解析 (電子メールが正しく送信されたかどうかを判断します)。</span><span class="sxs-lookup"><span data-stu-id="dc73a-165">Parsing the returned XML response to determine if the email was correctly sent.</span></span>
    
- <span data-ttu-id="dc73a-166">一般的な例外とエラー メッセージの処理。</span><span class="sxs-lookup"><span data-stu-id="dc73a-166">Handling common exceptions and error messages.</span></span>
    
<span data-ttu-id="dc73a-p116">main メソッドの後でスタブアウトされていた SendTestEmail メソッドに、次のコードを追加します。アプリケーションの実行後に、GetStartedWithEWS.log ファイルを開くと、Exchange サーバーに送信された XML 要求と、サーバーから返された応答を確認できます</span><span class="sxs-lookup"><span data-stu-id="dc73a-p116">Add the following code to the SendTestEmail method that was stubbed out after the main method. After you run the application, you can open the GetStartedWithEWS.log file to see the XML request that was sent to the Exchange server and the response that the server returned.</span></span>
  
```cs
var createItemSOAPRequest =
      "<?xml version=\"1.0\" encoding=\"utf-8\"?>\n" +
      "<soap:Envelope xmlns:xsi=\"http://www.w3.org/2001/XMLSchema-instance\" \n" +
      "               xmlns:m=\"https://schemas.microsoft.com/exchange/services/2006/messages\" \n" +
      "               xmlns:t=\"https://schemas.microsoft.com/exchange/services/2006/types\" \n" +
      "               xmlns:soap=\"https://schemas.xmlsoap.org/soap/envelope/\">\n" +
      "  <soap:Header>\n" +
      "    <t:RequestServerVersion Version=\"Exchange2007_SP1\" />\n" +
      "  </soap:Header>\n" +
      "  <soap:Body>\n" +
      "    <m:CreateItem MessageDisposition=\"SendAndSaveCopy\">\n" +
      "      <m:SavedItemFolderId>\n" +
      "        <t:DistinguishedFolderId Id=\"sentitems\" />\n" +
      "      </m:SavedItemFolderId>\n" +
      "      <m:Items>\n" +
      "        <t:Message>\n" +
      "          <t:Subject>Company Soccer Team</t:Subject>\n" +
      "          <t:Body BodyType=\"HTML\">Are you interested in joining?</t:Body>\n" +
      "          <t:ToRecipients>\n" +
      "            <t:Mailbox>\n" +
      "              <t:EmailAddress>sadie@contoso.com</t:EmailAddress>\n" +
      "              </t:Mailbox>\n" +
      "          </t:ToRecipients>\n" +
      "        </t:Message>\n" +
      "      </m:Items>\n" +
      "    </m:CreateItem>\n" +
      "  </soap:Body>\n" +
      "</soap:Envelope>\n";
      // Write the create item operation request to the console and log file.
      Tracing.WriteLine("Get folder operation request:");
      Tracing.WriteLine(createItemSOAPRequest);
      var getFolderRequest = WebRequest.CreateHttp(Office365WebServicesURL);
      getFolderRequest.AllowAutoRedirect = false;
      getFolderRequest.Credentials = userCredentials;
      getFolderRequest.Method = "POST";
      getFolderRequest.ContentType = "text/xml";
      var requestWriter = new StreamWriter(getFolderRequest.GetRequestStream());
      requestWriter.Write(createItemSOAPRequest);
      requestWriter.Close();
      try
      {
        var getFolderResponse = (HttpWebResponse)(getFolderRequest.GetResponse());
        if (getFolderResponse.StatusCode == HttpStatusCode.OK)
        {
          var responseStream = getFolderResponse.GetResponseStream();
          XElement responseEnvelope = XElement.Load(responseStream);
          if (responseEnvelope != null)
          {
            // Write the response to the console and log file.
            Tracing.WriteLine("Response:");
            StringBuilder stringBuilder = new StringBuilder();
            XmlWriterSettings settings = new XmlWriterSettings();
            settings.Indent = true;
            XmlWriter writer = XmlWriter.Create(stringBuilder, settings);
            responseEnvelope.Save(writer);
            writer.Close();
            Tracing.WriteLine(stringBuilder.ToString());
            // Check the response for error codes. If there is an error, throw an application exception.
            IEnumerable<XElement> errorCodes = from errorCode in responseEnvelope.Descendants
                                               ("{https://schemas.microsoft.com/exchange/services/2006/messages}ResponseCode")
                                               select errorCode;
            foreach (var errorCode in errorCodes)
            {
              if (errorCode.Value != "NoError")
              {
                switch (errorCode.Parent.Name.LocalName.ToString())
                {
                  case "Response":
                    string responseError = "Response-level error getting inbox information:\n" + errorCode.Value;
                    throw new ApplicationException(responseError);
                  case "UserResponse":
                    string userError = "User-level error getting inbox information:\n" + errorCode.Value;
                    throw new ApplicationException(userError);
                }
              }
            }
            Tracing.WriteLine("Message sent successfully.");
          }
        }
      }
      catch (WebException ex)
      {
        Tracing.WriteLine("Caught Web exception:");
        Tracing.WriteLine(ex.Message);
      }
      catch (ApplicationException ex)
      {
        Tracing.WriteLine("Caught application exception:");
        Tracing.WriteLine(ex.Message);
      }
```

<a name="bk_next"></a>

## <a name="next-steps"></a><span data-ttu-id="dc73a-169">次の手順</span><span class="sxs-lookup"><span data-stu-id="dc73a-169">Next steps</span></span>

<span data-ttu-id="dc73a-p117">初めての EWS アプリケーションの作成は完了しました。ここからは、EWS を使用する別の方法について見つけましょう。次に、入門編としてのアイデアをいくつか示します。</span><span class="sxs-lookup"><span data-stu-id="dc73a-p117">Now that you've written your first EWS application, you're ready to discover other ways to use EWS. Here are some ideas to get you started:</span></span>
  
- <span data-ttu-id="dc73a-p118">ユーザーの電子メール アドレスに応じて適切な Exchange サーバーに接続するように、アプリケーションに[自動検出](autodiscover-for-exchange.md)を実装する。「[Exchange 2013: Get user settings with Autodiscover](https://code.msdn.microsoft.com/Exchange-2013-Get-user-7e22c86e)」サンプルも参照してください。</span><span class="sxs-lookup"><span data-stu-id="dc73a-p118">Implement [Autodiscover](autodiscover-for-exchange.md) in your application so that your application will connect to the correct Exchange server based on the user's email address. See also the [Exchange 2013: Get user settings with Autodiscover](https://code.msdn.microsoft.com/Exchange-2013-Get-user-7e22c86e) sample.</span></span> 
    
- <span data-ttu-id="dc73a-174">EWS の詳細について、[EWS のリファレンス](https://msdn.microsoft.com/library/2a873474-1bb2-4cb1-a556-40e8c4159f4a%28Office.15%29.aspx)で調べる。</span><span class="sxs-lookup"><span data-stu-id="dc73a-174">Look at the [EWS reference](https://msdn.microsoft.com/library/2a873474-1bb2-4cb1-a556-40e8c4159f4a%28Office.15%29.aspx) for more information about EWS.</span></span> 
    
- <span data-ttu-id="dc73a-175">使用可能な操作について、[EWS の操作](https://msdn.microsoft.com/library/cf6fd871-9a65-4f34-8557-c8c71dd7ce09%28Office.15%29.aspx)で確認する。</span><span class="sxs-lookup"><span data-stu-id="dc73a-175">See the [EWS operations](https://msdn.microsoft.com/library/cf6fd871-9a65-4f34-8557-c8c71dd7ce09%28Office.15%29.aspx) for information about the operations that are available.</span></span> 
    
- <span data-ttu-id="dc73a-176">[EWS エディタ](http://ewseditor.codeplex.com/)を使用して、サーバーとやり取りされる SOAP トラフィックを確認する。</span><span class="sxs-lookup"><span data-stu-id="dc73a-176">Use [EWS Editor](http://ewseditor.codeplex.com/) to see the SOAP traffic sent to and from the server.</span></span> 
    
<span data-ttu-id="dc73a-177">カスタムアプリケーションに問題が発生したときには、[質問やコメントをフォーラムに投稿してみてください](https://social.technet.microsoft.com/Forums/exchange/home?forum=exchangesvrdevelopment) (最初の投稿は忘れずにお読みください)。</span><span class="sxs-lookup"><span data-stu-id="dc73a-177">If you run into any issues with your application, [try posting a question or comment in the forum](https://social.technet.microsoft.com/Forums/exchange/home?forum=exchangesvrdevelopment) (and don't forget to read the first post).</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="dc73a-178">関連項目</span><span class="sxs-lookup"><span data-stu-id="dc73a-178">See also</span></span>

- [<span data-ttu-id="dc73a-179">Exchange で Web サービスの使用を開始する</span><span class="sxs-lookup"><span data-stu-id="dc73a-179">Start using web services in Exchange</span></span>](start-using-web-services-in-exchange.md)   
- [<span data-ttu-id="dc73a-180">Exchange の EWS マネージ API、EWS、Web サービスについて探究してみましょう</span><span class="sxs-lookup"><span data-stu-id="dc73a-180">Explore the EWS Managed API, EWS, and web services in Exchange</span></span>](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) 
- [<span data-ttu-id="dc73a-181">Exchange の EWS クライアントの設計の概要</span><span class="sxs-lookup"><span data-stu-id="dc73a-181">EWS client design overview for Exchange</span></span>](ews-client-design-overview-for-exchange.md)   
- [<span data-ttu-id="dc73a-182">Exchange の Web サービス クライアントを開発する</span><span class="sxs-lookup"><span data-stu-id="dc73a-182">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)  
- [<span data-ttu-id="dc73a-183">EWS マネージ API クライアント アプリケーションの概要</span><span class="sxs-lookup"><span data-stu-id="dc73a-183">Get started with EWS Managed API client applications</span></span>](get-started-with-ews-managed-api-client-applications.md)
    