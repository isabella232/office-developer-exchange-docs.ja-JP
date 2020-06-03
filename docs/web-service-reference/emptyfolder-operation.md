---
title: EmptyFolder 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 98161486-e2f2-480f-8d5d-708ba81b208a
description: EmptyFolder 操作は、メールボックス内のフォルダーを空にします。 必要に応じて、この操作を使用して、指定したフォルダーのサブフォルダーを削除することもできます。 サブフォルダーを削除すると、サブフォルダーとサブフォルダー内のメッセージは削除されます。
ms.openlocfilehash: 1913db74d33f1e6750cd158df5870f257d0e7839
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530685"
---
# <a name="emptyfolder-operation"></a><span data-ttu-id="0c977-105">EmptyFolder 操作</span><span class="sxs-lookup"><span data-stu-id="0c977-105">EmptyFolder operation</span></span>

<span data-ttu-id="0c977-106">**Emptyfolder**操作は、メールボックス内のフォルダーを空にします。</span><span class="sxs-lookup"><span data-stu-id="0c977-106">The **EmptyFolder** operation empties folders in a mailbox.</span></span> <span data-ttu-id="0c977-107">必要に応じて、この操作を使用して、指定したフォルダーのサブフォルダーを削除することもできます。</span><span class="sxs-lookup"><span data-stu-id="0c977-107">Optionally, this operation enables you to delete the subfolders of the specified folder.</span></span> <span data-ttu-id="0c977-108">サブフォルダーを削除すると、サブフォルダーとサブフォルダー内のメッセージは削除されます。</span><span class="sxs-lookup"><span data-stu-id="0c977-108">When a subfolder is deleted, the subfolder and the messages within the subfolder are deleted.</span></span> 
  
## <a name="emptyfolder-request-example"></a><span data-ttu-id="0c977-109">EmptyFolder 要求の例</span><span class="sxs-lookup"><span data-stu-id="0c977-109">EmptyFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="0c977-110">Description</span><span class="sxs-lookup"><span data-stu-id="0c977-110">Description</span></span>

<span data-ttu-id="0c977-111">次の**emptyfolder**要求の例は、フォルダーを空にする要求を形成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="0c977-111">This following example of an **EmptyFolder** request shows how to form a request to empty a folder.</span></span> <span data-ttu-id="0c977-112">この例では、識別されたフォルダーのすべてのサブフォルダーを削除します。</span><span class="sxs-lookup"><span data-stu-id="0c977-112">This example deletes all subfolders of the identified folder.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="0c977-113">[FolderId](folderid.md)要素の**Id**および**changekey**属性の値は、読みやすくするために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="0c977-113">The values of the **Id** and the **ChangeKey** attributes of the [FolderId](folderid.md) element have been shortened for readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="0c977-114">コード</span><span class="sxs-lookup"><span data-stu-id="0c977-114">Code</span></span>

```XML
<soap:Envelope xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="0c977-115">コメント</span><span class="sxs-lookup"><span data-stu-id="0c977-115">Comments</span></span>

<span data-ttu-id="0c977-116">この例では、フォルダーに対してハード削除を実行します。</span><span class="sxs-lookup"><span data-stu-id="0c977-116">This example performs a hard delete on the folder.</span></span>
  
<span data-ttu-id="0c977-117">フォルダーは、 [FolderIds](folderids.md)要素で使用するために、 [DistinguishedFolderId](distinguishedfolderid.md)要素または[FolderId](folderid.md)要素のいずれかで識別できます。</span><span class="sxs-lookup"><span data-stu-id="0c977-117">Folders can be identified by either the [DistinguishedFolderId](distinguishedfolderid.md) element or the [FolderId](folderid.md) element for use in the [FolderIds](folderids.md) element.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="0c977-118">Request 要素</span><span class="sxs-lookup"><span data-stu-id="0c977-118">Request elements</span></span>

<span data-ttu-id="0c977-119">要求では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="0c977-119">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="0c977-120">EmptyFolder</span><span class="sxs-lookup"><span data-stu-id="0c977-120">EmptyFolder</span></span>](emptyfolder.md)
    
- [<span data-ttu-id="0c977-121">FolderIds</span><span class="sxs-lookup"><span data-stu-id="0c977-121">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="0c977-122">FolderId</span><span class="sxs-lookup"><span data-stu-id="0c977-122">FolderId</span></span>](folderid.md)
    
## <a name="successful-emptyfolder-response"></a><span data-ttu-id="0c977-123">正常な EmptyFolder 応答</span><span class="sxs-lookup"><span data-stu-id="0c977-123">Successful EmptyFolder response</span></span>

### <a name="description"></a><span data-ttu-id="0c977-124">Description</span><span class="sxs-lookup"><span data-stu-id="0c977-124">Description</span></span>

<span data-ttu-id="0c977-125">次の例は、 **Emptyfolder**要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="0c977-125">The following example shows a successful response to the **EmptyFolder** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="0c977-126">コード</span><span class="sxs-lookup"><span data-stu-id="0c977-126">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="1" 
                         MajorBuildNumber="164" 
                         MinorBuildNumber="0" 
                         Version="Exchange2010_SP1"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:EmptyFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                           xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:EmptyFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:EmptyFolderResponseMessage>
      </m:ResponseMessages>
    </m:EmptyFolderResponse>
  </s:Body>
</s:Envelope>

```

### <a name="successful-response-elements"></a><span data-ttu-id="0c977-127">成功した応答要素</span><span class="sxs-lookup"><span data-stu-id="0c977-127">Successful response elements</span></span>

<span data-ttu-id="0c977-128">応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="0c977-128">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="0c977-129">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="0c977-129">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="0c977-130">EmptyFolderResponse</span><span class="sxs-lookup"><span data-stu-id="0c977-130">EmptyFolderResponse</span></span>](emptyfolderresponse.md)
    
- [<span data-ttu-id="0c977-131">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="0c977-131">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="0c977-132">EmptyFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="0c977-132">EmptyFolderResponseMessage</span></span>](emptyfolderresponsemessage.md)
    
- [<span data-ttu-id="0c977-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="0c977-133">ResponseCode</span></span>](responsecode.md)
    
## <a name="emptyfolder-error-response"></a><span data-ttu-id="0c977-134">EmptyFolder エラー応答</span><span class="sxs-lookup"><span data-stu-id="0c977-134">EmptyFolder error response</span></span>

### <a name="description"></a><span data-ttu-id="0c977-135">Description</span><span class="sxs-lookup"><span data-stu-id="0c977-135">Description</span></span>

<span data-ttu-id="0c977-136">次の例は、 **Emptyfolder**要求に対するエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="0c977-136">The following example shows an error response to an **Emptyfolder** request.</span></span> <span data-ttu-id="0c977-137">この操作では、Exchange ストアに見つからないフォルダーを空にしようとしたため、エラーが作成されました。</span><span class="sxs-lookup"><span data-stu-id="0c977-137">The error was created because the operation tried to empty a folder that was not found in the Exchange store.</span></span> 
  
### <a name="code"></a><span data-ttu-id="0c977-138">コード</span><span class="sxs-lookup"><span data-stu-id="0c977-138">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
            MinorVersion="1" 
            MajorBuildNumber="164" 
            MinorBuildNumber="0" 
            Version="Exchange2010_SP1" 
            xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
            xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
            xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
            xmlns:xsd="http://www.w3.org/2001/XMLSchema" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
            xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetFolderResponse 
          xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

### <a name="error-response-elements"></a><span data-ttu-id="0c977-139">エラー応答要素</span><span class="sxs-lookup"><span data-stu-id="0c977-139">Error response elements</span></span>

<span data-ttu-id="0c977-140">応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="0c977-140">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="0c977-141">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="0c977-141">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="0c977-142">GetFolderResponse</span><span class="sxs-lookup"><span data-stu-id="0c977-142">GetFolderResponse</span></span>](getfolderresponse.md)
    
- [<span data-ttu-id="0c977-143">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="0c977-143">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="0c977-144">GetFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="0c977-144">GetFolderResponseMessage</span></span>](getfolderresponsemessage.md)
    
- [<span data-ttu-id="0c977-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="0c977-145">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="0c977-146">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="0c977-146">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="0c977-147">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="0c977-147">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="0c977-148">フォルダー</span><span class="sxs-lookup"><span data-stu-id="0c977-148">Folders</span></span>](folders-ex15websvcsotherref.md)
    
## <a name="see-also"></a><span data-ttu-id="0c977-149">関連項目</span><span class="sxs-lookup"><span data-stu-id="0c977-149">See also</span></span>

- [<span data-ttu-id="0c977-150">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="0c977-150">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

