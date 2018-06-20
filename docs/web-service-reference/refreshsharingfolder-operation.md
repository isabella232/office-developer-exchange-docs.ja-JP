---
title: RefreshSharingFolder 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RefreshSharingFolder
api_type:
- schema
ms.assetid: 1b047e34-40f0-459f-ac9e-e9f8e7349479
description: RefreshSharingFolder 操作は、共有されているフォルダーからの最新のデータで指定したローカル フォルダーを更新します。
ms.openlocfilehash: 0037de28f0720b97cd51c58a6ee7e3c06e84d642
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833041"
---
# <a name="refreshsharingfolder-operation"></a><span data-ttu-id="353e2-103">RefreshSharingFolder 操作</span><span class="sxs-lookup"><span data-stu-id="353e2-103">RefreshSharingFolder operation</span></span>

<span data-ttu-id="353e2-104">**RefreshSharingFolder**操作は、共有されているフォルダーからの最新のデータで指定したローカル フォルダーを更新します。</span><span class="sxs-lookup"><span data-stu-id="353e2-104">The **RefreshSharingFolder** operation refreshes the specified local folder with the latest data from the folder that is being shared.</span></span> 
  
## <a name="soap-headers"></a><span data-ttu-id="353e2-105">SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="353e2-105">SOAP Headers</span></span>

<span data-ttu-id="353e2-106">**RefreshSharingFolder**操作が一覧表示され、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="353e2-106">The **RefreshSharingFolder** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="353e2-107">**Header**</span><span class="sxs-lookup"><span data-stu-id="353e2-107">**Header**</span></span>|<span data-ttu-id="353e2-108">**要素**</span><span class="sxs-lookup"><span data-stu-id="353e2-108">**Element**</span></span>|<span data-ttu-id="353e2-109">**説明**</span><span class="sxs-lookup"><span data-stu-id="353e2-109">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="353e2-110">RequestVersion</span><span class="sxs-lookup"><span data-stu-id="353e2-110">RequestVersion</span></span>  <br/> |[<span data-ttu-id="353e2-111">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="353e2-111">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="353e2-112">操作要求のスキーマのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="353e2-112">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="353e2-113">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="353e2-113">ServerVersion</span></span>  <br/> |[<span data-ttu-id="353e2-114">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="353e2-114">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="353e2-115">要求に応答するサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="353e2-115">Identifies the version of the server that responded to the request.</span></span>  <br/> |
   
## <a name="refreshsharingfolder-request-example"></a><span data-ttu-id="353e2-116">RefreshSharingFolder 要求の例</span><span class="sxs-lookup"><span data-stu-id="353e2-116">RefreshSharingFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="353e2-117">説明</span><span class="sxs-lookup"><span data-stu-id="353e2-117">Description</span></span>

<span data-ttu-id="353e2-118">次の例では、共有されているフォルダーからの最新のデータで指定したローカル フォルダーを更新する要求を作成する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="353e2-118">The following example shows how to form a request to refresh the specified local folder with the latest data from the folder that is being shared.</span></span> <span data-ttu-id="353e2-119">[SharingFolderId](sharingfolderid.md)要素は、更新するローカル フォルダーの識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="353e2-119">The [SharingFolderId](sharingfolderid.md) element specifies the identifier of the local folder to be refreshed.</span></span> 
  
### <a name="code"></a><span data-ttu-id="353e2-120">コード</span><span class="sxs-lookup"><span data-stu-id="353e2-120">Code</span></span>

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
    <RefreshSharingFolder xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:SharingFolderId Id="AAMkAD=" ChangeKey="AwAAA=" />
    </RefreshSharingFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="353e2-121">要素を要求します。</span><span class="sxs-lookup"><span data-stu-id="353e2-121">Request elements</span></span>

<span data-ttu-id="353e2-122">次の要素は、要求で使用されます。</span><span class="sxs-lookup"><span data-stu-id="353e2-122">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="353e2-123">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="353e2-123">RequestServerVersion</span></span>](requestserverversion.md)
    
- [<span data-ttu-id="353e2-124">RefreshSharingFolder</span><span class="sxs-lookup"><span data-stu-id="353e2-124">RefreshSharingFolder</span></span>](refreshsharingfolder.md)
    
- [<span data-ttu-id="353e2-125">SharingFolderId</span><span class="sxs-lookup"><span data-stu-id="353e2-125">SharingFolderId</span></span>](sharingfolderid.md)
    
## <a name="successful-refreshsharingfolder-response"></a><span data-ttu-id="353e2-126">RefreshSharingFolder の正常な応答</span><span class="sxs-lookup"><span data-stu-id="353e2-126">Successful RefreshSharingFolder Response</span></span>

### <a name="description"></a><span data-ttu-id="353e2-127">説明</span><span class="sxs-lookup"><span data-stu-id="353e2-127">Description</span></span>

<span data-ttu-id="353e2-128">**RefreshSharingFolder**要求に正常な応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="353e2-128">The following example shows a successful response to a **RefreshSharingFolder** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="353e2-129">コード</span><span class="sxs-lookup"><span data-stu-id="353e2-129">Code</span></span>

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
    <RefreshSharingFolderResponseMessage ResponseClass="Success"
                                xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                                xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                                xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseCode>NoError</m:ResponseCode>
    </RefreshSharingFolderResponseMessage>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a><span data-ttu-id="353e2-130">正常な応答の要素</span><span class="sxs-lookup"><span data-stu-id="353e2-130">Successful response elements</span></span>

<span data-ttu-id="353e2-131">次の要素は、応答で使用されます。</span><span class="sxs-lookup"><span data-stu-id="353e2-131">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="353e2-132">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="353e2-132">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="353e2-133">RefreshSharingFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="353e2-133">RefreshSharingFolderResponseMessage</span></span>](refreshsharingfolderresponsemessage.md)
    
- [<span data-ttu-id="353e2-134">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="353e2-134">ResponseCode</span></span>](responsecode.md)
    
## <a name="refreshsharingfolder-error-response"></a><span data-ttu-id="353e2-135">RefreshSharingFolder エラー応答</span><span class="sxs-lookup"><span data-stu-id="353e2-135">RefreshSharingFolder error response</span></span>

### <a name="description"></a><span data-ttu-id="353e2-136">説明</span><span class="sxs-lookup"><span data-stu-id="353e2-136">Description</span></span>

<span data-ttu-id="353e2-137">**RefreshSharingFolder**要求に対してエラー応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="353e2-137">The following example shows an error response to a **RefreshSharingFolder** request.</span></span> <span data-ttu-id="353e2-138">この例では、指定したローカル フォルダーに対応するサブスクリプションが見つからなかったために**RefreshSharingFolder**要求が失敗しました。</span><span class="sxs-lookup"><span data-stu-id="353e2-138">In this example, the **RefreshSharingFolder** request failed because a subscription that corresponds to the specified local folder was not found.</span></span> 
  
### <a name="code"></a><span data-ttu-id="353e2-139">コード</span><span class="sxs-lookup"><span data-stu-id="353e2-139">Code</span></span>

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
    <RefreshSharingFolderResponseMessage ResponseClass="Error"
                                xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                                xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                                xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:MessageText>Failed to synchronize the sharing folder.</m:MessageText>
      <m:ResponseCode>ErrorSharingSynchronizationFailed</m:ResponseCode>
      <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
      <m:MessageXml>
        <t:Value Name="ErrorDetails">Microsoft.Exchange.InfoWorker.Common.Sharing.SubscriptionNotFoundException: The subscription wasn't found.;</t:Value>
      </m:MessageXml>
    </RefreshSharingFolderResponseMessage>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="353e2-140">エラー応答の要素</span><span class="sxs-lookup"><span data-stu-id="353e2-140">Error response elements</span></span>

<span data-ttu-id="353e2-141">エラー応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="353e2-141">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="353e2-142">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="353e2-142">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="353e2-143">RefreshSharingFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="353e2-143">RefreshSharingFolderResponseMessage</span></span>](refreshsharingfolderresponsemessage.md)
    
- [<span data-ttu-id="353e2-144">MessageText</span><span class="sxs-lookup"><span data-stu-id="353e2-144">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="353e2-145">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="353e2-145">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="353e2-146">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="353e2-146">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="353e2-147">MessageXml</span><span class="sxs-lookup"><span data-stu-id="353e2-147">MessageXml</span></span>](messagexml.md)
    
## <a name="see-also"></a><span data-ttu-id="353e2-148">関連項目</span><span class="sxs-lookup"><span data-stu-id="353e2-148">See also</span></span>



[<span data-ttu-id="353e2-149">RefreshSharingFolder</span><span class="sxs-lookup"><span data-stu-id="353e2-149">RefreshSharingFolder</span></span>](refreshsharingfolder.md)
  
[<span data-ttu-id="353e2-150">RefreshSharingFolderType</span><span class="sxs-lookup"><span data-stu-id="353e2-150">RefreshSharingFolderType</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.RefreshSharingFolderType.aspx)
  
[<span data-ttu-id="353e2-151">RefreshSharingFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="353e2-151">RefreshSharingFolderResponseMessage</span></span>](refreshsharingfolderresponsemessage.md)
  
[<span data-ttu-id="353e2-152">RefreshSharingFolderResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="353e2-152">RefreshSharingFolderResponseMessageType</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.RefreshSharingFolderResponseMessageType.aspx)


[<span data-ttu-id="353e2-153">Exchange での EWS の操作</span><span class="sxs-lookup"><span data-stu-id="353e2-153">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
  
- [<span data-ttu-id="353e2-154">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="353e2-154">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

