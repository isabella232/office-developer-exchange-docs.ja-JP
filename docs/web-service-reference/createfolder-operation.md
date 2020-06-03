---
title: CreateFolder 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateFolder
api_type:
- schema
ms.assetid: 6f6c334c-b190-4e55-8f0a-38f2a018d1b3
description: CreateFolder 操作は、フォルダー、予定表フォルダー、連絡先フォルダー、タスクフォルダー、および検索フォルダーを作成します。
ms.openlocfilehash: 125a6d212e5eaf85ace71c048de809f3a05ba9b6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457551"
---
# <a name="createfolder-operation"></a><span data-ttu-id="46a02-103">CreateFolder 操作</span><span class="sxs-lookup"><span data-stu-id="46a02-103">CreateFolder operation</span></span>

<span data-ttu-id="46a02-104">CreateFolder 操作は、フォルダー、予定表フォルダー、連絡先フォルダー、タスクフォルダー、および検索フォルダーを作成します。</span><span class="sxs-lookup"><span data-stu-id="46a02-104">The CreateFolder operation creates folders, calendar folders, contacts folders, tasks folders, and search folders.</span></span>
  
## <a name="createfolder-request-example"></a><span data-ttu-id="46a02-105">CreateFolder 要求の例</span><span class="sxs-lookup"><span data-stu-id="46a02-105">CreateFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="46a02-106">Description</span><span class="sxs-lookup"><span data-stu-id="46a02-106">Description</span></span>

<span data-ttu-id="46a02-107">CreateFolder 要求の次の例は、メールボックスルートに2つの新しいフォルダーを作成するための要求を形成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="46a02-107">The following example of a CreateFolder request shows how to form a request to create two new folders in the mailbox root.</span></span>
  
### <a name="code"></a><span data-ttu-id="46a02-108">コード</span><span class="sxs-lookup"><span data-stu-id="46a02-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateFolder xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ParentFolderId>
        <t:DistinguishedFolderId Id="msgfolderroot"/>
      </ParentFolderId>
      <Folders>
        <t:Folder>
          <t:DisplayName>Folder1</t:DisplayName>
        </t:Folder>
        <t:Folder>
          <t:DisplayName>Folder2</t:DisplayName>
        </t:Folder>
      </Folders>
    </CreateFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="46a02-109">Request 要素</span><span class="sxs-lookup"><span data-stu-id="46a02-109">Request elements</span></span>

<span data-ttu-id="46a02-110">要求では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="46a02-110">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="46a02-111">CreateFolder</span><span class="sxs-lookup"><span data-stu-id="46a02-111">CreateFolder</span></span>](createfolder.md)
    
- [<span data-ttu-id="46a02-112">ParentFolderId (TargetFolderIdType)</span><span class="sxs-lookup"><span data-stu-id="46a02-112">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md)
    
- [<span data-ttu-id="46a02-113">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="46a02-113">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="46a02-114">フォルダー</span><span class="sxs-lookup"><span data-stu-id="46a02-114">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="46a02-115">Folder</span><span class="sxs-lookup"><span data-stu-id="46a02-115">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="46a02-116">DisplayName (文字列)</span><span class="sxs-lookup"><span data-stu-id="46a02-116">DisplayName (string)</span></span>](displayname-string.md)
    
> [!NOTE]
> <span data-ttu-id="46a02-117">これらの要素を説明するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="46a02-117">The schema that describes these elements is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
<span data-ttu-id="46a02-118">CreateFolder 操作の要求メッセージに関するその他のオプションについては、スキーマ階層を参照してください。</span><span class="sxs-lookup"><span data-stu-id="46a02-118">To find other options for the request message of the CreateFolder operation, explore the schema hierarchy.</span></span> <span data-ttu-id="46a02-119">[CreateFolder](createfolder.md)要素から開始します。</span><span class="sxs-lookup"><span data-stu-id="46a02-119">Start at the [CreateFolder](createfolder.md) element.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="46a02-120">**Calendar: オーガナイザー**プロパティを使用して、制限付きの検索フォルダーを作成すると、それ以降の get フォルダー呼び出しでは、その場所にある**メッセージ: from**プロパティを使用して制限が返されます。</span><span class="sxs-lookup"><span data-stu-id="46a02-120">If you create a search folder with a restriction by using the **calendar:Organizer** property, a subsequent get folder call will return the restriction with the **message:from** property in its place.</span></span> <span data-ttu-id="46a02-121">これら2つのプロパティは、同じ基になる MAPI プロパティにマップされます。</span><span class="sxs-lookup"><span data-stu-id="46a02-121">These two properties map to the same underlying MAPI property.</span></span> 
  
<span data-ttu-id="46a02-122">CreateFolder 操作では、汎用フォルダーの種類要素を使用してフォルダーを作成し、 **Folderclass**要素を設定することによってのみ、カスタムフォルダークラスの作成がサポートされます。</span><span class="sxs-lookup"><span data-stu-id="46a02-122">The CreateFolder operation supports the creation of a custom folder class only when you create the folder by using a generic folder type element and set the **FolderClass** element.</span></span> 
  
## <a name="successful-createfolder-response-example"></a><span data-ttu-id="46a02-123">Successful CreateFolder response の例</span><span class="sxs-lookup"><span data-stu-id="46a02-123">Successful CreateFolder response example</span></span>

### <a name="description"></a><span data-ttu-id="46a02-124">Description</span><span class="sxs-lookup"><span data-stu-id="46a02-124">Description</span></span>

<span data-ttu-id="46a02-125">次の例は、CreateFolder 要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="46a02-125">The following example shows a successful response to the CreateFolder request.</span></span> <span data-ttu-id="46a02-126">この例では、応答は新しいフォルダーの識別子を返します。</span><span class="sxs-lookup"><span data-stu-id="46a02-126">In this example, the response returns the identifiers of the new folders.</span></span>
  
> [!NOTE]
> <span data-ttu-id="46a02-127">読みやすくするために、フォルダー ID と変更キーが短縮されています。</span><span class="sxs-lookup"><span data-stu-id="46a02-127">The folder ID and the change key have been shortened to preserve readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="46a02-128">コード</span><span class="sxs-lookup"><span data-stu-id="46a02-128">Code</span></span>

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
    <CreateFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="AS4AUn==" />
            </t:Folder>
          </m:Folders>
        </m:CreateFolderResponseMessage>
        <m:CreateFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="AS4AUn==" />
            </t:Folder>
          </m:Folders>
        </m:CreateFolderResponseMessage>
      </m:ResponseMessages>
    </CreateFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a><span data-ttu-id="46a02-129">成功した応答要素</span><span class="sxs-lookup"><span data-stu-id="46a02-129">Successful response elements</span></span>

<span data-ttu-id="46a02-130">応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="46a02-130">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="46a02-131">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="46a02-131">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="46a02-132">CreateFolderResponse</span><span class="sxs-lookup"><span data-stu-id="46a02-132">CreateFolderResponse</span></span>](createfolderresponse.md)
    
- [<span data-ttu-id="46a02-133">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="46a02-133">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="46a02-134">CreateFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="46a02-134">CreateFolderResponseMessage</span></span>](createfolderresponsemessage.md)
    
- [<span data-ttu-id="46a02-135">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="46a02-135">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="46a02-136">フォルダー</span><span class="sxs-lookup"><span data-stu-id="46a02-136">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="46a02-137">Folder</span><span class="sxs-lookup"><span data-stu-id="46a02-137">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="46a02-138">FolderId</span><span class="sxs-lookup"><span data-stu-id="46a02-138">FolderId</span></span>](folderid.md)
    
<span data-ttu-id="46a02-139">CreateFolder 操作の応答メッセージに関するその他のオプションについては、スキーマ階層を参照してください。</span><span class="sxs-lookup"><span data-stu-id="46a02-139">To find other options for the response message of the CreateFolder operation, explore the schema hierarchy.</span></span> <span data-ttu-id="46a02-140">[Createfolderresponse](createfolderresponse.md)要素から開始します。</span><span class="sxs-lookup"><span data-stu-id="46a02-140">Start at the [CreateFolderResponse](createfolderresponse.md) element.</span></span> 
  
## <a name="createfolder-error-response"></a><span data-ttu-id="46a02-141">CreateFolder エラー応答</span><span class="sxs-lookup"><span data-stu-id="46a02-141">CreateFolder error response</span></span>

### <a name="description"></a><span data-ttu-id="46a02-142">Description</span><span class="sxs-lookup"><span data-stu-id="46a02-142">Description</span></span>

<span data-ttu-id="46a02-143">次の例は、CreateFolder 要求に対するエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="46a02-143">The following example shows an error response to a CreateFolder request.</span></span>
  
### <a name="code"></a><span data-ttu-id="46a02-144">コード</span><span class="sxs-lookup"><span data-stu-id="46a02-144">Code</span></span>

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
    <CreateFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateFolderResponseMessage ResponseClass="Error">
          <m:MessageText>A folder with the specified name already exists.</m:MessageText>
          <m:ResponseCode>ErrorFolderExists</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Folders />
        </m:CreateFolderResponseMessage>
      </m:ResponseMessages>
    </CreateFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="46a02-145">エラー応答要素</span><span class="sxs-lookup"><span data-stu-id="46a02-145">Error response elements</span></span>

<span data-ttu-id="46a02-146">エラー応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="46a02-146">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="46a02-147">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="46a02-147">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="46a02-148">CreateFolderResponse</span><span class="sxs-lookup"><span data-stu-id="46a02-148">CreateFolderResponse</span></span>](createfolderresponse.md)
    
- [<span data-ttu-id="46a02-149">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="46a02-149">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="46a02-150">CreateFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="46a02-150">CreateFolderResponseMessage</span></span>](createfolderresponsemessage.md)
    
- [<span data-ttu-id="46a02-151">MessageText</span><span class="sxs-lookup"><span data-stu-id="46a02-151">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="46a02-152">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="46a02-152">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="46a02-153">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="46a02-153">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="46a02-154">フォルダー</span><span class="sxs-lookup"><span data-stu-id="46a02-154">Folders</span></span>](folders-ex15websvcsotherref.md)
    
<span data-ttu-id="46a02-155">CreateFolder 操作のエラー応答メッセージに関するその他のオプションについては、「スキーマ階層」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="46a02-155">To find other options for the error response message of the CreateFolder operation, explore the schema hierarchy.</span></span> <span data-ttu-id="46a02-156">[Createfolderresponse](createfolderresponse.md)要素から開始します。</span><span class="sxs-lookup"><span data-stu-id="46a02-156">Start at the [CreateFolderResponse](createfolderresponse.md) element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="46a02-157">関連項目</span><span class="sxs-lookup"><span data-stu-id="46a02-157">See also</span></span>



[<span data-ttu-id="46a02-158">FindItem 操作</span><span class="sxs-lookup"><span data-stu-id="46a02-158">FindItem operation</span></span>](finditem-operation.md)
  
[<span data-ttu-id="46a02-159">FindFolder 操作</span><span class="sxs-lookup"><span data-stu-id="46a02-159">FindFolder operation</span></span>](findfolder-operation.md)
  
 <span data-ttu-id="46a02-160">**CreateFolderType**</span><span class="sxs-lookup"><span data-stu-id="46a02-160">**CreateFolderType**</span></span>


- [<span data-ttu-id="46a02-161">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="46a02-161">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="46a02-162">フォルダーの作成 (Exchange Web サービス)</span><span class="sxs-lookup"><span data-stu-id="46a02-162">Creating Folders (Exchange Web Services)</span></span>](https://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

