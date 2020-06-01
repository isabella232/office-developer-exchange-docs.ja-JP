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
description: DeleteFolder 操作は、メールボックスからフォルダーを削除します。
ms.openlocfilehash: e9bb9199027c2af2cbbb664ef7ad4fa70b7ef718
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455745"
---
# <a name="deletefolder-operation"></a><span data-ttu-id="ee289-103">DeleteFolder 操作</span><span class="sxs-lookup"><span data-stu-id="ee289-103">DeleteFolder operation</span></span>

<span data-ttu-id="ee289-104">**Deletefolder**操作は、メールボックスからフォルダーを削除します。</span><span class="sxs-lookup"><span data-stu-id="ee289-104">The **DeleteFolder** operation deletes folders from a mailbox.</span></span> 
  
## <a name="deletefolder-request-example"></a><span data-ttu-id="ee289-105">DeleteFolder 要求の例</span><span class="sxs-lookup"><span data-stu-id="ee289-105">DeleteFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="ee289-106">説明</span><span class="sxs-lookup"><span data-stu-id="ee289-106">Description</span></span>

<span data-ttu-id="ee289-107">次の**deletefolder**要求の例は、フォルダーを削除する要求を形成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="ee289-107">This following example of a **DeleteFolder** request shows how to form a request to delete a folder.</span></span> 
  
### <a name="code"></a><span data-ttu-id="ee289-108">コード</span><span class="sxs-lookup"><span data-stu-id="ee289-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <DeleteFolder xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                  DeleteType="HardDelete" >
      <FolderIds>
        <t:FolderId Id="AS4AUnVz=" />
      </FolderIds>
    </DeleteFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="ee289-109">コメント</span><span class="sxs-lookup"><span data-stu-id="ee289-109">Comments</span></span>

<span data-ttu-id="ee289-110">この例では、フォルダーに対してハード削除を実行します。</span><span class="sxs-lookup"><span data-stu-id="ee289-110">This example performs a hard delete on the folder.</span></span>
  
> [!NOTE]
> <span data-ttu-id="ee289-111">フォルダー ID は読みやすくするために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="ee289-111">The folder ID has been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="ee289-112">Request 要素</span><span class="sxs-lookup"><span data-stu-id="ee289-112">Request elements</span></span>

<span data-ttu-id="ee289-113">要求では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="ee289-113">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="ee289-114">DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="ee289-114">DeleteFolder</span></span>](deletefolder.md)
    
- [<span data-ttu-id="ee289-115">FolderIds</span><span class="sxs-lookup"><span data-stu-id="ee289-115">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="ee289-116">FolderId</span><span class="sxs-lookup"><span data-stu-id="ee289-116">FolderId</span></span>](folderid.md)
    
> [!NOTE]
> <span data-ttu-id="ee289-117">この要素を記述するスキーマは、Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="ee289-117">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span> 
  
<span data-ttu-id="ee289-118">**Deletefolder**操作の要求メッセージに関するその他のオプションについては、スキーマ階層を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ee289-118">To find other options for the request message of the **DeleteFolder** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="ee289-119">[Deletefolder](deletefolder.md)要素から開始します。</span><span class="sxs-lookup"><span data-stu-id="ee289-119">Start at the [DeleteFolder](deletefolder.md) element.</span></span> 
  
## <a name="successful-deletefolder-response"></a><span data-ttu-id="ee289-120">正常な DeleteFolder 応答</span><span class="sxs-lookup"><span data-stu-id="ee289-120">Successful DeleteFolder response</span></span>

### <a name="description"></a><span data-ttu-id="ee289-121">説明</span><span class="sxs-lookup"><span data-stu-id="ee289-121">Description</span></span>

<span data-ttu-id="ee289-122">次の例は、 **Deletefolder**要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="ee289-122">The following example shows a successful response to the **DeleteFolder** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="ee289-123">コード</span><span class="sxs-lookup"><span data-stu-id="ee289-123">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <DeleteFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:DeleteFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:DeleteFolderResponseMessage>
      </m:ResponseMessages>
    </DeleteFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="response-elements"></a><span data-ttu-id="ee289-124">Response 要素</span><span class="sxs-lookup"><span data-stu-id="ee289-124">Response elements</span></span>

<span data-ttu-id="ee289-125">応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="ee289-125">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="ee289-126">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="ee289-126">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="ee289-127">DeleteFolderResponse</span><span class="sxs-lookup"><span data-stu-id="ee289-127">DeleteFolderResponse</span></span>](deletefolderresponse.md)
    
- [<span data-ttu-id="ee289-128">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="ee289-128">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="ee289-129">DeleteFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ee289-129">DeleteFolderResponseMessage</span></span>](deletefolderresponsemessage.md)
    
- [<span data-ttu-id="ee289-130">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="ee289-130">ResponseCode</span></span>](responsecode.md)
    
<span data-ttu-id="ee289-131">**Deletefolder**操作の応答メッセージに関するその他のオプションについては、スキーマ階層を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ee289-131">To find other options for the response message of the **DeleteFolder** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="ee289-132">[Deletefolderresponse](deletefolderresponse.md)要素から開始します。</span><span class="sxs-lookup"><span data-stu-id="ee289-132">Start at the [DeleteFolderResponse](deletefolderresponse.md) element.</span></span> 
  
## <a name="deletefolder-error-response"></a><span data-ttu-id="ee289-133">DeleteFolder エラー応答</span><span class="sxs-lookup"><span data-stu-id="ee289-133">DeleteFolder error response</span></span>

### <a name="description"></a><span data-ttu-id="ee289-134">説明</span><span class="sxs-lookup"><span data-stu-id="ee289-134">Description</span></span>

<span data-ttu-id="ee289-135">次の例は、 **Deletefolder**要求に対するエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="ee289-135">The following example shows an error response to a **DeleteFolder** request.</span></span> <span data-ttu-id="ee289-136">このエラーは、メールボックスに存在しないフォルダーを削除する要求が原因で発生しました。</span><span class="sxs-lookup"><span data-stu-id="ee289-136">The error was caused by a request to delete a folder that was not present in the mailbox.</span></span> 
  
### <a name="code"></a><span data-ttu-id="ee289-137">コード</span><span class="sxs-lookup"><span data-stu-id="ee289-137">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <DeleteFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="ee289-138">コメント</span><span class="sxs-lookup"><span data-stu-id="ee289-138">Comments</span></span>

<span data-ttu-id="ee289-139">**Deletefolder**操作は、識別フォルダーでは使用できません。</span><span class="sxs-lookup"><span data-stu-id="ee289-139">The **DeleteFolder** operation cannot be used on distinguished folders.</span></span> 
  
### <a name="error-response-elements"></a><span data-ttu-id="ee289-140">エラー応答要素</span><span class="sxs-lookup"><span data-stu-id="ee289-140">Error response elements</span></span>

<span data-ttu-id="ee289-141">エラー応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="ee289-141">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="ee289-142">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="ee289-142">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="ee289-143">DeleteFolderResponse</span><span class="sxs-lookup"><span data-stu-id="ee289-143">DeleteFolderResponse</span></span>](deletefolderresponse.md)
    
- [<span data-ttu-id="ee289-144">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="ee289-144">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="ee289-145">DeleteFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ee289-145">DeleteFolderResponseMessage</span></span>](deletefolderresponsemessage.md)
    
- [<span data-ttu-id="ee289-146">MessageText</span><span class="sxs-lookup"><span data-stu-id="ee289-146">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="ee289-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="ee289-147">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="ee289-148">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="ee289-148">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="ee289-149">**Deletefolder**操作のエラー応答メッセージに関するその他のオプションについては、スキーマ階層を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ee289-149">To find other options for the error response message of the **DeleteFolder** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="ee289-150">[Deletefolderresponse](deletefolderresponse.md)要素から開始します。</span><span class="sxs-lookup"><span data-stu-id="ee289-150">Start at the [DeleteFolderResponse](deletefolderresponse.md) element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="ee289-151">関連項目</span><span class="sxs-lookup"><span data-stu-id="ee289-151">See also</span></span>

- [<span data-ttu-id="ee289-152">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="ee289-152">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="ee289-153">フォルダーの削除</span><span class="sxs-lookup"><span data-stu-id="ee289-153">Deleting Folders</span></span>](https://msdn.microsoft.com/library/1958add5-5071-4239-adb2-40f7a7d74aee%28Office.15%29.aspx)

