---
title: SyncFolderHierarchy 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncFolderHierarchy
api_type:
- schema
ms.assetid: b31916b1-bc6c-4451-a475-b7c5417f752d
description: SyncFolderHierarchy 操作では、Microsoft Exchange Server 2010 を実行しているコンピューターとクライアントの間でフォルダーを同期します。
ms.openlocfilehash: 33c886d5eec64a9ff2ccc667eedfc2d4cc8dcfd5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839633"
---
# <a name="syncfolderhierarchy-operation"></a><span data-ttu-id="f5182-103">SyncFolderHierarchy 操作</span><span class="sxs-lookup"><span data-stu-id="f5182-103">SyncFolderHierarchy operation</span></span>

<span data-ttu-id="f5182-104">SyncFolderHierarchy 操作では、Microsoft Exchange Server 2010 を実行しているコンピューターとクライアントの間でフォルダーを同期します。</span><span class="sxs-lookup"><span data-stu-id="f5182-104">The SyncFolderHierarchy operation synchronizes folders between the computer that is running Microsoft Exchange Server 2010 and the client.</span></span>
  
> [!NOTE]
> <span data-ttu-id="f5182-105">SyncFolderHierarchy 操作では、 [TotalCount](totalcount.md)の[UnreadCount](unreadcount.md)プロパティが変更されたとき、フォルダーは返されません。</span><span class="sxs-lookup"><span data-stu-id="f5182-105">The SyncFolderHierarchy operation does not return folders when the [UnreadCount](unreadcount.md) or [TotalCount](totalcount.md) properties have changed.</span></span> 
  
## <a name="syncfolderhierarchy-request-example"></a><span data-ttu-id="f5182-106">SyncFolderHierarchy 要求の例</span><span class="sxs-lookup"><span data-stu-id="f5182-106">SyncFolderHierarchy request example</span></span>

### <a name="description"></a><span data-ttu-id="f5182-107">説明</span><span class="sxs-lookup"><span data-stu-id="f5182-107">Description</span></span>

<span data-ttu-id="f5182-108">SyncFolderHierarchy 要求の次の使用例は、Exchange サーバーとフォルダーの階層にクライアントを同期する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="f5182-108">The following example of a SyncFolderHierarchy request shows how to synchronize a client folder hierarchy with the Exchange server.</span></span> <span data-ttu-id="f5182-109">この例では、1 つ以上の時間が既に同期されているフォルダーの階層を示します。</span><span class="sxs-lookup"><span data-stu-id="f5182-109">This example shows a folder hierarchy that has already been synchronized at least one time.</span></span> <span data-ttu-id="f5182-110">クライアントが Exchange サーバーと同期する最初の試みの要求では、[同期状態](syncstate-ex15websvcsotherref.md)の要素は含まれません。</span><span class="sxs-lookup"><span data-stu-id="f5182-110">The [SyncState](syncstate-ex15websvcsotherref.md) element is not included in the request for the first attempt to synchronize a client with the Exchange server.</span></span> <span data-ttu-id="f5182-111">最初の要求は、メールボックス内のすべてのフォルダーが返されます。</span><span class="sxs-lookup"><span data-stu-id="f5182-111">The first request will return all the folders in the mailbox.</span></span> <span data-ttu-id="f5182-112">[同期状態](syncstate-ex15websvcsotherref.md)の要素は、 [SyncFolderHierarchyResponse](syncfolderhierarchyresponse.md)で返されます。</span><span class="sxs-lookup"><span data-stu-id="f5182-112">The [SyncState](syncstate-ex15websvcsotherref.md) element will be returned in the [SyncFolderHierarchyResponse](syncfolderhierarchyresponse.md).</span></span> <span data-ttu-id="f5182-113">SyncFolderHierarchy の後続の要求の状態を同期するのにはこの要素を使用します。</span><span class="sxs-lookup"><span data-stu-id="f5182-113">This element is used to synchronize the state for subsequent SyncFolderHierarchy requests.</span></span>
  
### <a name="code"></a><span data-ttu-id="f5182-114">コード</span><span class="sxs-lookup"><span data-stu-id="f5182-114">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <SyncFolderHierarchy  xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <FolderShape>
        <t:BaseShape>AllProperties</t:BaseShape>
      </FolderShape>
      <SyncState>H4sIA=</SyncState>
    </SyncFolderHierarchy>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="f5182-115">コメント</span><span class="sxs-lookup"><span data-stu-id="f5182-115">Comments</span></span>

<span data-ttu-id="f5182-116">[同期状態](syncstate-ex15websvcsotherref.md)の要素の base64 でエンコードされたデータは読みやすさを保持するために短縮されました。</span><span class="sxs-lookup"><span data-stu-id="f5182-116">The [SyncState](syncstate-ex15websvcsotherref.md) element base64-encoded data has been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="f5182-117">要素を要求します。</span><span class="sxs-lookup"><span data-stu-id="f5182-117">Request elements</span></span>

<span data-ttu-id="f5182-118">次の要素は、要求で使用されます。</span><span class="sxs-lookup"><span data-stu-id="f5182-118">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="f5182-119">SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="f5182-119">SyncFolderHierarchy</span></span>](syncfolderhierarchy.md)
    
- [<span data-ttu-id="f5182-120">FolderShape</span><span class="sxs-lookup"><span data-stu-id="f5182-120">FolderShape</span></span>](foldershape.md)
    
- [<span data-ttu-id="f5182-121">BaseShape</span><span class="sxs-lookup"><span data-stu-id="f5182-121">BaseShape</span></span>](baseshape.md)
    
- [<span data-ttu-id="f5182-122">同期状態</span><span class="sxs-lookup"><span data-stu-id="f5182-122">SyncState</span></span>](syncstate-ex15websvcsotherref.md)
    
> [!NOTE]
> <span data-ttu-id="f5182-123">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、これらの要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="f5182-123">The schema that describes these elements is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="successful-syncfolderhierarchy-response"></a><span data-ttu-id="f5182-124">SyncFolderHierarchy の正常な応答</span><span class="sxs-lookup"><span data-stu-id="f5182-124">Successful SyncFolderHierarchy Response</span></span>

### <a name="description"></a><span data-ttu-id="f5182-125">説明</span><span class="sxs-lookup"><span data-stu-id="f5182-125">Description</span></span>

<span data-ttu-id="f5182-126">SyncFolderHierarchy 要求に正常な応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f5182-126">The following example shows a successful response to the SyncFolderHierarchy request.</span></span> <span data-ttu-id="f5182-127">この例では、新しいフォルダーが同期されています。</span><span class="sxs-lookup"><span data-stu-id="f5182-127">In this example, a new folder has been synchronized.</span></span>
  
### <a name="code"></a><span data-ttu-id="f5182-128">コード</span><span class="sxs-lookup"><span data-stu-id="f5182-128">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" 
                         MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SyncFolderHierarchyResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                                 xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:SyncFolderHierarchyResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:SyncState>H4sIAAA==</m:SyncState>
          <m:IncludesLastFolderInRange>true</m:IncludesLastFolderInRange>
          <m:Changes>
            <t:Create>
              <t:Folder>
                <t:FolderId Id="AQApAHR=" ChangeKey="AQAAABY" />
                <t:ParentFolderId Id="AQApA=" ChangeKey="AQAAAA==" />
                <t:FolderClass>IPF.Note</t:FolderClass>
                <t:DisplayName>NewFolder</t:DisplayName>
                <t:TotalCount>0</t:TotalCount>
                <t:ChildFolderCount>0</t:ChildFolderCount>
                <t:UnreadCount>0</t:UnreadCount>
              </t:Folder>
            </t:Create>
          </m:Changes>
        </m:SyncFolderHierarchyResponseMessage>
      </m:ResponseMessages>
    </SyncFolderHierarchyResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="f5182-129">コメント</span><span class="sxs-lookup"><span data-stu-id="f5182-129">Comments</span></span>

<span data-ttu-id="f5182-130">[同期状態](syncstate-ex15websvcsotherref.md)の要素の base64 でエンコードされたデータやフォルダーの識別子のデータは、読みやすさを保持するために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="f5182-130">The [SyncState](syncstate-ex15websvcsotherref.md) element base64-encoded data and the folder identifier data have been shortened to preserve readability.</span></span> 
  
### <a name="successful-response-elements"></a><span data-ttu-id="f5182-131">正常な応答の要素</span><span class="sxs-lookup"><span data-stu-id="f5182-131">Successful response elements</span></span>

<span data-ttu-id="f5182-132">次の要素は、応答で使用されます。</span><span class="sxs-lookup"><span data-stu-id="f5182-132">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="f5182-133">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="f5182-133">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="f5182-134">SyncFolderHierarchyResponse</span><span class="sxs-lookup"><span data-stu-id="f5182-134">SyncFolderHierarchyResponse</span></span>](syncfolderhierarchyresponse.md)
    
- [<span data-ttu-id="f5182-135">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="f5182-135">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="f5182-136">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="f5182-136">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md)
    
- [<span data-ttu-id="f5182-137">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="f5182-137">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="f5182-138">同期状態</span><span class="sxs-lookup"><span data-stu-id="f5182-138">SyncState</span></span>](syncstate-ex15websvcsotherref.md)
    
- [<span data-ttu-id="f5182-139">IncludesLastFolderInRange</span><span class="sxs-lookup"><span data-stu-id="f5182-139">IncludesLastFolderInRange</span></span>](includeslastfolderinrange.md)
    
- [<span data-ttu-id="f5182-140">(階層) の変更</span><span class="sxs-lookup"><span data-stu-id="f5182-140">Changes (Hierarchy)</span></span>](changes-hierarchy.md)
    
- [<span data-ttu-id="f5182-141">(集合的) を作成します。</span><span class="sxs-lookup"><span data-stu-id="f5182-141">Create (FolderSync)</span></span>](create-foldersync.md)
    
- [<span data-ttu-id="f5182-142">Folder</span><span class="sxs-lookup"><span data-stu-id="f5182-142">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="f5182-143">フォルダー Id</span><span class="sxs-lookup"><span data-stu-id="f5182-143">FolderId</span></span>](folderid.md)
    
- [<span data-ttu-id="f5182-144">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="f5182-144">ParentFolderId</span></span>](parentfolderid.md)
    
- [<span data-ttu-id="f5182-145">FolderClass</span><span class="sxs-lookup"><span data-stu-id="f5182-145">FolderClass</span></span>](folderclass.md)
    
- [<span data-ttu-id="f5182-146">表示名 (文字列)</span><span class="sxs-lookup"><span data-stu-id="f5182-146">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="f5182-147">TotalCount</span><span class="sxs-lookup"><span data-stu-id="f5182-147">TotalCount</span></span>](totalcount.md)
    
- [<span data-ttu-id="f5182-148">ChildFolderCount</span><span class="sxs-lookup"><span data-stu-id="f5182-148">ChildFolderCount</span></span>](childfoldercount.md)
    
- [<span data-ttu-id="f5182-149">UnreadCount</span><span class="sxs-lookup"><span data-stu-id="f5182-149">UnreadCount</span></span>](unreadcount.md)
    
## <a name="syncfolderhierarchy-error-response"></a><span data-ttu-id="f5182-150">SyncFolderHierarchy エラー応答</span><span class="sxs-lookup"><span data-stu-id="f5182-150">SyncFolderHierarchy error response</span></span>

### <a name="description"></a><span data-ttu-id="f5182-151">説明</span><span class="sxs-lookup"><span data-stu-id="f5182-151">Description</span></span>

<span data-ttu-id="f5182-152">SyncFolderHierarchy 要求に対してエラー応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f5182-152">The following example shows an error response to a SyncFolderHierarchy request.</span></span> <span data-ttu-id="f5182-153">このエラーは、無効な同期状態が原因です。</span><span class="sxs-lookup"><span data-stu-id="f5182-153">This error was caused by an invalid SyncState.</span></span>
  
### <a name="code"></a><span data-ttu-id="f5182-154">コード</span><span class="sxs-lookup"><span data-stu-id="f5182-154">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" 
                         MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SyncFolderHierarchyResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                                 xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:SyncFolderHierarchyResponseMessage ResponseClass="Error">
          <m:MessageText>Synchronization state data is corrupted or otherwise invalid.</m:MessageText>
          <m:ResponseCode>ErrorInvalidSyncStateData</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:SyncState />
          <m:IncludesLastFolderInRange>true</m:IncludesLastFolderInRange>
        </m:SyncFolderHierarchyResponseMessage>
      </m:ResponseMessages>
    </SyncFolderHierarchyResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="f5182-155">エラー応答の要素</span><span class="sxs-lookup"><span data-stu-id="f5182-155">Error response elements</span></span>

<span data-ttu-id="f5182-156">エラー応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="f5182-156">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="f5182-157">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="f5182-157">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="f5182-158">SyncFolderHierarchyResponse</span><span class="sxs-lookup"><span data-stu-id="f5182-158">SyncFolderHierarchyResponse</span></span>](syncfolderhierarchyresponse.md)
    
- [<span data-ttu-id="f5182-159">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="f5182-159">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="f5182-160">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="f5182-160">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md)
    
- [<span data-ttu-id="f5182-161">MessageText</span><span class="sxs-lookup"><span data-stu-id="f5182-161">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="f5182-162">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="f5182-162">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="f5182-163">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="f5182-163">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="f5182-164">同期状態</span><span class="sxs-lookup"><span data-stu-id="f5182-164">SyncState</span></span>](syncstate-ex15websvcsotherref.md)
    
- [<span data-ttu-id="f5182-165">IncludesLastFolderInRange</span><span class="sxs-lookup"><span data-stu-id="f5182-165">IncludesLastFolderInRange</span></span>](includeslastfolderinrange.md)
    
## <a name="see-also"></a><span data-ttu-id="f5182-166">関連項目</span><span class="sxs-lookup"><span data-stu-id="f5182-166">See also</span></span>



- [<span data-ttu-id="f5182-167">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="f5182-167">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

