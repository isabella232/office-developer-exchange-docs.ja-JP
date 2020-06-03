---
title: SyncFolderItems 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncFolderItems
api_type:
- schema
ms.assetid: 7f0de089-8876-47ec-a871-df118ceae75d
description: SyncFolderItems 操作は、Exchange サーバーとクライアントの間でアイテムを同期します。
ms.openlocfilehash: 1a28d895eda11dd43f77ec2662a60a426cfc463c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468146"
---
# <a name="syncfolderitems-operation"></a><span data-ttu-id="421cc-103">SyncFolderItems 操作</span><span class="sxs-lookup"><span data-stu-id="421cc-103">SyncFolderItems operation</span></span>

<span data-ttu-id="421cc-104">SyncFolderItems 操作は、Exchange サーバーとクライアントの間でアイテムを同期します。</span><span class="sxs-lookup"><span data-stu-id="421cc-104">The SyncFolderItems operation synchronizes items between the Exchange server and the client.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="421cc-105">注釈</span><span class="sxs-lookup"><span data-stu-id="421cc-105">Remarks</span></span>

<span data-ttu-id="421cc-106">SyncFolderItems 操作は、最大512の変更を返します。</span><span class="sxs-lookup"><span data-stu-id="421cc-106">The SyncFolderItems operation will return a maximum of 512 changes.</span></span> <span data-ttu-id="421cc-107">追加の変更を取得するには、以降の SyncFolderItems 要求を実行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="421cc-107">Subsequent SyncFolderItems requests must be performed to get additional changes.</span></span> 
  
<span data-ttu-id="421cc-108">SyncFolderItems は FindItem 操作に似ていますが、本文や添付ファイルなどのプロパティを返すことはできません。</span><span class="sxs-lookup"><span data-stu-id="421cc-108">SyncFolderItems is similar to the FindItem operation in that it cannot return properties like Body or Attachments.</span></span> <span data-ttu-id="421cc-109">SyncFolderItems 操作が必要なプロパティを返さない場合は、 [GetItem 操作](getitem-operation.md)を使用して、syncfolderitems から返された各アイテムの特定のプロパティセットを取得できます。</span><span class="sxs-lookup"><span data-stu-id="421cc-109">If the SyncFolderItems operation does not return the properties that you need, you can use the [GetItem operation](getitem-operation.md) to get a specific set of properties for each item that it returned by SyncFolderItems.</span></span> 
  
## <a name="syncfolderitems-request-example"></a><span data-ttu-id="421cc-110">SyncFolderItems 要求の例</span><span class="sxs-lookup"><span data-stu-id="421cc-110">SyncFolderItems request example</span></span>

### <a name="description"></a><span data-ttu-id="421cc-111">Description</span><span class="sxs-lookup"><span data-stu-id="421cc-111">Description</span></span>

<span data-ttu-id="421cc-112">次の SyncFolderItems 要求の例は、フォルダー内のアイテムを同期する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="421cc-112">The following example of a SyncFolderItems request shows how to synchronize items in a folder.</span></span> <span data-ttu-id="421cc-113">この例では、[送信済みアイテム] フォルダーに対して行われた最初の同期ではないフォルダーアイテムの同期を示します。</span><span class="sxs-lookup"><span data-stu-id="421cc-113">This example shows a folder item's synchronization that is not the first synchronization to have occurred for the Sent Items folder.</span></span> <span data-ttu-id="421cc-114">クライアントと Exchange サーバーの同期を最初に試行する要求には、 [Syncstate](syncstate-ex15websvcsotherref.md)要素は含まれていません。</span><span class="sxs-lookup"><span data-stu-id="421cc-114">The [SyncState](syncstate-ex15websvcsotherref.md) element is not included in the request for the first attempt to synchronize a client with the Exchange server.</span></span> <span data-ttu-id="421cc-115">フォルダー階層内のアイテムを最初に同期しようとすると、そのメールボックス内のすべてのアイテムが返されます。[無視](ignore.md)要素で識別されるアイテムは除きます。</span><span class="sxs-lookup"><span data-stu-id="421cc-115">The first attempt to synchronize the items in a folder hierarchy will return all the items in the mailbox, excluding items that are identified in the [Ignore](ignore.md) element.</span></span> <span data-ttu-id="421cc-116">この SyncFolderItems 要求は、前回の同期以降のフォルダーアイテムへのすべての変更を同期しようとします。</span><span class="sxs-lookup"><span data-stu-id="421cc-116">This SyncFolderItems request will try to synchronize all changes to the folder items since the last synchronization.</span></span> <span data-ttu-id="421cc-117">この要求は、 [ignore](ignore.md)要素で識別される1つのアイテムを同期しようとする試行を無視します。</span><span class="sxs-lookup"><span data-stu-id="421cc-117">This request will ignore the attempt to synchronize the one item that is identified in the [Ignore](ignore.md) element.</span></span> 
  
### <a name="code"></a><span data-ttu-id="421cc-118">コード</span><span class="sxs-lookup"><span data-stu-id="421cc-118">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <SyncFolderItems xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemShape>
        <t:BaseShape>Default</t:BaseShape>
      </ItemShape>
      <SyncFolderId>
        <t:DistinguishedFolderId Id="sentitems"/>
      </SyncFolderId>
      <SyncState>AEbJ94eMOAAA=</SyncState>
      <Ignore>
        <t:ItemId Id="AQApAHRAA==" ChangeKey="CQAAABY"/>
      </Ignore>
      <MaxChangesReturned>100</MaxChangesReturned>
    </SyncFolderItems>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="421cc-119">コメント</span><span class="sxs-lookup"><span data-stu-id="421cc-119">Comments</span></span>

<span data-ttu-id="421cc-120">読みやすくするために、 [Syncstate](syncstate-ex15websvcsotherref.md)要素の base64 でエンコードされたデータと[ItemId](itemid.md)要素**Id**属性は短縮されています。</span><span class="sxs-lookup"><span data-stu-id="421cc-120">The [SyncState](syncstate-ex15websvcsotherref.md) element base64-encoded data and the [ItemId](itemid.md) element **Id** attribute have been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="421cc-121">Request 要素</span><span class="sxs-lookup"><span data-stu-id="421cc-121">Request elements</span></span>

<span data-ttu-id="421cc-122">要求では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="421cc-122">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="421cc-123">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="421cc-123">SyncFolderItems</span></span>](syncfolderitems.md)
    
- [<span data-ttu-id="421cc-124">ItemShape</span><span class="sxs-lookup"><span data-stu-id="421cc-124">ItemShape</span></span>](itemshape.md)
    
- [<span data-ttu-id="421cc-125">BaseShape</span><span class="sxs-lookup"><span data-stu-id="421cc-125">BaseShape</span></span>](baseshape.md)
    
- [<span data-ttu-id="421cc-126">SyncFolderId</span><span class="sxs-lookup"><span data-stu-id="421cc-126">SyncFolderId</span></span>](syncfolderid.md)
    
- [<span data-ttu-id="421cc-127">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="421cc-127">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="421cc-128">SyncState</span><span class="sxs-lookup"><span data-stu-id="421cc-128">SyncState</span></span>](syncstate-ex15websvcsotherref.md)
    
- [<span data-ttu-id="421cc-129">無視</span><span class="sxs-lookup"><span data-stu-id="421cc-129">Ignore</span></span>](ignore.md)
    
- [<span data-ttu-id="421cc-130">ItemId</span><span class="sxs-lookup"><span data-stu-id="421cc-130">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="421cc-131">Maxの戻り値</span><span class="sxs-lookup"><span data-stu-id="421cc-131">MaxChangesReturned</span></span>](maxchangesreturned.md)
    
## <a name="successful-syncfolderitems-response"></a><span data-ttu-id="421cc-132">正常な SyncFolderItems 応答</span><span class="sxs-lookup"><span data-stu-id="421cc-132">Successful SyncFolderItems Response</span></span>

### <a name="description"></a><span data-ttu-id="421cc-133">Description</span><span class="sxs-lookup"><span data-stu-id="421cc-133">Description</span></span>

<span data-ttu-id="421cc-134">次の例は、SyncFolderItems 要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="421cc-134">The following example shows a successful response to the SyncFolderItems request.</span></span> <span data-ttu-id="421cc-135">この例では、[送信済みアイテム] フォルダーから会議出席依頼が同期されます。</span><span class="sxs-lookup"><span data-stu-id="421cc-135">In this example, a meeting request is synchronized from the Sent Items folder.</span></span>
  
### <a name="code"></a><span data-ttu-id="421cc-136">コード</span><span class="sxs-lookup"><span data-stu-id="421cc-136">Code</span></span>

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
    <SyncFolderItemsResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                             xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                             xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:SyncFolderItemsResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:SyncState>H4sIAAAAA=</m:SyncState>
          <m:IncludesLastItemInRange>true</m:IncludesLastItemInRange>
          <m:Changes>
            <t:Create>
              <t:MeetingRequest>
                <t:ItemId Id="AQApAHRwA==" ChangeKey="CwAAABYA" />
                <t:Subject>Budget Q3</t:Subject>
                <t:Sensitivity>Normal</t:Sensitivity>
                <t:IsOutOfDate>false</t:IsOutOfDate>
                <t:HasBeenProcessed>true</t:HasBeenProcessed>
                <t:ResponseType>NoResponseReceived</t:ResponseType>
                <t:IntendedFreeBusyStatus>Busy</t:IntendedFreeBusyStatus>
                <t:Start>2006-08-02T17:30:00Z</t:Start>
                <t:End>2006-08-02T19:30:00Z</t:End>
                <t:Location>Conference Room 2</t:Location>
                <t:Organizer>
                  <t:Mailbox>
                    <t:Name>Dan Park</t:Name>
                    <t:EmailAddress>dpark@example.com</t:EmailAddress>
                    <t:RoutingType>SMTP</t:RoutingType>
                  </t:Mailbox>
                </t:Organizer>
              </t:MeetingRequest>
            </t:Create>
          </m:Changes>
        </m:SyncFolderItemsResponseMessage>
      </m:ResponseMessages>
    </SyncFolderItemsResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="421cc-137">コメント</span><span class="sxs-lookup"><span data-stu-id="421cc-137">Comments</span></span>

<span data-ttu-id="421cc-138">読みやすくするために、 [Syncstate](syncstate-ex15websvcsotherref.md)要素の base64 でエンコードされたデータと[ItemId](itemid.md)要素**Id**属性は短縮されています。</span><span class="sxs-lookup"><span data-stu-id="421cc-138">The [SyncState](syncstate-ex15websvcsotherref.md) element base64-encoded data and the [ItemId](itemid.md) element **Id** attribute have been shortened to preserve readability.</span></span> 
  
### <a name="successful-response-elements"></a><span data-ttu-id="421cc-139">成功した応答要素</span><span class="sxs-lookup"><span data-stu-id="421cc-139">Successful response elements</span></span>

<span data-ttu-id="421cc-140">応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="421cc-140">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="421cc-141">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="421cc-141">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="421cc-142">SyncFolderItemsResponse</span><span class="sxs-lookup"><span data-stu-id="421cc-142">SyncFolderItemsResponse</span></span>](syncfolderitemsresponse.md)
    
- [<span data-ttu-id="421cc-143">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="421cc-143">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="421cc-144">SyncFolderItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="421cc-144">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md)
    
- [<span data-ttu-id="421cc-145">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="421cc-145">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="421cc-146">SyncState</span><span class="sxs-lookup"><span data-stu-id="421cc-146">SyncState</span></span>](syncstate-ex15websvcsotherref.md)
    
- [<span data-ttu-id="421cc-147">IncludesLastItemInRange</span><span class="sxs-lookup"><span data-stu-id="421cc-147">IncludesLastItemInRange</span></span>](includeslastiteminrange.md)
    
- [<span data-ttu-id="421cc-148">変更 (アイテム)</span><span class="sxs-lookup"><span data-stu-id="421cc-148">Changes (Items)</span></span>](changes-items.md)
    
- [<span data-ttu-id="421cc-149">Create (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="421cc-149">Create (ItemSync)</span></span>](create-itemsync.md)
    
- [<span data-ttu-id="421cc-150">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="421cc-150">MeetingRequest</span></span>](meetingrequest.md)
    
- [<span data-ttu-id="421cc-151">ItemId</span><span class="sxs-lookup"><span data-stu-id="421cc-151">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="421cc-152">件名</span><span class="sxs-lookup"><span data-stu-id="421cc-152">Subject</span></span>](subject.md)
    
- [<span data-ttu-id="421cc-153">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="421cc-153">Sensitivity</span></span>](sensitivity.md)
    
- [<span data-ttu-id="421cc-154">IsOutOfDate</span><span class="sxs-lookup"><span data-stu-id="421cc-154">IsOutOfDate</span></span>](isoutofdate.md)
    
- [<span data-ttu-id="421cc-155">Hasが処理されました</span><span class="sxs-lookup"><span data-stu-id="421cc-155">HasBeenProcessed</span></span>](hasbeenprocessed.md)
    
- [<span data-ttu-id="421cc-156">ResponseType</span><span class="sxs-lookup"><span data-stu-id="421cc-156">ResponseType</span></span>](responsetype.md)
    
- [<span data-ttu-id="421cc-157">IntendedFreeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="421cc-157">IntendedFreeBusyStatus</span></span>](intendedfreebusystatus.md)
    
- [<span data-ttu-id="421cc-158">開始</span><span class="sxs-lookup"><span data-stu-id="421cc-158">Start</span></span>](start.md)
    
- [<span data-ttu-id="421cc-159">終わり</span><span class="sxs-lookup"><span data-stu-id="421cc-159">End </span></span>](end-ex15websvcsotherref.md)
    
- [<span data-ttu-id="421cc-160">場所</span><span class="sxs-lookup"><span data-stu-id="421cc-160">Location</span></span>](location.md)
    
- [<span data-ttu-id="421cc-161">Organizer</span><span class="sxs-lookup"><span data-stu-id="421cc-161">Organizer</span></span>](organizer.md)
    
- [<span data-ttu-id="421cc-162">メールボックス</span><span class="sxs-lookup"><span data-stu-id="421cc-162">Mailbox</span></span>](mailbox.md)
    
- [<span data-ttu-id="421cc-163">Name (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="421cc-163">Name (EmailAddressType)</span></span>](name-emailaddresstype.md)
    
- [<span data-ttu-id="421cc-164">EmailAddress (非 Emptystringtype)</span><span class="sxs-lookup"><span data-stu-id="421cc-164">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
- [<span data-ttu-id="421cc-165">RoutingType (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="421cc-165">RoutingType (EmailAddressType)</span></span>](routingtype-emailaddresstype.md)
    
## <a name="syncfolderitems-error-response"></a><span data-ttu-id="421cc-166">SyncFolderItems エラー応答</span><span class="sxs-lookup"><span data-stu-id="421cc-166">SyncFolderItems error response</span></span>

### <a name="description"></a><span data-ttu-id="421cc-167">Description</span><span class="sxs-lookup"><span data-stu-id="421cc-167">Description</span></span>

<span data-ttu-id="421cc-168">次の例は、SyncFolderItems 要求に対するエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="421cc-168">The following example shows an error response to a SyncFolderItems request.</span></span> <span data-ttu-id="421cc-169">このエラーは、無効な SyncState が原因で発生しました。</span><span class="sxs-lookup"><span data-stu-id="421cc-169">This error was caused by an invalid SyncState.</span></span>
  
### <a name="code"></a><span data-ttu-id="421cc-170">コード</span><span class="sxs-lookup"><span data-stu-id="421cc-170">Code</span></span>

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
    <SyncFolderItemsResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                             xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                             xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:SyncFolderItemsResponseMessage ResponseClass="Error">
          <m:MessageText>Synchronization state data is corrupt or otherwise invalid.</m:MessageText>
          <m:ResponseCode>ErrorInvalidSyncStateData</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:SyncState />
          <m:IncludesLastItemInRange>true</m:IncludesLastItemInRange>
        </m:SyncFolderItemsResponseMessage>
      </m:ResponseMessages>
    </SyncFolderItemsResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="421cc-171">エラー応答要素</span><span class="sxs-lookup"><span data-stu-id="421cc-171">Error response elements</span></span>

<span data-ttu-id="421cc-172">エラー応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="421cc-172">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="421cc-173">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="421cc-173">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="421cc-174">SyncFolderItemsResponse</span><span class="sxs-lookup"><span data-stu-id="421cc-174">SyncFolderItemsResponse</span></span>](syncfolderitemsresponse.md)
    
- [<span data-ttu-id="421cc-175">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="421cc-175">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="421cc-176">SyncFolderItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="421cc-176">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md)
    
- [<span data-ttu-id="421cc-177">MessageText</span><span class="sxs-lookup"><span data-stu-id="421cc-177">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="421cc-178">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="421cc-178">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="421cc-179">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="421cc-179">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="421cc-180">SyncState</span><span class="sxs-lookup"><span data-stu-id="421cc-180">SyncState</span></span>](syncstate-ex15websvcsotherref.md)
    
- [<span data-ttu-id="421cc-181">IncludesLastItemInRange</span><span class="sxs-lookup"><span data-stu-id="421cc-181">IncludesLastItemInRange</span></span>](includeslastiteminrange.md)
    
## <a name="see-also"></a><span data-ttu-id="421cc-182">関連項目</span><span class="sxs-lookup"><span data-stu-id="421cc-182">See also</span></span>



- [<span data-ttu-id="421cc-183">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="421cc-183">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

