---
title: EWS クライアント アプリケーションの概要
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: e6fd5c23-0ba5-4a7b-bdde-4a553447069f
description: Exchange Web サービス (EWS) を使用して、Exchange の初めてのアプリケーションを作成します。
ms.openlocfilehash: 06606bdc2b37c8bf65b8b10dc7a516bdc911b256
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353778"
---
# <a name="get-started-with-ews-client-applications"></a>EWS クライアント アプリケーションの概要

Exchange Web サービス (EWS) を使用して、Exchange の初めてのアプリケーションを作成します。
  
EWS とは、包括的なサービスです。これを使用すると、カスタムのアプリケーションは Exchange Online、Office 365 の一部としての Exchange Online、または Exchange オンプレミスのメールボックスに保存されている情報のほとんどすべてにアクセスできるようになります。EWS は標準の Web プロトコルを使用して、Exchange サーバーへのアクセスを提供します。[EWS マネージ API](get-started-with-ews-managed-api-client-applications.md) などのライブラリは、EWS の操作をラップして、オブジェクト指向のインターフェイス提供します。この記事の例の実行を完了する頃には、EWS によって実行できることについて、基本的な知識が身についていることでしょう。 
  
EWS 操作は、あらゆるオペレーティング システムまたは言語から呼び出すことができます。これは、EWS の要求と応答には SOAP プロトコルが使用されているためです。この記事の例は C# で記述されていて, .NET Framework の [HttpWebRequest](https://msdn.microsoft.com/library/System.Net.HttpWebRequest.aspx) オブジェクトと [HttpWebResponse](https://msdn.microsoft.com/library/System.Net.HttpWebResponse.aspx) オブジェクトを使用していますが、コードで重要なのは、EWS 要求の作成に使用される XML と、サーバーから返された XML 応答の部分です。コード例では、XML の処理ではなく、XML トランザクションの部分を目立たせています。 
  
## <a name="youll-need-an-exchange-server"></a>Exchange サーバーの準備

Exchange メールボックス アカウントを既に所有している場合は、この手順を省略してもかまいません。それ以外の場合は、次のいずれかの方法で、初めての EWS アプリケーション用の Exchange メールボックスをセットアップします。
  
- [Office 365 の開発者向けサイトを取得する](http://msdn.microsoft.com/ja-JP/library/office/fp179924.aspx) (推奨)。最も簡単に Exchange メールボックスを入手する方法です。
    
- [Exchange Server](http://office.microsoft.com/en-us/exchange/microsoft-exchange-try-or-buy-exchange-we-can-help-you-decide-FX103746846.aspx?WT%2Eintid1=ODC%5FENUS%5FFX103472230%5FXT103965589) をダウンロードする。
    
Exchange サーバーから電子メールを送受信できることを確認したら、開発環境をセットアップするための準備が完了します。Outlook Web App を使用して、電子メールが送信できることを確認します。
  
また、サーバーの EWS エンドポイントの URL を確認することも必要になります。実稼働アプリケーションでは、[自動検出](autodiscover-for-exchange.md)を使用して EWS の URL を判断します。この記事の例では、Office 365 EWS エンドポイント の URL `https://outlook.office365.com/EWS/Exchange.asmx` を使用します。「[次の手順](#bk_next)」のセクションには、自動検出に関する詳細へのリンクが掲載されています (必要になったら参照してください)。 
  
アプリケーションのテストに、既定の自己署名証明書がある Exchange サーバーを使用する場合は、自分の組織のセキュリティ要件に適合する[証明書の検証メソッド](how-to-validate-a-server-certificate-for-the-ews-managed-api.md)を作成する必要があります。 
  
## <a name="set-up-your-development-environment"></a>開発環境のセットアップ

初めての EWS アプリケーションの作成に使用するツールは、どのオペレーティング システムと言語を使用するかによって決まりますが、大部分は好みの問題になります。この記事の C# の例に沿って進めようとしている場合は、次のものが必要になります。 
  
- .NET Framework 4.0 をサポートしているバージョンの Visual Studio。 
    
- 開発マシンから Exchange サーバーへの接続に使用できるインターネット接続。IP アドレスではなく DNS 名で Exchange サーバーに接続する Outlook Web App を使用できる場合は、セットアップが完了しています。
    
## <a name="create-your-first-ews-application"></a>初めての EWS アプリケーションの作成

これから作成する EWS アプリケーションでは、EWS を使用する際の一般的な 2 つのシナリオについて示します。
  
1. Exchange メールボックスから情報を取得して、その情報をユーザーに表示する。
    
2. 電子メールの送信などのアクションを実行して、そのアクションが成功したかどうかを確認するために応答を調べる。
    
それでは始めましょう。
  
### <a name="set-up-the-solution"></a>ソリューションのセットアップ

まず、Visual Studio を使用して、新しいコンソール アプリケーション ソリューションを作成します。ソリューションの準備ができたら、Tracing.cs という名前の新しいオブジェクトを作成します。このオブジェクトを使用して、コンソールとログ ファイルの両方に情報を書き込み、コードの実行後に結果を確認できるようにします。Tracing.cs ファイルに、次のコードを貼り付けます。
  
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

次に、Program.cs ファイルを開きます。この例のコードの残りの部分は、このファイルに記述することになります。
  
まず、プログラムの外郭をセットアップします。プログラムでは、次を実行します。 
  
1. ログ ファイルを作成して、後からの調査のために要求と応答をディスクに書き込めるようにします。
    
2. アクセスするアカウントの電子メール アドレスとパスワードを取得します。
    
3. 簡単なメソッドを呼び出します。
    
Program.cs の  `Main` メソッドを次のコードに置き換えます。 
  
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

最後にもう 1 つ必要なことがあります。 `GetPasswordFromConsole` 静的メソッドの追加です。このメソッドは、コンソールで入力したパスワードを格納する [SecureString](https://msdn.microsoft.com/library/System.Security.SecureString.aspx) オブジェクトを返します。 
  
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

### <a name="get-the-number-of-new-messages-in-an-inbox"></a>受信トレイにある新しいメッセージ数の取得

EWS アプリケーションの一般的な操作とは、電子メール メッセージ、予定、会議、およびそれらを格納するフォルダーに関する情報を取得することです。この例では、アカウントの受信トレイ内にあるメッセージ数を取得して、合計メッセージ数と未読メッセージ数を表示します。ここでは、EWS アプリケーションにとって一般的な次のアクションについて示します
  
- Exchange サーバーへの EWS の要求。
    
- 要求した情報に対して返される XML 応答の解析。
    
- 一般的な例外とエラー メッセージの処理。
    
main メソッドの後でスタブ アウトされていた  `ShowNumberOfMessagesInInbox` メソッドに、次のコードを追加します。アプリケーションを実行すると、アカウントの受信トレイ内にあるメッセージの数と、受信トレイ内で未読のメッセージ数が出力されます。アプリケーションの実行後に、GetStartedWithEWS.log ファイルを開くと、Exchange サーバーに送信された XML 要求と、サーバーから返された応答を確認できます 
  
```cs
      /// This is the XML request that is sent to the Exchange server.
      var getFolderSOAPRequest =
"<?xml version=\"1.0\" encoding=\"utf-8\"?>\n" +
"<soap:Envelope xmlns:soap=\"http://schemas.xmlsoap.org/soap/envelope/\"\n" +
"   xmlns:t=\"http://schemas.microsoft.com/exchange/services/2006/types\">\n" +
"<soap:Header>\n" +
"    <t:RequestServerVersion Version=\"Exchange2007_SP1\" />\n" +
"  </soap:Header>\n" +
"  <soap:Body>\n" +
"    <GetFolder xmlns=\"http://schemas.microsoft.com/exchange/services/2006/messages\"\n" +
"               xmlns:t=\"http://schemas.microsoft.com/exchange/services/2006/types\">\n" +
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
                                               ("{http://schemas.microsoft.com/exchange/services/2006/messages}ResponseCode")
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
                                              ("{http://schemas.microsoft.com/exchange/services/2006/messages}Folders")
                                            select folderElement;
            foreach (var folder in folders)
            {
              Tracing.Write("Folder name:     ");
              var folderName = from folderElement in
                                 folder.Descendants
                                 ("{http://schemas.microsoft.com/exchange/services/2006/types}DisplayName")
                               select folderElement.Value;
              Tracing.WriteLine(folderName.ElementAt(0));
              Tracing.Write("Total messages:  ");
              var totalCount = from folderElement in
                                 folder.Descendants
                                   ("{http://schemas.microsoft.com/exchange/services/2006/types}TotalCount")
                               select folderElement.Value;
              Tracing.WriteLine(totalCount.ElementAt(0));
              Tracing.Write("Unread messages: ");
              var unreadCount = from folderElement in
                                 folder.Descendants
                                   ("{http://schemas.microsoft.com/exchange/services/2006/types}UnreadCount")
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

### <a name="send-an-email-message"></a>電子メール メッセージの送信

もう 1 つの EWS アプリケーションの一般的な操作は、電子メール メッセージや会議出席依頼の送信です。この例では、電子メール メッセージを作成して、以前に入力されたユーザーの資格情報を使用して送信します。ここでは、一般的な EWS アプリケーションの 3 つのタスクを例示しています。
  
- 電子メールの作成と送信。
    
- 返された XML 応答の解析 (電子メールが正しく送信されたかどうかを判断します)。
    
- 一般的な例外とエラー メッセージの処理。
    
main メソッドの後でスタブアウトされていた SendTestEmail メソッドに、次のコードを追加します。アプリケーションの実行後に、GetStartedWithEWS.log ファイルを開くと、Exchange サーバーに送信された XML 要求と、サーバーから返された応答を確認できます
  
```cs
var createItemSOAPRequest =
      "<?xml version=\"1.0\" encoding=\"utf-8\"?>\n" +
      "<soap:Envelope xmlns:xsi=\"http://www.w3.org/2001/XMLSchema-instance\" \n" +
      "               xmlns:m=\"http://schemas.microsoft.com/exchange/services/2006/messages\" \n" +
      "               xmlns:t=\"http://schemas.microsoft.com/exchange/services/2006/types\" \n" +
      "               xmlns:soap=\"http://schemas.xmlsoap.org/soap/envelope/\">\n" +
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
                                               ("{http://schemas.microsoft.com/exchange/services/2006/messages}ResponseCode")
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

## <a name="next-steps"></a>次の手順

初めての EWS アプリケーションの作成は完了しました。ここからは、EWS を使用する別の方法について見つけましょう。次に、入門編としてのアイデアをいくつか示します。
  
- ユーザーの電子メール アドレスに応じて適切な Exchange サーバーに接続するように、アプリケーションに[自動検出](autodiscover-for-exchange.md)を実装する。「[Exchange 2013: Get user settings with Autodiscover](http://code.msdn.microsoft.com/Exchange-2013-Get-user-7e22c86e)」サンプルも参照してください。 
    
- EWS の詳細について、[EWS のリファレンス](http://msdn.microsoft.com/library/2a873474-1bb2-4cb1-a556-40e8c4159f4a%28Office.15%29.aspx)で調べる。 
    
- 使用可能な操作について、[EWS の操作](http://msdn.microsoft.com/library/cf6fd871-9a65-4f34-8557-c8c71dd7ce09%28Office.15%29.aspx)で確認する。 
    
- [EWS エディタ](http://ewseditor.codeplex.com/)を使用して、サーバーとやり取りされる SOAP トラフィックを確認する。 
    
カスタムアプリケーションに問題が発生したときには、[質問やコメントをフォーラムに投稿してみてください](http://social.technet.microsoft.com/Forums/exchange/en-US/home?forum=exchangesvrdevelopment) (最初の投稿は忘れずにお読みください)。 
  
## <a name="see-also"></a>関連項目

- [Exchange で Web サービスの使用を開始する](start-using-web-services-in-exchange.md)   
- [Exchange の EWS Managed API、EWS、および Web サービスについて学ぶ](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) 
- [Exchange の EWS クライアントの設計の概要](ews-client-design-overview-for-exchange.md)   
- [Exchange の Web サービス クライアントを開発する](develop-web-service-clients-for-exchange.md)  
- [EWS マネージ API クライアント アプリケーションの概要](get-started-with-ews-managed-api-client-applications.md)
    

