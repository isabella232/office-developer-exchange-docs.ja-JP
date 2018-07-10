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
# <a name="communicate-with-ews-by-using-the-ews-managed-api"></a><span data-ttu-id="c81b3-103">EWS のマネージ API を使用して通信 EWS</span><span class="sxs-lookup"><span data-stu-id="c81b3-103">Communicate with EWS by using the EWS Managed API</span></span>

<span data-ttu-id="c81b3-104">Exchange で EWS マネージ API を使用して EWS と通信する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="c81b3-104">Find information about how to use the EWS Managed API to communicate with EWS in Exchange.</span></span>
  
<span data-ttu-id="c81b3-105">EWS のマネージ API では、 [ExchangeService](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)クラスには、メソッドとプロパティを使用して、ユーザーの資格情報を設定、EWS のエンドポイントを識別する、送信 SOAP メッセージを受信し、EWS を使って通信するためにバインドを設定することが含まれています。</span><span class="sxs-lookup"><span data-stu-id="c81b3-105">The [ExchangeService](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) class in the EWS Managed API contains the methods and properties that you use to set user credentials, identify the EWS endpoint, send and receive SOAP messages, and configure the binding to communicate with EWS.</span></span> <span data-ttu-id="c81b3-106">EWS のマネージ API を使用するには任意のタスクを実行するのには、前に、 **ExchangeService**クラスのインスタンスを作成し、EWS にバインドする必要があります。</span><span class="sxs-lookup"><span data-stu-id="c81b3-106">Before you can use the EWS Managed API to perform any task, you have to create an instance of the **ExchangeService** class and bind it to EWS.</span></span> 
  
<span data-ttu-id="c81b3-107">ユーザーの資格情報を持つ[ExchangeService](https://msdn.microsoft.com/library/Microsoft.Exchange.WebServices.Data.ExchangeService.aspx)オブジェクトと、EWS のエンドポイントを設定した後[ExchangeService](https://msdn.microsoft.com/library/Microsoft.Exchange.WebServices.Data.ExchangeService.aspx)オブジェクトを参照するすべてのメールボックス オブジェクトは、EWS を使って通信するために次のメソッドの型を使用できます。</span><span class="sxs-lookup"><span data-stu-id="c81b3-107">After you set up an [ExchangeService](https://msdn.microsoft.com/library/Microsoft.Exchange.WebServices.Data.ExchangeService.aspx) object with user credentials and the EWS endpoint, any mailbox object that references the [ExchangeService](https://msdn.microsoft.com/library/Microsoft.Exchange.WebServices.Data.ExchangeService.aspx) object can use the following method types to communicate with EWS:</span></span> 
  
- <span data-ttu-id="c81b3-108">ExchangeService オブジェクトのメソッド、**オブジェクト**の基本型から継承されていない**ExchangeService**オブジェクト上のすべてのメソッドは、EWS に電話をかけます。</span><span class="sxs-lookup"><span data-stu-id="c81b3-108">ExchangeService object methods — All the methods on the **ExchangeService** object that are not inherited from the base **Object** type make calls to EWS.</span></span> 
    
- <span data-ttu-id="c81b3-109">Exchange のメールボックス アイテム タイプ メソッドとフォルダー タイプ メソッド。</span><span class="sxs-lookup"><span data-stu-id="c81b3-109">Exchange mailbox item and folder type methods.</span></span>
    
<span data-ttu-id="c81b3-110">**表 1 です。メールボックス アイテムおよびフォルダー通信 EWS のメソッドを入力します。**</span><span class="sxs-lookup"><span data-stu-id="c81b3-110">**Table 1. Mailbox item and folder type methods that communicate with EWS**</span></span>

|<span data-ttu-id="c81b3-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="c81b3-111">Method</span></span>|<span data-ttu-id="c81b3-112">できること</span><span class="sxs-lookup"><span data-stu-id="c81b3-112">What it does</span></span>|<span data-ttu-id="c81b3-113">呼び出す操作</span><span class="sxs-lookup"><span data-stu-id="c81b3-113">Operations that it calls</span></span>|
|:-----|:-----|:-----|
|[<span data-ttu-id="c81b3-114">Load</span><span class="sxs-lookup"><span data-stu-id="c81b3-114">Load</span></span>](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.item.load%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="c81b3-115">アイテム、添付ファイル、またはユーザー構成オブジェクトのプロパティを取得します。 </span><span class="sxs-lookup"><span data-stu-id="c81b3-115">Gets properties on an item, attachment, or user configuration object.</span></span>  <br/> |<span data-ttu-id="c81b3-116">
  [GetItem 操作](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="c81b3-116">[GetItem operation](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx)</span></span> <br/><br/> [<span data-ttu-id="c81b3-117">GetAttachment 操作</span><span class="sxs-lookup"><span data-stu-id="c81b3-117">GetAttachment operation</span></span>](http://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx) <br/><br/> [<span data-ttu-id="c81b3-118">GetUserConfiguration 操作</span><span class="sxs-lookup"><span data-stu-id="c81b3-118">GetUserConfiguration operation</span></span>](http://msdn.microsoft.com/library/71d50e3c-92bd-435f-8118-b28bb85f8138%28Office.15%29.aspx) <br/> |
|[<span data-ttu-id="c81b3-119">バインド</span><span class="sxs-lookup"><span data-stu-id="c81b3-119">Bind</span></span>](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="c81b3-120">クライアント上の新しいアイテムに、サーバー上の既存のアイテムからの情報を取り込みます</span><span class="sxs-lookup"><span data-stu-id="c81b3-120">Populates a new item on the client with information from an existing item on the server.</span></span>  <br/> |<span data-ttu-id="c81b3-121">
  [GetItem 操作](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="c81b3-121">[GetItem operation](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx)</span></span> <br/> |
|[<span data-ttu-id="c81b3-122">Save</span><span class="sxs-lookup"><span data-stu-id="c81b3-122">Save</span></span>](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.item.save%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="c81b3-123">サーバー上のクライアント アイテムのコピーを保存します。</span><span class="sxs-lookup"><span data-stu-id="c81b3-123">Saves the copy of the client item on the server.</span></span>  <br/> |<span data-ttu-id="c81b3-124">
  [UpdateItem 操作](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="c81b3-124">[UpdateItem operation](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span></span> <br/><br/> <span data-ttu-id="c81b3-125">
  [UpdateFolder 操作](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="c81b3-125">[UpdateFolder operation](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx)</span></span> <br/><br/><span data-ttu-id="c81b3-126">
  [CreateItem 操作](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="c81b3-126">[CreateItem operation](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx)</span></span> <br/><br/><span data-ttu-id="c81b3-127">
  [CreateFolder 操作](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="c81b3-127">[CreateFolder operation](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx)</span></span> <br/> |
|[<span data-ttu-id="c81b3-128">Update</span><span class="sxs-lookup"><span data-stu-id="c81b3-128">Update</span></span>](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.item.update%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="c81b3-129">クライアント上で加えられた変更でサーバーを更新します。</span><span class="sxs-lookup"><span data-stu-id="c81b3-129">Updates the server with the changes made on the client.</span></span><br/><br/><span data-ttu-id="c81b3-130">アイテムとフォルダーの場合は、 **Update**メソッドは、 [UpdateItem 操作](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)および[UpdateFolder 操作](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx)を使用します。</span><span class="sxs-lookup"><span data-stu-id="c81b3-130">For items and folders, the **Update** method uses the [UpdateItem operation](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) and the [UpdateFolder operation](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx).</span></span>  <br/> |<span data-ttu-id="c81b3-131">
  [UpdateItem 操作](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="c81b3-131">[UpdateItem operation](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span></span> <br/><br/><span data-ttu-id="c81b3-132">
  [UpdateFolder 操作](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="c81b3-132">[UpdateFolder operation](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx)</span></span> <br/> |
|[<span data-ttu-id="c81b3-133">Delete</span><span class="sxs-lookup"><span data-stu-id="c81b3-133">Delete</span></span>](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.item.delete%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="c81b3-134">サーバー上のアイテムを削除します。</span><span class="sxs-lookup"><span data-stu-id="c81b3-134">Deletes an item on the server.</span></span><br/><br/><span data-ttu-id="c81b3-135">アイテムとフォルダーの場合は、 **Delete**メソッドと、 [DeleteFolder の操作](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx)を使用します。</span><span class="sxs-lookup"><span data-stu-id="c81b3-135">For items and folders, the **Delete** method uses the and the [DeleteFolder operation](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx).</span></span>  <br/> |[<span data-ttu-id="c81b3-136">DeleteItem の操作</span><span class="sxs-lookup"><span data-stu-id="c81b3-136">DeleteItem operation</span></span>](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/><br/> [<span data-ttu-id="c81b3-137">DeleteFolder 操作</span><span class="sxs-lookup"><span data-stu-id="c81b3-137">DeleteFolder operation</span></span>](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |
|[<span data-ttu-id="c81b3-138">Copy</span><span class="sxs-lookup"><span data-stu-id="c81b3-138">Copy</span></span>](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.item.copy%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="c81b3-139">サーバー上のアイテムまたはフォルダーのコピーを作成します。 </span><span class="sxs-lookup"><span data-stu-id="c81b3-139">Creates a copy of the item or folders on the server.</span></span>  <br/> |<span data-ttu-id="c81b3-140">
  [CopyItem 操作](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="c81b3-140">[CopyItem operation](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx)</span></span> <br/><br/> [<span data-ttu-id="c81b3-141">CopyFolder 操作</span><span class="sxs-lookup"><span data-stu-id="c81b3-141">CopyFolder operation</span></span>](http://msdn.microsoft.com/library/c7ea0d68-9793-4144-b378-d99536776db9%28Office.15%29.aspx) <br/> |
|[<span data-ttu-id="c81b3-142">移動</span><span class="sxs-lookup"><span data-stu-id="c81b3-142">Move</span></span>](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.item.move%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="c81b3-143">サーバー上のアイテムまたはフォルダーを移動します。 </span><span class="sxs-lookup"><span data-stu-id="c81b3-143">Moves items or folders on the server.</span></span>  <br/> |<span data-ttu-id="c81b3-144">
  [MoveItem 操作](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="c81b3-144">[MoveItem operation](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx)</span></span> <br/><br/> [<span data-ttu-id="c81b3-145">MoveFolder 操作</span><span class="sxs-lookup"><span data-stu-id="c81b3-145">MoveFolder operation</span></span>](http://msdn.microsoft.com/library/c7233966-6c87-4a14-8156-b1610760176d%28Office.15%29.aspx) <br/> |
   
## <a name="to-use-the-ews-managed-api-to-communicate-with-ews"></a><span data-ttu-id="c81b3-146">EWS マネージ API を使用して EWS と通信するには</span><span class="sxs-lookup"><span data-stu-id="c81b3-146">To use the EWS Managed API to communicate with EWS</span></span>

1. <span data-ttu-id="c81b3-147">**ExchangeService**クラスのインスタンスを作成します。</span><span class="sxs-lookup"><span data-stu-id="c81b3-147">Instantiate the **ExchangeService** class.</span></span> 
    
   ```csharp
    ExchangeService service = new ExchangeService();
   ```

   > [!NOTE]
   > <span data-ttu-id="c81b3-148">**ExchangeService**の空のコンス トラクターでインスタンス化すると、Exchange の最新の既知のバージョンにバインドされているインスタンスが作成されます。</span><span class="sxs-lookup"><span data-stu-id="c81b3-148">Instantiating **ExchangeService** with an empty constructor will create an instance that is bound to the latest known version of Exchange.</span></span> <span data-ttu-id="c81b3-149">代わりに、パラメーターとしてバージョンを指定することによって Exchange の特定のバージョンをターゲットことができます。</span><span class="sxs-lookup"><span data-stu-id="c81b3-149">Alternatively, you can target a specific version of Exchange by specifying version as a parameter.</span></span> `ExchangeService service = new ExchangeService(ExchangeVersion.Exchange2007_SP1);`
  
2. <span data-ttu-id="c81b3-150">Exchange サーバーに要求を送信したユーザーの資格情報を設定します。</span><span class="sxs-lookup"><span data-stu-id="c81b3-150">Set the credentials of the user who sends requests to the Exchange server.</span></span> <span data-ttu-id="c81b3-151">EWS にドメインにログオンしているコンピューターから接続する場合は、場合は、 **true を指定**する**ExchangeService**オブジェクトを**偽造している**プロパティを設定、認証されたユーザーの資格情報を使用します。</span><span class="sxs-lookup"><span data-stu-id="c81b3-151">If you want to connect to EWS from a computer that is logged on to the domain, using the credentials of the authenticated user, set the **UseDefaultCredentials** property on the **ExchangeService** object to **true**.</span></span>
    
   ```cs
    // Connect by using the default credentials of the authenticated user.
    service.UseDefaultCredentials = true;
   ```

   <span data-ttu-id="c81b3-152">既定のユーザー資格情報を使用して接続したくない場合は、別のユーザーの資格情報を明示的に指定する**ExchangeService**オブジェクトに**資格情報**のプロパティを設定します。</span><span class="sxs-lookup"><span data-stu-id="c81b3-152">If you do not want to connect by using the default user credentials, set the **Credentials** property on the **ExchangeService** object to explicitly specify the credentials of a different user.</span></span> <span data-ttu-id="c81b3-153">Office 365 の一部として Exchange Online または Exchange Online を使用する場合、ユーザー名とパスワードだけで基本認証を使用します。</span><span class="sxs-lookup"><span data-stu-id="c81b3-153">If you are using Exchange Online or Exchange Online as part of Office 365, you'll use basic authentication, with just a user name and password.</span></span> <span data-ttu-id="c81b3-154">ドメイン名は、NTLM 認証に必要です。</span><span class="sxs-lookup"><span data-stu-id="c81b3-154">A domain name is required for NTLM authentication.</span></span> 
    
   ```cs
    // Connect by using the credentials of user1 at contoso.com.
    service.Credentials = new WebCredentials("user1@contoso.com", "password");
   ```

   <span data-ttu-id="c81b3-155">ユーザーのドメイン名とパスワードを使用して、ユーザーの資格情報を指定することもできます。</span><span class="sxs-lookup"><span data-stu-id="c81b3-155">You can also specify the credentials of the user by using the user's domain name and password.</span></span>
    
   ```cs
    // Connect by using the credentials of contoso/user1.
    service.Credentials = new WebCredentials("user1", "password", "contoso");
   ```

   > [!NOTE]
   > <span data-ttu-id="c81b3-156">**偽造している****場合は true**に設定すると、**資格情報**のプロパティの値は無視されます。</span><span class="sxs-lookup"><span data-stu-id="c81b3-156">If the **UseDefaultCredentials** property is set to **true**, the value of the **Credentials** property is ignored.</span></span> 
  
3. <span data-ttu-id="c81b3-p105">EWS エンドポイントの URL を設定します。この URL は、クライアント アクセス サーバー上の exchange.asmx ファイルの場所を示します。</span><span class="sxs-lookup"><span data-stu-id="c81b3-p105">Set the URL of the EWS endpoint. This URL locates the exchange.asmx file on Client Access server.</span></span>
    
   ```cs
    // Use Autodiscover to set the URL endpoint.
    service.AutodiscoverUrl("user1@contoso.com");
   ```

   > [!NOTE]
   >  <span data-ttu-id="c81b3-159">ハードコードされた値を**ExchangeService**の**Url**プロパティを明示的に設定することができます、お勧めする自動検出サービス代わりに使用する、次の理由で: > 自動検出は、ユーザーごとに最適なエンドポイントを決定(エンドポイントは、ユーザーのメールボックス サーバーに最も近い) です。</span><span class="sxs-lookup"><span data-stu-id="c81b3-159">Although you can explicitly set the **Url** property of the **ExchangeService** to a hardcoded value, we recommend that you use the Autodiscover service instead, for the following reasons: >  Autodiscover determines the best endpoint for a given user (the endpoint that is closest to the user's Mailbox server).</span></span> <span data-ttu-id="c81b3-160">> EWS の URL は、新しいクライアント アクセス サーバーが配置されている場合に変更可能性があります。</span><span class="sxs-lookup"><span data-stu-id="c81b3-160">>  The EWS URL might change if new Client Access servers are deployed.</span></span> <span data-ttu-id="c81b3-161">このシナリオでは、[自動検出](autodiscover-for-exchange.md)を使用することを意味コードを変更する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="c81b3-161">In this scenario, using [Autodiscover](autodiscover-for-exchange.md) means no code changes are necessary.</span></span> <span data-ttu-id="c81b3-162">> する必要がありますか、URL を明示的に設定、または**AutodiscoverUrl**が、どちらも行う必要があります。</span><span class="sxs-lookup"><span data-stu-id="c81b3-162">>  You should either set the URL explicitly or call **AutodiscoverUrl**, but you should not do both.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="c81b3-163">関連項目</span><span class="sxs-lookup"><span data-stu-id="c81b3-163">See also</span></span>

- [<span data-ttu-id="c81b3-164">EWS マネージ API クライアント アプリケーションの概要</span><span class="sxs-lookup"><span data-stu-id="c81b3-164">Get started with EWS Managed API client applications</span></span>](get-started-with-ews-managed-api-client-applications.md) 
- [<span data-ttu-id="c81b3-165">自動検出を使用してコネクション ポイントを検索するには</span><span class="sxs-lookup"><span data-stu-id="c81b3-165">Use Autodiscover to find connection points</span></span>](how-to-use-autodiscover-to-find-connection-points.md)   
- [<span data-ttu-id="c81b3-166">Exchange の Web サービス クライアントを開発する</span><span class="sxs-lookup"><span data-stu-id="c81b3-166">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    

