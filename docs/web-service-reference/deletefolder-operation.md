---
title: DeleteFolder 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteFolder
api_type:
- schema
ms.assetid: b0f92682-4895-4bcf-a4a1-e4c2e8403979
description: DeleteFolder 操作では、メールボックスからフォルダーを削除します。
ms.openlocfilehash: 0fd7c9d4b04a706dcdb83f41087eaa4f3d45f129
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759975"
---
# <a name="deletefolder-operation"></a><span data-ttu-id="03de3-103">DeleteFolder 操作</span><span class="sxs-lookup"><span data-stu-id="03de3-103">DeleteFolder operation</span></span>

<span data-ttu-id="03de3-104">**DeleteFolder**操作では、メールボックスからフォルダーを削除します。</span><span class="sxs-lookup"><span data-stu-id="03de3-104">The **DeleteFolder** operation deletes folders from a mailbox.</span></span> 
  
## <a name="deletefolder-request-example"></a><span data-ttu-id="03de3-105">DeleteFolder 要求の例</span><span class="sxs-lookup"><span data-stu-id="03de3-105">DeleteFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="03de3-106">説明</span><span class="sxs-lookup"><span data-stu-id="03de3-106">Description</span></span>

<span data-ttu-id="03de3-107">**DeleteFolder**要求の次の例では、フォルダーを削除する要求を作成する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="03de3-107">This following example of a **DeleteFolder** request shows how to form a request to delete a folder.</span></span> 
  
### <a name="code"></a><span data-ttu-id="03de3-108">コード</span><span class="sxs-lookup"><span data-stu-id="03de3-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <DeleteFolder xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                  DeleteType="HardDelete" >
      <FolderIds>
        <t:FolderId Id="AS4AUnVz=" />
      </FolderIds>
    </DeleteFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="03de3-109">コメント</span><span class="sxs-lookup"><span data-stu-id="03de3-109">Comments</span></span>

<span data-ttu-id="03de3-110">この例では、フォルダーのハード削除を実行します。</span><span class="sxs-lookup"><span data-stu-id="03de3-110">This example performs a hard delete on the folder.</span></span>
  
> [!NOTE]
> <span data-ttu-id="03de3-111">フォルダー ID が小さすぎると読みやすさを保持します。</span><span class="sxs-lookup"><span data-stu-id="03de3-111">The folder ID has been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="03de3-112">要素を要求します。</span><span class="sxs-lookup"><span data-stu-id="03de3-112">Request elements</span></span>

<span data-ttu-id="03de3-113">次の要素は、要求で使用されます。</span><span class="sxs-lookup"><span data-stu-id="03de3-113">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="03de3-114">DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="03de3-114">DeleteFolder</span></span>](deletefolder.md)
    
- [<span data-ttu-id="03de3-115">FolderIds</span><span class="sxs-lookup"><span data-stu-id="03de3-115">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="03de3-116">フォルダー Id</span><span class="sxs-lookup"><span data-stu-id="03de3-116">FolderId</span></span>](folderid.md)
    
> [!NOTE]
> <span data-ttu-id="03de3-117">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="03de3-117">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span> 
  
<span data-ttu-id="03de3-118">**DeleteFolder**操作の要求メッセージには、他のオプションを検索するには、スキーマの階層構造を表示します。</span><span class="sxs-lookup"><span data-stu-id="03de3-118">To find other options for the request message of the **DeleteFolder** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="03de3-119">[DeleteFolder](deletefolder.md)要素から開始します。</span><span class="sxs-lookup"><span data-stu-id="03de3-119">Start at the [DeleteFolder](deletefolder.md) element.</span></span> 
  
## <a name="successful-deletefolder-response"></a><span data-ttu-id="03de3-120">DeleteFolder の正常な応答</span><span class="sxs-lookup"><span data-stu-id="03de3-120">Successful DeleteFolder response</span></span>

### <a name="description"></a><span data-ttu-id="03de3-121">説明</span><span class="sxs-lookup"><span data-stu-id="03de3-121">Description</span></span>

<span data-ttu-id="03de3-122">**DeleteFolder**要求に正常な応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="03de3-122">The following example shows a successful response to the **DeleteFolder** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="03de3-123">コード</span><span class="sxs-lookup"><span data-stu-id="03de3-123">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <DeleteFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:DeleteFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:DeleteFolderResponseMessage>
      </m:ResponseMessages>
    </DeleteFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="response-elements"></a><span data-ttu-id="03de3-124">応答の要素</span><span class="sxs-lookup"><span data-stu-id="03de3-124">Response elements</span></span>

<span data-ttu-id="03de3-125">次の要素は、応答で使用されます。</span><span class="sxs-lookup"><span data-stu-id="03de3-125">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="03de3-126">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="03de3-126">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="03de3-127">DeleteFolderResponse</span><span class="sxs-lookup"><span data-stu-id="03de3-127">DeleteFolderResponse</span></span>](deletefolderresponse.md)
    
- [<span data-ttu-id="03de3-128">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="03de3-128">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="03de3-129">DeleteFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="03de3-129">DeleteFolderResponseMessage</span></span>](deletefolderresponsemessage.md)
    
- [<span data-ttu-id="03de3-130">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="03de3-130">ResponseCode</span></span>](responsecode.md)
    
<span data-ttu-id="03de3-131">**DeleteFolder**操作の応答メッセージには、他のオプションを検索するには、スキーマの階層構造を表示します。</span><span class="sxs-lookup"><span data-stu-id="03de3-131">To find other options for the response message of the **DeleteFolder** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="03de3-132">[DeleteFolderResponse](deletefolderresponse.md)要素から開始します。</span><span class="sxs-lookup"><span data-stu-id="03de3-132">Start at the [DeleteFolderResponse](deletefolderresponse.md) element.</span></span> 
  
## <a name="deletefolder-error-response"></a><span data-ttu-id="03de3-133">DeleteFolder エラー応答</span><span class="sxs-lookup"><span data-stu-id="03de3-133">DeleteFolder error response</span></span>

### <a name="description"></a><span data-ttu-id="03de3-134">説明</span><span class="sxs-lookup"><span data-stu-id="03de3-134">Description</span></span>

<span data-ttu-id="03de3-135">**DeleteFolder**要求に対してエラー応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="03de3-135">The following example shows an error response to a **DeleteFolder** request.</span></span> <span data-ttu-id="03de3-136">いないメールボックス内に存在するフォルダーを削除する要求でエラーが発生しました。</span><span class="sxs-lookup"><span data-stu-id="03de3-136">The error was caused by a request to delete a folder that was not present in the mailbox.</span></span> 
  
### <a name="code"></a><span data-ttu-id="03de3-137">コード</span><span class="sxs-lookup"><span data-stu-id="03de3-137">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <DeleteFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:DeleteFolderResponseMessage ResponseClass="Error">
          <m:MessageText>The specified object was not found in the store.</m:MessageText>
          <m:ResponseCode>ErrorItemNotFound</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:DeleteFolderResponseMessage>
      </m:ResponseMessages>
    </DeleteFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="03de3-138">コメント</span><span class="sxs-lookup"><span data-stu-id="03de3-138">Comments</span></span>

<span data-ttu-id="03de3-139">識別フォルダーでは、 **DeleteFolder**操作を使用できません。</span><span class="sxs-lookup"><span data-stu-id="03de3-139">The **DeleteFolder** operation cannot be used on distinguished folders.</span></span> 
  
### <a name="error-response-elements"></a><span data-ttu-id="03de3-140">エラー応答の要素</span><span class="sxs-lookup"><span data-stu-id="03de3-140">Error response elements</span></span>

<span data-ttu-id="03de3-141">エラー応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="03de3-141">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="03de3-142">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="03de3-142">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="03de3-143">DeleteFolderResponse</span><span class="sxs-lookup"><span data-stu-id="03de3-143">DeleteFolderResponse</span></span>](deletefolderresponse.md)
    
- [<span data-ttu-id="03de3-144">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="03de3-144">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="03de3-145">DeleteFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="03de3-145">DeleteFolderResponseMessage</span></span>](deletefolderresponsemessage.md)
    
- [<span data-ttu-id="03de3-146">MessageText</span><span class="sxs-lookup"><span data-stu-id="03de3-146">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="03de3-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="03de3-147">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="03de3-148">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="03de3-148">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="03de3-149">**DeleteFolder**操作の応答のエラー メッセージには、他のオプションを検索するには、スキーマの階層構造を表示します。</span><span class="sxs-lookup"><span data-stu-id="03de3-149">To find other options for the error response message of the **DeleteFolder** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="03de3-150">[DeleteFolderResponse](deletefolderresponse.md)要素から開始します。</span><span class="sxs-lookup"><span data-stu-id="03de3-150">Start at the [DeleteFolderResponse](deletefolderresponse.md) element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="03de3-151">関連項目</span><span class="sxs-lookup"><span data-stu-id="03de3-151">See also</span></span>

- [<span data-ttu-id="03de3-152">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="03de3-152">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="03de3-153">フォルダーを削除します。</span><span class="sxs-lookup"><span data-stu-id="03de3-153">Deleting Folders</span></span>](http://msdn.microsoft.com/library/1958add5-5071-4239-adb2-40f7a7d74aee%28Office.15%29.aspx)

