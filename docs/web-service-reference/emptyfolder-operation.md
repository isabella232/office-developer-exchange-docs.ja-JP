---
title: EmptyFolder 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 98161486-e2f2-480f-8d5d-708ba81b208a
description: EmptyFolder 操作は、メールボックス内のフォルダーを空にします。 必要に応じて、この操作を使用すると、指定したフォルダーのサブフォルダーを削除できます。 サブフォルダーを削除すると、サブフォルダーおよびサブフォルダー内のメッセージは削除されます。
ms.openlocfilehash: 0192744516c5a6d24b95915452bfcffecc2d92b7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760268"
---
# <a name="emptyfolder-operation"></a><span data-ttu-id="ab0b3-105">EmptyFolder 操作</span><span class="sxs-lookup"><span data-stu-id="ab0b3-105">EmptyFolder operation</span></span>

<span data-ttu-id="ab0b3-106">**EmptyFolder**操作は、メールボックス内のフォルダーを空にします。</span><span class="sxs-lookup"><span data-stu-id="ab0b3-106">The **EmptyFolder** operation empties folders in a mailbox.</span></span> <span data-ttu-id="ab0b3-107">必要に応じて、この操作を使用すると、指定したフォルダーのサブフォルダーを削除できます。</span><span class="sxs-lookup"><span data-stu-id="ab0b3-107">Optionally, this operation enables you to delete the subfolders of the specified folder.</span></span> <span data-ttu-id="ab0b3-108">サブフォルダーを削除すると、サブフォルダーおよびサブフォルダー内のメッセージは削除されます。</span><span class="sxs-lookup"><span data-stu-id="ab0b3-108">When a subfolder is deleted, the subfolder and the messages within the subfolder are deleted.</span></span> 
  
## <a name="emptyfolder-request-example"></a><span data-ttu-id="ab0b3-109">EmptyFolder 要求の例</span><span class="sxs-lookup"><span data-stu-id="ab0b3-109">EmptyFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="ab0b3-110">説明</span><span class="sxs-lookup"><span data-stu-id="ab0b3-110">Description</span></span>

<span data-ttu-id="ab0b3-111">**EmptyFolder**要求の次の例では、フォルダーを空にするための要求を作成する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="ab0b3-111">This following example of an **EmptyFolder** request shows how to form a request to empty a folder.</span></span> <span data-ttu-id="ab0b3-112">この例では、識別されたフォルダーのすべてのサブフォルダーを削除します。</span><span class="sxs-lookup"><span data-stu-id="ab0b3-112">This example deletes all subfolders of the identified folder.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="ab0b3-113">[フォルダー Id](folderid.md)の要素の**変更キー**属性と**Id**の値は、読みやすさに短縮されています。</span><span class="sxs-lookup"><span data-stu-id="ab0b3-113">The values of the **Id** and the **ChangeKey** attributes of the [FolderId](folderid.md) element have been shortened for readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="ab0b3-114">コード</span><span class="sxs-lookup"><span data-stu-id="ab0b3-114">Code</span></span>

```XML
<soap:Envelope xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version ="Exchange2010_SP1"/>
    </soap:Header>
    <soap:Body>
      <m:EmptyFolder DeleteType="HardDelete" DeleteSubFolders="true">
        <m:FolderIds>
          <t:FolderId Id="AQMkADhhOGU0"  ChangeKey="AQAAABYAAABsMB" />
        </m:FolderIds>
      </m:EmptyFolder>
    </soap:Body>
</soap:Envelope>

```

### <a name="comments"></a><span data-ttu-id="ab0b3-115">コメント</span><span class="sxs-lookup"><span data-stu-id="ab0b3-115">Comments</span></span>

<span data-ttu-id="ab0b3-116">この例では、フォルダーのハード削除を実行します。</span><span class="sxs-lookup"><span data-stu-id="ab0b3-116">This example performs a hard delete on the folder.</span></span>
  
<span data-ttu-id="ab0b3-117">フォルダーは、 [DistinguishedFolderId](distinguishedfolderid.md)要素または[FolderIds](folderids.md)要素で使用するための[フォルダー Id](folderid.md)の要素のいずれかで識別できます。</span><span class="sxs-lookup"><span data-stu-id="ab0b3-117">Folders can be identified by either the [DistinguishedFolderId](distinguishedfolderid.md) element or the [FolderId](folderid.md) element for use in the [FolderIds](folderids.md) element.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="ab0b3-118">要素を要求します。</span><span class="sxs-lookup"><span data-stu-id="ab0b3-118">Request elements</span></span>

<span data-ttu-id="ab0b3-119">次の要素は、要求で使用されます。</span><span class="sxs-lookup"><span data-stu-id="ab0b3-119">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="ab0b3-120">EmptyFolder</span><span class="sxs-lookup"><span data-stu-id="ab0b3-120">EmptyFolder</span></span>](emptyfolder.md)
    
- [<span data-ttu-id="ab0b3-121">FolderIds</span><span class="sxs-lookup"><span data-stu-id="ab0b3-121">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="ab0b3-122">フォルダー Id</span><span class="sxs-lookup"><span data-stu-id="ab0b3-122">FolderId</span></span>](folderid.md)
    
## <a name="successful-emptyfolder-response"></a><span data-ttu-id="ab0b3-123">EmptyFolder の正常な応答</span><span class="sxs-lookup"><span data-stu-id="ab0b3-123">Successful EmptyFolder response</span></span>

### <a name="description"></a><span data-ttu-id="ab0b3-124">説明</span><span class="sxs-lookup"><span data-stu-id="ab0b3-124">Description</span></span>

<span data-ttu-id="ab0b3-125">**EmptyFolder**要求に正常な応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ab0b3-125">The following example shows a successful response to the **EmptyFolder** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="ab0b3-126">コード</span><span class="sxs-lookup"><span data-stu-id="ab0b3-126">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="1" 
                         MajorBuildNumber="164" 
                         MinorBuildNumber="0" 
                         Version="Exchange2010_SP1"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:EmptyFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                           xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:EmptyFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:EmptyFolderResponseMessage>
      </m:ResponseMessages>
    </m:EmptyFolderResponse>
  </s:Body>
</s:Envelope>

```

### <a name="successful-response-elements"></a><span data-ttu-id="ab0b3-127">正常な応答の要素</span><span class="sxs-lookup"><span data-stu-id="ab0b3-127">Successful response elements</span></span>

<span data-ttu-id="ab0b3-128">次の要素は、応答で使用されます。</span><span class="sxs-lookup"><span data-stu-id="ab0b3-128">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="ab0b3-129">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="ab0b3-129">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="ab0b3-130">EmptyFolderResponse</span><span class="sxs-lookup"><span data-stu-id="ab0b3-130">EmptyFolderResponse</span></span>](emptyfolderresponse.md)
    
- [<span data-ttu-id="ab0b3-131">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="ab0b3-131">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="ab0b3-132">EmptyFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ab0b3-132">EmptyFolderResponseMessage</span></span>](emptyfolderresponsemessage.md)
    
- [<span data-ttu-id="ab0b3-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="ab0b3-133">ResponseCode</span></span>](responsecode.md)
    
## <a name="emptyfolder-error-response"></a><span data-ttu-id="ab0b3-134">EmptyFolder エラー応答</span><span class="sxs-lookup"><span data-stu-id="ab0b3-134">EmptyFolder error response</span></span>

### <a name="description"></a><span data-ttu-id="ab0b3-135">説明</span><span class="sxs-lookup"><span data-stu-id="ab0b3-135">Description</span></span>

<span data-ttu-id="ab0b3-136">**Emptyfolder**要求に対するエラー応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ab0b3-136">The following example shows an error response to an **Emptyfolder** request.</span></span> <span data-ttu-id="ab0b3-137">操作がないフォルダーを空にしようとしたため、エラーが作成された Exchange ストアにします。</span><span class="sxs-lookup"><span data-stu-id="ab0b3-137">The error was created because the operation tried to empty a folder that was not found in the Exchange store.</span></span> 
  
### <a name="code"></a><span data-ttu-id="ab0b3-138">コード</span><span class="sxs-lookup"><span data-stu-id="ab0b3-138">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
            MinorVersion="1" 
            MajorBuildNumber="164" 
            MinorBuildNumber="0" 
            Version="Exchange2010_SP1" 
            xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
            xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
            xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
            xmlns:xsd="http://www.w3.org/2001/XMLSchema" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
            xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetFolderResponse 
          xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetFolderResponseMessage ResponseClass="Error">
          <m:MessageText>Id is malformed.</m:MessageText>
          <m:ResponseCode>ErrorInvalidIdMalformed</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Folders />
        </m:GetFolderResponseMessage>
      </m:ResponseMessages>
    </m:GetFolderResponse>
  </s:Body>
</s:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="ab0b3-139">エラー応答の要素</span><span class="sxs-lookup"><span data-stu-id="ab0b3-139">Error response elements</span></span>

<span data-ttu-id="ab0b3-140">次の要素は、応答で使用されます。</span><span class="sxs-lookup"><span data-stu-id="ab0b3-140">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="ab0b3-141">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="ab0b3-141">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="ab0b3-142">GetFolderResponse</span><span class="sxs-lookup"><span data-stu-id="ab0b3-142">GetFolderResponse</span></span>](getfolderresponse.md)
    
- [<span data-ttu-id="ab0b3-143">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="ab0b3-143">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="ab0b3-144">GetFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ab0b3-144">GetFolderResponseMessage</span></span>](getfolderresponsemessage.md)
    
- [<span data-ttu-id="ab0b3-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="ab0b3-145">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="ab0b3-146">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="ab0b3-146">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="ab0b3-147">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="ab0b3-147">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="ab0b3-148">フォルダー</span><span class="sxs-lookup"><span data-stu-id="ab0b3-148">Folders</span></span>](folders-ex15websvcsotherref.md)
    
## <a name="see-also"></a><span data-ttu-id="ab0b3-149">関連項目</span><span class="sxs-lookup"><span data-stu-id="ab0b3-149">See also</span></span>

- [<span data-ttu-id="ab0b3-150">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="ab0b3-150">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

