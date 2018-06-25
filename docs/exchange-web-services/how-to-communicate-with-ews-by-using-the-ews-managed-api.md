---
title: EWS のマネージ API を使用して通信 EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: d1b78293-da02-413a-875c-681e99146af3
description: Exchange で EWS マネージ API を使用して EWS と通信する方法について説明します。
ms.openlocfilehash: 773fcc3f7e95d25effb5a686d4b79ec22610df8c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758937"
---
# <a name="communicate-with-ews-by-using-the-ews-managed-api"></a>EWS のマネージ API を使用して通信 EWS

Exchange で EWS マネージ API を使用して EWS と通信する方法について説明します。
  
EWS のマネージ API では、 [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)クラスには、メソッドとプロパティを使用して、ユーザーの資格情報を設定、EWS のエンドポイントを識別する、送信 SOAP メッセージを受信し、EWS を使って通信するためにバインドを設定することが含まれています。 EWS のマネージ API を使用するには任意のタスクを実行するのには、前に、 **ExchangeService**クラスのインスタンスを作成し、EWS にバインドする必要があります。 
  
ユーザーの資格情報を持つ[ExchangeService](https://msdn.microsoft.com/library/Microsoft.Exchange.WebServices.Data.ExchangeService.aspx)オブジェクトと、EWS のエンドポイントを設定した後[ExchangeService](https://msdn.microsoft.com/library/Microsoft.Exchange.WebServices.Data.ExchangeService.aspx)オブジェクトを参照するすべてのメールボックス オブジェクトは、EWS を使って通信するために次のメソッドの型を使用できます。 
  
- ExchangeService オブジェクトのメソッド、**オブジェクト**の基本型から継承されていない**ExchangeService**オブジェクト上のすべてのメソッドは、EWS に電話をかけます。 
    
- Exchange のメールボックス アイテム タイプ メソッドとフォルダー タイプ メソッド。
    
**表 1 です。メールボックス アイテムおよびフォルダー通信 EWS のメソッドを入力します。**

|メソッド|できること|呼び出す操作|
|:-----|:-----|:-----|
|[Load](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.load%28v=exchg.80%29.aspx) <br/> |アイテム、添付ファイル、またはユーザー構成オブジェクトのプロパティを取得します。   <br/> |
  [GetItem 操作](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/><br/> [GetAttachment 操作](http://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx) <br/><br/> [GetUserConfiguration 操作](http://msdn.microsoft.com/library/71d50e3c-92bd-435f-8118-b28bb85f8138%28Office.15%29.aspx) <br/> |
|[バインド](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) <br/> |クライアント上の新しいアイテムに、サーバー上の既存のアイテムからの情報を取り込みます  <br/> |
  [GetItem 操作](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> |
|[Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.save%28v=exchg.80%29.aspx) <br/> |サーバー上のクライアント アイテムのコピーを保存します。  <br/> |
  [UpdateItem 操作](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/><br/> 
  [UpdateFolder 操作](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/><br/>
  [CreateItem 操作](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/><br/>
  [CreateFolder 操作](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> |
|[Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.update%28v=exchg.80%29.aspx) <br/> |クライアント上で加えられた変更でサーバーを更新します。<br/><br/>アイテムとフォルダーの場合は、 **Update**メソッドは、 [UpdateItem 操作](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)および[UpdateFolder 操作](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx)を使用します。  <br/> |
  [UpdateItem 操作](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/><br/>
  [UpdateFolder 操作](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> |
|[Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.delete%28v=exchg.80%29.aspx) <br/> |サーバー上のアイテムを削除します。<br/><br/>アイテムとフォルダーの場合は、 **Delete**メソッドと、 [DeleteFolder の操作](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx)を使用します。  <br/> |[DeleteItem の操作](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/><br/> [DeleteFolder 操作](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |
|[Copy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.copy%28v=exchg.80%29.aspx) <br/> |サーバー上のアイテムまたはフォルダーのコピーを作成します。   <br/> |
  [CopyItem 操作](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/><br/> [CopyFolder 操作](http://msdn.microsoft.com/library/c7ea0d68-9793-4144-b378-d99536776db9%28Office.15%29.aspx) <br/> |
|[移動](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.move%28v=exchg.80%29.aspx) <br/> |サーバー上のアイテムまたはフォルダーを移動します。   <br/> |
  [MoveItem 操作](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/><br/> [MoveFolder 操作](http://msdn.microsoft.com/library/c7233966-6c87-4a14-8156-b1610760176d%28Office.15%29.aspx) <br/> |
   
## <a name="to-use-the-ews-managed-api-to-communicate-with-ews"></a>EWS マネージ API を使用して EWS と通信するには

1. **ExchangeService**クラスのインスタンスを作成します。 
    
   ```csharp
    ExchangeService service = new ExchangeService();
   ```

   > [!NOTE]
   > **ExchangeService**の空のコンス トラクターでインスタンス化すると、Exchange の最新の既知のバージョンにバインドされているインスタンスが作成されます。 代わりに、パラメーターとしてバージョンを指定することによって Exchange の特定のバージョンをターゲットことができます。 `ExchangeService service = new ExchangeService(ExchangeVersion.Exchange2007_SP1);`
  
2. Exchange サーバーに要求を送信したユーザーの資格情報を設定します。 EWS にドメインにログオンしているコンピューターから接続する場合は、場合は、 **true を指定**する**ExchangeService**オブジェクトを**偽造している**プロパティを設定、認証されたユーザーの資格情報を使用します。
    
   ```cs
    // Connect by using the default credentials of the authenticated user.
    service.UseDefaultCredentials = true;
   ```

   既定のユーザー資格情報を使用して接続したくない場合は、別のユーザーの資格情報を明示的に指定する**ExchangeService**オブジェクトに**資格情報**のプロパティを設定します。 Office 365 の一部として Exchange Online または Exchange Online を使用する場合、ユーザー名とパスワードだけで基本認証を使用します。 ドメイン名は、NTLM 認証に必要です。 
    
   ```cs
    // Connect by using the credentials of user1 at contoso.com.
    service.Credentials = new WebCredentials("user1@contoso.com", "password");
   ```

   ユーザーのドメイン名とパスワードを使用して、ユーザーの資格情報を指定することもできます。
    
   ```cs
    // Connect by using the credentials of contoso/user1.
    service.Credentials = new WebCredentials("user1", "password", "contoso");
   ```

   > [!NOTE]
   > **偽造している****場合は true**に設定すると、**資格情報**のプロパティの値は無視されます。 
  
3. EWS エンドポイントの URL を設定します。この URL は、クライアント アクセス サーバー上の exchange.asmx ファイルの場所を示します。
    
   ```cs
    // Use Autodiscover to set the URL endpoint.
    service.AutodiscoverUrl("user1@contoso.com");
   ```

   > [!NOTE]
   >  ハードコードされた値を**ExchangeService**の**Url**プロパティを明示的に設定することができます、お勧めする自動検出サービス代わりに使用する、次の理由で: > 自動検出は、ユーザーごとに最適なエンドポイントを決定(エンドポイントは、ユーザーのメールボックス サーバーに最も近い) です。 > EWS の URL は、新しいクライアント アクセス サーバーが配置されている場合に変更可能性があります。 このシナリオでは、[自動検出](autodiscover-for-exchange.md)を使用することを意味コードを変更する必要はありません。 > する必要がありますか、URL を明示的に設定、または**AutodiscoverUrl**が、どちらも行う必要があります。 
  
## <a name="see-also"></a>関連項目

- [EWS マネージ API クライアント アプリケーションの概要](get-started-with-ews-managed-api-client-applications.md) 
- [自動検出を使用してコネクション ポイントを検索するには](how-to-use-autodiscover-to-find-connection-points.md)   
- [Exchange の Web サービス クライアントを開発する](develop-web-service-clients-for-exchange.md)
    

