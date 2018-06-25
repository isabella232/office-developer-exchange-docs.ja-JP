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
description: CreateManagedFolder 操作は、Exchange ストア内の管理フォルダーを作成します。
ms.openlocfilehash: 2c2af53dc5dbe1e6fcbc7f3b1174a856e51e4905
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759851"
---
# <a name="createmanagedfolder-operation"></a><span data-ttu-id="8c090-103">CreateManagedFolder 操作</span><span class="sxs-lookup"><span data-stu-id="8c090-103">CreateManagedFolder operation</span></span>

<span data-ttu-id="8c090-104">CreateManagedFolder 操作は、Exchange ストア内の管理フォルダーを作成します。</span><span class="sxs-lookup"><span data-stu-id="8c090-104">The CreateManagedFolder operation creates a managed folder in the Exchange store.</span></span>
  
## <a name="using-the-createmanagedfolder-operation"></a><span data-ttu-id="8c090-105">CreateManagedFolder 操作を使用します。</span><span class="sxs-lookup"><span data-stu-id="8c090-105">Using the CreateManagedFolder Operation</span></span>

<span data-ttu-id="8c090-106">CreateManagedFolder 操作では、ユーザーのメールボックスに管理されたカスタム フォルダーを追加します。</span><span class="sxs-lookup"><span data-stu-id="8c090-106">The CreateManagedFolder operation adds a managed custom folder to a user's mailbox.</span></span> <span data-ttu-id="8c090-107">**Get ManagedFolder**の Exchange 管理シェル コマンドレットを使用するには追加するのには使用可能な管理対象のフォルダーを検索します。</span><span class="sxs-lookup"><span data-stu-id="8c090-107">You can use the Exchange Management Shell **Get-ManagedFolder** cmdlet to find available managed folders to add.</span></span> <span data-ttu-id="8c090-108">このコマンドレットを返します管理されたカスタム フォルダーと管理された既定フォルダーの両方、のみ管理カスタム フォルダーを追加することができます。</span><span class="sxs-lookup"><span data-stu-id="8c090-108">Although this cmdlet returns both managed custom folders and managed default folders, only managed custom folders can be added.</span></span> <span data-ttu-id="8c090-109">管理されたカスタム フォルダーは、ManagedCustomFolder フォルダーの種類によって識別されます。</span><span class="sxs-lookup"><span data-stu-id="8c090-109">Managed custom folders are identified by the ManagedCustomFolder folder type.</span></span> <span data-ttu-id="8c090-110">System.DirectoryServices 名前空間には、利用可能な管理対象フォルダーの名前を検出するために使用する型も含まれています。</span><span class="sxs-lookup"><span data-stu-id="8c090-110">The System.DirectoryServices namespace also includes types that can be used to discover the names of available managed folders.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="8c090-111">メールボックスに追加する利用可能な管理対象のフォルダーの名前を検索するのには、Exchange Web サービスを使うことはできません。</span><span class="sxs-lookup"><span data-stu-id="8c090-111">You cannot use Exchange Web Services to find the names of available managed folders to add to a mailbox.</span></span> 
  
<span data-ttu-id="8c090-112">FindFolder、GetFolder の操作を使用するには管理対象のフォルダーにアクセスします。</span><span class="sxs-lookup"><span data-stu-id="8c090-112">You can use the FindFolder and GetFolder operations to access managed folders.</span></span> <span data-ttu-id="8c090-113">FindFolder を使用して、指定された親フォルダー内のフォルダーを検索します。</span><span class="sxs-lookup"><span data-stu-id="8c090-113">FindFolder is used to search for folders in a specified parent folder.</span></span> <span data-ttu-id="8c090-114">これは、重複して同じディレクトリに、カスタム フォルダーの管理を追加する前にフォルダー内の管理フォルダーを検出できるように、使用できます。</span><span class="sxs-lookup"><span data-stu-id="8c090-114">This can be used so that managed folders can be discovered in a folder before trying to add a duplicate managed custom folder to the same directory.</span></span> <span data-ttu-id="8c090-115">FindFolder 操作の完了後は、GetFolder を使用して管理されたカスタム フォルダーの詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="8c090-115">GetFolder is used after the FindFolder operation to get more information about a managed custom folder.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8c090-116">備考</span><span class="sxs-lookup"><span data-stu-id="8c090-116">Remarks</span></span>

<span data-ttu-id="8c090-117">メッセージング レコード管理 (MRM) ポリシーを設定する方法の詳細については、[管理フォルダー メールボックス ポリシーを作成する方法](http://go.microsoft.com/fwlink/?LinkId=100975)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8c090-117">For information about how to set up messaging records management (MRM) policy, see [How to Create a Managed Folder Mailbox Policy](http://go.microsoft.com/fwlink/?LinkId=100975).</span></span>
  
<span data-ttu-id="8c090-118">管理されたカスタム フォルダーをメールボックスから削除する方法の詳細については、[削除 ManagedFolder](http://go.microsoft.com/fwlink/?LinkId=100976)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8c090-118">For information about how to remove managed custom folders from a mailbox, see [Remove-ManagedFolder](http://go.microsoft.com/fwlink/?LinkId=100976).</span></span>
  
## <a name="createmanagedfolder-request-example"></a><span data-ttu-id="8c090-119">CreateManagedFolder 要求の例</span><span class="sxs-lookup"><span data-stu-id="8c090-119">CreateManagedFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="8c090-120">説明</span><span class="sxs-lookup"><span data-stu-id="8c090-120">Description</span></span>

<span data-ttu-id="8c090-121">CreateManagedFolder 要求の次の例では、テストの管理フォルダーをという名前のメールボックスに管理フォルダーを追加する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="8c090-121">The following example of a CreateManagedFolder request shows how to add a managed folder named Test Managed Folder to a mailbox.</span></span>
  
> [!NOTE]
> <span data-ttu-id="8c090-122">管理されたカスタム フォルダーを追加するのには代理人アクセスを使用することもできます。</span><span class="sxs-lookup"><span data-stu-id="8c090-122">You can also use delegate access to add managed custom folders.</span></span> 
  
### <a name="code"></a><span data-ttu-id="8c090-123">コード</span><span class="sxs-lookup"><span data-stu-id="8c090-123">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateManagedFolder xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <FolderNames>
        <t:FolderName>Test Managed Folder</t:FolderName>
      </FolderNames>
    </CreateManagedFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="8c090-124">要素を要求します。</span><span class="sxs-lookup"><span data-stu-id="8c090-124">Request elements</span></span>

<span data-ttu-id="8c090-125">次の要素は、要求で使用されます。</span><span class="sxs-lookup"><span data-stu-id="8c090-125">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="8c090-126">CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="8c090-126">CreateManagedFolder</span></span>](createmanagedfolder.md)
    
- [<span data-ttu-id="8c090-127">表示</span><span class="sxs-lookup"><span data-stu-id="8c090-127">FolderNames</span></span>](foldernames.md)
    
- [<span data-ttu-id="8c090-128">フォルダー名</span><span class="sxs-lookup"><span data-stu-id="8c090-128">FolderName</span></span>](foldername.md)
    
<span data-ttu-id="8c090-129">CreateManagedFolder 操作の要求メッセージには、他のオプションを検索するには、スキーマの階層構造を表示します。</span><span class="sxs-lookup"><span data-stu-id="8c090-129">To find other options for the request message of the CreateManagedFolder operation, explore the schema hierarchy.</span></span> <span data-ttu-id="8c090-130">[CreateManagedFolder](createmanagedfolder.md)要素から開始します。</span><span class="sxs-lookup"><span data-stu-id="8c090-130">Start at the [CreateManagedFolder](createmanagedfolder.md) element.</span></span> 
  
## <a name="successful-createmanagedfolder-response"></a><span data-ttu-id="8c090-131">CreateManagedFolder の正常な応答</span><span class="sxs-lookup"><span data-stu-id="8c090-131">Successful CreateManagedFolder Response</span></span>

### <a name="description"></a><span data-ttu-id="8c090-132">説明</span><span class="sxs-lookup"><span data-stu-id="8c090-132">Description</span></span>

<span data-ttu-id="8c090-133">CreateManagedFolder 要求に正常な応答を次のコード例に示します。</span><span class="sxs-lookup"><span data-stu-id="8c090-133">The following code example shows a successful response to a CreateManagedFolder request.</span></span>
  
> [!NOTE]
> <span data-ttu-id="8c090-134">**Id**と**変更キー**の属性の値は、読みやすさを保持するために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="8c090-134">The **Id** and **ChangeKey** attribute values have been shortened to preserve readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="8c090-135">コード</span><span class="sxs-lookup"><span data-stu-id="8c090-135">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="598" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateManagedFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                                 xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="successful-response-elements"></a><span data-ttu-id="8c090-136">正常な応答の要素</span><span class="sxs-lookup"><span data-stu-id="8c090-136">Successful response elements</span></span>

<span data-ttu-id="8c090-137">次の要素は、応答で使用されます。</span><span class="sxs-lookup"><span data-stu-id="8c090-137">The following elements are used in the response:</span></span> 
  
- [<span data-ttu-id="8c090-138">CreateManagedFolderResponse</span><span class="sxs-lookup"><span data-stu-id="8c090-138">CreateManagedFolderResponse</span></span>](createmanagedfolderresponse.md)
    
- [<span data-ttu-id="8c090-139">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="8c090-139">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="8c090-140">CreateManagedFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="8c090-140">CreateManagedFolderResponseMessage</span></span>](createmanagedfolderresponsemessage.md)
    
- [<span data-ttu-id="8c090-141">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="8c090-141">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="8c090-142">フォルダー</span><span class="sxs-lookup"><span data-stu-id="8c090-142">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="8c090-143">Folder</span><span class="sxs-lookup"><span data-stu-id="8c090-143">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="8c090-144">フォルダー Id</span><span class="sxs-lookup"><span data-stu-id="8c090-144">FolderId</span></span>](folderid.md)
    
<span data-ttu-id="8c090-145">CreateManagedFolder 操作の応答メッセージには、他のオプションを検索するには、スキーマの階層構造を表示します。</span><span class="sxs-lookup"><span data-stu-id="8c090-145">To find other options for the response messages of the CreateManagedFolder operation, explore the schema hierarchy.</span></span> <span data-ttu-id="8c090-146">[CreateManagedFolderResponse](createmanagedfolderresponse.md)要素から開始します。</span><span class="sxs-lookup"><span data-stu-id="8c090-146">Start at the [CreateManagedFolderResponse](createmanagedfolderresponse.md) element.</span></span> 
  
## <a name="createmanagedfolder-error-response"></a><span data-ttu-id="8c090-147">CreateManagedFolder エラー応答</span><span class="sxs-lookup"><span data-stu-id="8c090-147">CreateManagedFolder error response</span></span>

### <a name="description"></a><span data-ttu-id="8c090-148">説明</span><span class="sxs-lookup"><span data-stu-id="8c090-148">Description</span></span>

<span data-ttu-id="8c090-149">CreateManagedFolder 要求に対してエラー応答をコード例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8c090-149">The following code example shows an error response to a CreateManagedFolder request.</span></span>
  
### <a name="code"></a><span data-ttu-id="8c090-150">コード</span><span class="sxs-lookup"><span data-stu-id="8c090-150">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="598" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateManagedFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                                 xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="error-response-elements"></a><span data-ttu-id="8c090-151">エラー応答の要素</span><span class="sxs-lookup"><span data-stu-id="8c090-151">Error response elements</span></span>

<span data-ttu-id="8c090-152">エラー応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="8c090-152">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="8c090-153">CreateManagedFolderResponse</span><span class="sxs-lookup"><span data-stu-id="8c090-153">CreateManagedFolderResponse</span></span>](createmanagedfolderresponse.md)
    
- [<span data-ttu-id="8c090-154">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="8c090-154">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="8c090-155">CreateManagedFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="8c090-155">CreateManagedFolderResponseMessage</span></span>](createmanagedfolderresponsemessage.md)
    
- [<span data-ttu-id="8c090-156">MessageText</span><span class="sxs-lookup"><span data-stu-id="8c090-156">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="8c090-157">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="8c090-157">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="8c090-158">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="8c090-158">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="8c090-159">フォルダー</span><span class="sxs-lookup"><span data-stu-id="8c090-159">Folders</span></span>](folders-ex15websvcsotherref.md)
    
## <a name="see-also"></a><span data-ttu-id="8c090-160">関連項目</span><span class="sxs-lookup"><span data-stu-id="8c090-160">See also</span></span>



<span data-ttu-id="8c090-161">
  [GetFolder 操作](getfolder-operation.md)</span><span class="sxs-lookup"><span data-stu-id="8c090-161">[GetFolder operation](getfolder-operation.md)</span></span>
  
<span data-ttu-id="8c090-162">
  [FindFolder 操作](findfolder-operation.md)</span><span class="sxs-lookup"><span data-stu-id="8c090-162">[FindFolder operation](findfolder-operation.md)</span></span>


[<span data-ttu-id="8c090-163">フォルダーを検索します。</span><span class="sxs-lookup"><span data-stu-id="8c090-163">Finding Folders</span></span>](http://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)
  
[<span data-ttu-id="8c090-164">管理フォルダーを追加します。</span><span class="sxs-lookup"><span data-stu-id="8c090-164">Adding Managed Folders</span></span>](http://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

