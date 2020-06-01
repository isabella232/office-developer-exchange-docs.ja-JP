---
title: MoveFolder 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MoveFolder
api_type:
- schema
ms.assetid: c7233966-6c87-4a14-8156-b1610760176d
description: MoveFolder 操作は、指定されたフォルダーからフォルダーを移動して、別のフォルダーに格納します。
ms.openlocfilehash: dc572130ca3b2f2b152abbb4a8b68cc6f67790e8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460583"
---
# <a name="movefolder-operation"></a><span data-ttu-id="74acb-103">MoveFolder 操作</span><span class="sxs-lookup"><span data-stu-id="74acb-103">MoveFolder operation</span></span>

<span data-ttu-id="74acb-104">MoveFolder 操作は、指定されたフォルダーからフォルダーを移動して、別のフォルダーに格納します。</span><span class="sxs-lookup"><span data-stu-id="74acb-104">The MoveFolder operation moves folders from a specified folder and puts them in another folder.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="74acb-105">注釈</span><span class="sxs-lookup"><span data-stu-id="74acb-105">Remarks</span></span>

<span data-ttu-id="74acb-106">MoveFolder 操作は、CopyFolder 操作に似ています。</span><span class="sxs-lookup"><span data-stu-id="74acb-106">The MoveFolder operation is similar to the CopyFolder operation.</span></span> <span data-ttu-id="74acb-107">識別フォルダーを移動することはできません。</span><span class="sxs-lookup"><span data-stu-id="74acb-107">You cannot move distinguished folders.</span></span> <span data-ttu-id="74acb-108">複数のフォルダーを、宛先フォルダーに一度に移動できます。</span><span class="sxs-lookup"><span data-stu-id="74acb-108">You can move multiple folders at one time to the destination folder.</span></span>
  
## <a name="movefolder-request-example"></a><span data-ttu-id="74acb-109">MoveFolder 要求の例</span><span class="sxs-lookup"><span data-stu-id="74acb-109">MoveFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="74acb-110">説明</span><span class="sxs-lookup"><span data-stu-id="74acb-110">Description</span></span>

<span data-ttu-id="74acb-111">次の MoveFolder 要求の例は、 [FolderId](folderid.md)によって識別されるフォルダーを移動する要求を形成し、フォルダーを迷惑メールの識別フォルダーに入れる方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="74acb-111">The following example of a MoveFolder request shows how to form a request to move a folder identified by the [FolderId](folderid.md) and put the folder in the Junk E-mail distinguished folder.</span></span> 
  
### <a name="code"></a><span data-ttu-id="74acb-112">コード</span><span class="sxs-lookup"><span data-stu-id="74acb-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <MoveFolder xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ToFolderId>
        <t:DistinguishedFolderId Id="junkemail"/>
      </ToFolderId>
      <FolderIds>
        <t:FolderId Id="AScAc"/>
      </FolderIds>
    </MoveFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="74acb-113">コメント</span><span class="sxs-lookup"><span data-stu-id="74acb-113">Comments</span></span>

> [!NOTE]
> <span data-ttu-id="74acb-114">[FolderId](folderid.md)要素の ID 属性の値は、読みやすくするために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="74acb-114">The value of the ID attribute of the [FolderId](folderid.md) element has been shortened for readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="74acb-115">Request 要素</span><span class="sxs-lookup"><span data-stu-id="74acb-115">Request elements</span></span>

<span data-ttu-id="74acb-116">この MoveFolder 要求には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="74acb-116">This MoveFolder request includes the following elements:</span></span>
  
- [<span data-ttu-id="74acb-117">MoveFolder</span><span class="sxs-lookup"><span data-stu-id="74acb-117">MoveFolder</span></span>](movefolder.md)
    
- [<span data-ttu-id="74acb-118">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="74acb-118">ToFolderId</span></span>](tofolderid.md)
    
- [<span data-ttu-id="74acb-119">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="74acb-119">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="74acb-120">FolderIds</span><span class="sxs-lookup"><span data-stu-id="74acb-120">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="74acb-121">FolderId</span><span class="sxs-lookup"><span data-stu-id="74acb-121">FolderId</span></span>](folderid.md)
    
<span data-ttu-id="74acb-122">MoveFolder 要求の形成に使用できるその他の要素については、スキーマを参照してください。</span><span class="sxs-lookup"><span data-stu-id="74acb-122">See the schema for additional elements that you can use to form a MoveFolder request.</span></span>
  
> [!NOTE]
> <span data-ttu-id="74acb-123">スキーマの既定の場所は、クライアントアクセスサーバーの役割がインストールされているコンピューター上の EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="74acb-123">The default location of the schema is in the EWS virtual directory on the computer that has the Client Access server role installed.</span></span> 
  
## <a name="successful-movefolder-response-example"></a><span data-ttu-id="74acb-124">成功した MoveFolder 応答の例</span><span class="sxs-lookup"><span data-stu-id="74acb-124">Successful MoveFolder response example</span></span>

### <a name="description"></a><span data-ttu-id="74acb-125">説明</span><span class="sxs-lookup"><span data-stu-id="74acb-125">Description</span></span>

<span data-ttu-id="74acb-126">次の例は、MoveFolder 要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="74acb-126">The following example shows a successful response to the MoveFolder request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="74acb-127">コード</span><span class="sxs-lookup"><span data-stu-id="74acb-127">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <MoveFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:MoveFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="AAAlAFV" ChangeKey="AQAAAB" />
            </t:Folder>
          </m:Folders>
        </m:MoveFolderResponseMessage>
      </m:ResponseMessages>
    </MoveFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="74acb-128">コメント</span><span class="sxs-lookup"><span data-stu-id="74acb-128">Comments</span></span>

> [!NOTE]
> <span data-ttu-id="74acb-129">読みやすくするために、フォルダー ID と変更キーが短縮されています。</span><span class="sxs-lookup"><span data-stu-id="74acb-129">The folder ID and the change key have been shortened to preserve readability.</span></span> 
  
<span data-ttu-id="74acb-130">応答で返される FolderId は、新しいフォルダーの場所に移動されたフォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="74acb-130">The FolderId that is returned in the response represents the folder that was moved to the new the folder location.</span></span>
  
### <a name="response-elements"></a><span data-ttu-id="74acb-131">Response 要素</span><span class="sxs-lookup"><span data-stu-id="74acb-131">Response elements</span></span>

<span data-ttu-id="74acb-132">MoveFolder 応答には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="74acb-132">The MoveFolder response includes the following elements:</span></span>
  
- [<span data-ttu-id="74acb-133">MoveFolderResponse</span><span class="sxs-lookup"><span data-stu-id="74acb-133">MoveFolderResponse</span></span>](movefolderresponse.md)
    
- [<span data-ttu-id="74acb-134">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="74acb-134">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="74acb-135">MoveFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="74acb-135">MoveFolderResponseMessage</span></span>](movefolderresponsemessage.md)
    
- [<span data-ttu-id="74acb-136">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="74acb-136">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="74acb-137">フォルダー</span><span class="sxs-lookup"><span data-stu-id="74acb-137">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="74acb-138">Folder</span><span class="sxs-lookup"><span data-stu-id="74acb-138">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="74acb-139">FolderId</span><span class="sxs-lookup"><span data-stu-id="74acb-139">FolderId</span></span>](folderid.md)
    
## <a name="movefolder-error-response-example"></a><span data-ttu-id="74acb-140">MoveFolder エラー応答の例</span><span class="sxs-lookup"><span data-stu-id="74acb-140">MoveFolder Error response example</span></span>

### <a name="description"></a><span data-ttu-id="74acb-141">説明</span><span class="sxs-lookup"><span data-stu-id="74acb-141">Description</span></span>

<span data-ttu-id="74acb-142">次の例は、識別フォルダーを移動しようとしたときに発生するエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="74acb-142">The following example shows an error response that occurs when you try to move a distinguished folder.</span></span>
  
### <a name="code"></a><span data-ttu-id="74acb-143">コード</span><span class="sxs-lookup"><span data-stu-id="74acb-143">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
                 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                 xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <MoveFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:MoveFolderResponseMessage ResponseClass="Error">
          <m:MessageText>Cannot move distinguished folder.</m:MessageText>
          <m:ResponseCode>ErrorMoveDistinguishedFolder</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Folders />
        </m:MoveFolderResponseMessage>
      </m:ResponseMessages>
    </MoveFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="74acb-144">エラー応答要素</span><span class="sxs-lookup"><span data-stu-id="74acb-144">Error response elements</span></span>

<span data-ttu-id="74acb-145">MoveFolder エラー応答には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="74acb-145">The MoveFolder error response includes the following elements:</span></span>
  
- [<span data-ttu-id="74acb-146">MoveFolderResponse</span><span class="sxs-lookup"><span data-stu-id="74acb-146">MoveFolderResponse</span></span>](movefolderresponse.md)
    
- [<span data-ttu-id="74acb-147">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="74acb-147">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="74acb-148">MoveFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="74acb-148">MoveFolderResponseMessage</span></span>](movefolderresponsemessage.md)
    
- [<span data-ttu-id="74acb-149">MessageText</span><span class="sxs-lookup"><span data-stu-id="74acb-149">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="74acb-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="74acb-150">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="74acb-151">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="74acb-151">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="74acb-152">フォルダー</span><span class="sxs-lookup"><span data-stu-id="74acb-152">Folders</span></span>](folders-ex15websvcsotherref.md)
    
## <a name="see-also"></a><span data-ttu-id="74acb-153">関連項目</span><span class="sxs-lookup"><span data-stu-id="74acb-153">See also</span></span>



[<span data-ttu-id="74acb-154">CopyFolder 操作</span><span class="sxs-lookup"><span data-stu-id="74acb-154">CopyFolder operation</span></span>](copyfolder-operation.md)

