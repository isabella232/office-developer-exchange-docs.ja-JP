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
ms.openlocfilehash: a83444ff0927a3c8fe075c79d44d02357a737773
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759777"
---
# <a name="copyfolder-operation"></a><span data-ttu-id="94f7a-103">CopyFolder 操作</span><span class="sxs-lookup"><span data-stu-id="94f7a-103">CopyFolder operation</span></span>

<span data-ttu-id="94f7a-104">CopyFolder 操作は、メールボックス内のフォルダーをコピーします。</span><span class="sxs-lookup"><span data-stu-id="94f7a-104">The CopyFolder operation copies folders in a mailbox.</span></span>
  
## <a name="using-the-copyfolder-operation"></a><span data-ttu-id="94f7a-105">CopyFolder 操作を使用します。</span><span class="sxs-lookup"><span data-stu-id="94f7a-105">Using the CopyFolder operation</span></span>

<span data-ttu-id="94f7a-106">CopyFolder 操作は、 [MoveFolder 操作](movefolder-operation.md)に似ています。</span><span class="sxs-lookup"><span data-stu-id="94f7a-106">The CopyFolder operation is similar to the [MoveFolder operation](movefolder-operation.md).</span></span> <span data-ttu-id="94f7a-107">指定されたフォルダーにコピーし、 **Id**と、コピーしたフォルダーの**変更キー**を取得します。</span><span class="sxs-lookup"><span data-stu-id="94f7a-107">It copies identified folders and returns the **Id** and **ChangeKey** of the copied folders.</span></span> 
  
## <a name="copyfolder-request-example"></a><span data-ttu-id="94f7a-108">CopyFolder 要求の例</span><span class="sxs-lookup"><span data-stu-id="94f7a-108">CopyFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="94f7a-109">説明</span><span class="sxs-lookup"><span data-stu-id="94f7a-109">Description</span></span>

<span data-ttu-id="94f7a-110">CopyFolder 要求の次の例では、受信トレイ フォルダーにフォルダーをコピーする方法を示します。</span><span class="sxs-lookup"><span data-stu-id="94f7a-110">The following example of a CopyFolder request shows how to copy folders into the Inbox folder.</span></span>
  
> [!NOTE]
> <span data-ttu-id="94f7a-111">[フォルダー Id](folderid.md)要素の**Id**属性の値が小さすぎると読みやすくするためです。</span><span class="sxs-lookup"><span data-stu-id="94f7a-111">The value of the **Id** attribute of the [FolderId](folderid.md) element has been shortened for readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="94f7a-112">コード</span><span class="sxs-lookup"><span data-stu-id="94f7a-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CopyFolder xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="94f7a-113">コメント</span><span class="sxs-lookup"><span data-stu-id="94f7a-113">Comments</span></span>

<span data-ttu-id="94f7a-114">フォルダーは、 [DistinguishedFolderId](distinguishedfolderid.md)要素またはいずれか、 [ToFolderId](tofolderid.md)で使用するための[フォルダー Id](folderid.md)の要素または[FolderIds](folderids.md)要素のいずれかで識別できます。</span><span class="sxs-lookup"><span data-stu-id="94f7a-114">Folders can be identified by either the [DistinguishedFolderId](distinguishedfolderid.md) element or the [FolderId](folderid.md) element for use in either the [ToFolderId](tofolderid.md) or the [FolderIds](folderids.md) elements.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="94f7a-115">要素を要求します。</span><span class="sxs-lookup"><span data-stu-id="94f7a-115">Request elements</span></span>

<span data-ttu-id="94f7a-116">次の要素は、要求で使用されます。</span><span class="sxs-lookup"><span data-stu-id="94f7a-116">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="94f7a-117">CopyFolder</span><span class="sxs-lookup"><span data-stu-id="94f7a-117">CopyFolder</span></span>](copyfolder.md)
    
- [<span data-ttu-id="94f7a-118">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="94f7a-118">ToFolderId</span></span>](tofolderid.md)
    
- [<span data-ttu-id="94f7a-119">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="94f7a-119">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="94f7a-120">FolderIds</span><span class="sxs-lookup"><span data-stu-id="94f7a-120">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="94f7a-121">フォルダー Id</span><span class="sxs-lookup"><span data-stu-id="94f7a-121">FolderId</span></span>](folderid.md)
    
> [!NOTE]
> <span data-ttu-id="94f7a-122">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="94f7a-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
<span data-ttu-id="94f7a-123">CopyFolder 操作の要求メッセージには、他のオプションを検索するには、スキーマの階層構造を表示します。</span><span class="sxs-lookup"><span data-stu-id="94f7a-123">To find other options for the request message of the CopyFolder operation, explore the schema hierarchy.</span></span> <span data-ttu-id="94f7a-124">[CopyFolder](copyfolder.md)要素から開始します。</span><span class="sxs-lookup"><span data-stu-id="94f7a-124">Start at the [CopyFolder](copyfolder.md) element.</span></span> 
  
## <a name="successful-copyfolder-response"></a><span data-ttu-id="94f7a-125">CopyFolder の正常な応答</span><span class="sxs-lookup"><span data-stu-id="94f7a-125">Successful CopyFolder response</span></span>

### <a name="description"></a><span data-ttu-id="94f7a-126">説明</span><span class="sxs-lookup"><span data-stu-id="94f7a-126">Description</span></span>

<span data-ttu-id="94f7a-127">CopyFolder 要求に正常な応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="94f7a-127">The following example shows a successful response to the CopyFolder request.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="94f7a-128">フォルダー ID と変更キーは、読みやすさを保持するために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="94f7a-128">The folder ID and the change key have been shortened to preserve readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="94f7a-129">コード</span><span class="sxs-lookup"><span data-stu-id="94f7a-129">Code</span></span>

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
    <CopyFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comment"></a><span data-ttu-id="94f7a-130">Comment</span><span class="sxs-lookup"><span data-stu-id="94f7a-130">Comment</span></span>

<span data-ttu-id="94f7a-131">応答で返される[フォルダー Id](folderid.md)要素は、新しいフォルダーの場所にコピーしたフォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="94f7a-131">The [FolderId](folderid.md) element that is returned in the response represents the folder that was copied in the new folder location.</span></span> 
  
### <a name="response-elements"></a><span data-ttu-id="94f7a-132">応答の要素</span><span class="sxs-lookup"><span data-stu-id="94f7a-132">Response elements</span></span>

<span data-ttu-id="94f7a-133">次の要素は、応答で使用されます。</span><span class="sxs-lookup"><span data-stu-id="94f7a-133">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="94f7a-134">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="94f7a-134">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="94f7a-135">CopyFolderResponse</span><span class="sxs-lookup"><span data-stu-id="94f7a-135">CopyFolderResponse</span></span>](copyfolderresponse.md)
    
- [<span data-ttu-id="94f7a-136">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="94f7a-136">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="94f7a-137">CopyFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="94f7a-137">CopyFolderResponseMessage</span></span>](copyfolderresponsemessage.md)
    
- [<span data-ttu-id="94f7a-138">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="94f7a-138">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="94f7a-139">フォルダー</span><span class="sxs-lookup"><span data-stu-id="94f7a-139">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="94f7a-140">Folder</span><span class="sxs-lookup"><span data-stu-id="94f7a-140">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="94f7a-141">フォルダー Id</span><span class="sxs-lookup"><span data-stu-id="94f7a-141">FolderId</span></span>](folderid.md)
    
<span data-ttu-id="94f7a-142">CopyFolder 操作の応答メッセージには、他のオプションを検索するには、スキーマの階層構造を表示します。</span><span class="sxs-lookup"><span data-stu-id="94f7a-142">To find other options for the response message of the CopyFolder operation, explore the schema hierarchy.</span></span> <span data-ttu-id="94f7a-143">[CopyFolderResponse](copyfolderresponse.md)要素から開始します。</span><span class="sxs-lookup"><span data-stu-id="94f7a-143">Start at the [CopyFolderResponse](copyfolderresponse.md) element.</span></span> 
  
## <a name="copyfolder-error-response"></a><span data-ttu-id="94f7a-144">CopyFolder エラー応答</span><span class="sxs-lookup"><span data-stu-id="94f7a-144">CopyFolder error response</span></span>

### <a name="description"></a><span data-ttu-id="94f7a-145">説明</span><span class="sxs-lookup"><span data-stu-id="94f7a-145">Description</span></span>

<span data-ttu-id="94f7a-146">CopyFolder 要求に対してエラー応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="94f7a-146">The following example shows an error response to a CopyFolder request.</span></span> <span data-ttu-id="94f7a-147">同じ表示名を持つフォルダーが既に存在するため、エラーが発生しました。</span><span class="sxs-lookup"><span data-stu-id="94f7a-147">The error occurred because a folder with the same display name already exists.</span></span>
  
### <a name="code"></a><span data-ttu-id="94f7a-148">コード</span><span class="sxs-lookup"><span data-stu-id="94f7a-148">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CopyFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="error-response-elements"></a><span data-ttu-id="94f7a-149">エラー応答の要素</span><span class="sxs-lookup"><span data-stu-id="94f7a-149">Error response elements</span></span>

<span data-ttu-id="94f7a-150">エラー応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="94f7a-150">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="94f7a-151">CopyFolderResponse</span><span class="sxs-lookup"><span data-stu-id="94f7a-151">CopyFolderResponse</span></span>](copyfolderresponse.md)
    
- [<span data-ttu-id="94f7a-152">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="94f7a-152">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="94f7a-153">CopyFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="94f7a-153">CopyFolderResponseMessage</span></span>](copyfolderresponsemessage.md)
    
- [<span data-ttu-id="94f7a-154">MessageText</span><span class="sxs-lookup"><span data-stu-id="94f7a-154">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="94f7a-155">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="94f7a-155">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="94f7a-156">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="94f7a-156">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="94f7a-157">フォルダー</span><span class="sxs-lookup"><span data-stu-id="94f7a-157">Folders</span></span>](folders-ex15websvcsotherref.md)
    
<span data-ttu-id="94f7a-158">CopyFolder 操作の応答のエラー メッセージには、他のオプションを検索するには、スキーマの階層構造を表示します。</span><span class="sxs-lookup"><span data-stu-id="94f7a-158">To find other options for the error response message of the CopyFolder operation, explore the schema hierarchy.</span></span> <span data-ttu-id="94f7a-159">[CopyFolderResponse](copyfolderresponse.md)要素から開始します。</span><span class="sxs-lookup"><span data-stu-id="94f7a-159">Start at the [CopyFolderResponse](copyfolderresponse.md) element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="94f7a-160">関連項目</span><span class="sxs-lookup"><span data-stu-id="94f7a-160">See also</span></span>

- [<span data-ttu-id="94f7a-161">MoveFolder 操作</span><span class="sxs-lookup"><span data-stu-id="94f7a-161">MoveFolder operation</span></span>](movefolder-operation.md)
- [<span data-ttu-id="94f7a-162">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="94f7a-162">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

