---
title: UpdateFolder 操作
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateFolder
api_type:
- schema
ms.assetid: 3494c996-b834-4813-b1ca-d99642d8b4e7
description: UpdateFolder 操作は、Exchange ストア内の既存のアイテムのプロパティを変更するために使用されます。 各 UpdateFolder 操作は、次の要素で構成されます。
ms.openlocfilehash: fb894d9f42358b67f81e9fe8ae41ba61e6f46460
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467362"
---
# <a name="updatefolder-operation"></a><span data-ttu-id="2cb27-104">UpdateFolder 操作</span><span class="sxs-lookup"><span data-stu-id="2cb27-104">UpdateFolder operation</span></span>

<span data-ttu-id="2cb27-105">UpdateFolder 操作は、Exchange ストア内の既存のアイテムのプロパティを変更するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="2cb27-105">The UpdateFolder operation is used to modify properties of an existing item in the Exchange store.</span></span> <span data-ttu-id="2cb27-106">各 UpdateFolder 操作は、次の要素で構成されます。</span><span class="sxs-lookup"><span data-stu-id="2cb27-106">Each UpdateFolder operation consists of the following:</span></span>
  
- <span data-ttu-id="2cb27-107">更新するフォルダーを指定する[FolderId](folderid.md)要素。</span><span class="sxs-lookup"><span data-stu-id="2cb27-107">A [FolderId](folderid.md) element that specifies a folder to update.</span></span> 
    
- <span data-ttu-id="2cb27-108">Folder 図形で指定された、フォルダー内の要素の内部パス。更新するデータを指定します。</span><span class="sxs-lookup"><span data-stu-id="2cb27-108">An internal path of an element in the folder, as specified by the folder shape, which specifies the data to update.</span></span>
    
- <span data-ttu-id="2cb27-109">更新が削除されていない場合は、更新されたフィールドの新しい値を含むフォルダー。</span><span class="sxs-lookup"><span data-stu-id="2cb27-109">A folder that contains the new value of the updated field, if the update is not a deletion.</span></span>
    
## <a name="remarks"></a><span data-ttu-id="2cb27-110">注釈</span><span class="sxs-lookup"><span data-stu-id="2cb27-110">Remarks</span></span>

<span data-ttu-id="2cb27-111">アイテムに対して3つの基本的な更新操作を実行できます。</span><span class="sxs-lookup"><span data-stu-id="2cb27-111">Three basic update actions can be performed on an item.</span></span> <span data-ttu-id="2cb27-112">これらのアクションを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="2cb27-112">These actions are listed in the following table.</span></span>
  
|<span data-ttu-id="2cb27-113">**操作**</span><span class="sxs-lookup"><span data-stu-id="2cb27-113">**Action**</span></span>|<span data-ttu-id="2cb27-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="2cb27-114">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2cb27-115">追加</span><span class="sxs-lookup"><span data-stu-id="2cb27-115">Append</span></span>  <br/> |<span data-ttu-id="2cb27-116">Append アクションは、既存のプロパティにデータを追加します。</span><span class="sxs-lookup"><span data-stu-id="2cb27-116">The append action adds data to an existing property.</span></span> <span data-ttu-id="2cb27-117">現在のデータは保持されます。</span><span class="sxs-lookup"><span data-stu-id="2cb27-117">It preserves the data that is currently there.</span></span> <span data-ttu-id="2cb27-118">追加はすべてのプロパティに適用されません。</span><span class="sxs-lookup"><span data-stu-id="2cb27-118">Append is not applicable to all properties.</span></span>  <br/> |
|<span data-ttu-id="2cb27-119">Set</span><span class="sxs-lookup"><span data-stu-id="2cb27-119">Set</span></span>  <br/> |<span data-ttu-id="2cb27-120">Set アクションは、データが含まれている場合はプロパティのデータを置き換えます。存在しない場合は、プロパティを作成して、その値を設定します。</span><span class="sxs-lookup"><span data-stu-id="2cb27-120">The set action replaces data for a property if it contains data, or creates the property and sets its value if it does not exist.</span></span> <span data-ttu-id="2cb27-121">Set アクションは、書き込み可能なプロパティにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="2cb27-121">The set action is only applicable to writable properties.</span></span>  <br/> |
|<span data-ttu-id="2cb27-122">削除</span><span class="sxs-lookup"><span data-stu-id="2cb27-122">Delete</span></span>  <br/> |<span data-ttu-id="2cb27-123">削除アクションは、フォルダーからプロパティを削除します。</span><span class="sxs-lookup"><span data-stu-id="2cb27-123">The delete action removes a property from a folder.</span></span> <span data-ttu-id="2cb27-124">これは、空の値に設定するのとは異なります。</span><span class="sxs-lookup"><span data-stu-id="2cb27-124">This is different than setting it to an empty value.</span></span> <span data-ttu-id="2cb27-125">完了すると、フォルダーのプロパティは存在しません。</span><span class="sxs-lookup"><span data-stu-id="2cb27-125">When complete, the property does not exist for the folder.</span></span> <span data-ttu-id="2cb27-126">Delete は、書き込み可能なプロパティにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="2cb27-126">Delete is only applicable to writable properties.</span></span>  <br/> |
   
## <a name="updatefolder-request-example"></a><span data-ttu-id="2cb27-127">UpdateFolder 要求の例</span><span class="sxs-lookup"><span data-stu-id="2cb27-127">UpdateFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="2cb27-128">Description</span><span class="sxs-lookup"><span data-stu-id="2cb27-128">Description</span></span>

<span data-ttu-id="2cb27-129">次の UpdateFolder 要求の例は、フォルダーの表示名を更新する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="2cb27-129">The following example of an UpdateFolder request shows how to update a folder display name.</span></span> 
  
### <a name="code"></a><span data-ttu-id="2cb27-130">コード</span><span class="sxs-lookup"><span data-stu-id="2cb27-130">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateFolder xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <FolderChanges>
        <t:FolderChange>
          <t:FolderId Id="AScA" ChangeKey="GO3u/"/>
          <t:Updates>
            <t:SetFolderField>
              <t:FieldURI FieldURI="folder:DisplayName"/>
              <t:Folder>
                <t:DisplayName>NewFolderName</t:DisplayName>
              </t:Folder>
            </t:SetFolderField>
          </t:Updates>
        </t:FolderChange>
      </FolderChanges>
    </UpdateFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="2cb27-131">コメント</span><span class="sxs-lookup"><span data-stu-id="2cb27-131">Comments</span></span>

<span data-ttu-id="2cb27-132">次の使用例は、フォルダーの表示名を NewFolderName に変更します。</span><span class="sxs-lookup"><span data-stu-id="2cb27-132">This example changes the display name of the folder to NewFolderName.</span></span>
  
> [!NOTE]
> <span data-ttu-id="2cb27-133">[FolderId](folderid.md)要素の**Id**および**changekey**属性の値は、読みやすくするために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="2cb27-133">The values of the **Id** and **ChangeKey** attributes of the [FolderId](folderid.md) element have been shortened for readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="2cb27-134">Request 要素</span><span class="sxs-lookup"><span data-stu-id="2cb27-134">Request elements</span></span>

<span data-ttu-id="2cb27-135">要求では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="2cb27-135">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="2cb27-136">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="2cb27-136">UpdateFolder</span></span>](updatefolder.md)
    
- [<span data-ttu-id="2cb27-137">FolderChanges 変更</span><span class="sxs-lookup"><span data-stu-id="2cb27-137">FolderChanges</span></span>](folderchanges.md)
    
- [<span data-ttu-id="2cb27-138">FolderChange</span><span class="sxs-lookup"><span data-stu-id="2cb27-138">FolderChange</span></span>](folderchange.md)
    
- [<span data-ttu-id="2cb27-139">FolderId</span><span class="sxs-lookup"><span data-stu-id="2cb27-139">FolderId</span></span>](folderid.md)
    
- [<span data-ttu-id="2cb27-140">Updates (フォルダー)</span><span class="sxs-lookup"><span data-stu-id="2cb27-140">Updates (Folder)</span></span>](updates-folder.md)
    
- [<span data-ttu-id="2cb27-141">SetFolderField</span><span class="sxs-lookup"><span data-stu-id="2cb27-141">SetFolderField</span></span>](setfolderfield.md)
    
- [<span data-ttu-id="2cb27-142">FieldURI</span><span class="sxs-lookup"><span data-stu-id="2cb27-142">FieldURI</span></span>](fielduri.md)
    
- [<span data-ttu-id="2cb27-143">Folder</span><span class="sxs-lookup"><span data-stu-id="2cb27-143">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="2cb27-144">DisplayName (文字列)</span><span class="sxs-lookup"><span data-stu-id="2cb27-144">DisplayName (string)</span></span>](displayname-string.md)
    
<span data-ttu-id="2cb27-145">UpdateFolder 要求の形成に使用できるその他の要素については、スキーマを参照してください。</span><span class="sxs-lookup"><span data-stu-id="2cb27-145">See the schema for additional elements that you can use to form an UpdateFolder request.</span></span>
  
> [!NOTE]
> <span data-ttu-id="2cb27-146">スキーマの既定の場所は、クライアントアクセスサーバーの役割がインストールされているコンピューター上の EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="2cb27-146">The default location of the schema is in the EWS virtual directory on the computer that has the Client Access server role installed.</span></span> 
  
## <a name="updatefolder-response-example"></a><span data-ttu-id="2cb27-147">UpdateFolder 応答の例</span><span class="sxs-lookup"><span data-stu-id="2cb27-147">UpdateFolder response example</span></span>

### <a name="description"></a><span data-ttu-id="2cb27-148">Description</span><span class="sxs-lookup"><span data-stu-id="2cb27-148">Description</span></span>

<span data-ttu-id="2cb27-149">次の例は、UpdateFolder 要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="2cb27-149">The following example shows a successful response to the UpdateFolder request.</span></span> <span data-ttu-id="2cb27-150">この例では、フォルダーの更新された状態を反映するために新しい変更キーが返されます。</span><span class="sxs-lookup"><span data-stu-id="2cb27-150">In this example, the new change key is returned to reflect the updated status of the folder.</span></span>
  
### <a name="code"></a><span data-ttu-id="2cb27-151">コード</span><span class="sxs-lookup"><span data-stu-id="2cb27-151">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <UpdateFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:UpdateFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="AAAlAFVz" ChangeKey="AQAAAB" />
            </t:Folder>
          </m:Folders>
        </m:UpdateFolderResponseMessage>
      </m:ResponseMessages>
    </UpdateFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="2cb27-152">コメント</span><span class="sxs-lookup"><span data-stu-id="2cb27-152">Comments</span></span>

> [!NOTE]
> <span data-ttu-id="2cb27-153">読みやすくするために、フォルダー ID と変更キーが短縮されています。</span><span class="sxs-lookup"><span data-stu-id="2cb27-153">The folder ID and the change key have been shortened to preserve readability.</span></span> 
  
<span data-ttu-id="2cb27-154">応答で返されるフォルダー ID は、更新されたフォルダーを表しています。</span><span class="sxs-lookup"><span data-stu-id="2cb27-154">The folder ID that is returned in the response represents the updated folder.</span></span>
  
### <a name="successful-response-elements"></a><span data-ttu-id="2cb27-155">成功した応答要素</span><span class="sxs-lookup"><span data-stu-id="2cb27-155">Successful response elements</span></span>

<span data-ttu-id="2cb27-156">応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="2cb27-156">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="2cb27-157">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="2cb27-157">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="2cb27-158">UpdateFolderResponse</span><span class="sxs-lookup"><span data-stu-id="2cb27-158">UpdateFolderResponse</span></span>](updatefolderresponse.md)
    
- [<span data-ttu-id="2cb27-159">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="2cb27-159">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="2cb27-160">UpdateFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="2cb27-160">UpdateFolderResponseMessage</span></span>](updatefolderresponsemessage.md)
    
- [<span data-ttu-id="2cb27-161">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="2cb27-161">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="2cb27-162">フォルダー</span><span class="sxs-lookup"><span data-stu-id="2cb27-162">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="2cb27-163">Folder</span><span class="sxs-lookup"><span data-stu-id="2cb27-163">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="2cb27-164">FolderId</span><span class="sxs-lookup"><span data-stu-id="2cb27-164">FolderId</span></span>](folderid.md)
    
## <a name="updatefolder-error-response-example"></a><span data-ttu-id="2cb27-165">UpdateFolder エラー応答の例</span><span class="sxs-lookup"><span data-stu-id="2cb27-165">UpdateFolder Error response example</span></span>

### <a name="description"></a><span data-ttu-id="2cb27-166">Description</span><span class="sxs-lookup"><span data-stu-id="2cb27-166">Description</span></span>

<span data-ttu-id="2cb27-167">次の例は、UpdateFolder 要求に対するエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="2cb27-167">The following example shows an error response to an UpdateFolder request.</span></span>
  
### <a name="code"></a><span data-ttu-id="2cb27-168">コード</span><span class="sxs-lookup"><span data-stu-id="2cb27-168">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <UpdateFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:UpdateFolderResponseMessage ResponseClass="Error">
          <m:MessageText>The change key is invalid.</m:MessageText>
          <m:ResponseCode>ErrorInvalidChangeKey</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Folders />
        </m:UpdateFolderResponseMessage>
      </m:ResponseMessages>
    </UpdateFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="2cb27-169">コメント</span><span class="sxs-lookup"><span data-stu-id="2cb27-169">Comments</span></span>

<span data-ttu-id="2cb27-170">この例では、要求内の無効な**Changekey**属性によって発生するエラー応答を示します。</span><span class="sxs-lookup"><span data-stu-id="2cb27-170">This example shows an error response that is caused by an invalid **ChangeKey** attribute in the request.</span></span> 
  
### <a name="error-response-elements"></a><span data-ttu-id="2cb27-171">エラー応答要素</span><span class="sxs-lookup"><span data-stu-id="2cb27-171">Error response elements</span></span>

<span data-ttu-id="2cb27-172">エラー応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="2cb27-172">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="2cb27-173">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="2cb27-173">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="2cb27-174">UpdateFolderResponse</span><span class="sxs-lookup"><span data-stu-id="2cb27-174">UpdateFolderResponse</span></span>](updatefolderresponse.md)
    
- [<span data-ttu-id="2cb27-175">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="2cb27-175">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="2cb27-176">UpdateFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="2cb27-176">UpdateFolderResponseMessage</span></span>](updatefolderresponsemessage.md)
    
- [<span data-ttu-id="2cb27-177">MessageText</span><span class="sxs-lookup"><span data-stu-id="2cb27-177">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="2cb27-178">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="2cb27-178">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="2cb27-179">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="2cb27-179">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="2cb27-180">フォルダー</span><span class="sxs-lookup"><span data-stu-id="2cb27-180">Folders</span></span>](folders-ex15websvcsotherref.md)
    
## <a name="see-also"></a><span data-ttu-id="2cb27-181">関連項目</span><span class="sxs-lookup"><span data-stu-id="2cb27-181">See also</span></span>



- [<span data-ttu-id="2cb27-182">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="2cb27-182">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

