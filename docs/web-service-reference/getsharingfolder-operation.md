---
title: GetSharingFolder 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetSharingFolder
api_type:
- schema
ms.assetid: 75fee92a-a7f8-4a62-ad2b-17acbaada186
description: GetSharingFolder 操作は、指定された共有フォルダーのローカルフォルダー識別子を取得します。
ms.openlocfilehash: cf66eb390b0287e89bb8402f26a2e728868a2b18
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460513"
---
# <a name="getsharingfolder-operation"></a><span data-ttu-id="66b5f-103">GetSharingFolder 操作</span><span class="sxs-lookup"><span data-stu-id="66b5f-103">GetSharingFolder operation</span></span>

<span data-ttu-id="66b5f-104">**Getsharingfolder**操作は、指定された共有フォルダーのローカルフォルダー識別子を取得します。</span><span class="sxs-lookup"><span data-stu-id="66b5f-104">The **GetSharingFolder** operation gets the local folder identifier of a specified shared folder.</span></span> 
  
## <a name="soap-headers"></a><span data-ttu-id="66b5f-105">SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="66b5f-105">SOAP Headers</span></span>

<span data-ttu-id="66b5f-106">**Getsharingfolder**操作では、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="66b5f-106">The **GetSharingFolder** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="66b5f-107">**Header**</span><span class="sxs-lookup"><span data-stu-id="66b5f-107">**Header**</span></span>|<span data-ttu-id="66b5f-108">**要素**</span><span class="sxs-lookup"><span data-stu-id="66b5f-108">**Element**</span></span>|<span data-ttu-id="66b5f-109">**説明**</span><span class="sxs-lookup"><span data-stu-id="66b5f-109">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="66b5f-110">RequestVersion</span><span class="sxs-lookup"><span data-stu-id="66b5f-110">RequestVersion</span></span>  <br/> |[<span data-ttu-id="66b5f-111">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="66b5f-111">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="66b5f-112">操作要求のスキーマバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="66b5f-112">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="66b5f-113">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="66b5f-113">ServerVersion</span></span>  <br/> |[<span data-ttu-id="66b5f-114">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="66b5f-114">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="66b5f-115">要求に応答したサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="66b5f-115">Identifies the version of the server that responded to the request.</span></span>  <br/> |
   
## <a name="getsharingfolder-request-example"></a><span data-ttu-id="66b5f-116">GetSharingFolder 要求の例</span><span class="sxs-lookup"><span data-stu-id="66b5f-116">GetSharingFolder request example</span></span>

### <a name="getting-the-local-folder-identifier-by-specifying-the-sharedfolderid-element-of-the-folder-being-shared"></a><span data-ttu-id="66b5f-117">共有するフォルダーの SharedFolderId 要素を指定して、ローカルフォルダーの識別子を取得する</span><span class="sxs-lookup"><span data-stu-id="66b5f-117">Getting the Local Folder Identifier by Specifying the SharedFolderId Element of the Folder Being Shared</span></span>

<span data-ttu-id="66b5f-118">次のコード例は、共有されているフォルダーに対応するローカルフォルダーの識別子を取得する要求を形成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="66b5f-118">The following code example shows how to form a request to get the identifier of the local folder that corresponds to the folder that is being shared.</span></span> <span data-ttu-id="66b5f-119">共有されているフォルダーは、共有されるフォルダーが含まれているメールボックスの SMTP アドレスと、そのフォルダーの識別子を表す[SharedFolderId](sharedfolderid.md)要素によって識別されます。</span><span class="sxs-lookup"><span data-stu-id="66b5f-119">The folder that is being shared is identified by the SMTP address of the mailbox that contains the folder that is being shared and by the [SharedFolderId](sharedfolderid.md) element that represents the identifier of that folder.</span></span> <span data-ttu-id="66b5f-120">この例では、共有されているフォルダーが user1@contoso.com によって所有されています。</span><span class="sxs-lookup"><span data-stu-id="66b5f-120">In this example, the folder that is being shared is owned by user1@contoso.com.</span></span> 
  
### <a name="code"></a><span data-ttu-id="66b5f-121">コード</span><span class="sxs-lookup"><span data-stu-id="66b5f-121">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010"/>
  </soap:Header>
  <soap:Body>
    <m:GetSharingFolder>
      <m:SmtpAddress>user1@contoso.com</m:SmtpAddress>
      <m:SharedFolderId>AAMkA=</m:SharedFolderId>
    </m:GetSharingFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="getting-the-local-folder-identifier-by-specifying-the-datatype-element-of-the-folder-being-shared"></a><span data-ttu-id="66b5f-122">共有するフォルダーの DataType 要素を指定してローカルフォルダーの識別子を取得する</span><span class="sxs-lookup"><span data-stu-id="66b5f-122">Getting the Local Folder Identifier by Specifying the DataType Element of the Folder Being Shared</span></span>

<span data-ttu-id="66b5f-123">次のコード例は、共有されているフォルダーに対応するローカルフォルダーの識別子を取得する要求を形成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="66b5f-123">The following code example shows how to form a request to get the identifier of the local folder that corresponds to the folder that is being shared.</span></span> <span data-ttu-id="66b5f-124">共有されているフォルダーは、共有されるフォルダーが含まれているメールボックスの SMTP アドレスと、そのフォルダー内のデータの種類を表す[DataType](datatype.md)要素によって識別されます。</span><span class="sxs-lookup"><span data-stu-id="66b5f-124">The folder that is being shared is identified by the SMTP address of the mailbox that contains the folder that is being shared and by the [DataType](datatype.md) element that represents the type of data in that folder.</span></span> <span data-ttu-id="66b5f-125">この例では、共有されているフォルダーは、user1@contoso.com によって所有されている連絡先フォルダーです。</span><span class="sxs-lookup"><span data-stu-id="66b5f-125">In this example, the folder that is being shared is the Contacts folder that is owned by user1@contoso.com.</span></span> 
  
### <a name="code"></a><span data-ttu-id="66b5f-126">コード</span><span class="sxs-lookup"><span data-stu-id="66b5f-126">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010"/>
  </soap:Header>
  <soap:Body>
    <m:GetSharingFolder>
      <m:SmtpAddress>user1@contoso.com</m:SmtpAddress>
      <m:DataType>Contacts</m:DataType>
    </m:GetSharingFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="66b5f-127">コメント</span><span class="sxs-lookup"><span data-stu-id="66b5f-127">Comments</span></span>

<span data-ttu-id="66b5f-128">**Datatype**要素に指定できる値の詳細については、「 [datatype](datatype.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="66b5f-128">For information about the possible values of the **DataType** element, see [DataType](datatype.md).</span></span>
  
## <a name="successful-getsharingfolder-response"></a><span data-ttu-id="66b5f-129">成功した GetSharingFolder 応答</span><span class="sxs-lookup"><span data-stu-id="66b5f-129">Successful GetSharingFolder Response</span></span>

### <a name="description"></a><span data-ttu-id="66b5f-130">説明</span><span class="sxs-lookup"><span data-stu-id="66b5f-130">Description</span></span>

<span data-ttu-id="66b5f-131">次の例は、 **Getsharingfolder**要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="66b5f-131">The following example shows a successful response to a **GetSharingFolder** request.</span></span> <span data-ttu-id="66b5f-132">[SharingFolderId](sharingfolderid.md)要素の**Id**属性は、共有関係のローカルフォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="66b5f-132">The **Id** attribute of the [SharingFolderId](sharingfolderid.md) element represents the identifier of the local folder in the sharing relationship.</span></span> 
  
### <a name="code"></a><span data-ttu-id="66b5f-133">コード</span><span class="sxs-lookup"><span data-stu-id="66b5f-133">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="11" 
                         Version="Exchange2010" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetSharingFolderResponseMessage ResponseClass="Success"
                                xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                                xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                                xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseCode>NoError</m:ResponseCode>
      <m:SharingFolderId Id="AAMkAD=" ChangeKey="AwAAA=" />
    </GetSharingFolderResponseMessage>
  </soap:Body>
</soap:Envelope>
```

## <a name="getsharingfolder-error-response"></a><span data-ttu-id="66b5f-134">GetSharingFolder エラー応答</span><span class="sxs-lookup"><span data-stu-id="66b5f-134">GetSharingFolder error response</span></span>

### <a name="description"></a><span data-ttu-id="66b5f-135">説明</span><span class="sxs-lookup"><span data-stu-id="66b5f-135">Description</span></span>

<span data-ttu-id="66b5f-136">次の例は、 **Getsharingfolder**要求に対するエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="66b5f-136">The following example shows an error response to a **GetSharingFolder** request.</span></span> <span data-ttu-id="66b5f-137">この例では、要求で[SharingFolderId](sharingfolderid.md)要素と[DataType](datatype.md)要素の両方が指定されているため、エラーが発生しました。</span><span class="sxs-lookup"><span data-stu-id="66b5f-137">In this example, the error occurred because the request specified both the [SharingFolderId](sharingfolderid.md) and [DataType](datatype.md) elements.</span></span> <span data-ttu-id="66b5f-138">これら2つの要素のどちらか一方のみを指定できますが、両方を指定することはできません。</span><span class="sxs-lookup"><span data-stu-id="66b5f-138">Note that only one or the other of those two elements can be specified, but not both.</span></span> 
  
### <a name="code"></a><span data-ttu-id="66b5f-139">コード</span><span class="sxs-lookup"><span data-stu-id="66b5f-139">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="11" 
                         Version="Exchange2010" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetSharingFolderResponseMessage ResponseClass="Error" 
                                xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                                xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                                xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:MessageText>Either DataType or SharedFolderId must be specified, but not both.</m:MessageText>
      <m:ResponseCode>ErrorInvalidGetSharingFolderRequest</m:ResponseCode>
      <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
    </GetSharingFolderResponseMessage>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="66b5f-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="66b5f-140">See also</span></span>



[<span data-ttu-id="66b5f-141">GetSharingFolder</span><span class="sxs-lookup"><span data-stu-id="66b5f-141">GetSharingFolder</span></span>](getsharingfolder.md)
  
[<span data-ttu-id="66b5f-142">GetSharingFolderType</span><span class="sxs-lookup"><span data-stu-id="66b5f-142">GetSharingFolderType</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.GetSharingFolderType.aspx)
  
[<span data-ttu-id="66b5f-143">GetSharingFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="66b5f-143">GetSharingFolderResponseMessage</span></span>](getsharingfolderresponsemessage.md)
  
[<span data-ttu-id="66b5f-144">GetSharingFolderResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="66b5f-144">GetSharingFolderResponseMessageType</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.GetSharingFolderResponseMessageType.aspx)


[<span data-ttu-id="66b5f-145">Exchange での EWS 操作</span><span class="sxs-lookup"><span data-stu-id="66b5f-145">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
  
- [<span data-ttu-id="66b5f-146">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="66b5f-146">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

