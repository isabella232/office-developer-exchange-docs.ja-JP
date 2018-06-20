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
description: CreateFolder 操作フォルダー、予定表フォルダー、連絡先フォルダー、仕事フォルダー、および検索を作成するフォルダーです。
ms.openlocfilehash: 97156d4a3747cacbdcf9563d21d93a0aa44c3358
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759816"
---
# <a name="createfolder-operation"></a><span data-ttu-id="1d5e9-103">CreateFolder 操作</span><span class="sxs-lookup"><span data-stu-id="1d5e9-103">CreateFolder operation</span></span>

<span data-ttu-id="1d5e9-104">CreateFolder 操作フォルダー、予定表フォルダー、連絡先フォルダー、仕事フォルダー、および検索を作成するフォルダーです。</span><span class="sxs-lookup"><span data-stu-id="1d5e9-104">The CreateFolder operation creates folders, calendar folders, contacts folders, tasks folders, and search folders.</span></span>
  
## <a name="createfolder-request-example"></a><span data-ttu-id="1d5e9-105">CreateFolder 要求の例</span><span class="sxs-lookup"><span data-stu-id="1d5e9-105">CreateFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="1d5e9-106">説明</span><span class="sxs-lookup"><span data-stu-id="1d5e9-106">Description</span></span>

<span data-ttu-id="1d5e9-107">CreateFolder 要求の次の例では、メールボックスのルートに 2 つの新しいフォルダーを作成する要求を作成する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="1d5e9-107">The following example of a CreateFolder request shows how to form a request to create two new folders in the mailbox root.</span></span>
  
### <a name="code"></a><span data-ttu-id="1d5e9-108">コード</span><span class="sxs-lookup"><span data-stu-id="1d5e9-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateFolder xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="request-elements"></a><span data-ttu-id="1d5e9-109">要素を要求します。</span><span class="sxs-lookup"><span data-stu-id="1d5e9-109">Request elements</span></span>

<span data-ttu-id="1d5e9-110">次の要素は、要求で使用されます。</span><span class="sxs-lookup"><span data-stu-id="1d5e9-110">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="1d5e9-111">CreateFolder</span><span class="sxs-lookup"><span data-stu-id="1d5e9-111">CreateFolder</span></span>](createfolder.md)
    
- [<span data-ttu-id="1d5e9-112">ParentFolderId (TargetFolderIdType)</span><span class="sxs-lookup"><span data-stu-id="1d5e9-112">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md)
    
- [<span data-ttu-id="1d5e9-113">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="1d5e9-113">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="1d5e9-114">フォルダー</span><span class="sxs-lookup"><span data-stu-id="1d5e9-114">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="1d5e9-115">Folder</span><span class="sxs-lookup"><span data-stu-id="1d5e9-115">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="1d5e9-116">表示名 (文字列)</span><span class="sxs-lookup"><span data-stu-id="1d5e9-116">DisplayName (string)</span></span>](displayname-string.md)
    
> [!NOTE]
> <span data-ttu-id="1d5e9-117">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、これらの要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="1d5e9-117">The schema that describes these elements is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
<span data-ttu-id="1d5e9-118">CreateFolder 操作の要求メッセージには、他のオプションを検索するには、スキーマの階層構造を表示します。</span><span class="sxs-lookup"><span data-stu-id="1d5e9-118">To find other options for the request message of the CreateFolder operation, explore the schema hierarchy.</span></span> <span data-ttu-id="1d5e9-119">[CreateFolder](createfolder.md)要素から開始します。</span><span class="sxs-lookup"><span data-stu-id="1d5e9-119">Start at the [CreateFolder](createfolder.md) element.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="1d5e9-120">フォルダーの後で行う get 呼び出しの制限に戻ります **: 開催者の予定表**のプロパティを使用して、制限付き検索フォルダーを作成する場合、**メッセージ: から**プロパティを所定の位置にします。</span><span class="sxs-lookup"><span data-stu-id="1d5e9-120">If you create a search folder with a restriction by using the **calendar:Organizer** property, a subsequent get folder call will return the restriction with the **message:from** property in its place.</span></span> <span data-ttu-id="1d5e9-121">これら 2 つのプロパティは、同じ基になる MAPI プロパティにマップします。</span><span class="sxs-lookup"><span data-stu-id="1d5e9-121">These two properties map to the same underlying MAPI property.</span></span> 
  
<span data-ttu-id="1d5e9-122">CreateFolder 操作は、汎用フォルダーの種類の要素を使用してフォルダーを作成し、 **FolderClass**の要素を設定するときにのみ、フォルダーのカスタム クラスの作成をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="1d5e9-122">The CreateFolder operation supports the creation of a custom folder class only when you create the folder by using a generic folder type element and set the **FolderClass** element.</span></span> 
  
## <a name="successful-createfolder-response-example"></a><span data-ttu-id="1d5e9-123">CreateFolder 応答の成功の例</span><span class="sxs-lookup"><span data-stu-id="1d5e9-123">Successful CreateFolder response example</span></span>

### <a name="description"></a><span data-ttu-id="1d5e9-124">説明</span><span class="sxs-lookup"><span data-stu-id="1d5e9-124">Description</span></span>

<span data-ttu-id="1d5e9-125">CreateFolder 要求に正常な応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1d5e9-125">The following example shows a successful response to the CreateFolder request.</span></span> <span data-ttu-id="1d5e9-126">この例では、応答は、新しいフォルダーの識別子を返します。</span><span class="sxs-lookup"><span data-stu-id="1d5e9-126">In this example, the response returns the identifiers of the new folders.</span></span>
  
> [!NOTE]
> <span data-ttu-id="1d5e9-127">フォルダー ID と変更キーは、読みやすさを保持するために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="1d5e9-127">The folder ID and the change key have been shortened to preserve readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="1d5e9-128">コード</span><span class="sxs-lookup"><span data-stu-id="1d5e9-128">Code</span></span>

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
    <CreateFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="successful-response-elements"></a><span data-ttu-id="1d5e9-129">正常な応答の要素</span><span class="sxs-lookup"><span data-stu-id="1d5e9-129">Successful response elements</span></span>

<span data-ttu-id="1d5e9-130">次の要素は、応答で使用されます。</span><span class="sxs-lookup"><span data-stu-id="1d5e9-130">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="1d5e9-131">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="1d5e9-131">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="1d5e9-132">CreateFolderResponse</span><span class="sxs-lookup"><span data-stu-id="1d5e9-132">CreateFolderResponse</span></span>](createfolderresponse.md)
    
- [<span data-ttu-id="1d5e9-133">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="1d5e9-133">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="1d5e9-134">CreateFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="1d5e9-134">CreateFolderResponseMessage</span></span>](createfolderresponsemessage.md)
    
- [<span data-ttu-id="1d5e9-135">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="1d5e9-135">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="1d5e9-136">フォルダー</span><span class="sxs-lookup"><span data-stu-id="1d5e9-136">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="1d5e9-137">Folder</span><span class="sxs-lookup"><span data-stu-id="1d5e9-137">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="1d5e9-138">フォルダー Id</span><span class="sxs-lookup"><span data-stu-id="1d5e9-138">FolderId</span></span>](folderid.md)
    
<span data-ttu-id="1d5e9-139">CreateFolder 操作の応答メッセージには、他のオプションを検索するには、スキーマの階層構造を表示します。</span><span class="sxs-lookup"><span data-stu-id="1d5e9-139">To find other options for the response message of the CreateFolder operation, explore the schema hierarchy.</span></span> <span data-ttu-id="1d5e9-140">[CreateFolderResponse](createfolderresponse.md)要素から開始します。</span><span class="sxs-lookup"><span data-stu-id="1d5e9-140">Start at the [CreateFolderResponse](createfolderresponse.md) element.</span></span> 
  
## <a name="createfolder-error-response"></a><span data-ttu-id="1d5e9-141">CreateFolder エラー応答</span><span class="sxs-lookup"><span data-stu-id="1d5e9-141">CreateFolder error response</span></span>

### <a name="description"></a><span data-ttu-id="1d5e9-142">説明</span><span class="sxs-lookup"><span data-stu-id="1d5e9-142">Description</span></span>

<span data-ttu-id="1d5e9-143">CreateFolder 要求に対してエラー応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1d5e9-143">The following example shows an error response to a CreateFolder request.</span></span>
  
### <a name="code"></a><span data-ttu-id="1d5e9-144">コード</span><span class="sxs-lookup"><span data-stu-id="1d5e9-144">Code</span></span>

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
    <CreateFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="error-response-elements"></a><span data-ttu-id="1d5e9-145">エラー応答の要素</span><span class="sxs-lookup"><span data-stu-id="1d5e9-145">Error response elements</span></span>

<span data-ttu-id="1d5e9-146">エラー応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="1d5e9-146">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="1d5e9-147">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="1d5e9-147">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="1d5e9-148">CreateFolderResponse</span><span class="sxs-lookup"><span data-stu-id="1d5e9-148">CreateFolderResponse</span></span>](createfolderresponse.md)
    
- [<span data-ttu-id="1d5e9-149">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="1d5e9-149">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="1d5e9-150">CreateFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="1d5e9-150">CreateFolderResponseMessage</span></span>](createfolderresponsemessage.md)
    
- [<span data-ttu-id="1d5e9-151">MessageText</span><span class="sxs-lookup"><span data-stu-id="1d5e9-151">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="1d5e9-152">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="1d5e9-152">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="1d5e9-153">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="1d5e9-153">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="1d5e9-154">フォルダー</span><span class="sxs-lookup"><span data-stu-id="1d5e9-154">Folders</span></span>](folders-ex15websvcsotherref.md)
    
<span data-ttu-id="1d5e9-155">CreateFolder 操作の応答のエラー メッセージについては、他のオプションを検索するには、スキーマの階層構造を表示します。</span><span class="sxs-lookup"><span data-stu-id="1d5e9-155">To find other options for the error response message of the CreateFolder operation, explore the schema hierarchy.</span></span> <span data-ttu-id="1d5e9-156">[CreateFolderResponse](createfolderresponse.md)要素から開始します。</span><span class="sxs-lookup"><span data-stu-id="1d5e9-156">Start at the [CreateFolderResponse](createfolderresponse.md) element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="1d5e9-157">関連項目</span><span class="sxs-lookup"><span data-stu-id="1d5e9-157">See also</span></span>



<span data-ttu-id="1d5e9-158">
  [FindItem 操作](finditem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="1d5e9-158">[FindItem operation](finditem-operation.md)</span></span>
  
<span data-ttu-id="1d5e9-159">
  [FindFolder 操作](findfolder-operation.md)</span><span class="sxs-lookup"><span data-stu-id="1d5e9-159">[FindFolder operation](findfolder-operation.md)</span></span>
  
 <span data-ttu-id="1d5e9-160">**CreateFolderType**</span><span class="sxs-lookup"><span data-stu-id="1d5e9-160">**CreateFolderType**</span></span>


- [<span data-ttu-id="1d5e9-161">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="1d5e9-161">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="1d5e9-162">フォルダー (Exchange Web サービス) を作成します。</span><span class="sxs-lookup"><span data-stu-id="1d5e9-162">Creating Folders (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

