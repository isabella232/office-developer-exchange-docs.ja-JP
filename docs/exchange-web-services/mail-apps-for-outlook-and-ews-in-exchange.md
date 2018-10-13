---
title: Outlook アドインと Exchange の EWS
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 821c8eb9-bb58-42e8-9a3a-61ca635cba59
description: Outlook アドインについての情報と、そのアドインが Exchange の EWS で動作するしくみを説明します。
ms.openlocfilehash: 7eae834fe0bb93e2e94f094e811ab6cf002fc71b
ms.sourcegitcommit: 42eecc78e7aed7e95f73370d6c39ab8f4e96bf68
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/12/2018
ms.locfileid: "25541639"
---
# <a name="outlook-add-ins-and-ews-in-exchange"></a>Outlook アドインと Exchange の EWS

Outlook アドインについての情報と、そのアドインが Exchange の EWS で動作するしくみを説明します。

Outlook アドインは、メール ユーザー向けに操作をカスタマイズできるよう、Web 標準のシングル インターフェイスとプログラミング モデルを提供しています。 Outlook でホストされている HTML5 フレームを使用して、コンテキスト情報や役立つ情報を表示するメール アプリを作成できます。たとえば、メール メッセージに住所が含まれている場合、メール アプリで、住所を強調表示した Bing マップを表示させることも可能です。 あるいは、ユーザーがメッセージを作成しているときに、メール アプリが受信者の追加情報を表示し、ボタンをクリックするだけで一般的なあいさつ文をメールに挿入することもできます。

> [!NOTE]
> この記事において "Outlook" は、Outlook リッチ クライアント、Outlook RT、Outlook Web App、およびデバイス用 OWA に適用されます。

メール アプリのインターフェイスは、Office 用の JavaScript API の一部です。API を使用して Exchange の情報にアクセスし、メール アプリで次のことを行えます。

- メール中の住所、電話番号、タスクのヒント、提案された会議などの[エンティティを認識する](http://msdn.microsoft.com/library/a6b0904b-afe9-4882-9136-3d8cfd57fcf8%28Office.15%29.aspx)。

- 既存の[メッセージ](http://msdn.microsoft.com/library/d0bca550-70c3-457c-85f8-e19b39e3b892%28Office.15%29.aspx)と[予定](http://msdn.microsoft.com/library/6cfbc29d-8581-474e-9a8b-510471e4bf8b%28Office.15%29.aspx)を別々のビューで開いて表示し、1 つ以上のメッセージ情報をユーザーが相互参照できるようにする。

- ユーザーのメール ボックスをホストしている Exchange サーバーに [EWS 要求を行う](http://msdn.microsoft.com/library/2ec380e0-4a67-4146-92a6-6a39f65dc6f2%28Office.15%29.aspx)。 メール アプリは、たとえば、フォルダーの一覧を取得できます。ユーザーは、その中の 1 つのフォルダーを選択してメッセージを格納したり、スレッド内のすべてのアイテムを表示したり、メール メッセージに迷惑メールのマークを付けたりできます。

- メール アカウントを一意に識別する[トークンを取得する](http://msdn.microsoft.com/library/c658518b-6867-41a0-99cf-810303e4c539%28Office.15%29.aspx)。そのトークンを使用して、サードパーティのサービスでシングル サインオンを行うことができます。

- サードパーティのサービスがユーザーの代わりに EWS 要求を行うことが可能になる[トークンを取得する](http://msdn.microsoft.com/library/c658518b-6867-41a0-99cf-810303e4c539%28Office.15%29.aspx)。アイテムから添付物を抽出する、追加の処理のために Exchange サーバーからアイテムを取得することなどが行えます。

メール アプリを使用して、ユーザー向けの Outlook Web App エクスペリエンスをカスタマイズできます。ただし、Outlook Web App の "外観" をカスタマイズするには、TechNet の次の資料をご覧ください。

- [Outlook Web App のテーマの作成](http://technet.microsoft.com/en-us/library/bb201700%28v=exchg.150%29.aspx)

- [Outlook Web App サインイン、言語選択、エラー ページをカスタマイズする](http://technet.microsoft.com/en-us/library/ee633483%28v=exchg.150%29.aspx)

組織は、内部サーバーにメール アプリをインストールして、権限を持つユーザーだけにアクセスを制限できます。また、お客様や他のメール アプリ開発者が、[Office ストア](http://office.microsoft.com/store/)にメール アプリを置き、一般に公開して販売することも可能です。 Outlook を実行しているすべての人が、マーケットプレースからメール アプリをダウンロードし、インストールし、使用できます。

メール アプリ作成の詳細については、「[Outlook アドイン](/outlook/add-ins)」の文書、または「[EWS 要求を行う](http://code.msdn.microsoft.com/exchange/Mail-apps-for-Outlook-Make-770b2528)」のサンプルをご覧ください。

## <a name="ews-and-outlook-add-ins"></a>EWS と Outlook アドイン

メール アプリを実行するアカウントをホストしている Exchange サーバーでは、EWS 操作のサブセットを使用できます。

[mailbox.makeEwsRequestAsync](http://msdn.microsoft.com/library/2ec380e0-4a67-4146-92a6-6a39f65dc6f2%28Office.15%29.aspx) 関数を使用して、メール アプリから、ユーザーのメールボックスをホストしているサーバーに EWS 要求を行うことができます。 SOAP エンベロープと XML 要求を作成し、次いで **makeEwsRequestAsync** 関数が認証トークンを使用して EWS を呼び出します。そのトークンは、メールボックスと要求を行っているメール アプリを識別します。 ユーザーのメールボックスをセキュリティ保護するため、Exchange サーバーは、メール アプリ以外からのすべての要求、およびそのサーバーでホストされていないメールボックスからのすべての要求を拒否します。

他のアプリと同様に、メール アプリも機能へのアクセス許可が必要です。管理者は次のことを行う必要があります。

- メール アプリのユーザーに [EWS アクセスを許可する](controlling-client-application-access-to-ews-in-exchange.md)。

- Client Access Server EWS ディレクトリで ["OAuthAuthentication" を true に設定する](http://technet.microsoft.com/en-us/library/aa997233%28v=exchg.150%29.aspx)。

Office の[アクセス許可モデル](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md)用のアプリで、お客様のアプリがメールボックスの読み書きアクセス許可を要求する必要があります。

これらの手順を完了すると、フォルダーのサブセットとアイテムの EWS 操作がメール アプリで使用可能になります。

**表 1. メール アプリが使用できる EWS フォルダー操作とアイテム操作**

|**フォルダー操作**|**アイテム操作**|
|:-----|:-----|
|[CreateFolder 操作](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> [FindFolder 操作](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> [GetFolder 操作](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> [UpdateFolder 操作](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> |[CopyItem 操作](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> [CreateItem 操作](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/> [FindItem 操作](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) <br/> [FindConversation 操作](http://msdn.microsoft.com/library/2384908a-c203-45b6-98aa-efd6a4c23aac%28Office.15%29.aspx) <br/> [GetConversationItems 操作](http://msdn.microsoft.com/library/8ae00a99-b37b-4194-829c-fe300db6ab99%28Office.15%29.aspx) <br/> [GetItem 操作](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> [MarkAsJunk 操作](http://msdn.microsoft.com/library/1f71f04d-56a9-4fee-a4e7-d1034438329e%28Office.15%29.aspx) <br/> [MoveItem 操作](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/> [SendItem 操作](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) <br/> [UpdateItem 操作](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |

### <a name="service-callback-tokens"></a>サービス コールバック トークン

サービス コールバック トークンは、メール アプリがアクセス トークンをサード パーティのサービスに渡せるようにします。それによって、サービスは、メールボックスをホストする Exchange サーバーに EWS 要求を行うことができます。 たとえば、メール アプリは、メールに添付された画像の添付ファイル ID の一覧と一緒に、サービス コールバック トークンをサードパーティのサービスに渡すことができます。 サービスは、次に添付ファイル ID とコールバック トークンを使用して、ユーザーの Exchange サーバーに EWS 要求を行い、添付画像を取得します。 メール アプリは、サービス コールバック トークンをアイテム ID の一覧と一緒に使用して、Exchange サーバーからメールと予定アイテムを取得することもできます。

サービス コールバック トークンは、サードパーティのサービスがベアラー認証ヘッダーの EWS 要求に添付する不透明なトークンです。 トークンは、EWS 要求をセキュリティで保護するメール アプリとメールボックスを識別します。 サービス コールバック トークンの使用方法については、「[Outlook アドイン: Exchange サーバーから添付物を取得する](http://code.msdn.microsoft.com/exchange/Mail-apps-for-Office-Get-38babdc9)」のサンプルをご覧ください。

## <a name="see-also"></a>関連項目


- [Exchange で EWS へのクライアント アプリケーションのアクセスを制御する](controlling-client-application-access-to-ews-in-exchange.md)

- [Mailbox.makeEwsRequestAsync メソッド (JavaScript API for Office)](http://msdn.microsoft.com/library/2ec380e0-4a67-4146-92a6-6a39f65dc6f2%28Office.15%29.aspx)

- [Outlook アドイン](https://docs.microsoft.com/outlook/add-ins)

- [Mailbox.getUserIdentityTokenAsync メソッド (JavaScript API for Office)](http://msdn.microsoft.com/library/c658518b-6867-41a0-99cf-810303e4c539%28Office.15%29.aspx)

- [Exchange の ID トークンを使用して Outlook アドインを認証する](http://msdn.microsoft.com/library/c0520a1e-d9ba-495a-a99f-6816d7d2a23e%28Office.15%29.aspx)

- [Outlook アドインのアクセス許可を理解する](https://docs.microsoft.com/en-us/outlook/add-ins/understanding-outlook-add-in-permissions)

- [Set-WebServicesVirtualDirectory](http://technet.microsoft.com/en-us/library/aa997233%28v=exchg.150%29.aspx)

- [Outlook アドイン: EWS 要求を行う](http://code.msdn.microsoft.com/office/Mail-apps-for-Outlook-Make-770b2528)

- [Outlook アドイン: クライアント ID トークンを使用する](http://code.msdn.microsoft.com/Mail-apps-for-Outlook-Use-b20a66b6)

- [Outlook アドイン: Exchange サーバーから添付物を取得する](http://code.msdn.microsoft.com/office/Mail-apps-for-Office-Get-38babdc9)
