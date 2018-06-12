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
# <a name="get-started-with-ews-managed-api-client-applications"></a>EWS マネージ API クライアント アプリケーションの概要

EWS マネージ API を使用して、Exchange 用の単純な Hello World メール クライアント アプリケーションを開発します。 
  
[EWS マネージ API](http://aka.ms/ews-managed-api-readme) では、クライアント アプリケーション、ポータル アプリケーション、サービス アプリケーションから Web サービス メッセージを送受信するための、直観的で使いやすいオブジェクト モデルが用意されています。EWS マネージ API を使用して、Exchange Online、Office 365 の一部としての Exchange Online、Exchange サーバー メールボックスに格納されているほとんどすべての情報にアクセスすることができます。この記事にある情報は、初めて EWS マネージ API のクライアント アプリケーションを開発する場合に役立ちます。 
  
> [!NOTE]
> [!メモ]  EWS マネージ API が、 [GitHub](https://github.com/officedev/ews-managed-api) のオープン ソース プロジェクトとして利用できるようになりました。オープン ソース ライブラリを使用して、次のことができます。 >  バグ修正と API の機能強化に貢献します。 >  公式のリリースで利用可能になる前に、修正プログラムや拡張機能を取得できます。 >  API の最も包括的かつ最新の実装にアクセスして、参照として使用するか、新しいプラットフォームで新しいライブラリを作成します。 >  GitHub による [貢献](https://github.com/OfficeDev/ews-managed-api/blob/master/CONTRIBUTING.md)を歓迎いたします。 
  
## <a name="youll-need-an-exchange-server"></a>Exchange サーバーの準備
<a name="NeedExchange"> </a>

Exchange メールボックス アカウントを既に所有している場合は、このセクションを省略してもかまいません。それ以外の場合は、次のいずれかの方法で、初めての EWS クライアント アプリケーション用の Exchange メールボックスをセットアップします。
  
- [Office 365 開発者向けサイト](http://msdn.microsoft.com/en-us/library/office/fp179924.aspx)を取得します (推奨)。これが最も簡単に Exchange メールボックスをセットアップする方法です。 
    
- [Exchange Server](http://office.microsoft.com/en-us/exchange/microsoft-exchange-try-or-buy-exchange-we-can-help-you-decide-FX103746846.aspx?WT%2Eintid1=ODC%5FENUS%5FFX103472230%5FXT103965589) をダウンロードします。
    
Exchange からメールを送受信できることが確認できたら、開発環境をセットアップする準備ができています。Exchange Web クライアントの [Outlook Web App](http://technet.microsoft.com/en-us/library/jj657718%28v=exchg.150%29.aspx) を使用して、メールが送信できることを確認します。 
  
## <a name="set-up-your-development-environment"></a>開発環境のセットアップ
<a name="Setup"> </a>

以下にアクセスできることを確認してください。
  
- .NET Framework 4 をサポートしているバージョンの [Visual Studio](http://www.visualstudio.com/en-us/downloads/download-visual-studio-vs.aspx)。技術的には、どの C# コンパイラでも使用できるため Visual Studio は必ず必要であるというわけではありませんが、Visual Studio を使用することをお勧めします。 
    
- [EWS マネージ API](http://aka.ms/ews-managed-api-readme)。システムに応じて、64 ビット バージョンと 32 ビット バージョンのどちらかをインストールします。既定のインストール場所を使用します。 
    
## <a name="create-your-first-ews-managed-api-application"></a>初めての EWS マネージ API アプリケーションの作成
<a name="Create"> </a>

次の手順は、Office 365 開発者向けサイトをセットアップすることを前提としています。Exchange をダウンロードしてインストールした場合、Exchange サーバーに[有効な証明書をインストール](http://technet.microsoft.com/en-us/library/bb310769%28v=exchg.141%29.aspx)するか、既定で提供されている自己署名証明書用に[証明書の検証コールバックを実装](how-to-validate-a-server-certificate-for-the-ews-managed-api.md)する必要があります。なお、これらの手順は、使用している Visual Studio のバージョンによって若干異なる場合がありますのでご注意ください。 
  
### <a name="step-1-create-a-project-in-visual-studio"></a>手順 1: Visual Studio でプロジェクトを作成する

1. Visual Studio の **[ファイル]** メニューで、 **[新規]** を選択してから、 **[プロジェクト]** を選択します。 **[新しいプロジェクト]** ダイアログ ボックスが表示されます。 
    
2. **C# コンソール アプリケーション** を作成します。 **[テンプレート]** ウィンドウで、 **[Visual C#]** を選択してから、 **[コンソール アプリケーション]** を選択します。 
    
3. プロジェクトに「HelloWorld」という名前を付けて、 **[OK]** を選択します。
    
Visual Studio は、プロジェクトを作成し、Program.cs コードのドキュメント ウィンドウを開きます。

### <a name="step-2-add-a-reference-to-the-ews-managed-api"></a>手順 2:EWS マネージ API の参照を追加する

1. **[ソリューション エクスプ ローラー]** ウィンドウが既に開いている場合、この手順を省略し、手順 2 に進みます。 **[ソリューション エクスプ ローラー]** ウィンドウを開くには、 **[ビュー]** メニューで **[ソリューション エクスプ ローラー]** を選択します。 
    
2. **[ソリューション エクスプ ローラー]** の **HelloWorld** プロジェクトで **[参照]** のショートカット メニュー (右クリック) を開き、コンテキスト メニューから **[参照の追加]** を選択します。プロジェクトの参照を管理するためのダイアログ ボックスが開きます。 
    
3. [**参照**] オプションを選択します。 EWS マネージ API DLL がインストールされている場所を参照します。 インストーラーにより設定の既定のパスは、次: C:\Program Files\Microsoft\Exchange\Web サービス\<バージョン >\. パスは、32 ビットまたは 64 ビット バージョンの Microsoft.Exchange.WebServices.dll をダウンロードするかどうか異なります。 **Microsoft.Exchange.WebServices.dll**を選択し、 **[ok]** または [**追加**を選択します。 EWS のマネージ API の参照をプロジェクトに追加します。 
    
4. EWS Managed API 2.0 を使用している場合は, .NET Framework 4 を対象とするよう HelloWorld プロジェクトを変更します。EWS マネージ API の他のバージョンでは、別の .NET Framework のターゲット バージョンを使用する可能性があります。
    
5. 正しい .NET Framework のターゲット バージョンを使用していることを確認します。 **[ソリューション エクスプ ローラー]** で、 **HelloWorld** プロジェクトのショートカット メニュー (右クリック) を開き、 **[プロパティ]** を選択します。 **[ターゲット フレームワーク]** ドロップダウン ボックスで、 **[.NET Framework 4]** が選択されていることを確認します。 
    
プロジェクトをセットアップし、EWS マネージ API への参照を作成したので、最初のアプリケーションを作成する準備ができました。 簡潔にするために、Program.cs ファイルにコードを追加します。 EWS のマネージ API の参照の詳細については[、EWS のマネージ API のアセンブリの参照](how-to-reference-the-ews-managed-api-assembly.md)を参照してください。 次の手順では、ほとんどの EWS マネージ API クライアント アプリケーションを作成するための基本的なコードを開発します。 
### <a name="step-3-set-up-url-redirection-validation-for-autodiscover"></a>手順 3:自動検出のための URL リダイレクト検証を設定します。

- **Main(string[] args)** メソッドの後に、次のリダイレクト検証コールバック メソッドを追加します。これは、 [自動検出](autodiscover-for-exchange.md)によって返される、リダイレクトされた URL が HTTPS エンドポイントを表すかどうかを検証します。 
    
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

この検証コールバックは、手順 4 で **ExchangeService** オブジェクトに渡されます。アプリケーションが自動検出リダイレクトを信頼してそれに従うようにするには、これが必要です。自動検出リダイレクトの結果は、アプリケーションの EWS エンドポイントを提供します。 

### <a name="step-4-prepare-the-exchangeservice-object"></a>手順 4:ExchangeService オブジェクトを準備する

1. **using** ディレクティブ参照を EWS マネージ API に追加します。Program.cs の上部の最後の **using** ディレクティブに次のコードを追加します。 
    
   ```cs
    using Microsoft.Exchange.WebServices.Data;
   ```

2. **Main** メソッドで、対象とするサービス バージョンの [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトをインスタン化します。この例では、EWS スキーマの初期のバージョンを対象とします。 
    
   ```cs
    ExchangeService service = new ExchangeService(ExchangeVersion.Exchange2007_SP1);
   ```

3. Exchange オンプレミス サーバーを対象としており、クライアントがドメインに参加している場合は、手順 4 に進みます。クライアントが Exchange Online または Office 365 開発者向けサイトのメールボックスを対象としている場合、明示的な資格情報を渡す必要があります。 **ExchangeService** オブジェクトのインスタンス化の後ろに次のコードを追加し、メールボックス アカウントの資格情報を設定します。ユーザー名は、ユーザー プリンシパル名でなければなりません。手順 5 に進んでください。 
    
   ```cs
    service.Credentials = new WebCredentials("user1@contoso.com", "password");
   ```

4. オンプレミス Exchange サーバーを対象とする、ドメインに参加しているクライアントは、ログオンしているユーザーの既定の資格情報を使用できます。ここでは、この資格情報がメールボックスに関連付けられていることを想定しています。 **ExchangeService** オブジェクトのインスタンス化の後ろに、次のコードを追加します。 
    
   ```cs
    service.UseDefaultCredentials = true;
   ```

   クライアントが Exchange Online または Office 365 開発者向けサイトのメールボックスを対象とする場合、[UseDefaultCredentials](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.usedefaultcredentials%28v=exchg.80%29.aspx) が既定値である **false** に設定されていることを確認します。クライアントは、EWS サービスを呼び出すサービス URL を取得するために自動検出サービスの最初の呼び出しを行う準備ができました。
    
5. **ExchangeService** オブジェクトの **AutodiscoverUrl** メソッドは、自動検出サービスに対して一連の呼び出しを実行してサービス URL を取得します。このメソッドの呼び出しが成功した場合、 **ExchangeService** オブジェクトの URL プロパティがサービス URL を使用して設定されます。ユーザーのメール アドレスおよび **RedirectionUrlValidationCallback** を **AutodiscoverUrl** メソッドに渡します。手順 3 または 手順 4 で資格情報を指定したら、次のコードを追加します。  `user1@contoso.com` を使用するメール アドレスに変更し、自動検出サービスが EWS エンドポイントを検索できるようにします。 
    
   ```cs
    service.AutodiscoverUrl("user1@contoso.com", RedirectionUrlValidationCallback);
   ```

この時点で、EWS を呼び出してメールボックスのデータにアクセスできるようにクライアントが設定されています。 コードを今すぐ実行する場合は、**ExchangeService.Url** プロパティの内容を調べて、 [AutodiscoverUrl](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) メソッド呼び出しが動作することを確認してください。 このプロパティに URL が含まれる場合、呼び出しは正常に行われています。 これは、アプリケーションが正常にサービスで認証され、メールボックスの EWS エンドポイントを検出したことを意味します。 これで、初めての EWS の呼び出しを行う準備が整いました。 EWS の URL を設定の詳細については[、EWS のマネージ API を使用して、EWS のサービスの URL の設定](how-to-set-the-ews-service-url-by-using-the-ews-managed-api.md)を参照してください。 

### <a name="step-6-create-your-first-hello-world-email-message"></a>手順 6:初めての Hello World メール メッセージを作成する

1. **AutodiscoverUrl** メソッド呼び出しの後に、新しい **EmailMessage** オブジェクトをインスタンス化し、作成したサービス オブジェクトに渡します。 
    
   ```cs
    EmailMessage email = new EmailMessage(service);
   ```

   これで、サービス バインドが設定されているメール メッセージが作成されます。 **EmailMessage** オブジェクトで開始されるすべての呼び出しは、サービスの対象となります。 
    
2. 次に、メール メッセージの宛先行の受信者を設定します。これを行うには、 `user1@contoso.com` を変更して SMTP アドレスを使用します。 
    
   ```cs
    email.ToRecipients.Add("user1@contoso.com");
   ```

3. メール メッセージの件名および本文を設定します。
    
   ```cs
    email.Subject = "HelloWorld";
    email.Body = new MessageBody("This is the first email I've sent by using the EWS Managed API.");
   ```

4. EWS マネージ API を使用して、最初のメール メッセージを送信する準備が整いました。 **Send** メソッドは、サービスを呼び出し、配信用にメール メッセージを送信します。 Exchange との通信に使用することが他のメソッドの詳細については、 [EWS のマネージ API を使用して、EWS を使ってコミュニケーション](how-to-communicate-with-ews-by-using-the-ews-managed-api.md)を参照してください。 
    
   ```cs
    email.Send();
   ```

5. Hello World アプリケーションを実行する準備が整いました。Visual Studio で、 **[F5]** を選択します。空のコンソール ウィンドウが開きます。アプリケーションが認証を行い、自動検出リダイレクトに従い、自分自身に送信するメール メッセージを作成するための最初の呼び出しを行っている間、コンソール ウィンドウには何も表示されません。実行されている呼び出しを表示する場合は、 **AutodiscoverUrl** メソッドが呼び出される前のところに次の 2 行のコードを追加します。F5 キーを押します。これで、コンソール ウィンドウに [EWS 要求と応答のトレースが出力されます](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md)。 
    
   ```cs
    service.TraceEnabled = true;
    service.TraceFlags = TraceFlags.All;
   ```

EWS マネージ API クライアント アプリケーションが作動するようになりました。利便性を考慮して、次の使用例では、Hello World アプリケーションを作成するために Program.cs に追加したすべてのコードを示します。

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

## <a name="next-steps"></a>次の手順
<a name="Next"> </a>

最初の EWS マネージ API クライアント アプリケーションでより多くの作業を行う準備ができている場合、次のリソースを参照します。
  
- [Exchange 2013:101 コード サンプル](http://code.msdn.microsoft.com/exchange/Exchange-2013-101-Code-3c38582c)
    
- [フォルダーとアイテム](folders-and-items-in-ews-in-exchange.md)
    
- [EWSEditor](http://ewseditor.codeplex.com/)
    
カスタム アプリケーションで問題が発生したときには、[質問やコメントをフォーラムに投稿してみてください](http://social.technet.microsoft.com/Forums/exchange/en-US/home?forum=exchangesvrdevelopment) (最初の投稿は忘れずにお読みください)。 
  
## <a name="in-this-section"></a>このセクションの内容
<a name="Next"> </a>

- [EWS のマネージ API のアセンブリを参照します。](how-to-reference-the-ews-managed-api-assembly.md)
    
- [EWS のマネージ API を使用して、EWS のサービスの URL を設定します。](how-to-set-the-ews-service-url-by-using-the-ews-managed-api.md)
    
- [EWS のマネージ API を使用して通信 EWS](how-to-communicate-with-ews-by-using-the-ews-managed-api.md)
    
## <a name="see-also"></a>関連項目

- [Exchange で Web サービスの使用を開始する](start-using-web-services-in-exchange.md)    
- [Exchange の EWS クライアントの設計の概要](ews-client-design-overview-for-exchange.md)    
- [Exchange の Web サービス クライアントを開発する](develop-web-service-clients-for-exchange.md)   
- [EWS のマネージ API アプリケーションのトラブルシューティングを行うには、要求と応答をトレースします。](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md)
    

