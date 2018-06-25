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
description: GetSharingFolder 操作は、指定した共有フォルダーのローカル フォルダーの識別子を取得します。
ms.openlocfilehash: 23adb10b22623fcbc1dd6b33bd674afafdaa8b19
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831670"
---
# <a name="getsharingfolder-operation"></a><span data-ttu-id="bf6e1-103">GetSharingFolder 操作</span><span class="sxs-lookup"><span data-stu-id="bf6e1-103">GetSharingFolder operation</span></span>

<span data-ttu-id="bf6e1-104">**GetSharingFolder**操作は、指定した共有フォルダーのローカル フォルダーの識別子を取得します。</span><span class="sxs-lookup"><span data-stu-id="bf6e1-104">The **GetSharingFolder** operation gets the local folder identifier of a specified shared folder.</span></span> 
  
## <a name="soap-headers"></a><span data-ttu-id="bf6e1-105">SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bf6e1-105">SOAP Headers</span></span>

<span data-ttu-id="bf6e1-106">**GetSharingFolder**操作が一覧表示され、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="bf6e1-106">The **GetSharingFolder** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="bf6e1-107">**Header**</span><span class="sxs-lookup"><span data-stu-id="bf6e1-107">**Header**</span></span>|<span data-ttu-id="bf6e1-108">**要素**</span><span class="sxs-lookup"><span data-stu-id="bf6e1-108">**Element**</span></span>|<span data-ttu-id="bf6e1-109">**説明**</span><span class="sxs-lookup"><span data-stu-id="bf6e1-109">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="bf6e1-110">RequestVersion</span><span class="sxs-lookup"><span data-stu-id="bf6e1-110">RequestVersion</span></span>  <br/> |[<span data-ttu-id="bf6e1-111">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="bf6e1-111">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="bf6e1-112">操作要求のスキーマのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="bf6e1-112">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="bf6e1-113">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="bf6e1-113">ServerVersion</span></span>  <br/> |[<span data-ttu-id="bf6e1-114">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="bf6e1-114">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="bf6e1-115">要求に応答するサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="bf6e1-115">Identifies the version of the server that responded to the request.</span></span>  <br/> |
   
## <a name="getsharingfolder-request-example"></a><span data-ttu-id="bf6e1-116">GetSharingFolder 要求の例</span><span class="sxs-lookup"><span data-stu-id="bf6e1-116">GetSharingFolder request example</span></span>

### <a name="getting-the-local-folder-identifier-by-specifying-the-sharedfolderid-element-of-the-folder-being-shared"></a><span data-ttu-id="bf6e1-117">共有フォルダーの SharedFolderId 要素を指定することによってローカル フォルダーの識別子を取得します。</span><span class="sxs-lookup"><span data-stu-id="bf6e1-117">Getting the Local Folder Identifier by Specifying the SharedFolderId Element of the Folder Being Shared</span></span>

<span data-ttu-id="bf6e1-118">次のコード例では、共有されているフォルダーに対応するローカル フォルダーの識別子を取得する要求を作成する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="bf6e1-118">The following code example shows how to form a request to get the identifier of the local folder that corresponds to the folder that is being shared.</span></span> <span data-ttu-id="bf6e1-119">共有されているフォルダーは、共有されているフォルダーを含むメールボックスの SMTP アドレスを使用して、そのフォルダーの識別子を表す、 [SharedFolderId](sharedfolderid.md)要素によって識別されます。</span><span class="sxs-lookup"><span data-stu-id="bf6e1-119">The folder that is being shared is identified by the SMTP address of the mailbox that contains the folder that is being shared and by the [SharedFolderId](sharedfolderid.md) element that represents the identifier of that folder.</span></span> <span data-ttu-id="bf6e1-120">この例では、共有されているフォルダーは user1@contoso.com によって所有されています。</span><span class="sxs-lookup"><span data-stu-id="bf6e1-120">In this example, the folder that is being shared is owned by user1@contoso.com.</span></span> 
  
### <a name="code"></a><span data-ttu-id="bf6e1-121">コード</span><span class="sxs-lookup"><span data-stu-id="bf6e1-121">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

### <a name="getting-the-local-folder-identifier-by-specifying-the-datatype-element-of-the-folder-being-shared"></a><span data-ttu-id="bf6e1-122">共有フォルダーのデータ型の要素を指定することによってローカル フォルダーの識別子を取得します。</span><span class="sxs-lookup"><span data-stu-id="bf6e1-122">Getting the Local Folder Identifier by Specifying the DataType Element of the Folder Being Shared</span></span>

<span data-ttu-id="bf6e1-123">次のコード例では、共有されているフォルダーに対応するローカル フォルダーの識別子を取得する要求を作成する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="bf6e1-123">The following code example shows how to form a request to get the identifier of the local folder that corresponds to the folder that is being shared.</span></span> <span data-ttu-id="bf6e1-124">共有されているフォルダーは、共有されているフォルダーを含むメールボックスの SMTP アドレスを使用して、そのフォルダー内のデータの種類を表す[データ型](datatype.md)の要素で識別されます。</span><span class="sxs-lookup"><span data-stu-id="bf6e1-124">The folder that is being shared is identified by the SMTP address of the mailbox that contains the folder that is being shared and by the [DataType](datatype.md) element that represents the type of data in that folder.</span></span> <span data-ttu-id="bf6e1-125">この例では、user1@contoso.com によって所有されている [連絡先] フォルダーが共有されているフォルダーです。</span><span class="sxs-lookup"><span data-stu-id="bf6e1-125">In this example, the folder that is being shared is the Contacts folder that is owned by user1@contoso.com.</span></span> 
  
### <a name="code"></a><span data-ttu-id="bf6e1-126">コード</span><span class="sxs-lookup"><span data-stu-id="bf6e1-126">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

### <a name="comments"></a><span data-ttu-id="bf6e1-127">コメント</span><span class="sxs-lookup"><span data-stu-id="bf6e1-127">Comments</span></span>

<span data-ttu-id="bf6e1-128">**データ型**の要素の有効な値については、[データ型](datatype.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bf6e1-128">For information about the possible values of the **DataType** element, see [DataType](datatype.md).</span></span>
  
## <a name="successful-getsharingfolder-response"></a><span data-ttu-id="bf6e1-129">GetSharingFolder の正常な応答</span><span class="sxs-lookup"><span data-stu-id="bf6e1-129">Successful GetSharingFolder Response</span></span>

### <a name="description"></a><span data-ttu-id="bf6e1-130">説明</span><span class="sxs-lookup"><span data-stu-id="bf6e1-130">Description</span></span>

<span data-ttu-id="bf6e1-131">**GetSharingFolder**要求に正常な応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="bf6e1-131">The following example shows a successful response to a **GetSharingFolder** request.</span></span> <span data-ttu-id="bf6e1-132">[SharingFolderId](sharingfolderid.md)要素の**Id**属性は、共有のローカル フォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="bf6e1-132">The **Id** attribute of the [SharingFolderId](sharingfolderid.md) element represents the identifier of the local folder in the sharing relationship.</span></span> 
  
### <a name="code"></a><span data-ttu-id="bf6e1-133">コード</span><span class="sxs-lookup"><span data-stu-id="bf6e1-133">Code</span></span>

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
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetSharingFolderResponseMessage ResponseClass="Success"
                                xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                                xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                                xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseCode>NoError</m:ResponseCode>
      <m:SharingFolderId Id="AAMkAD=" ChangeKey="AwAAA=" />
    </GetSharingFolderResponseMessage>
  </soap:Body>
</soap:Envelope>
```

## <a name="getsharingfolder-error-response"></a><span data-ttu-id="bf6e1-134">GetSharingFolder エラー応答</span><span class="sxs-lookup"><span data-stu-id="bf6e1-134">GetSharingFolder error response</span></span>

### <a name="description"></a><span data-ttu-id="bf6e1-135">説明</span><span class="sxs-lookup"><span data-stu-id="bf6e1-135">Description</span></span>

<span data-ttu-id="bf6e1-136">**GetSharingFolder**要求に対してエラー応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="bf6e1-136">The following example shows an error response to a **GetSharingFolder** request.</span></span> <span data-ttu-id="bf6e1-137">この例では、要求には、 [SharingFolderId](sharingfolderid.md)と[データ型](datatype.md)の両方の要素が指定されているためエラーが発生しました。</span><span class="sxs-lookup"><span data-stu-id="bf6e1-137">In this example, the error occurred because the request specified both the [SharingFolderId](sharingfolderid.md) and [DataType](datatype.md) elements.</span></span> <span data-ttu-id="bf6e1-138">これら 2 つの要素のいずれか一方だけを指定できること、いずれか一方に注意してください。</span><span class="sxs-lookup"><span data-stu-id="bf6e1-138">Note that only one or the other of those two elements can be specified, but not both.</span></span> 
  
### <a name="code"></a><span data-ttu-id="bf6e1-139">コード</span><span class="sxs-lookup"><span data-stu-id="bf6e1-139">Code</span></span>

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
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetSharingFolderResponseMessage ResponseClass="Error" 
                                xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                                xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                                xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:MessageText>Either DataType or SharedFolderId must be specified, but not both.</m:MessageText>
      <m:ResponseCode>ErrorInvalidGetSharingFolderRequest</m:ResponseCode>
      <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
    </GetSharingFolderResponseMessage>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="bf6e1-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="bf6e1-140">See also</span></span>



[<span data-ttu-id="bf6e1-141">GetSharingFolder</span><span class="sxs-lookup"><span data-stu-id="bf6e1-141">GetSharingFolder</span></span>](getsharingfolder.md)
  
[<span data-ttu-id="bf6e1-142">GetSharingFolderType</span><span class="sxs-lookup"><span data-stu-id="bf6e1-142">GetSharingFolderType</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.GetSharingFolderType.aspx)
  
[<span data-ttu-id="bf6e1-143">GetSharingFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="bf6e1-143">GetSharingFolderResponseMessage</span></span>](getsharingfolderresponsemessage.md)
  
[<span data-ttu-id="bf6e1-144">GetSharingFolderResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="bf6e1-144">GetSharingFolderResponseMessageType</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.GetSharingFolderResponseMessageType.aspx)


[<span data-ttu-id="bf6e1-145">Exchange での EWS の操作</span><span class="sxs-lookup"><span data-stu-id="bf6e1-145">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
  
- [<span data-ttu-id="bf6e1-146">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="bf6e1-146">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

