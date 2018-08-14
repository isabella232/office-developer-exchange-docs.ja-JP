---
title: Exchange で EWS を使用してユーザーの写真を取得する
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: f86d1099-1f57-47dc-abf2-4d5ae4e900a9
description: Exchange の EWS マネージ API または EWS を使用して、メールボックスまたは連絡先に関連付けられているユーザーの写真を取得する方法について説明します。
ms.openlocfilehash: f0f5cddd41fc563fb9ed38e75b505830a3992411
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758987"
---
# <a name="get-user-photos-by-using-ews-in-exchange"></a><span data-ttu-id="791b2-103">Exchange で EWS を使用してユーザーの写真を取得する</span><span class="sxs-lookup"><span data-stu-id="791b2-103">How to: Get user photos by using EWS in Exchange</span></span>

<span data-ttu-id="791b2-104">Exchange の EWS マネージ API または EWS を使用して、メールボックスまたは連絡先に関連付けられているユーザーの写真を取得する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="791b2-104">Learn how to get user photos that are associated with a mailbox or contact by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="791b2-p101">顔と名前を並べて配置すると便利です。ユーザーが顔と名前を並べて配置することを望む場合は、アプリケーションから Exchange にある電子メール アカウントを表すイメージ (通常は写真) を要求できます。Exchange サーバーに保存されたメールボックス用のユーザーの写真を取得することも、自分のメールボックスに保存されている連絡先から得た連絡先の写真を取得することもできます。</span><span class="sxs-lookup"><span data-stu-id="791b2-p101">It's nice to put a face to a name. If your users like to put names to faces, your application can request an image, typically a photo, from Exchange that represents an email account. You can get a user photo stored on an Exchange server for a mailbox, or you can get a contact photo from contacts stored in your mailbox.</span></span>
  
<span data-ttu-id="791b2-108">数種のテクノロジを使用して、メールボックスまたは Active Directory ドメイン サービス (AD DS) から写真を取得できます。</span><span class="sxs-lookup"><span data-stu-id="791b2-108">You can use several different technologies to get photos from mailboxes or Active Directory Domain Services (AD DS).</span></span> <span data-ttu-id="791b2-109">写真を取得するための最適な方法は、どの種類の連絡先から写真を取得するかによって異なります。</span><span class="sxs-lookup"><span data-stu-id="791b2-109">You can use several different technologies to get photos from mailboxes or Active Directory Domain Services (AD DS). The best way to get a photo depends on the type of contact that you want to get a photo from.</span></span> 
  
<span data-ttu-id="791b2-110">**表 1. ユーザーの写真を取得するために連絡先の種類に基づいて使用するテクノロジ**</span><span class="sxs-lookup"><span data-stu-id="791b2-110">**Table 1.  Technologies to use to get user photos based on contact type**</span></span>

|<span data-ttu-id="791b2-111">**連絡先の種類**</span><span class="sxs-lookup"><span data-stu-id="791b2-111">**Contact type**</span></span>|<span data-ttu-id="791b2-112">**使用するテクノロジ**</span><span class="sxs-lookup"><span data-stu-id="791b2-112">**Technologies to use**</span></span>|
|:-----|:-----|
|<span data-ttu-id="791b2-113">メールボックス ユーザーの写真</span><span class="sxs-lookup"><span data-stu-id="791b2-113">Mailbox user photo</span></span>  <br/> |[<span data-ttu-id="791b2-114">REST を使用してメールボックス ユーザーの写真を取得する</span><span class="sxs-lookup"><span data-stu-id="791b2-114">Get a mailbox user photo by using REST</span></span>](#bk_REST)<br/><br/> [<span data-ttu-id="791b2-115">EWS を使用してユーザーの写真を取得する</span><span class="sxs-lookup"><span data-stu-id="791b2-115">Get a contact user photo by using EWS Managed API</span></span>](#bk_EWS) <br/> |
|<span data-ttu-id="791b2-116">連絡先ユーザーの写真</span><span class="sxs-lookup"><span data-stu-id="791b2-116">Contact user photo</span></span>  <br/> |[<span data-ttu-id="791b2-117">EWS マネージ API を使用して連絡先ユーザーの写真を取得する</span><span class="sxs-lookup"><span data-stu-id="791b2-117">Get a contact user photo by using EWS Managed API</span></span>](#bk_EWSMA)<br/><br/> [<span data-ttu-id="791b2-118">EWS を使用してユーザーの写真を取得する</span><span class="sxs-lookup"><span data-stu-id="791b2-118">Get a contact user photo by using EWS Managed API</span></span>](#bk_EWS) <br/> |

<span data-ttu-id="791b2-119"><a name="bk_REST"> </a></span><span class="sxs-lookup"><span data-stu-id="791b2-119"></span></span>

## <a name="get-a-mailbox-user-photo-by-using-rest"></a><span data-ttu-id="791b2-120">REST を使用してメールボックス ユーザーの写真を取得する</span><span class="sxs-lookup"><span data-stu-id="791b2-120">Get a mailbox user photo by using REST</span></span>

<span data-ttu-id="791b2-121">標準の HTTPS **GET** 要求を使用することで、Exchange サーバーのユーザーの写真を要求できます。</span><span class="sxs-lookup"><span data-stu-id="791b2-121">You can request user photos from an Exchange server by using a standard HTTPS **GET** request. In the request, specify the email account address and a size code for the image, as shown in the following example.</span></span> <span data-ttu-id="791b2-122">この要求では、次の例に示すように、電子メール アカウント アドレスとイメージのサイズ コードを指定しています。</span><span class="sxs-lookup"><span data-stu-id="791b2-122">You can request user photos from an Exchange server by using a standard HTTPS GET request. In the request, specify the email account address and a size code for the image, as shown in the following example.</span></span> 
  
```HTML
https://Exchange Server/ews/Exchange.asmx/s/GetUserPhoto?email=email address&amp;size=size code
```

<span data-ttu-id="791b2-123">自動検出サービスの [GetUserSettings](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) 操作を使用して **ExternalEwsUrl** 設定を取得します。この設定には、Exchange Web サービス (EWS) エンドポイントの URL と、ユーザーの写真を返す **Exchange.asmx** HTTP ハンドラーの場所が含まれています。</span><span class="sxs-lookup"><span data-stu-id="791b2-123">Use the Autodiscover service [GetUserSettings](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) operation to retrieve the **ExternalEwsUrl** setting, which contains the URL of the Exchange Web Services (EWS) endpoint and the location of the **Exchange.asmx** HTTP handler that returns the user photos.</span></span> 
  
<span data-ttu-id="791b2-124">それぞれのサイズ コードは、イメージの高さと幅をピクセル単位で示しています。</span><span class="sxs-lookup"><span data-stu-id="791b2-124">Each size code indicates the height and width of the image in pixels.</span></span> <span data-ttu-id="791b2-125">たとえば、サイズ コード **HR48x48** は、高さ 48 ピクセル × 幅 48 ピクセルのイメージを返します。</span><span class="sxs-lookup"><span data-stu-id="791b2-125">For example, the size code **HR48x48** returns an image that is 48 pixels high by 48 pixels wide.</span></span> <span data-ttu-id="791b2-126">サイズ コード パラメーターに有効な値は、[SizeRequested](http://msdn.microsoft.com/library/e86f98b6-83b5-4530-80eb-dc5df42e2c62%28Office.15%29.aspx) 要素に有効な値と同じになります。</span><span class="sxs-lookup"><span data-stu-id="791b2-126">The possible values for the size code parameter are the same as the possible values for the [SizeRequested](http://msdn.microsoft.com/library/e86f98b6-83b5-4530-80eb-dc5df42e2c62%28Office.15%29.aspx) element.</span></span> <span data-ttu-id="791b2-127">要求で指定したサイズが使用できない場合は、使用可能な最大の写真が返されます。</span><span class="sxs-lookup"><span data-stu-id="791b2-127">If the request specifies a size that is not available, the largest available photo will be returned.</span></span> <span data-ttu-id="791b2-128">Exchange サーバーに写真が保存されていない場合は、そのアカウント用に AD DS に保存されているサムネイル イメージが返されます。</span><span class="sxs-lookup"><span data-stu-id="791b2-128">If no photo is stored on the Exchange server, the thumbnail image stored in AD DS for the account will be returned.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="791b2-129">**HR48x48** サイズ コードは、常に AD DS サムネイル イメージを返します (使用可能な場合)。</span><span class="sxs-lookup"><span data-stu-id="791b2-129">The **HR48x48** size code always returns the AD DS thumbnail image if it is available.</span></span> 
  
<span data-ttu-id="791b2-130">次の例は、GET 要求を使用して Sadie のユーザー写真を取得して、ローカル コンピューターに保存する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="791b2-130">The following example shows how you can use the GET request to retrieve the user photo for Sadie and save it to your local computer.</span></span>
  
```cs
// Create the web request with the REST URL.
HttpWebRequest request = 
   WebRequest.Create("https://www.contoso.com/ews/exchange.asmx/s/GetUserPhoto?email=sadie@contoso.com&amp;size=HR240x240") 
   as HttpWebRequest;
// Submit the request.
using (HttpWebResponse resp = request.GetResponse() as HttpWebResponse)
{
   // Take the response and save it as an image.
   Bitmap image = new Bitmap(resp.GetResponseStream());
   image.Save("Sadie.jpg");
}

```

<span data-ttu-id="791b2-131">この要求により、HTTP 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="791b2-131">The request will return an HTTP response.</span></span> 
  
<span data-ttu-id="791b2-132">**表 2. GetUserPhoto 要求の応答コード**</span><span class="sxs-lookup"><span data-stu-id="791b2-132">**Table 2.  Response codes for a GetUserPhoto request**</span></span>

|<span data-ttu-id="791b2-133">**応答コード**</span><span class="sxs-lookup"><span data-stu-id="791b2-133">**Response code**</span></span>|<span data-ttu-id="791b2-134">**説明**</span><span class="sxs-lookup"><span data-stu-id="791b2-134">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="791b2-135">200</span><span class="sxs-lookup"><span data-stu-id="791b2-135">200</span></span>  <br/> |<span data-ttu-id="791b2-136">指定された電子メール アカウントのイメージが使用可能であり、応答にはバイナリ イメージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="791b2-136">An image is available for the specified email account and the binary image is contained in the response.</span></span>  <br/> |
|<span data-ttu-id="791b2-137">304</span><span class="sxs-lookup"><span data-stu-id="791b2-137">304</span></span>  <br/> |<span data-ttu-id="791b2-138">イメージは前回 **ETag** がアプリケーションに返したものから変更されていません。</span><span class="sxs-lookup"><span data-stu-id="791b2-138">The image has not changed since the last time the **ETag** was returned to the application.</span></span>  <br/> |
|<span data-ttu-id="791b2-139">404</span><span class="sxs-lookup"><span data-stu-id="791b2-139">404</span></span>  <br/> |<span data-ttu-id="791b2-140">指定された電子メール アカウントに使用可能なイメージがありません。</span><span class="sxs-lookup"><span data-stu-id="791b2-140">No image is available for the specified email account.</span></span>  <br/> |

<span data-ttu-id="791b2-141"><a name="bk_REST"> </a></span><span class="sxs-lookup"><span data-stu-id="791b2-141"></span></span>

## <a name="cache-user-photos"></a><span data-ttu-id="791b2-142">ユーザーの写真をキャッシュする</span><span class="sxs-lookup"><span data-stu-id="791b2-142">Cache user photos</span></span>

<span data-ttu-id="791b2-143">Exchange は、コンテンツの種類が image/jpeg のデータをヘッダー値のコレクションと共に返します。</span><span class="sxs-lookup"><span data-stu-id="791b2-143">Exchange returns the data with a content type of image/jpeg, along with a collection of header values.</span></span> <span data-ttu-id="791b2-144">**ETag** ヘッダーは、変更キーと同様のものです。</span><span class="sxs-lookup"><span data-stu-id="791b2-144">The **ETag** header is similar to a change key.</span></span> <span data-ttu-id="791b2-145">この値は、前回写真が更新されたことを表す文字列です。</span><span class="sxs-lookup"><span data-stu-id="791b2-145">The value is a string that represents the last time the photo was updated.</span></span> <span data-ttu-id="791b2-146">**ETag** は、写真が変更されるまでユーザーの写真に対して同じままに保たれます。</span><span class="sxs-lookup"><span data-stu-id="791b2-146">The **ETag** remains the same for the user photo until the photo is changed.</span></span> <span data-ttu-id="791b2-147">この **ETag** 値は、HTTPS **GET** 要求の **If-None-Match** ヘッダーでサーバーに送信できます。</span><span class="sxs-lookup"><span data-stu-id="791b2-147">You can send this **ETag** value to the server in the HTTPS **GET** request in an **If-None-Match** header.</span></span> <span data-ttu-id="791b2-148">前回の要求以降に写真が変更されていない場合は、それを表す HTTP 304 応答でサーバーが応答します。</span><span class="sxs-lookup"><span data-stu-id="791b2-148">If the photo hasn't changed since the last request, the server will respond with an HTTP 304 response that indicates as such.</span></span> <span data-ttu-id="791b2-149">そのため、新しいユーザーの写真を処理するのではなく、以前に要求して保存しておいたものを使用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="791b2-149">This means that you can use the user photo that you previously requested and saved rather than processing a new one.</span></span> 

<span data-ttu-id="791b2-150"><a name="bk_EWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="791b2-150"></span></span>

## <a name="get-a-contact-user-photo-by-using-ews-managed-api"></a><span data-ttu-id="791b2-151">EWS マネージ API を使用して連絡先ユーザーの写真を取得する</span><span class="sxs-lookup"><span data-stu-id="791b2-151">Get a contact user photo by using EWS Managed API</span></span>

<span data-ttu-id="791b2-152">アプリケーションでは EWS マネージ API を使用して連絡先の写真を取得できます (連絡先がユーザーのメールボックスの連絡先フォルダーに保存されている場合)。</span><span class="sxs-lookup"><span data-stu-id="791b2-152">Your application can use the EWS Managed API to retrieve photos for contacts, if the contact is stored in a contact folder in the user's mailbox.</span></span> <span data-ttu-id="791b2-153">これを行うには、まず、使用する連絡先の **ItemId** を見つけます。</span><span class="sxs-lookup"><span data-stu-id="791b2-153">To do this, first, find the **ItemId** for the contact you want use.</span></span> <span data-ttu-id="791b2-154">次に、その連絡先にバインドしてから、添付ファイルのコレクションに読み込みます。</span><span class="sxs-lookup"><span data-stu-id="791b2-154">Then, after you bind to that contact, load it to the attachments collection.</span></span> <span data-ttu-id="791b2-155">連絡先に写真がある場合は、写真が添付ファイルの 1 つに含まれています。</span><span class="sxs-lookup"><span data-stu-id="791b2-155">If the contact has a photo, the photo will be one of the attachments.</span></span> <span data-ttu-id="791b2-156">添付ファイルのコレクションをループして、**IsContactPhoto** プロパティの値を確認します。</span><span class="sxs-lookup"><span data-stu-id="791b2-156">Loop through the attachments collection, checking the value of the **IsContactPhoto** property.</span></span> <span data-ttu-id="791b2-157">連絡先の写真を見つけたら、その写真をローカル コンピューターに保存して、アプリケーションからアクセスできるようにします。</span><span class="sxs-lookup"><span data-stu-id="791b2-157">When you find the contact photo, you can save it to your local computer, and your application can access it.</span></span> 
  
<span data-ttu-id="791b2-158">次の例は、このプロセスを示しています。</span><span class="sxs-lookup"><span data-stu-id="791b2-158">The following code example shows this operation.</span></span> <span data-ttu-id="791b2-159">この例では、**service** が有効な [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーから既に認証されていると想定しています。</span><span class="sxs-lookup"><span data-stu-id="791b2-159">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
private static void GetContactPhoto(ExchangeService service, string ItemId)
{
   // Bind to an existing contact by using the ItemId passed into this function.
   Contact contact = Contact.Bind(service, ItemId);
   // Load the contact to get access to the collection of attachments.
   contact.Load(new PropertySet(ContactSchema.Attachments));
   // Loop through the attachments looking for a contact photo.
   foreach (Attachment attachment in contact.Attachments)
   {
      if ((attachment as FileAttachment).IsContactPhoto)
      {
         // Load the attachment to access the content.
         attachment.Load();
      }
   }
   FileAttachment photo = contact.GetContactPictureAttachment();
   // Create a file stream and save the contact photo to your computer.
   using (FileStream file = new FileStream(photo.Name, FileMode.Create, System.IO.FileAccess.Write))
   {
      photo.Load(file);
   }
}

```

<span data-ttu-id="791b2-160"><a name="bk_EWS"> </a></span><span class="sxs-lookup"><span data-stu-id="791b2-160"></span></span>

## <a name="get-a-user-photo-by-using-ews"></a><span data-ttu-id="791b2-161">EWS を使用してユーザーの写真を取得する</span><span class="sxs-lookup"><span data-stu-id="791b2-161">Get a contact user photo by using EWS Managed API</span></span>

<span data-ttu-id="791b2-162">ユーザーの写真を AD DS から取得するときに、電子メール アドレスがわかっている場合は [GetUserPhoto](http://msdn.microsoft.com/library/f6e8143d-4235-428e-8f9c-ab6e9b1cfa6e%28Office.15%29.aspx) 操作を使用し、電子メール アドレスがわからない場合は [ResolveNames](http://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) 操作を使用します。</span><span class="sxs-lookup"><span data-stu-id="791b2-162">If you're getting a user photo from AD DS, you can use the [GetUserPhoto](http://msdn.microsoft.com/library/f6e8143d-4235-428e-8f9c-ab6e9b1cfa6e%28Office.15%29.aspx) operation (if you know the email address) or the [ResolveNames](http://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) operation (if you don't know the email address).</span></span> <span data-ttu-id="791b2-163">メールボックスの連絡先フォルダーからユーザーの写真を取得する場合は、[GetItem](http://msdn.microsoft.com/library/6b96dace-1260-4b83-869a-7c31c5583daa%28Office.15%29.aspx) 操作に続けて [GetAttachment](http://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx) 操作を使用します。</span><span class="sxs-lookup"><span data-stu-id="791b2-163">If you're getting a user photo from a contacts folder in the mailbox, use the [GetItem](http://msdn.microsoft.com/library/6b96dace-1260-4b83-869a-7c31c5583daa%28Office.15%29.aspx) operation followed by the [GetAttachment](http://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx) operation.</span></span> <span data-ttu-id="791b2-164">どちらの場合も、写真は Base64 エンコード文字列として XML 応答で返されます。</span><span class="sxs-lookup"><span data-stu-id="791b2-164">In either case, the photo is returned as a Base64-encoded string in the XML response.</span></span> 
  
### <a name="get-a-mailbox-user-photo-by-using-the-getuserphoto-operation"></a><span data-ttu-id="791b2-165">GetUserPhoto 操作を使用してメールボックス ユーザーの写真を取得する</span><span class="sxs-lookup"><span data-stu-id="791b2-165">Get a mailbox user photo by using the GetUserPhoto operation</span></span>

<span data-ttu-id="791b2-166">**GetUserPhoto** 操作を使用すると、簡単になります。</span><span class="sxs-lookup"><span data-stu-id="791b2-166">Using the **GetUserPhoto** operation is straightforward.</span></span> <span data-ttu-id="791b2-167">XML 要求では、ユーザーの電子メール アドレスと、返される[写真のサイズ](http://msdn.microsoft.com/library/e86f98b6-83b5-4530-80eb-dc5df42e2c62%28Office.15%29.aspx)を指定します ([SizeRequested](http://msdn.microsoft.com/library/e86f98b6-83b5-4530-80eb-dc5df42e2c62%28Office.15%29.aspx) 要素内)。</span><span class="sxs-lookup"><span data-stu-id="791b2-167">Using the GetUserPhoto operation is straightforward. In the XML request, specify the email address of the user, and the [size of the photo](http://msdn.microsoft.com/library/e86f98b6-83b5-4530-80eb-dc5df42e2c62%28Office.15%29.aspx) to return (in the [SizeRequested](http://msdn.microsoft.com/library/e86f98b6-83b5-4530-80eb-dc5df42e2c62%28Office.15%29.aspx) element). The following XML request example shows how to get a photo for Sadie Daniels that's 360 pixels wide by 360 pixels high.</span></span> <span data-ttu-id="791b2-168">次の XML 要求の例は、幅 360 ピクセル×高さ 360 ピクセルの Sadie Daniels の写真を取得する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="791b2-168">Using the GetUserPhoto operation is straightforward. In the XML request, specify the email address of the user, and the size of the photo to return (in the SizeRequested element). The following XML request example shows how to get a photo for Sadie Daniels that's 360 pixels wide by 360 pixels high.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013 "/>
   </soap:Header>
   <soap:Body>
      <m:GetUserPhoto>
         <m:Email>sadie@contoso.com</m:Email>
         <m:SizeRequested>HR360x360</m:SizeRequested>
      </m:GetUserPhoto>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="791b2-169">次に、XML 応答を示します。</span><span class="sxs-lookup"><span data-stu-id="791b2-169">The following is the XML response.</span></span> <span data-ttu-id="791b2-170">Base64 エンコードされた写真が [PictureData](http://msdn.microsoft.com/library/1124eac3-ebf2-4b81-96d3-96838c840433%28Office.15%29.aspx) 要素に含まれています (読みやすくするために内容が短縮されています)。</span><span class="sxs-lookup"><span data-stu-id="791b2-170">The following is the XML response. The Base64-encoded photo is contained in the [PictureData](http://msdn.microsoft.com/library/1124eac3-ebf2-4b81-96d3-96838c840433%28Office.15%29.aspx) element (the content has been shortened for readability).</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
         xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetUserPhotoResponse ResponseClass="Success" 
         xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <HasChanged>true</HasChanged>
      <PictureData>/9j/4AAQSkZJRgABAQEAYABgAAD/2wBDAAg... wATRRRSuB//2Q==</PictureData>
    </GetUserPhotoResponse>
  </s:Body>
</s:Envelope>

```

### <a name="get-a-mailbox-user-photo-by-using-the-resolvenames-operation"></a><span data-ttu-id="791b2-171">ResolveNames 操作を使用してメールボックス ユーザーの写真を取得する</span><span class="sxs-lookup"><span data-stu-id="791b2-171">Get a mailbox user photo by using the ResolveNames operation</span></span>

<span data-ttu-id="791b2-172">写真を取得するユーザーの電子メール アドレスがわからない場合は、[ResolveNames 操作を使用する](how-to-resolve-ambiguous-names-by-using-ews-in-exchange-2013.md)ことで一致する可能性のある候補を取得できます。</span><span class="sxs-lookup"><span data-stu-id="791b2-172">If you don't know the email address of the user for whom you are getting a photo, you can [use the ResolveNames operation](how-to-resolve-ambiguous-names-by-using-ews-in-exchange-2013.md) to get candidates for a possible match.</span></span> <span data-ttu-id="791b2-173">[ResolveNames](http://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx) 要素の **ContactDataShape** 属性に "AllProperties" を指定すると、候補ごとに大量のデータ (ユーザーの写真を含む) が返されます。</span><span class="sxs-lookup"><span data-stu-id="791b2-173">If you specify "AllProperties" for the **ContactDataShape** attribute of the [ResolveNames](http://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx) element, a lot of data, including user photos, will be returned for each candidate.</span></span> <span data-ttu-id="791b2-174">次の例は、名前 "Sadie" を解決して、候補ごとにプロパティをすべて返す XML 要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="791b2-174">The following example shows the XML request to resolve the name "Sadie" and return all the properties for each candidate.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
<soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>  
<soap:Body>
  <m:ResolveNames ReturnFullContactData="true" ContactDataShape="AllProperties">
      <m:UnresolvedEntry>sadie</m:UnresolvedEntry>
    </m:ResolveNames>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="791b2-175">この応答では、大量のデータが返されます。</span><span class="sxs-lookup"><span data-stu-id="791b2-175">A lot of data will be returned in the response.</span></span> <span data-ttu-id="791b2-176">次の例は、ユーザーの写真に関連するデータのみを示しています。</span><span class="sxs-lookup"><span data-stu-id="791b2-176">The following example shows only the data that is relevant to the user photo.</span></span> <span data-ttu-id="791b2-177">**Photo** 要素には、Base64 エンコードされたユーザーの写真が含まれています (読みやすくするために内容が短縮されています)。</span><span class="sxs-lookup"><span data-stu-id="791b2-177">The **Photo** element contains the Base64-encoded user photo (the content has been shortened for readability).</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
         xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:ResolveNamesResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:ResolveNamesResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:ResolutionSet TotalItemsInView="1" IncludesLastItemInRange="true">
            <t:Resolution>
              <t:Mailbox>
                <t:Name>Sadie Daniels</t:Name>
                <t:EmailAddress>sadie@contoso.com</t:EmailAddress>
                <t:RoutingType>SMTP</t:RoutingType>
                <t:MailboxType>Mailbox</t:MailboxType>
              </t:Mailbox>
              <t:Contact>
                <t:DisplayName>Sadie Daniels</t:DisplayName>
                <t:GivenName>Sadie</t:GivenName>
                <t:Initials/>
                <t:CompanyName>CONTOSO</t:CompanyName>
......
                <t:Photo>/9j/4AAQSkZJRgABAQE...qKKKAP/2Q==</t:Photo>
......
              </t:Contact>
            </t:Resolution>
          </m:ResolutionSet>
        </m:ResolveNamesResponseMessage>
      </m:ResponseMessages>
    </m:ResolveNamesResponse>
  </s:Body>
</s:Envelope>

```

### <a name="get-a-contact-user-photo-by-using-the-getattachment-operation"></a><span data-ttu-id="791b2-178">GetAttachment 操作を使用して連絡先ユーザーの写真を取得する</span><span class="sxs-lookup"><span data-stu-id="791b2-178">Get a contact user photo by using the GetAttachment operation</span></span>

<span data-ttu-id="791b2-179">EWS を使用すると、メールボックスに保存された連絡先から写真を取得できます。</span><span class="sxs-lookup"><span data-stu-id="791b2-179">You can use EWS to get photos from contacts stored in your mailbox.</span></span> <span data-ttu-id="791b2-180">まず、**GetItem** 操作を使用してプロパティをすべて返して、写真を探せるようにします。</span><span class="sxs-lookup"><span data-stu-id="791b2-180">First, you use the **GetItem** operation to return all properties so you can look for photos.</span></span> <span data-ttu-id="791b2-181">次の例は、連絡先アイテムを取得する XML 要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="791b2-181">The following example shows an XML request to get a contact item.</span></span> <span data-ttu-id="791b2-182">アイテム ID は、読みやすくするために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="791b2-182">The ItemId value has been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetItem xmlns='http://schemas.microsoft.com/exchange/services/2006/messages'>
      <ItemShape>
        <t:BaseShape>AllProperties</t:BaseShape>
      </ItemShape>
      <ItemIds>
        <t:ItemId Id="AAAAGECXAAA=" ChangeKey="EQAAABYAAAD2WuN+TpqwSrNP9JCCMKC0AABLzXRv"/>
      </ItemIds>
    </GetItem>
  </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="791b2-183">[HasPicture](http://msdn.microsoft.com/library/922a43fe-01bd-49f2-9261-e00e4699b8da%28Office.15%29.aspx) 要素を調べて、連絡先に関連付けられた写真があることを確認します。</span><span class="sxs-lookup"><span data-stu-id="791b2-183">Look for the [HasPicture](http://msdn.microsoft.com/library/922a43fe-01bd-49f2-9261-e00e4699b8da%28Office.15%29.aspx) element to verify that the contact has an associated photo.</span></span> <span data-ttu-id="791b2-184">その後で、添付ファイルのコレクションを 1 つずつ調べて、値が true の [IsContactPhoto](http://msdn.microsoft.com/library/ae36b5f9-a787-4863-9dbc-258ad724801d%28Office.15%29.aspx) 要素を見つけます。</span><span class="sxs-lookup"><span data-stu-id="791b2-184">Then look through the collection of attachments for one that has a value of true for the [IsContactPhoto](http://msdn.microsoft.com/library/ae36b5f9-a787-4863-9dbc-258ad724801d%28Office.15%29.aspx) element.</span></span> <span data-ttu-id="791b2-185">次の応答例は、関連するデータのみを示しています。</span><span class="sxs-lookup"><span data-stu-id="791b2-185">The following example shows only the relevant code.</span></span> <span data-ttu-id="791b2-186">ID の値は読みやすくするために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="791b2-186">The FolderId values are shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
         xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Contact>
              <t:ItemId Id="AAAAGECXAAA=" ChangeKey="EQAAABYAAAD2WuN+TpqwSrNP9JCCMKC0AABLzXRv"/>
              <t:ParentFolderId Id="nIxIAAA=" ChangeKey="AQAAAA=="/>
              <t:ItemClass>IPM.Contact</t:ItemClass>
              <t:Subject>Hope Gross</t:Subject>
              <t:Sensitivity>Normal</t:Sensitivity>
......
              <t:Attachments>
                <t:FileAttachment>
                  <t:AttachmentId Id="1LGlhgpgoA="/>
                  <t:Name>ContactPicture.jpg</t:Name>
                  <t:Size>6260</t:Size>
                  <t:LastModifiedTime>2011-03-09T16:55:55</t:LastModifiedTime>
                  <t:IsInline>false</t:IsInline>
                  <t:IsContactPhoto>true</t:IsContactPhoto>
                </t:FileAttachment>
              </t:Attachments>
......
              <t:HasPicture>true</t:HasPicture>
            </t:Contact>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </m:GetItemResponse>
  </s:Body>
</s:Envelope>

```

次に、**AttachmentId** を指定した **GetAttachment** 操作を使用して、連絡先の写真がある添付ファイルを要求します。 次の例は、添付ファイルを取得する XML 要求を示しています。 <span data-ttu-id="791b2-189">ID は読みやすくするために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="791b2-189">The FolderId value is shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
xmlns:xsd="http://www.w3.org/2001/XMLSchema"
xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetAttachment xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <AttachmentShape/>
      <AttachmentIds>
         <t:AttachmentId Id="1LGlhgpgoA="/>
      </AttachmentIds>
    </GetAttachment>
  </soap:Body>
</soap:Envelope>

```

次の例は、要求した添付ファイルに関する情報を含む XML 応答を示しています。 <span data-ttu-id="791b2-191">[Content](http://msdn.microsoft.com/library/24f8c54a-505f-4fc0-b7e7-93ad50b97070%28Office.15%29.aspx) 要素には、ユーザーの写真の Base64 エンコード文字列が含まれています。読みやすくするために、この例の文字列は短縮されています。</span><span class="sxs-lookup"><span data-stu-id="791b2-191">The following example shows the XML response with the information about the attachment you requested. The [Content](http://msdn.microsoft.com/library/24f8c54a-505f-4fc0-b7e7-93ad50b97070%28Office.15%29.aspx) element contains the Base64-encoded string for the user photo, shortened in this example for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
         xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetAttachmentResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetAttachmentResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Attachments>
            <t:FileAttachment>
              <t:AttachmentId Id="+KsDBEr1LGlhgpgoA="/>
              <t:Name>ContactPicture.jpg</t:Name>
              <t:Content>/9j/4AAQSkZJRgABAQEAYABgAAD/2wBDAAg...D//2Q==</t:Content>
            </t:FileAttachment>
          </m:Attachments>
        </m:GetAttachmentResponseMessage>
      </m:ResponseMessages>
    </m:GetAttachmentResponse>
  </s:Body>
</s:Envelope>

```

<span data-ttu-id="791b2-192"><a name="bk_EWS"> </a></span><span class="sxs-lookup"><span data-stu-id="791b2-192"></span></span>

## <a name="decode-a-base64-encoded-string"></a><span data-ttu-id="791b2-193">Base64 エンコード文字列をデコードする</span><span class="sxs-lookup"><span data-stu-id="791b2-193">Decoding a Base64-encoded string</span></span>

<span data-ttu-id="791b2-p117">どの操作を使用してユーザーの写真を取得したとしても、その文字列をデコードしてアプリケーションで使用できるようにする必要があります。次の例は、文字列をデコードし、ローカル コンピューターに保存して、後からアプリケーションでアクセスできるようにする方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="791b2-p117">Regardless of the operation you use to get a user photo, you'll need to decode that string so you can use it in your application. The following example shows how to decode the string, and then save it to your local computer so you application can access it later.</span></span>
  
```cs
// Convert the encoded string into a byte array.
byte[] data = System.Convert.FromBase64String(Photo);
// Create a memory stream to read the data.
MemoryStream ms = new MemoryStream(data);
// Save the data on your local computer as a JPG image.
using (FileStream file = new FileStream(ContactName + ".jpg", FileMode.Create, System.IO.FileAccess.Write))
{
   byte[] bytes = new byte[ms.Length];
   ms.Read(bytes, 0, (int)ms.Length);
   file.Write(bytes, 0, bytes.Length);
   ms.Close();
}

```

## <a name="see-also"></a><span data-ttu-id="791b2-196">関連項目</span><span class="sxs-lookup"><span data-stu-id="791b2-196">See also</span></span>

- [<span data-ttu-id="791b2-197">Exchange 内の EWS のユーザーと連絡先</span><span class="sxs-lookup"><span data-stu-id="791b2-197">People and contacts in EWS in Exchange</span></span>](people-and-contacts-in-ews-in-exchange.md)    
- [<span data-ttu-id="791b2-198">Exchange 2013 の EWS を使用して、あいまいな名前を解決する</span><span class="sxs-lookup"><span data-stu-id="791b2-198">How to: Resolve ambiguous names by using EWS in Exchange 2013</span></span>](how-to-resolve-ambiguous-names-by-using-ews-in-exchange-2013.md)    
- [<span data-ttu-id="791b2-199">Exchange において EWS を使用してバッチ処理で連絡先を処理する</span><span class="sxs-lookup"><span data-stu-id="791b2-199">How to: Process contacts in batches by using EWS in Exchange</span></span>](how-to-process-contacts-in-batches-by-using-ews-in-exchange.md)
    

