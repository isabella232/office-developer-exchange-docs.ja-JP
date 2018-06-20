---
title: GetUserPhoto 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f6e8143d-4235-428e-8f9c-ab6e9b1cfa6e
description: 操作 GetUserPhoto EWS についての情報を検索します。
ms.openlocfilehash: 4465ac7115d96f5b6ef39e467663c9bf1c70e99e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831694"
---
# <a name="getuserphoto-operation"></a><span data-ttu-id="28f70-103">GetUserPhoto 操作</span><span class="sxs-lookup"><span data-stu-id="28f70-103">GetUserPhoto operation</span></span>

<span data-ttu-id="28f70-104">**GetUserPhoto** EWS の操作に関する情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="28f70-104">Find information about the **GetUserPhoto** EWS operation.</span></span> 
  
<span data-ttu-id="28f70-105">**GetUserPhoto**操作は、Active Directory ドメイン サービス (AD DS) からのユーザーの写真を取得します。</span><span class="sxs-lookup"><span data-stu-id="28f70-105">The **GetUserPhoto** operation gets a user photo from Active Directory Domain Services (AD DS).</span></span> 
  
<span data-ttu-id="28f70-106">この操作は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="28f70-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getuserphoto-operation"></a><span data-ttu-id="28f70-107">GetUserPhoto 操作を使用します。</span><span class="sxs-lookup"><span data-stu-id="28f70-107">Using the GetUserPhoto operation</span></span>

<span data-ttu-id="28f70-108">**RemoveContactFromImList**操作は、単純な操作をユーザーの電子メール アドレスと要求された写真のサイズを受け取り、応答でフォト ストリームを返します。</span><span class="sxs-lookup"><span data-stu-id="28f70-108">The **RemoveContactFromImList** operation is a simple operation that accepts a user's email address and the requested photo size and returns the photo stream in the response.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="28f70-109">EWS が、SOAP と REST ベースの操作の両方がユーザーの写真を取得します。</span><span class="sxs-lookup"><span data-stu-id="28f70-109">EWS has both a SOAP and a REST-based operation to get user photos.</span></span> <span data-ttu-id="28f70-110">REST インターフェイスの詳細については、 [Exchange での EWS を使用して、ユーザーの写真の取り込み](http://msdn.microsoft.com/library/f86d1099-1f57-47dc-abf2-4d5ae4e900a9%28Office.15%29.aspx)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="28f70-110">For information about the REST interface, see [Get user photos by using EWS in Exchange](http://msdn.microsoft.com/library/f86d1099-1f57-47dc-abf2-4d5ae4e900a9%28Office.15%29.aspx).</span></span> 
  
### <a name="getuserphoto-operation-soap-headers"></a><span data-ttu-id="28f70-111">GetUserPhoto 操作の SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="28f70-111">GetUserPhoto operation SOAP headers</span></span>

<span data-ttu-id="28f70-112">**GetUserPhoto**操作は、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="28f70-112">The **GetUserPhoto** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="28f70-113">**ヘッダー名**</span><span class="sxs-lookup"><span data-stu-id="28f70-113">**Header name**</span></span>|<span data-ttu-id="28f70-114">**要素**</span><span class="sxs-lookup"><span data-stu-id="28f70-114">**Element**</span></span>|<span data-ttu-id="28f70-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="28f70-115">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="28f70-116">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="28f70-116">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="28f70-117">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="28f70-117">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="28f70-118">操作要求のスキーマのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="28f70-118">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="28f70-119">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="28f70-119">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="28f70-120">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="28f70-120">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="28f70-121">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="28f70-121">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="28f70-122">要求に応答するサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="28f70-122">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="28f70-123">このヘッダーは、応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="28f70-123">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getuserphoto-operation-request-example-get-a-users-photo"></a><span data-ttu-id="28f70-124">GetUserPhoto 操作の要求の使用例: ユーザーの写真を取得します。</span><span class="sxs-lookup"><span data-stu-id="28f70-124">GetUserPhoto operation request example: Get a user's photo</span></span>

<span data-ttu-id="28f70-125">**GetUserPhoto**操作要求の次の例では、ユーザーの写真を取得する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="28f70-125">The following example of a **GetUserPhoto** operation request shows how to get a user's photo.</span></span> <span data-ttu-id="28f70-126">次の使用例は、48 x 48 ピクセル、ユーザーの写真を要求します。</span><span class="sxs-lookup"><span data-stu-id="28f70-126">This example requests a user photo that is 48x48 pixels.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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

<span data-ttu-id="28f70-127">次の要素は、SOAP 本文の要求で使用されます。</span><span class="sxs-lookup"><span data-stu-id="28f70-127">The following elements are used in the request SOAP body:</span></span>
  
- [<span data-ttu-id="28f70-128">GetUserPhoto</span><span class="sxs-lookup"><span data-stu-id="28f70-128">GetUserPhoto</span></span>](getuserphoto.md)
    
- [<span data-ttu-id="28f70-129">電子メール (文字列)</span><span class="sxs-lookup"><span data-stu-id="28f70-129">Email (String)</span></span>](email-string.md)
    
- [<span data-ttu-id="28f70-130">SizeRequested</span><span class="sxs-lookup"><span data-stu-id="28f70-130">SizeRequested</span></span>](sizerequested.md)
    
## <a name="successful-getuserphoto-operation-response"></a><span data-ttu-id="28f70-131">GetUserPhoto 操作の成功の応答</span><span class="sxs-lookup"><span data-stu-id="28f70-131">Successful GetUserPhoto operation response</span></span>

<span data-ttu-id="28f70-132">次の例では、ユーザーの写真を取得するのには、 **GetUserPhoto**の操作を正常な応答を示します。</span><span class="sxs-lookup"><span data-stu-id="28f70-132">The following example shows a successful response to a **GetUserPhoto** operation to get a user's photo.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="8" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetUserPhotoResponse ResponseClass="Success" 
                            xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <HasChanged>true</HasChanged>
         <PictureData>/9j/4AAQSkZJRgABAQEAYABgAAD/02</PictureData>
      </GetUserPhotoResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="28f70-133">応答 SOAP 本文では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="28f70-133">The following elements are used in the response SOAP body:</span></span>
  
- [<span data-ttu-id="28f70-134">GetUserPhotoResponse</span><span class="sxs-lookup"><span data-stu-id="28f70-134">GetUserPhotoResponse</span></span>](getuserphotoresponse.md)
    
- [<span data-ttu-id="28f70-135">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="28f70-135">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="28f70-136">HasChanged</span><span class="sxs-lookup"><span data-stu-id="28f70-136">HasChanged</span></span>](haschanged.md)
    
- [<span data-ttu-id="28f70-137">GetUserPhotoResponse</span><span class="sxs-lookup"><span data-stu-id="28f70-137">GetUserPhotoResponse</span></span>](getuserphotoresponse.md)
    
## <a name="getuserphoto-operation-error-response"></a><span data-ttu-id="28f70-138">GetUserPhoto 操作のエラー応答</span><span class="sxs-lookup"><span data-stu-id="28f70-138">GetUserPhoto operation error response</span></span>

<span data-ttu-id="28f70-139">組織に存在しない電子メール アドレスのユーザーの写真を取得しようとした場合に、SOAP エンベロープはエラー コードを返しません。</span><span class="sxs-lookup"><span data-stu-id="28f70-139">The SOAP envelope will not return an error code if an attempt is made to get a user photo for an email address that doesn't exist in the organization.</span></span> <span data-ttu-id="28f70-140">500 HTTP ステータス コードは、要求が失敗したことを示す応答で返されます。</span><span class="sxs-lookup"><span data-stu-id="28f70-140">A 500 HTTP status code will be returned in the response to indicate that the request was unsuccessful.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="28f70-141">関連項目</span><span class="sxs-lookup"><span data-stu-id="28f70-141">See also</span></span>

- [<span data-ttu-id="28f70-142">Exchange での EWS の操作</span><span class="sxs-lookup"><span data-stu-id="28f70-142">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)   
- [<span data-ttu-id="28f70-143">EWS を使用して Exchange でのユーザーの写真を取り込み</span><span class="sxs-lookup"><span data-stu-id="28f70-143">Get user photos by using EWS in Exchange</span></span>](http://msdn.microsoft.com/library/f86d1099-1f57-47dc-abf2-4d5ae4e900a9%28Office.15%29.aspx)
    

