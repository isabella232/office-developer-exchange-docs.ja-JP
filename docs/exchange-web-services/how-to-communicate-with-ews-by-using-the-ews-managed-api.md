---
title: EWS マネージ API を使用して EWS と通信する
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: d1b78293-da02-413a-875c-681e99146af3
description: Exchange で EWS マネージ API を使用して EWS と通信する方法について説明します。
localization_priority: Priority
ms.openlocfilehash: be807f2d936bf79d181476ec8eb12f20fca7950f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528245"
---
# <a name="communicate-with-ews-by-using-the-ews-managed-api"></a>EWS マネージ API を使用して EWS と通信する

Exchange で EWS マネージ API を使用して EWS と通信する方法について説明します。
  
EWS マネージ API の [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) クラスには、ユーザー資格情報の設定、EWS エンドポイントの特定、SOAP メッセージの送受信、および EWS と通信するためのバインドの構成に使用するメソッドとプロパティが含まれます。 EWS マネージ API を使用して何らかのタスクを実行するためには、**ExchangeService** クラスのインスタンスを作成して、それを EWS にバインドしておく必要があります。 
  
ユーザー資格情報と EWS エンドポイントを指定して [ExchangeService](https://msdn.microsoft.com/library/Microsoft.Exchange.WebServices.Data.ExchangeService.aspx) オブジェクトをセットアップすると、[ExchangeService](https://msdn.microsoft.com/library/Microsoft.Exchange.WebServices.Data.ExchangeService.aspx) オブジェクトを参照するメールボックス オブジェクトは、次のメソッド タイプを使用して EWS と通信できるようになります。 
  
- ExchangeService オブジェクト メソッド — **ExchangeService** オブジェクトのうち、基本 **Object** タイプから継承されたのではないすべてのメソッドが EWS の呼び出しを実行します。 
    
- Exchange のメールボックス アイテム タイプ メソッドとフォルダー タイプ メソッド。
    
**表 1. EWS と通信するメールボックス アイテム タイプ メソッドとフォルダー タイプ メソッド**

|メソッド|できること|呼び出す操作|
|:-----|:-----|:-----|
|[Load](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.load%28v=exchg.80%29.aspx) <br/> |アイテム、添付物、またはユーザー構成オブジェクトのプロパティを取得します。  <br/> |[GetItem 操作](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/><br/> [GetAttachment 操作](https://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx) <br/><br/> [GetUserConfiguration 操作](https://msdn.microsoft.com/library/71d50e3c-92bd-435f-8118-b28bb85f8138%28Office.15%29.aspx) <br/> |
|[Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) <br/> |クライアント上の新しいアイテムに、サーバー上の既存のアイテムからの情報を取り込みます。  <br/> |[GetItem 操作](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> |
|[Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.save%28v=exchg.80%29.aspx) <br/> |クライアント アイテムのコピーをサーバーに保存します。  <br/> |[UpdateItem 操作](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/><br/> [UpdateFolder 操作](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/><br/>[CreateItem 操作](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/><br/>[CreateFolder 操作](https://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> |
|[Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.update%28v=exchg.80%29.aspx) <br/> |クライアント上で加えられた変更に基づいてサーバーを更新します。<br/><br/>アイテムおよびフォルダーの場合、**Update** メソッドは [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) 操作および [UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) 操作を使用します。  <br/> |[UpdateItem 操作](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/><br/>[UpdateFolder 操作](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> |
|[Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.delete%28v=exchg.80%29.aspx) <br/> |サーバー上のアイテムを削除します。<br/><br/>アイテムおよびフォルダーの場合、**Delete** メソッドは [DeleteFolder](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) 操作を使用します。  <br/> |[DeleteItem 操作](https://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/><br/> [DeleteFolder 操作 ](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |
|[Copy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.copy%28v=exchg.80%29.aspx) <br/> |サーバー上のアイテムまたはフォルダーのコピーを作成します。  <br/> |[CopyItem 操作](https://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/><br/> [CopyFolder 操作](https://msdn.microsoft.com/library/c7ea0d68-9793-4144-b378-d99536776db9%28Office.15%29.aspx) <br/> |
|[Move](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.move%28v=exchg.80%29.aspx) <br/> |サーバー上のアイテムまたはフォルダーを移動します。  <br/> |[MoveItem 操作](https://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/><br/> [MoveFolder 操作](https://msdn.microsoft.com/library/c7233966-6c87-4a14-8156-b1610760176d%28Office.15%29.aspx) <br/> |
   
## <a name="to-use-the-ews-managed-api-to-communicate-with-ews"></a>EWS マネージ API を使用して EWS と通信するには

1. **ExchangeService** クラスをインスタンス化します。 
    
   ```csharp
    ExchangeService service = new ExchangeService();
   ```

   > [!NOTE]
   > 空のコンストラクターで **ExchangeService** をインスタンス化すると、既知の最新バージョンの Exchange にバインドされたインスタンスが作成されます。 あるいは、バージョンをパラメーターとして指定することにより、特定のバージョンの Exchange を対象にすることもできます。 `ExchangeService service = new ExchangeService(ExchangeVersion.Exchange2007_SP1);`
  
2. Exchange サーバーに要求を送信するユーザーの資格情報を設定します。 ドメインにログオンしているコンピューターから EWS に接続する場合は、認証されたユーザーの資格情報を使用して、**ExchangeService** オブジェクトの **UseDefaultCredentials** プロパティを **true** に設定します。
    
   ```cs
    // Connect by using the default credentials of the authenticated user.
    service.UseDefaultCredentials = true;
   ```

   既定ユーザーの資格情報を使用して接続したくない場合は、**ExchangeService** オブジェクトの **Credentials** プロパティを設定することにより、異なるユーザーの資格情報を明示的に指定します。 Exchange Online を使用する場合、または Office 365 の一部として Exchange Online を使用する場合は、ユーザー名とパスワードのみによる基本認証を使用することになります。 NTLM 認証にはドメイン名が必要です。 
    
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
   > **UseDefaultCredentials** プロパティを **true** に設定した場合、**Credentials** プロパティの値は無視されます。 
  
3. EWS エンドポイントの URL を設定します。この URL は、クライアント アクセス サーバー上の exchange.asmx ファイルの位置を示します。
    
   ```cs
    // Use Autodiscover to set the URL endpoint.
    service.AutodiscoverUrl("user1@contoso.com");
   ```

   > [!NOTE]
   >  **ExchangeService** の **Url** プロパティをハードコーディング値に明示的に設定することもできますが、できれば次の理由で、自動検出サービスを使用することをお勧めします。>  自動検出サービスでは、特定のユーザーのための最適なエンドポイント (そのユーザーのメールボックス サーバーに最も近いエンドポイント) が判別されます。 >  新しいクライアント アクセス サーバーが配置されると、EWS URL が変わる可能性があります。 このシナリオの場合、[自動検出](autodiscover-for-exchange.md)を使用するとコード変更が必要なくなります。 >  URL を明示的に設定するか、または **AutodiscoverUrl** を呼び出す必要がありますが、両方を行うべきではありません。 
  
## <a name="see-also"></a>関連項目

- [EWS マネージ API クライアント アプリケーションの概要](get-started-with-ews-managed-api-client-applications.md) 
- [自動検出を使用して接続ポイントを検索する](how-to-use-autodiscover-to-find-connection-points.md)   
- [Exchange の Web サービス クライアントを開発する](develop-web-service-clients-for-exchange.md)
    

