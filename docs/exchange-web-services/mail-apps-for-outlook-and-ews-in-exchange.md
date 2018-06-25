---
title: Exchange での Outlook 用メール アプリと EWS
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 821c8eb9-bb58-42e8-9a3a-61ca635cba59
description: Outlook 用メール アプリについての情報と、そのアプリが Exchange の EWS で動作するしくみを説明します。
ms.openlocfilehash: 2f44045d80a74ed6a835604d516949ca3bc27379
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759088"
---
# <a name="mail-apps-for-outlook-and-ews-in-exchange"></a>Exchange での Outlook 用メール アプリと EWS

ここでは、Outlook 用メール アプリについて説明し、それらのアプリが Exchange で EWS を使用してどのように動作するのかについて解説します。
  
Outlook 用メール アプリは、メール ユーザー向けに操作をカスタマイズできるよう、Web 標準のシングル インターフェイスとプログラミング モデルを提供しています。Outlook でホストされている HTML5 フレームを使用して、コンテキスト情報や役立つ情報を表示するメール アプリを作成できます。たとえば、メール メッセージに住所が含まれている場合、メール アプリで、住所を強調表示した Bing マップを表示させることも可能です。あるいは、ユーザーがメッセージを作成しているときに、メール アプリが受信者の追加情報を表示し、ボタンをクリックするだけで一般的なあいさつ文をメールに挿入することもできます。
  
> [!NOTE]
> この記事において "Outlook" は、Outlook リッチ クライアント、Outlook RT、Outlook Web App、および デバイス用 OWA に適用されます。 
  
メール アプリのインターフェイスは、Office 用の JavaScript API の一部です。API を使用して Exchange の情報にアクセスし、メール アプリで次のことを行えます。
  
- [エンティティの認識](http://msdn.microsoft.com/library/a6b0904b-afe9-4882-9136-3d8cfd57fcf8%28Office.15%29.aspx)、アドレス、電話番号、タスクの提案、または電子メールで会議の提案のようにします。 
    
- 開き、既存の[メッセージ](http://msdn.microsoft.com/library/d0bca550-70c3-457c-85f8-e19b39e3b892%28Office.15%29.aspx)や[予定](http://msdn.microsoft.com/library/6cfbc29d-8581-474e-9a8b-510471e4bf8b%28Office.15%29.aspx)ビューに表示する別のユーザーが 1 つまたは複数のメッセージ内の情報を相互参照できますようにします。 
    
- [EWS の確認要求](http://msdn.microsoft.com/library/2ec380e0-4a67-4146-92a6-6a39f65dc6f2%28Office.15%29.aspx)をユーザーのメールボックスをホストする Exchange サーバーにします。 メール アプリケーションは、ユーザーは、メッセージの格納や、会話のすべての項目を表示するいずれかを選択したり、迷惑メールとして電子メール メッセージをマークするため、フォルダーの一覧を取得など、です。 
    
- サードパーティ製のサービスにサインオン[トークンを取得](http://msdn.microsoft.com/library/c658518b-6867-41a0-99cf-810303e4c539%28Office.15%29.aspx)する 1 つを有効にする電子メール アカウントを一意に識別するします。 
    
- [トークンを取得する](http://msdn.microsoft.com/library/c658518b-6867-41a0-99cf-810303e4c539%28Office.15%29.aspx)など、ユーザーのための EWS の要求を作成する、アイテムから添付ファイルを抽出する、またはさらに処理するため、Exchange サーバーからアイテムを取得するのにはサードパーティ製のサービスを有効にします。 
    
メール アプリケーションを使用するには、ユーザーの Outlook Web App のエクスペリエンスをカスタマイズするのには場合は、ただし、Outlook Web App の「外観」をカスタマイズするのには、TechNet の以下の資料を参照してください。
  
- [Outlook Web App のテーマを作成します。](http://technet.microsoft.com/en-us/library/bb201700%28v=exchg.150%29.aspx)
    
- [Outlook Web App サインイン、言語選択、およびエラー ページをカスタマイズします。](http://technet.microsoft.com/en-us/library/ee633483%28v=exchg.150%29.aspx)
    
組織は権限のあるユーザーへのアクセスを制限する内部サーバーにメール アプリケーションをインストールすることができ、他のメール アプリケーションの開発者追加またはメール アプリケーション販売用の[Office ストア](http://office.microsoft.com/store/)で一般に公開します。 ダウンロード、インストール、および市場からのメール アプリケーションを使用して Outlook を実行しているすべての人ことができます。 
  
メール アプリケーションを作成する方法の詳細については、場合は、 [Outlook のドキュメントのメール アプリケーション](http://msdn.microsoft.com/library/71e64bc9-e347-4f5d-8948-0a47b5dd93e6%28Office.15%29.aspx)または[EWS 要求を行う](http://code.msdn.microsoft.com/exchange/Mail-apps-for-Outlook-Make-770b2528)例を確認してください。 
  
## <a name="ews-and-mail-apps-for-outlook"></a>EWS と Outlook 用メール アプリ

メール アプリを実行するアカウントをホストしている Exchange サーバーでは、EWS 操作のサブセットを使用できます。
  
[Mailbox.makeEwsRequestAsync](http://msdn.microsoft.com/library/2ec380e0-4a67-4146-92a6-6a39f65dc6f2%28Office.15%29.aspx)関数を使用すると、ユーザーのメールボックスをホストするサーバーに、メール アプリから EWS 要求を行うことができます。 メールボックスを識別する認証トークンとして SOAP エンベロープと XML 要求では、EWS の**makeEwsRequestAsync**関数呼び出しを作成し、要求を行っているアプリケーションをメールするとします。 ユーザーのメールボックスをセキュリティで保護するのには、Exchange サーバーが付属していないメール アプリケーションやホストされていないメールボックス サーバー上のすべての要求を拒否します。 
  
他のアプリと同様に、メール アプリも機能へのアクセス許可が必要です。管理者は、次のことを行う必要があります。
  
- メール アプリケーションのユーザーに[与える EWS のアクセス](controlling-client-application-access-to-ews-in-exchange.md)をします。 
    
- クライアント アクセス サーバーの EWS のディレクトリの[設定を true に設定するには、"OAuthAuthentication"](http://technet.microsoft.com/en-us/library/aa997233%28v=exchg.150%29.aspx)を。 
    
アプリが Office[のアクセス許可モデル](http://msdn.microsoft.com/library/5bca69f2-b287-4e19-8f0f-78d896b2a3d3%28Office.15%29.aspx)のアプリケーションで読み取り/書き込みのメールボックスのアクセス許可を要求するかどうかを確認する必要があります。
  
これらの手順を完了すると、フォルダーのサブセットとアイテムの EWS 操作がメール アプリで使用可能になります。  
  
**表 1 です。アプリをメール EWS のフォルダーとアイテムの操作を使用できます。**

|**フォルダーの操作**|**項目の操作**|
|:-----|:-----|
|
  [CreateFolder 操作](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> 
  [FindFolder 操作](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> 
  [GetFolder 操作](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> 
  [UpdateFolder 操作](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> |
  [CopyItem 操作](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> 
  [CreateItem 操作](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/> 
  [FindItem 操作](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) <br/> 
  [FindConversation 操作](http://msdn.microsoft.com/library/2384908a-c203-45b6-98aa-efd6a4c23aac%28Office.15%29.aspx) <br/> 
  [GetConversationItems 操作](http://msdn.microsoft.com/library/8ae00a99-b37b-4194-829c-fe300db6ab99%28Office.15%29.aspx) <br/> 
  [GetItem 操作](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> [MarkAsJunk の操作](http://msdn.microsoft.com/library/1f71f04d-56a9-4fee-a4e7-d1034438329e%28Office.15%29.aspx) <br/> 
  [MoveItem 操作](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/> 
  [SendItem 操作](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) <br/> 
  [UpdateItem 操作](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |
   
### <a name="service-callback-tokens"></a>サービス コールバック トークン

サービスのコールバックのトークンは、サービスは、メールボックスをホストする Exchange サーバーに EWS 要求を行うことができるように、サード パーティのサービスをアクセス トークンを渡すためのメール アプリケーションを有効にします。 たとえば、メール アプリケーションは、電子メールに添付して画像を添付ファイルの Id の一覧にサードパーティのサービスにサービス コールバックのトークンを渡すことができます。 サービスは、添付された画像を取得するのにユーザーの Exchange サーバーに、EWS の要求に添付ファイルの Id、コールバックのトークンを使用できます。 メール アプリケーションもトークンを使用できる、サービスのコールバック項目 Id の一覧が Exchange サーバーからの電子メールや予定の項目を取得します。
  
サービスのコールバックのトークンは、サードパーティ製のサービスは、ベアラー認証ヘッダーでは、EWS 要求にアタッチする不明確なトークンです。 トークンでは、メール ・ アプリケーションおよび EWS 要求をセキュリティで保護するメールボックスを識別します。 サービスのコールバックのトークンを使用する方法についてを参照してください、[アプリケーションを Outlook のメール: Exchange サーバーからの添付ファイルを取得する](http://code.msdn.microsoft.com/exchange/Mail-apps-for-Office-Get-38babdc9)サンプルです。 
  
## <a name="see-also"></a>関連項目


- [Exchange クライアント アプリケーションの EWS へのアクセスを制御します。](controlling-client-application-access-to-ews-in-exchange.md)
    
- [Mailbox.makeEwsRequestAsync メソッド (Office の JavaScript API)](http://msdn.microsoft.com/library/2ec380e0-4a67-4146-92a6-6a39f65dc6f2%28Office.15%29.aspx)
    
- [Outlook アドイン](http://msdn.microsoft.com/library/71e64bc9-e347-4f5d-8948-0a47b5dd93e6%28Office.15%29.aspx)
    
- [Mailbox.getUserIdentityTokenAsync メソッド (Office の JavaScript API)](http://msdn.microsoft.com/library/c658518b-6867-41a0-99cf-810303e4c539%28Office.15%29.aspx)
    
- [Exchange の ID トークンを使用して Outlook アドインを認証する](http://msdn.microsoft.com/library/c0520a1e-d9ba-495a-a99f-6816d7d2a23e%28Office.15%29.aspx)
    
- [Outlook 2013 プレビューのメール アプリでアクセス許可モデルを使用する](http://msdn.microsoft.com/library/5bca69f2-b287-4e19-8f0f-78d896b2a3d3%28Office.15%29.aspx)
    
- [セット WebServicesVirtualDirectory](http://technet.microsoft.com/en-us/library/aa997233%28v=exchg.150%29.aspx)
    
- [アプリを Outlook のメール: EWS 要求を行う](http://code.msdn.microsoft.com/office/Mail-apps-for-Outlook-Make-770b2528)
    
- [アプリを Outlook のメール: クライアントの id トークンを使用します。](http://code.msdn.microsoft.com/Mail-apps-for-Outlook-Use-b20a66b6)
    
- [アプリを Outlook のメール: Exchange サーバーからの添付ファイルを取得します。](http://code.msdn.microsoft.com/office/Mail-apps-for-Office-Get-38babdc9)
    

