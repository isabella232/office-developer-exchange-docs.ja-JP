---
title: CopyFolder 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopyFolder
api_type:
- schema
ms.assetid: c7ea0d68-9793-4144-b378-d99536776db9
description: CopyFolder 操作は、メールボックス内のフォルダーをコピーします。
ms.openlocfilehash: 1f9a7a3f3ede2d3cf8f9d41677d8ce0487266f17
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/01/2020
ms.locfileid: "44468895"
---
# <a name="copyfolder-operation"></a><span data-ttu-id="2544a-103">CopyFolder 操作</span><span class="sxs-lookup"><span data-stu-id="2544a-103">CopyFolder operation</span></span>

<span data-ttu-id="2544a-104">CopyFolder 操作は、メールボックス内のフォルダーをコピーします。</span><span class="sxs-lookup"><span data-stu-id="2544a-104">The CopyFolder operation copies folders in a mailbox.</span></span>
  
## <a name="using-the-copyfolder-operation"></a><span data-ttu-id="2544a-105">CopyFolder 操作の使用</span><span class="sxs-lookup"><span data-stu-id="2544a-105">Using the CopyFolder operation</span></span>

<span data-ttu-id="2544a-106">CopyFolder 操作は、 [movefolder 操作](movefolder-operation.md)に似ています。</span><span class="sxs-lookup"><span data-stu-id="2544a-106">The CopyFolder operation is similar to the [MoveFolder operation](movefolder-operation.md).</span></span> <span data-ttu-id="2544a-107">識別されたフォルダーをコピーし、コピーしたフォルダーの**Id**および**changekey**を返します。</span><span class="sxs-lookup"><span data-stu-id="2544a-107">It copies identified folders and returns the **Id** and **ChangeKey** of the copied folders.</span></span> 
  
## <a name="copyfolder-request-example"></a><span data-ttu-id="2544a-108">CopyFolder 要求の例</span><span class="sxs-lookup"><span data-stu-id="2544a-108">CopyFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="2544a-109">説明</span><span class="sxs-lookup"><span data-stu-id="2544a-109">Description</span></span>

<span data-ttu-id="2544a-110">次の CopyFolder 要求の例は、フォルダーを受信トレイフォルダーにコピーする方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="2544a-110">The following example of a CopyFolder request shows how to copy folders into the Inbox folder.</span></span>
  
> [!NOTE]
> <span data-ttu-id="2544a-111">[FolderId](folderid.md)要素の**Id**属性の値は、読みやすくするために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="2544a-111">The value of the **Id** attribute of the [FolderId](folderid.md) element has been shortened for readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="2544a-112">コード</span><span class="sxs-lookup"><span data-stu-id="2544a-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CopyFolder xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ToFolderId>
        <t:DistinguishedFolderId Id="inbox"/>
      </ToFolderId>
      <FolderIds>
        <t:FolderId Id="AS4A=" ChangeKey="fsVU4=="/>
        <t:FolderId Id="AS4AU=" ChangeKey="fsVU4o=="/>
      </FolderIds>
    </CopyFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="2544a-113">コメント</span><span class="sxs-lookup"><span data-stu-id="2544a-113">Comments</span></span>

<span data-ttu-id="2544a-114">フォルダーは、 [ToFolderId](tofolderid.md)または[FolderIds](folderids.md)要素で使用するために、 [DistinguishedFolderId](distinguishedfolderid.md)要素または[FolderId](folderid.md)要素のいずれかで識別できます。</span><span class="sxs-lookup"><span data-stu-id="2544a-114">Folders can be identified by either the [DistinguishedFolderId](distinguishedfolderid.md) element or the [FolderId](folderid.md) element for use in either the [ToFolderId](tofolderid.md) or the [FolderIds](folderids.md) elements.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="2544a-115">Request 要素</span><span class="sxs-lookup"><span data-stu-id="2544a-115">Request elements</span></span>

<span data-ttu-id="2544a-116">要求では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="2544a-116">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="2544a-117">CopyFolder</span><span class="sxs-lookup"><span data-stu-id="2544a-117">CopyFolder</span></span>](copyfolder.md)
    
- [<span data-ttu-id="2544a-118">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="2544a-118">ToFolderId</span></span>](tofolderid.md)
    
- [<span data-ttu-id="2544a-119">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="2544a-119">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="2544a-120">FolderIds</span><span class="sxs-lookup"><span data-stu-id="2544a-120">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="2544a-121">FolderId</span><span class="sxs-lookup"><span data-stu-id="2544a-121">FolderId</span></span>](folderid.md)
    
> [!NOTE]
> <span data-ttu-id="2544a-122">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="2544a-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
<span data-ttu-id="2544a-123">CopyFolder 操作の要求メッセージに関するその他のオプションについては、スキーマ階層を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2544a-123">To find other options for the request message of the CopyFolder operation, explore the schema hierarchy.</span></span> <span data-ttu-id="2544a-124">[Copyfolder](copyfolder.md)要素から開始します。</span><span class="sxs-lookup"><span data-stu-id="2544a-124">Start at the [CopyFolder](copyfolder.md) element.</span></span> 
  
## <a name="successful-copyfolder-response"></a><span data-ttu-id="2544a-125">成功した CopyFolder 応答</span><span class="sxs-lookup"><span data-stu-id="2544a-125">Successful CopyFolder response</span></span>

### <a name="description"></a><span data-ttu-id="2544a-126">説明</span><span class="sxs-lookup"><span data-stu-id="2544a-126">Description</span></span>

<span data-ttu-id="2544a-127">次の例は、CopyFolder 要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="2544a-127">The following example shows a successful response to the CopyFolder request.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="2544a-128">読みやすくするために、フォルダー ID と変更キーが短縮されています。</span><span class="sxs-lookup"><span data-stu-id="2544a-128">The folder ID and the change key have been shortened to preserve readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="2544a-129">コード</span><span class="sxs-lookup"><span data-stu-id="2544a-129">Code</span></span>

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
    <CopyFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CopyFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="AS4AUn=" ChangeKey="fsVU4o==" />
            </t:Folder>
          </m:Folders>
        </m:CopyFolderResponseMessage>
      </m:ResponseMessages>
    </CopyFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comment"></a><span data-ttu-id="2544a-130">コメント</span><span class="sxs-lookup"><span data-stu-id="2544a-130">Comment</span></span>

<span data-ttu-id="2544a-131">応答で返される[FolderId](folderid.md)要素は、新しいフォルダーの場所にコピーされたフォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="2544a-131">The [FolderId](folderid.md) element that is returned in the response represents the folder that was copied in the new folder location.</span></span> 
  
### <a name="response-elements"></a><span data-ttu-id="2544a-132">Response 要素</span><span class="sxs-lookup"><span data-stu-id="2544a-132">Response elements</span></span>

<span data-ttu-id="2544a-133">応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="2544a-133">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="2544a-134">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="2544a-134">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="2544a-135">CopyFolderResponse</span><span class="sxs-lookup"><span data-stu-id="2544a-135">CopyFolderResponse</span></span>](copyfolderresponse.md)
    
- [<span data-ttu-id="2544a-136">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="2544a-136">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="2544a-137">CopyFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="2544a-137">CopyFolderResponseMessage</span></span>](copyfolderresponsemessage.md)
    
- [<span data-ttu-id="2544a-138">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="2544a-138">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="2544a-139">フォルダー</span><span class="sxs-lookup"><span data-stu-id="2544a-139">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="2544a-140">Folder</span><span class="sxs-lookup"><span data-stu-id="2544a-140">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="2544a-141">FolderId</span><span class="sxs-lookup"><span data-stu-id="2544a-141">FolderId</span></span>](folderid.md)
    
<span data-ttu-id="2544a-142">CopyFolder 操作の応答メッセージに関するその他のオプションについては、スキーマ階層を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2544a-142">To find other options for the response message of the CopyFolder operation, explore the schema hierarchy.</span></span> <span data-ttu-id="2544a-143">[Copyfolderresponse](copyfolderresponse.md)要素から開始します。</span><span class="sxs-lookup"><span data-stu-id="2544a-143">Start at the [CopyFolderResponse](copyfolderresponse.md) element.</span></span> 
  
## <a name="copyfolder-error-response"></a><span data-ttu-id="2544a-144">CopyFolder エラー応答</span><span class="sxs-lookup"><span data-stu-id="2544a-144">CopyFolder error response</span></span>

### <a name="description"></a><span data-ttu-id="2544a-145">説明</span><span class="sxs-lookup"><span data-stu-id="2544a-145">Description</span></span>

<span data-ttu-id="2544a-146">次の例は、CopyFolder 要求に対するエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="2544a-146">The following example shows an error response to a CopyFolder request.</span></span> <span data-ttu-id="2544a-147">同じ表示名のフォルダーが既に存在するため、エラーが発生しました。</span><span class="sxs-lookup"><span data-stu-id="2544a-147">The error occurred because a folder with the same display name already exists.</span></span>
  
### <a name="code"></a><span data-ttu-id="2544a-148">コード</span><span class="sxs-lookup"><span data-stu-id="2544a-148">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CopyFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CopyFolderResponseMessage ResponseClass="Error">
          <m:MessageText>The move or copy operation failed.</m:MessageText>
          <m:ResponseCode>ErrorMoveCopyFailed</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Folders />
        </m:CopyFolderResponseMessage>
      </m:ResponseMessages>
    </CopyFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="2544a-149">エラー応答要素</span><span class="sxs-lookup"><span data-stu-id="2544a-149">Error response elements</span></span>

<span data-ttu-id="2544a-150">エラー応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="2544a-150">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="2544a-151">CopyFolderResponse</span><span class="sxs-lookup"><span data-stu-id="2544a-151">CopyFolderResponse</span></span>](copyfolderresponse.md)
    
- [<span data-ttu-id="2544a-152">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="2544a-152">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="2544a-153">CopyFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="2544a-153">CopyFolderResponseMessage</span></span>](copyfolderresponsemessage.md)
    
- [<span data-ttu-id="2544a-154">MessageText</span><span class="sxs-lookup"><span data-stu-id="2544a-154">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="2544a-155">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="2544a-155">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="2544a-156">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="2544a-156">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="2544a-157">フォルダー</span><span class="sxs-lookup"><span data-stu-id="2544a-157">Folders</span></span>](folders-ex15websvcsotherref.md)
    
<span data-ttu-id="2544a-158">CopyFolder 操作のエラー応答メッセージに関するその他のオプションについては、スキーマ階層を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2544a-158">To find other options for the error response message of the CopyFolder operation, explore the schema hierarchy.</span></span> <span data-ttu-id="2544a-159">[Copyfolderresponse](copyfolderresponse.md)要素から開始します。</span><span class="sxs-lookup"><span data-stu-id="2544a-159">Start at the [CopyFolderResponse](copyfolderresponse.md) element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="2544a-160">関連項目</span><span class="sxs-lookup"><span data-stu-id="2544a-160">See also</span></span>

- [<span data-ttu-id="2544a-161">MoveFolder 操作</span><span class="sxs-lookup"><span data-stu-id="2544a-161">MoveFolder operation</span></span>](movefolder-operation.md)
- [<span data-ttu-id="2544a-162">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="2544a-162">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

