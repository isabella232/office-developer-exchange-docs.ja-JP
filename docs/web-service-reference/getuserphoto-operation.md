---
title: GetUserPhoto 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f6e8143d-4235-428e-8f9c-ab6e9b1cfa6e
description: GetUserPhoto EWS 操作に関する情報を検索します。
ms.openlocfilehash: 6769842d31519f0aac2cf9bda10c1cab70558301
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461815"
---
# <a name="getuserphoto-operation"></a><span data-ttu-id="b7c02-103">GetUserPhoto 操作</span><span class="sxs-lookup"><span data-stu-id="b7c02-103">GetUserPhoto operation</span></span>

<span data-ttu-id="b7c02-104">**Getuserphoto** EWS 操作に関する情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="b7c02-104">Find information about the **GetUserPhoto** EWS operation.</span></span> 
  
<span data-ttu-id="b7c02-105">**Getuserphoto**操作は、Active Directory ドメインサービス (AD DS) からユーザーの写真を取得します。</span><span class="sxs-lookup"><span data-stu-id="b7c02-105">The **GetUserPhoto** operation gets a user photo from Active Directory Domain Services (AD DS).</span></span> 
  
<span data-ttu-id="b7c02-106">この操作は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="b7c02-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getuserphoto-operation"></a><span data-ttu-id="b7c02-107">GetUserPhoto 操作の使用</span><span class="sxs-lookup"><span data-stu-id="b7c02-107">Using the GetUserPhoto operation</span></span>

<span data-ttu-id="b7c02-108">**RemoveContactFromImList**操作は、ユーザーの電子メールアドレスと要求された写真のサイズを受け取り、応答で写真ストリームを返す簡単な操作です。</span><span class="sxs-lookup"><span data-stu-id="b7c02-108">The **RemoveContactFromImList** operation is a simple operation that accepts a user's email address and the requested photo size and returns the photo stream in the response.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="b7c02-109">EWS には、ユーザーの写真を取得するための SOAP と REST ベースの操作の両方があります。</span><span class="sxs-lookup"><span data-stu-id="b7c02-109">EWS has both a SOAP and a REST-based operation to get user photos.</span></span> <span data-ttu-id="b7c02-110">REST インターフェイスの詳細については、「 [Exchange で EWS を使用してユーザーの写真を取得する](https://msdn.microsoft.com/library/f86d1099-1f57-47dc-abf2-4d5ae4e900a9%28Office.15%29.aspx)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b7c02-110">For information about the REST interface, see [Get user photos by using EWS in Exchange](https://msdn.microsoft.com/library/f86d1099-1f57-47dc-abf2-4d5ae4e900a9%28Office.15%29.aspx).</span></span> 
  
### <a name="getuserphoto-operation-soap-headers"></a><span data-ttu-id="b7c02-111">GetUserPhoto operation SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b7c02-111">GetUserPhoto operation SOAP headers</span></span>

<span data-ttu-id="b7c02-112">**Getuserphoto**操作では、次の表に示す SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="b7c02-112">The **GetUserPhoto** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="b7c02-113">**ヘッダー名**</span><span class="sxs-lookup"><span data-stu-id="b7c02-113">**Header name**</span></span>|<span data-ttu-id="b7c02-114">**要素**</span><span class="sxs-lookup"><span data-stu-id="b7c02-114">**Element**</span></span>|<span data-ttu-id="b7c02-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="b7c02-115">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="b7c02-116">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="b7c02-116">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="b7c02-117">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="b7c02-117">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="b7c02-118">操作要求のスキーマバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="b7c02-118">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="b7c02-119">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="b7c02-119">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="b7c02-120">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="b7c02-120">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="b7c02-121">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="b7c02-121">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="b7c02-122">要求に応答したサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="b7c02-122">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="b7c02-123">このヘッダーは応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="b7c02-123">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getuserphoto-operation-request-example-get-a-users-photo"></a><span data-ttu-id="b7c02-124">GetUserPhoto 操作要求の例: ユーザーの写真を取得する</span><span class="sxs-lookup"><span data-stu-id="b7c02-124">GetUserPhoto operation request example: Get a user's photo</span></span>

<span data-ttu-id="b7c02-125">次の**getuserphoto**操作要求の例は、ユーザーの写真を取得する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="b7c02-125">The following example of a **GetUserPhoto** operation request shows how to get a user's photo.</span></span> <span data-ttu-id="b7c02-126">この例では、48x48 ピクセルのユーザー写真を要求します。</span><span class="sxs-lookup"><span data-stu-id="b7c02-126">This example requests a user photo that is 48x48 pixels.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013"/>
   </soap:Header>
   <soap:Body>
      <m:GetUserPhoto>
         <m:Email>user1@contoso.com</m:Email>
         <m:SizeRequested>HR48x48</m:SizeRequested>
      </m:GetUserPhoto>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="b7c02-127">要求 SOAP 本文では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="b7c02-127">The following elements are used in the request SOAP body:</span></span>
  
- [<span data-ttu-id="b7c02-128">GetUserPhoto</span><span class="sxs-lookup"><span data-stu-id="b7c02-128">GetUserPhoto</span></span>](getuserphoto.md)
    
- [<span data-ttu-id="b7c02-129">電子メール (文字列)</span><span class="sxs-lookup"><span data-stu-id="b7c02-129">Email (String)</span></span>](email-string.md)
    
- [<span data-ttu-id="b7c02-130">SizeRequested</span><span class="sxs-lookup"><span data-stu-id="b7c02-130">SizeRequested</span></span>](sizerequested.md)
    
## <a name="successful-getuserphoto-operation-response"></a><span data-ttu-id="b7c02-131">正常な GetUserPhoto 操作応答</span><span class="sxs-lookup"><span data-stu-id="b7c02-131">Successful GetUserPhoto operation response</span></span>

<span data-ttu-id="b7c02-132">次の例は、ユーザーの写真を取得するための**getuserphoto**操作に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="b7c02-132">The following example shows a successful response to a **GetUserPhoto** operation to get a user's photo.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="8" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetUserPhotoResponse ResponseClass="Success" 
                            xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <HasChanged>true</HasChanged>
         <PictureData>/9j/4AAQSkZJRgABAQEAYABgAAD/02</PictureData>
      </GetUserPhotoResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="b7c02-133">応答 SOAP 本文では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="b7c02-133">The following elements are used in the response SOAP body:</span></span>
  
- [<span data-ttu-id="b7c02-134">GetUserPhotoResponse</span><span class="sxs-lookup"><span data-stu-id="b7c02-134">GetUserPhotoResponse</span></span>](getuserphotoresponse.md)
    
- [<span data-ttu-id="b7c02-135">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="b7c02-135">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="b7c02-136">HasChanged</span><span class="sxs-lookup"><span data-stu-id="b7c02-136">HasChanged</span></span>](haschanged.md)
    
- [<span data-ttu-id="b7c02-137">GetUserPhotoResponse</span><span class="sxs-lookup"><span data-stu-id="b7c02-137">GetUserPhotoResponse</span></span>](getuserphotoresponse.md)
    
## <a name="getuserphoto-operation-error-response"></a><span data-ttu-id="b7c02-138">GetUserPhoto 操作エラー応答</span><span class="sxs-lookup"><span data-stu-id="b7c02-138">GetUserPhoto operation error response</span></span>

<span data-ttu-id="b7c02-139">組織に存在しない電子メールアドレスに対してユーザーの写真を取得しようとした場合、SOAP エンベロープはエラーコードを返しません。</span><span class="sxs-lookup"><span data-stu-id="b7c02-139">The SOAP envelope will not return an error code if an attempt is made to get a user photo for an email address that doesn't exist in the organization.</span></span> <span data-ttu-id="b7c02-140">応答で 500 HTTP 状態コードが返され、要求が失敗したことが示されます。</span><span class="sxs-lookup"><span data-stu-id="b7c02-140">A 500 HTTP status code will be returned in the response to indicate that the request was unsuccessful.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="b7c02-141">関連項目</span><span class="sxs-lookup"><span data-stu-id="b7c02-141">See also</span></span>

- [<span data-ttu-id="b7c02-142">Exchange での EWS 操作</span><span class="sxs-lookup"><span data-stu-id="b7c02-142">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)   
- [<span data-ttu-id="b7c02-143">Exchange で EWS を使用してユーザーの写真を取得する</span><span class="sxs-lookup"><span data-stu-id="b7c02-143">Get user photos by using EWS in Exchange</span></span>](https://msdn.microsoft.com/library/f86d1099-1f57-47dc-abf2-4d5ae4e900a9%28Office.15%29.aspx)
    

