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
description: SyncFolderHierarchy 操作は、Microsoft Exchange Server 2010 とクライアントを実行しているコンピューター間でフォルダーを同期します。
ms.openlocfilehash: 1c7ad2413064161ba54e8a7a30bfcd6f23f218bd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456431"
---
# <a name="syncfolderhierarchy-operation"></a><span data-ttu-id="35c57-103">SyncFolderHierarchy 操作</span><span class="sxs-lookup"><span data-stu-id="35c57-103">SyncFolderHierarchy operation</span></span>

<span data-ttu-id="35c57-104">SyncFolderHierarchy 操作は、Microsoft Exchange Server 2010 とクライアントを実行しているコンピューター間でフォルダーを同期します。</span><span class="sxs-lookup"><span data-stu-id="35c57-104">The SyncFolderHierarchy operation synchronizes folders between the computer that is running Microsoft Exchange Server 2010 and the client.</span></span>
  
> [!NOTE]
> <span data-ttu-id="35c57-105">SyncFolderHierarchy 操作では、 [UnreadCount](unreadcount.md)または[totalcount](totalcount.md)のプロパティが変更されたときにフォルダーは返されません。</span><span class="sxs-lookup"><span data-stu-id="35c57-105">The SyncFolderHierarchy operation does not return folders when the [UnreadCount](unreadcount.md) or [TotalCount](totalcount.md) properties have changed.</span></span> 
  
## <a name="syncfolderhierarchy-request-example"></a><span data-ttu-id="35c57-106">SyncFolderHierarchy 要求の例</span><span class="sxs-lookup"><span data-stu-id="35c57-106">SyncFolderHierarchy request example</span></span>

### <a name="description"></a><span data-ttu-id="35c57-107">説明</span><span class="sxs-lookup"><span data-stu-id="35c57-107">Description</span></span>

<span data-ttu-id="35c57-108">次の SyncFolderHierarchy 要求の例は、クライアントフォルダー階層を Exchange サーバーと同期する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="35c57-108">The following example of a SyncFolderHierarchy request shows how to synchronize a client folder hierarchy with the Exchange server.</span></span> <span data-ttu-id="35c57-109">この例では、少なくとも1回同期されているフォルダー階層を示します。</span><span class="sxs-lookup"><span data-stu-id="35c57-109">This example shows a folder hierarchy that has already been synchronized at least one time.</span></span> <span data-ttu-id="35c57-110">クライアントと Exchange サーバーの同期を最初に試行する要求には、 [Syncstate](syncstate-ex15websvcsotherref.md)要素は含まれていません。</span><span class="sxs-lookup"><span data-stu-id="35c57-110">The [SyncState](syncstate-ex15websvcsotherref.md) element is not included in the request for the first attempt to synchronize a client with the Exchange server.</span></span> <span data-ttu-id="35c57-111">最初の要求では、メールボックス内のすべてのフォルダーが返されます。</span><span class="sxs-lookup"><span data-stu-id="35c57-111">The first request will return all the folders in the mailbox.</span></span> <span data-ttu-id="35c57-112">[Syncstate](syncstate-ex15websvcsotherref.md)要素は、 [SyncFolderHierarchyResponse](syncfolderhierarchyresponse.md)で返されます。</span><span class="sxs-lookup"><span data-stu-id="35c57-112">The [SyncState](syncstate-ex15websvcsotherref.md) element will be returned in the [SyncFolderHierarchyResponse](syncfolderhierarchyresponse.md).</span></span> <span data-ttu-id="35c57-113">この要素は、後続の SyncFolderHierarchy 要求の状態を同期するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="35c57-113">This element is used to synchronize the state for subsequent SyncFolderHierarchy requests.</span></span>
  
### <a name="code"></a><span data-ttu-id="35c57-114">コード</span><span class="sxs-lookup"><span data-stu-id="35c57-114">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <SyncFolderHierarchy  xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <FolderShape>
        <t:BaseShape>AllProperties</t:BaseShape>
      </FolderShape>
      <SyncState>H4sIA=</SyncState>
    </SyncFolderHierarchy>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="35c57-115">コメント</span><span class="sxs-lookup"><span data-stu-id="35c57-115">Comments</span></span>

<span data-ttu-id="35c57-116">読み取りやすさを維持するために、 [Syncstate](syncstate-ex15websvcsotherref.md)要素の base64 でエンコードされたデータは短縮されています。</span><span class="sxs-lookup"><span data-stu-id="35c57-116">The [SyncState](syncstate-ex15websvcsotherref.md) element base64-encoded data has been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="35c57-117">Request 要素</span><span class="sxs-lookup"><span data-stu-id="35c57-117">Request elements</span></span>

<span data-ttu-id="35c57-118">要求では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="35c57-118">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="35c57-119">SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="35c57-119">SyncFolderHierarchy</span></span>](syncfolderhierarchy.md)
    
- [<span data-ttu-id="35c57-120">FolderShape</span><span class="sxs-lookup"><span data-stu-id="35c57-120">FolderShape</span></span>](foldershape.md)
    
- [<span data-ttu-id="35c57-121">BaseShape</span><span class="sxs-lookup"><span data-stu-id="35c57-121">BaseShape</span></span>](baseshape.md)
    
- [<span data-ttu-id="35c57-122">SyncState</span><span class="sxs-lookup"><span data-stu-id="35c57-122">SyncState</span></span>](syncstate-ex15websvcsotherref.md)
    
> [!NOTE]
> <span data-ttu-id="35c57-123">これらの要素を説明するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="35c57-123">The schema that describes these elements is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="successful-syncfolderhierarchy-response"></a><span data-ttu-id="35c57-124">成功した SyncFolderHierarchy 応答</span><span class="sxs-lookup"><span data-stu-id="35c57-124">Successful SyncFolderHierarchy Response</span></span>

### <a name="description"></a><span data-ttu-id="35c57-125">説明</span><span class="sxs-lookup"><span data-stu-id="35c57-125">Description</span></span>

<span data-ttu-id="35c57-126">次の例は、SyncFolderHierarchy 要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="35c57-126">The following example shows a successful response to the SyncFolderHierarchy request.</span></span> <span data-ttu-id="35c57-127">この例では、新しいフォルダーが同期されています。</span><span class="sxs-lookup"><span data-stu-id="35c57-127">In this example, a new folder has been synchronized.</span></span>
  
### <a name="code"></a><span data-ttu-id="35c57-128">コード</span><span class="sxs-lookup"><span data-stu-id="35c57-128">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" 
                         MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SyncFolderHierarchyResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                                 xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="35c57-129">コメント</span><span class="sxs-lookup"><span data-stu-id="35c57-129">Comments</span></span>

<span data-ttu-id="35c57-130">読みやすくするために、 [Syncstate](syncstate-ex15websvcsotherref.md)要素の base64 でエンコードされたデータとフォルダー識別子データは短縮されています。</span><span class="sxs-lookup"><span data-stu-id="35c57-130">The [SyncState](syncstate-ex15websvcsotherref.md) element base64-encoded data and the folder identifier data have been shortened to preserve readability.</span></span> 
  
### <a name="successful-response-elements"></a><span data-ttu-id="35c57-131">成功した応答要素</span><span class="sxs-lookup"><span data-stu-id="35c57-131">Successful response elements</span></span>

<span data-ttu-id="35c57-132">応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="35c57-132">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="35c57-133">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="35c57-133">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="35c57-134">SyncFolderHierarchyResponse</span><span class="sxs-lookup"><span data-stu-id="35c57-134">SyncFolderHierarchyResponse</span></span>](syncfolderhierarchyresponse.md)
    
- [<span data-ttu-id="35c57-135">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="35c57-135">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="35c57-136">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="35c57-136">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md)
    
- [<span data-ttu-id="35c57-137">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="35c57-137">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="35c57-138">SyncState</span><span class="sxs-lookup"><span data-stu-id="35c57-138">SyncState</span></span>](syncstate-ex15websvcsotherref.md)
    
- [<span data-ttu-id="35c57-139">フォルダーに Lastfolderinrange</span><span class="sxs-lookup"><span data-stu-id="35c57-139">IncludesLastFolderInRange</span></span>](includeslastfolderinrange.md)
    
- [<span data-ttu-id="35c57-140">変更 (階層)</span><span class="sxs-lookup"><span data-stu-id="35c57-140">Changes (Hierarchy)</span></span>](changes-hierarchy.md)
    
- [<span data-ttu-id="35c57-141">Create (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="35c57-141">Create (FolderSync)</span></span>](create-foldersync.md)
    
- [<span data-ttu-id="35c57-142">Folder</span><span class="sxs-lookup"><span data-stu-id="35c57-142">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="35c57-143">FolderId</span><span class="sxs-lookup"><span data-stu-id="35c57-143">FolderId</span></span>](folderid.md)
    
- [<span data-ttu-id="35c57-144">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="35c57-144">ParentFolderId</span></span>](parentfolderid.md)
    
- [<span data-ttu-id="35c57-145">FolderClass</span><span class="sxs-lookup"><span data-stu-id="35c57-145">FolderClass</span></span>](folderclass.md)
    
- [<span data-ttu-id="35c57-146">DisplayName (文字列)</span><span class="sxs-lookup"><span data-stu-id="35c57-146">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="35c57-147">TotalCount</span><span class="sxs-lookup"><span data-stu-id="35c57-147">TotalCount</span></span>](totalcount.md)
    
- [<span data-ttu-id="35c57-148">ChildFolderCount</span><span class="sxs-lookup"><span data-stu-id="35c57-148">ChildFolderCount</span></span>](childfoldercount.md)
    
- [<span data-ttu-id="35c57-149">UnreadCount</span><span class="sxs-lookup"><span data-stu-id="35c57-149">UnreadCount</span></span>](unreadcount.md)
    
## <a name="syncfolderhierarchy-error-response"></a><span data-ttu-id="35c57-150">SyncFolderHierarchy のエラー応答</span><span class="sxs-lookup"><span data-stu-id="35c57-150">SyncFolderHierarchy error response</span></span>

### <a name="description"></a><span data-ttu-id="35c57-151">説明</span><span class="sxs-lookup"><span data-stu-id="35c57-151">Description</span></span>

<span data-ttu-id="35c57-152">次の例は、SyncFolderHierarchy 要求に対するエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="35c57-152">The following example shows an error response to a SyncFolderHierarchy request.</span></span> <span data-ttu-id="35c57-153">このエラーは、無効な SyncState が原因で発生しました。</span><span class="sxs-lookup"><span data-stu-id="35c57-153">This error was caused by an invalid SyncState.</span></span>
  
### <a name="code"></a><span data-ttu-id="35c57-154">コード</span><span class="sxs-lookup"><span data-stu-id="35c57-154">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" 
                         MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SyncFolderHierarchyResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                                 xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="error-response-elements"></a><span data-ttu-id="35c57-155">エラー応答要素</span><span class="sxs-lookup"><span data-stu-id="35c57-155">Error response elements</span></span>

<span data-ttu-id="35c57-156">エラー応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="35c57-156">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="35c57-157">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="35c57-157">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="35c57-158">SyncFolderHierarchyResponse</span><span class="sxs-lookup"><span data-stu-id="35c57-158">SyncFolderHierarchyResponse</span></span>](syncfolderhierarchyresponse.md)
    
- [<span data-ttu-id="35c57-159">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="35c57-159">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="35c57-160">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="35c57-160">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md)
    
- [<span data-ttu-id="35c57-161">MessageText</span><span class="sxs-lookup"><span data-stu-id="35c57-161">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="35c57-162">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="35c57-162">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="35c57-163">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="35c57-163">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="35c57-164">SyncState</span><span class="sxs-lookup"><span data-stu-id="35c57-164">SyncState</span></span>](syncstate-ex15websvcsotherref.md)
    
- [<span data-ttu-id="35c57-165">フォルダーに Lastfolderinrange</span><span class="sxs-lookup"><span data-stu-id="35c57-165">IncludesLastFolderInRange</span></span>](includeslastfolderinrange.md)
    
## <a name="see-also"></a><span data-ttu-id="35c57-166">関連項目</span><span class="sxs-lookup"><span data-stu-id="35c57-166">See also</span></span>



- [<span data-ttu-id="35c57-167">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="35c57-167">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

