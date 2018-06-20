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
description: MoveFolder 操作は、指定したフォルダーからフォルダーを移動して、別のフォルダーに保存します。
ms.openlocfilehash: 5da6929f11ce9ba74db190db6d799f25974d2192
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832490"
---
# <a name="movefolder-operation"></a><span data-ttu-id="ba0b8-103">MoveFolder 操作</span><span class="sxs-lookup"><span data-stu-id="ba0b8-103">MoveFolder operation</span></span>

<span data-ttu-id="ba0b8-104">MoveFolder 操作は、指定したフォルダーからフォルダーを移動して、別のフォルダーに保存します。</span><span class="sxs-lookup"><span data-stu-id="ba0b8-104">The MoveFolder operation moves folders from a specified folder and puts them in another folder.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ba0b8-105">備考</span><span class="sxs-lookup"><span data-stu-id="ba0b8-105">Remarks</span></span>

<span data-ttu-id="ba0b8-106">MoveFolder 操作は、CopyFolder 操作に似ています。</span><span class="sxs-lookup"><span data-stu-id="ba0b8-106">The MoveFolder operation is similar to the CopyFolder operation.</span></span> <span data-ttu-id="ba0b8-107">識別フォルダーを移動することはできません。</span><span class="sxs-lookup"><span data-stu-id="ba0b8-107">You cannot move distinguished folders.</span></span> <span data-ttu-id="ba0b8-108">コピー先のフォルダーを同時に複数のフォルダーを移動できます。</span><span class="sxs-lookup"><span data-stu-id="ba0b8-108">You can move multiple folders at one time to the destination folder.</span></span>
  
## <a name="movefolder-request-example"></a><span data-ttu-id="ba0b8-109">MoveFolder 要求の例</span><span class="sxs-lookup"><span data-stu-id="ba0b8-109">MoveFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="ba0b8-110">説明</span><span class="sxs-lookup"><span data-stu-id="ba0b8-110">Description</span></span>

<span data-ttu-id="ba0b8-111">MoveFolder 要求の次の例では、[フォルダー Id](folderid.md)で識別されるフォルダーに移動し、[迷惑メールの識別フォルダーでフォルダーを配置する要求を作成する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="ba0b8-111">The following example of a MoveFolder request shows how to form a request to move a folder identified by the [FolderId](folderid.md) and put the folder in the Junk E-mail distinguished folder.</span></span> 
  
### <a name="code"></a><span data-ttu-id="ba0b8-112">コード</span><span class="sxs-lookup"><span data-stu-id="ba0b8-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <MoveFolder xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="ba0b8-113">コメント</span><span class="sxs-lookup"><span data-stu-id="ba0b8-113">Comments</span></span>

> [!NOTE]
> <span data-ttu-id="ba0b8-114">[フォルダー Id](folderid.md)要素の ID 属性の値が小さすぎると読みやすくするためです。</span><span class="sxs-lookup"><span data-stu-id="ba0b8-114">The value of the ID attribute of the [FolderId](folderid.md) element has been shortened for readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="ba0b8-115">要素を要求します。</span><span class="sxs-lookup"><span data-stu-id="ba0b8-115">Request elements</span></span>

<span data-ttu-id="ba0b8-116">MoveFolder 要求には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ba0b8-116">This MoveFolder request includes the following elements:</span></span>
  
- [<span data-ttu-id="ba0b8-117">MoveFolder</span><span class="sxs-lookup"><span data-stu-id="ba0b8-117">MoveFolder</span></span>](movefolder.md)
    
- [<span data-ttu-id="ba0b8-118">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="ba0b8-118">ToFolderId</span></span>](tofolderid.md)
    
- [<span data-ttu-id="ba0b8-119">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="ba0b8-119">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="ba0b8-120">FolderIds</span><span class="sxs-lookup"><span data-stu-id="ba0b8-120">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="ba0b8-121">フォルダー Id</span><span class="sxs-lookup"><span data-stu-id="ba0b8-121">FolderId</span></span>](folderid.md)
    
<span data-ttu-id="ba0b8-122">MoveFolder 要求を形成するために使用できるその他の要素のスキーマを参照してください。</span><span class="sxs-lookup"><span data-stu-id="ba0b8-122">See the schema for additional elements that you can use to form a MoveFolder request.</span></span>
  
> [!NOTE]
> <span data-ttu-id="ba0b8-123">スキーマの既定の場所は、クライアント アクセス サーバーの役割がインストールされているコンピューターで EWS 仮想ディレクトリには。</span><span class="sxs-lookup"><span data-stu-id="ba0b8-123">The default location of the schema is in the EWS virtual directory on the computer that has the Client Access server role installed.</span></span> 
  
## <a name="successful-movefolder-response-example"></a><span data-ttu-id="ba0b8-124">MoveFolder 応答の成功の例</span><span class="sxs-lookup"><span data-stu-id="ba0b8-124">Successful MoveFolder response example</span></span>

### <a name="description"></a><span data-ttu-id="ba0b8-125">説明</span><span class="sxs-lookup"><span data-stu-id="ba0b8-125">Description</span></span>

<span data-ttu-id="ba0b8-126">MoveFolder 要求に正常な応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ba0b8-126">The following example shows a successful response to the MoveFolder request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="ba0b8-127">コード</span><span class="sxs-lookup"><span data-stu-id="ba0b8-127">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <MoveFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="ba0b8-128">コメント</span><span class="sxs-lookup"><span data-stu-id="ba0b8-128">Comments</span></span>

> [!NOTE]
> <span data-ttu-id="ba0b8-129">フォルダー ID と変更キーは、読みやすさを保持するために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="ba0b8-129">The folder ID and the change key have been shortened to preserve readability.</span></span> 
  
<span data-ttu-id="ba0b8-130">応答で返されるフォルダー Id があったフォルダーを表す新しいフォルダーの場所に移動します。</span><span class="sxs-lookup"><span data-stu-id="ba0b8-130">The FolderId that is returned in the response represents the folder that was moved to the new the folder location.</span></span>
  
### <a name="response-elements"></a><span data-ttu-id="ba0b8-131">応答の要素</span><span class="sxs-lookup"><span data-stu-id="ba0b8-131">Response elements</span></span>

<span data-ttu-id="ba0b8-132">MoveFolder の応答には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ba0b8-132">The MoveFolder response includes the following elements:</span></span>
  
- [<span data-ttu-id="ba0b8-133">MoveFolderResponse</span><span class="sxs-lookup"><span data-stu-id="ba0b8-133">MoveFolderResponse</span></span>](movefolderresponse.md)
    
- [<span data-ttu-id="ba0b8-134">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="ba0b8-134">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="ba0b8-135">MoveFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ba0b8-135">MoveFolderResponseMessage</span></span>](movefolderresponsemessage.md)
    
- [<span data-ttu-id="ba0b8-136">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="ba0b8-136">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="ba0b8-137">フォルダー</span><span class="sxs-lookup"><span data-stu-id="ba0b8-137">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="ba0b8-138">Folder</span><span class="sxs-lookup"><span data-stu-id="ba0b8-138">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="ba0b8-139">フォルダー Id</span><span class="sxs-lookup"><span data-stu-id="ba0b8-139">FolderId</span></span>](folderid.md)
    
## <a name="movefolder-error-response-example"></a><span data-ttu-id="ba0b8-140">MoveFolder エラー応答の例</span><span class="sxs-lookup"><span data-stu-id="ba0b8-140">MoveFolder Error response example</span></span>

### <a name="description"></a><span data-ttu-id="ba0b8-141">説明</span><span class="sxs-lookup"><span data-stu-id="ba0b8-141">Description</span></span>

<span data-ttu-id="ba0b8-142">識別フォルダーを移動しようとするときに発生するエラー応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ba0b8-142">The following example shows an error response that occurs when you try to move a distinguished folder.</span></span>
  
### <a name="code"></a><span data-ttu-id="ba0b8-143">コード</span><span class="sxs-lookup"><span data-stu-id="ba0b8-143">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
                 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                 xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <MoveFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="error-response-elements"></a><span data-ttu-id="ba0b8-144">エラー応答の要素</span><span class="sxs-lookup"><span data-stu-id="ba0b8-144">Error response elements</span></span>

<span data-ttu-id="ba0b8-145">MoveFolder エラー応答には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ba0b8-145">The MoveFolder error response includes the following elements:</span></span>
  
- [<span data-ttu-id="ba0b8-146">MoveFolderResponse</span><span class="sxs-lookup"><span data-stu-id="ba0b8-146">MoveFolderResponse</span></span>](movefolderresponse.md)
    
- [<span data-ttu-id="ba0b8-147">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="ba0b8-147">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="ba0b8-148">MoveFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ba0b8-148">MoveFolderResponseMessage</span></span>](movefolderresponsemessage.md)
    
- [<span data-ttu-id="ba0b8-149">MessageText</span><span class="sxs-lookup"><span data-stu-id="ba0b8-149">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="ba0b8-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="ba0b8-150">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="ba0b8-151">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="ba0b8-151">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="ba0b8-152">フォルダー</span><span class="sxs-lookup"><span data-stu-id="ba0b8-152">Folders</span></span>](folders-ex15websvcsotherref.md)
    
## <a name="see-also"></a><span data-ttu-id="ba0b8-153">関連項目</span><span class="sxs-lookup"><span data-stu-id="ba0b8-153">See also</span></span>



[<span data-ttu-id="ba0b8-154">CopyFolder 操作</span><span class="sxs-lookup"><span data-stu-id="ba0b8-154">CopyFolder operation</span></span>](copyfolder-operation.md)

