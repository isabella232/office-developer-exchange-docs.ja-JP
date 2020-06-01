---
title: CreateManagedFolder 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateManagedFolder
api_type:
- schema
ms.assetid: 60a668a2-b4e9-4db9-ac76-9b181e47b302
description: CreateManagedFolder 操作は、Exchange ストアに管理フォルダーを作成します。
ms.openlocfilehash: 779c730b55b9b441644108a6837f9e22d39cc2f4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44444594"
---
# <a name="createmanagedfolder-operation"></a><span data-ttu-id="e2be0-103">CreateManagedFolder 操作</span><span class="sxs-lookup"><span data-stu-id="e2be0-103">CreateManagedFolder operation</span></span>

<span data-ttu-id="e2be0-104">CreateManagedFolder 操作は、Exchange ストアに管理フォルダーを作成します。</span><span class="sxs-lookup"><span data-stu-id="e2be0-104">The CreateManagedFolder operation creates a managed folder in the Exchange store.</span></span>
  
## <a name="using-the-createmanagedfolder-operation"></a><span data-ttu-id="e2be0-105">CreateManagedFolder 操作の使用</span><span class="sxs-lookup"><span data-stu-id="e2be0-105">Using the CreateManagedFolder Operation</span></span>

<span data-ttu-id="e2be0-106">CreateManagedFolder 操作は、管理されたカスタムフォルダーをユーザーのメールボックスに追加します。</span><span class="sxs-lookup"><span data-stu-id="e2be0-106">The CreateManagedFolder operation adds a managed custom folder to a user's mailbox.</span></span> <span data-ttu-id="e2be0-107">Exchange 管理シェルの**Get-ManagedFolder**コマンドレットを使用して、追加できる利用可能な管理フォルダーを見つけることができます。</span><span class="sxs-lookup"><span data-stu-id="e2be0-107">You can use the Exchange Management Shell **Get-ManagedFolder** cmdlet to find available managed folders to add.</span></span> <span data-ttu-id="e2be0-108">このコマンドレットは、管理されたカスタムフォルダーと管理された既定のフォルダーの両方を返しますが、管理されたカスタムフォルダーのみを追加できます。</span><span class="sxs-lookup"><span data-stu-id="e2be0-108">Although this cmdlet returns both managed custom folders and managed default folders, only managed custom folders can be added.</span></span> <span data-ttu-id="e2be0-109">管理されたカスタムフォルダーは、ManagedCustomFolder フォルダーの種類によって識別されます。</span><span class="sxs-lookup"><span data-stu-id="e2be0-109">Managed custom folders are identified by the ManagedCustomFolder folder type.</span></span> <span data-ttu-id="e2be0-110">System.directoryservices 名前空間には、使用可能な管理フォルダーの名前を検出するために使用できる型も含まれています。</span><span class="sxs-lookup"><span data-stu-id="e2be0-110">The System.DirectoryServices namespace also includes types that can be used to discover the names of available managed folders.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="e2be0-111">Exchange Web サービスを使用して、メールボックスに追加する使用可能な管理フォルダーの名前を検索することはできません。</span><span class="sxs-lookup"><span data-stu-id="e2be0-111">You cannot use Exchange Web Services to find the names of available managed folders to add to a mailbox.</span></span> 
  
<span data-ttu-id="e2be0-112">FindFolder および GetFolder 操作を使用して、管理フォルダーにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="e2be0-112">You can use the FindFolder and GetFolder operations to access managed folders.</span></span> <span data-ttu-id="e2be0-113">FindFolder は、指定された親フォルダー内のフォルダーを検索するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="e2be0-113">FindFolder is used to search for folders in a specified parent folder.</span></span> <span data-ttu-id="e2be0-114">これは、同じディレクトリに重複した管理されたカスタムフォルダーを追加しようとする前に、フォルダーで管理フォルダーを検出できるようにするために使用できます。</span><span class="sxs-lookup"><span data-stu-id="e2be0-114">This can be used so that managed folders can be discovered in a folder before trying to add a duplicate managed custom folder to the same directory.</span></span> <span data-ttu-id="e2be0-115">GetFolder は、FindFolder 操作の後に使用され、管理されたカスタムフォルダーに関する詳細情報を取得します。</span><span class="sxs-lookup"><span data-stu-id="e2be0-115">GetFolder is used after the FindFolder operation to get more information about a managed custom folder.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e2be0-116">注釈</span><span class="sxs-lookup"><span data-stu-id="e2be0-116">Remarks</span></span>

<span data-ttu-id="e2be0-117">メッセージングレコード管理 (MRM) ポリシーを設定する方法については、「 [how To Create a Managed Folder Mailbox policy](https://go.microsoft.com/fwlink/?LinkId=100975)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e2be0-117">For information about how to set up messaging records management (MRM) policy, see [How to Create a Managed Folder Mailbox Policy](https://go.microsoft.com/fwlink/?LinkId=100975).</span></span>
  
<span data-ttu-id="e2be0-118">管理されたカスタムフォルダーをメールボックスから削除する方法については、「[削除-ManagedFolder](https://go.microsoft.com/fwlink/?LinkId=100976)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e2be0-118">For information about how to remove managed custom folders from a mailbox, see [Remove-ManagedFolder](https://go.microsoft.com/fwlink/?LinkId=100976).</span></span>
  
## <a name="createmanagedfolder-request-example"></a><span data-ttu-id="e2be0-119">CreateManagedFolder 要求の例</span><span class="sxs-lookup"><span data-stu-id="e2be0-119">CreateManagedFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="e2be0-120">説明</span><span class="sxs-lookup"><span data-stu-id="e2be0-120">Description</span></span>

<span data-ttu-id="e2be0-121">次の CreateManagedFolder 要求の例は、Test 管理フォルダーという名前の管理フォルダーをメールボックスに追加する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="e2be0-121">The following example of a CreateManagedFolder request shows how to add a managed folder named Test Managed Folder to a mailbox.</span></span>
  
> [!NOTE]
> <span data-ttu-id="e2be0-122">代理人アクセスを使用して、管理されたカスタムフォルダーを追加することもできます。</span><span class="sxs-lookup"><span data-stu-id="e2be0-122">You can also use delegate access to add managed custom folders.</span></span> 
  
### <a name="code"></a><span data-ttu-id="e2be0-123">コード</span><span class="sxs-lookup"><span data-stu-id="e2be0-123">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateManagedFolder xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <FolderNames>
        <t:FolderName>Test Managed Folder</t:FolderName>
      </FolderNames>
    </CreateManagedFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="e2be0-124">Request 要素</span><span class="sxs-lookup"><span data-stu-id="e2be0-124">Request elements</span></span>

<span data-ttu-id="e2be0-125">要求では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="e2be0-125">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="e2be0-126">CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="e2be0-126">CreateManagedFolder</span></span>](createmanagedfolder.md)
    
- [<span data-ttu-id="e2be0-127">FolderNames</span><span class="sxs-lookup"><span data-stu-id="e2be0-127">FolderNames</span></span>](foldernames.md)
    
- [<span data-ttu-id="e2be0-128">FolderName</span><span class="sxs-lookup"><span data-stu-id="e2be0-128">FolderName</span></span>](foldername.md)
    
<span data-ttu-id="e2be0-129">CreateManagedFolder 操作の要求メッセージに関するその他のオプションについては、スキーマ階層を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e2be0-129">To find other options for the request message of the CreateManagedFolder operation, explore the schema hierarchy.</span></span> <span data-ttu-id="e2be0-130">[CreateManagedFolder](createmanagedfolder.md)要素から開始します。</span><span class="sxs-lookup"><span data-stu-id="e2be0-130">Start at the [CreateManagedFolder](createmanagedfolder.md) element.</span></span> 
  
## <a name="successful-createmanagedfolder-response"></a><span data-ttu-id="e2be0-131">成功した CreateManagedFolder 応答</span><span class="sxs-lookup"><span data-stu-id="e2be0-131">Successful CreateManagedFolder Response</span></span>

### <a name="description"></a><span data-ttu-id="e2be0-132">説明</span><span class="sxs-lookup"><span data-stu-id="e2be0-132">Description</span></span>

<span data-ttu-id="e2be0-133">次のコード例は、CreateManagedFolder 要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="e2be0-133">The following code example shows a successful response to a CreateManagedFolder request.</span></span>
  
> [!NOTE]
> <span data-ttu-id="e2be0-134">**Id**および**changekey**属性の値は、読みやすくするために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="e2be0-134">The **Id** and **ChangeKey** attribute values have been shortened to preserve readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="e2be0-135">コード</span><span class="sxs-lookup"><span data-stu-id="e2be0-135">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="598" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateManagedFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                                 xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateManagedFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="AS0AdX=" ChangeKey="AACADA=="/>
            </t:Folder>
          </m:Folders>
        </m:CreateManagedFolderResponseMessage>
      </m:ResponseMessages>
    </CreateManagedFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a><span data-ttu-id="e2be0-136">成功した応答要素</span><span class="sxs-lookup"><span data-stu-id="e2be0-136">Successful response elements</span></span>

<span data-ttu-id="e2be0-137">応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="e2be0-137">The following elements are used in the response:</span></span> 
  
- [<span data-ttu-id="e2be0-138">CreateManagedFolderResponse</span><span class="sxs-lookup"><span data-stu-id="e2be0-138">CreateManagedFolderResponse</span></span>](createmanagedfolderresponse.md)
    
- [<span data-ttu-id="e2be0-139">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="e2be0-139">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="e2be0-140">CreateManagedFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="e2be0-140">CreateManagedFolderResponseMessage</span></span>](createmanagedfolderresponsemessage.md)
    
- [<span data-ttu-id="e2be0-141">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="e2be0-141">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="e2be0-142">フォルダー</span><span class="sxs-lookup"><span data-stu-id="e2be0-142">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="e2be0-143">Folder</span><span class="sxs-lookup"><span data-stu-id="e2be0-143">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="e2be0-144">FolderId</span><span class="sxs-lookup"><span data-stu-id="e2be0-144">FolderId</span></span>](folderid.md)
    
<span data-ttu-id="e2be0-145">CreateManagedFolder 操作の応答メッセージに関するその他のオプションについては、スキーマ階層を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e2be0-145">To find other options for the response messages of the CreateManagedFolder operation, explore the schema hierarchy.</span></span> <span data-ttu-id="e2be0-146">[CreateManagedFolderResponse](createmanagedfolderresponse.md)要素から開始します。</span><span class="sxs-lookup"><span data-stu-id="e2be0-146">Start at the [CreateManagedFolderResponse](createmanagedfolderresponse.md) element.</span></span> 
  
## <a name="createmanagedfolder-error-response"></a><span data-ttu-id="e2be0-147">CreateManagedFolder エラー応答</span><span class="sxs-lookup"><span data-stu-id="e2be0-147">CreateManagedFolder error response</span></span>

### <a name="description"></a><span data-ttu-id="e2be0-148">説明</span><span class="sxs-lookup"><span data-stu-id="e2be0-148">Description</span></span>

<span data-ttu-id="e2be0-149">次のコード例は、CreateManagedFolder 要求に対するエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="e2be0-149">The following code example shows an error response to a CreateManagedFolder request.</span></span>
  
### <a name="code"></a><span data-ttu-id="e2be0-150">コード</span><span class="sxs-lookup"><span data-stu-id="e2be0-150">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="598" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateManagedFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                                 xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateManagedFolderResponseMessage ResponseClass="Error">
          <m:MessageText>A specified managed folder already exists in the mailbox.</m:MessageText>
          <m:ResponseCode>ErrorManagedFolderAlreadyExists</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Folders/>
        </m:CreateManagedFolderResponseMessage>
      </m:ResponseMessages>
    </CreateManagedFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="e2be0-151">エラー応答要素</span><span class="sxs-lookup"><span data-stu-id="e2be0-151">Error response elements</span></span>

<span data-ttu-id="e2be0-152">エラー応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="e2be0-152">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="e2be0-153">CreateManagedFolderResponse</span><span class="sxs-lookup"><span data-stu-id="e2be0-153">CreateManagedFolderResponse</span></span>](createmanagedfolderresponse.md)
    
- [<span data-ttu-id="e2be0-154">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="e2be0-154">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="e2be0-155">CreateManagedFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="e2be0-155">CreateManagedFolderResponseMessage</span></span>](createmanagedfolderresponsemessage.md)
    
- [<span data-ttu-id="e2be0-156">MessageText</span><span class="sxs-lookup"><span data-stu-id="e2be0-156">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="e2be0-157">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="e2be0-157">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="e2be0-158">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="e2be0-158">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="e2be0-159">フォルダー</span><span class="sxs-lookup"><span data-stu-id="e2be0-159">Folders</span></span>](folders-ex15websvcsotherref.md)
    
## <a name="see-also"></a><span data-ttu-id="e2be0-160">関連項目</span><span class="sxs-lookup"><span data-stu-id="e2be0-160">See also</span></span>



<span data-ttu-id="e2be0-161">
  [GetFolder 操作](getfolder-operation.md)</span><span class="sxs-lookup"><span data-stu-id="e2be0-161">[GetFolder operation](getfolder-operation.md)</span></span>
  
<span data-ttu-id="e2be0-162">
  [FindFolder 操作](findfolder-operation.md)</span><span class="sxs-lookup"><span data-stu-id="e2be0-162">[FindFolder operation](findfolder-operation.md)</span></span>


[<span data-ttu-id="e2be0-163">フォルダーの検索</span><span class="sxs-lookup"><span data-stu-id="e2be0-163">Finding Folders</span></span>](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)
  
[<span data-ttu-id="e2be0-164">管理フォルダーの追加</span><span class="sxs-lookup"><span data-stu-id="e2be0-164">Adding Managed Folders</span></span>](https://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

