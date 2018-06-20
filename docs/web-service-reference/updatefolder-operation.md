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
description: UpdateFolder 操作を使用して、Exchange ストア内の既存のアイテムのプロパティを変更します。 各 UpdateFolder 操作は、次ので構成されます。
ms.openlocfilehash: b33937bb09f0dcbe3d3ed61bbf5233423f320d9c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839836"
---
# <a name="updatefolder-operation"></a><span data-ttu-id="23530-104">UpdateFolder 操作</span><span class="sxs-lookup"><span data-stu-id="23530-104">UpdateFolder operation</span></span>

<span data-ttu-id="23530-105">UpdateFolder 操作を使用して、Exchange ストア内の既存のアイテムのプロパティを変更します。</span><span class="sxs-lookup"><span data-stu-id="23530-105">The UpdateFolder operation is used to modify properties of an existing item in the Exchange store.</span></span> <span data-ttu-id="23530-106">各 UpdateFolder 操作は、次ので構成されます。</span><span class="sxs-lookup"><span data-stu-id="23530-106">Each UpdateFolder operation consists of the following:</span></span>
  
- <span data-ttu-id="23530-107">[フォルダー Id](folderid.md)の要素で、更新するフォルダーを指定します。</span><span class="sxs-lookup"><span data-stu-id="23530-107">A [FolderId](folderid.md) element that specifies a folder to update.</span></span> 
    
- <span data-ttu-id="23530-108">更新するデータを指定するフォルダーの図形で指定したフォルダー内の要素の内部のパスです。</span><span class="sxs-lookup"><span data-stu-id="23530-108">An internal path of an element in the folder, as specified by the folder shape, which specifies the data to update.</span></span>
    
- <span data-ttu-id="23530-109">更新プログラムが削除できない場合、更新されたフィールドの新しい値を格納するフォルダーです。</span><span class="sxs-lookup"><span data-stu-id="23530-109">A folder that contains the new value of the updated field, if the update is not a deletion.</span></span>
    
## <a name="remarks"></a><span data-ttu-id="23530-110">備考</span><span class="sxs-lookup"><span data-stu-id="23530-110">Remarks</span></span>

<span data-ttu-id="23530-111">アイテムには、3 つの更新プログラムの基本的な操作を実行できます。</span><span class="sxs-lookup"><span data-stu-id="23530-111">Three basic update actions can be performed on an item.</span></span> <span data-ttu-id="23530-112">これらのアクションは、次の表に表示されます。</span><span class="sxs-lookup"><span data-stu-id="23530-112">These actions are listed in the following table.</span></span>
  
|<span data-ttu-id="23530-113">**アクション**</span><span class="sxs-lookup"><span data-stu-id="23530-113">**Action**</span></span>|<span data-ttu-id="23530-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="23530-114">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="23530-115">追加</span><span class="sxs-lookup"><span data-stu-id="23530-115">Append</span></span>  <br/> |<span data-ttu-id="23530-116">追加操作では、既存のプロパティにデータを追加します。</span><span class="sxs-lookup"><span data-stu-id="23530-116">The append action adds data to an existing property.</span></span> <span data-ttu-id="23530-117">そこにある現在のデータが保持されます。</span><span class="sxs-lookup"><span data-stu-id="23530-117">It preserves the data that is currently there.</span></span> <span data-ttu-id="23530-118">追加のすべてのプロパティには適用できません。</span><span class="sxs-lookup"><span data-stu-id="23530-118">Append is not applicable to all properties.</span></span>  <br/> |
|<span data-ttu-id="23530-119">設定</span><span class="sxs-lookup"><span data-stu-id="23530-119">Set</span></span>  <br/> |<span data-ttu-id="23530-120">設定のアクションでは、データが含まれていますまたはプロパティが作成され、存在しない場合、その値を設定する場合、プロパティのデータが置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="23530-120">The set action replaces data for a property if it contains data, or creates the property and sets its value if it does not exist.</span></span> <span data-ttu-id="23530-121">アクションのセットは、書き込み可能なプロパティに適用できるのみです。</span><span class="sxs-lookup"><span data-stu-id="23530-121">The set action is only applicable to writable properties.</span></span>  <br/> |
|<span data-ttu-id="23530-122">削除</span><span class="sxs-lookup"><span data-stu-id="23530-122">Delete</span></span>  <br/> |<span data-ttu-id="23530-123">削除操作では、フォルダーからプロパティを削除します。</span><span class="sxs-lookup"><span data-stu-id="23530-123">The delete action removes a property from a folder.</span></span> <span data-ttu-id="23530-124">これは、空の値を設定することとは異なります。</span><span class="sxs-lookup"><span data-stu-id="23530-124">This is different than setting it to an empty value.</span></span> <span data-ttu-id="23530-125">完了すると、フォルダーのプロパティが存在しません。</span><span class="sxs-lookup"><span data-stu-id="23530-125">When complete, the property does not exist for the folder.</span></span> <span data-ttu-id="23530-126">削除は、書き込み可能なプロパティに該当する場合のみです。</span><span class="sxs-lookup"><span data-stu-id="23530-126">Delete is only applicable to writable properties.</span></span>  <br/> |
   
## <a name="updatefolder-request-example"></a><span data-ttu-id="23530-127">UpdateFolder 要求の例</span><span class="sxs-lookup"><span data-stu-id="23530-127">UpdateFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="23530-128">説明</span><span class="sxs-lookup"><span data-stu-id="23530-128">Description</span></span>

<span data-ttu-id="23530-129">UpdateFolder 要求の次の使用例は、フォルダーの表示名を更新する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="23530-129">The following example of an UpdateFolder request shows how to update a folder display name.</span></span> 
  
### <a name="code"></a><span data-ttu-id="23530-130">コード</span><span class="sxs-lookup"><span data-stu-id="23530-130">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateFolder xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

### <a name="comments"></a><span data-ttu-id="23530-131">コメント</span><span class="sxs-lookup"><span data-stu-id="23530-131">Comments</span></span>

<span data-ttu-id="23530-132">NewFolderName] にフォルダーの表示名を変更します。</span><span class="sxs-lookup"><span data-stu-id="23530-132">This example changes the display name of the folder to NewFolderName.</span></span>
  
> [!NOTE]
> <span data-ttu-id="23530-133">[フォルダー Id](folderid.md)要素の属性を**変更キー**と**Id**の値は、読みやすさに短縮されています。</span><span class="sxs-lookup"><span data-stu-id="23530-133">The values of the **Id** and **ChangeKey** attributes of the [FolderId](folderid.md) element have been shortened for readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="23530-134">要素を要求します。</span><span class="sxs-lookup"><span data-stu-id="23530-134">Request elements</span></span>

<span data-ttu-id="23530-135">次の要素は、要求で使用されます。</span><span class="sxs-lookup"><span data-stu-id="23530-135">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="23530-136">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="23530-136">UpdateFolder</span></span>](updatefolder.md)
    
- [<span data-ttu-id="23530-137">FolderChanges</span><span class="sxs-lookup"><span data-stu-id="23530-137">FolderChanges</span></span>](folderchanges.md)
    
- [<span data-ttu-id="23530-138">FolderChange</span><span class="sxs-lookup"><span data-stu-id="23530-138">FolderChange</span></span>](folderchange.md)
    
- [<span data-ttu-id="23530-139">フォルダー Id</span><span class="sxs-lookup"><span data-stu-id="23530-139">FolderId</span></span>](folderid.md)
    
- [<span data-ttu-id="23530-140">更新 (アイテム)</span><span class="sxs-lookup"><span data-stu-id="23530-140">Updates (Item)</span></span>](updates-item.md)
    
- [<span data-ttu-id="23530-141">SetFolderField</span><span class="sxs-lookup"><span data-stu-id="23530-141">SetFolderField</span></span>](setfolderfield.md)
    
- [<span data-ttu-id="23530-142">FieldURI</span><span class="sxs-lookup"><span data-stu-id="23530-142">FieldURI</span></span>](fielduri.md)
    
- [<span data-ttu-id="23530-143">Folder</span><span class="sxs-lookup"><span data-stu-id="23530-143">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="23530-144">表示名 (文字列)</span><span class="sxs-lookup"><span data-stu-id="23530-144">DisplayName (string)</span></span>](displayname-string.md)
    
<span data-ttu-id="23530-145">UpdateFolder 要求を形成するために使用できるその他の要素のスキーマを参照してください。</span><span class="sxs-lookup"><span data-stu-id="23530-145">See the schema for additional elements that you can use to form an UpdateFolder request.</span></span>
  
> [!NOTE]
> <span data-ttu-id="23530-146">スキーマの既定の場所は、クライアント アクセス サーバーの役割がインストールされているコンピューターで EWS 仮想ディレクトリには。</span><span class="sxs-lookup"><span data-stu-id="23530-146">The default location of the schema is in the EWS virtual directory on the computer that has the Client Access server role installed.</span></span> 
  
## <a name="updatefolder-response-example"></a><span data-ttu-id="23530-147">UpdateFolder 応答の例</span><span class="sxs-lookup"><span data-stu-id="23530-147">UpdateFolder response example</span></span>

### <a name="description"></a><span data-ttu-id="23530-148">説明</span><span class="sxs-lookup"><span data-stu-id="23530-148">Description</span></span>

<span data-ttu-id="23530-149">UpdateFolder 要求に正常な応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="23530-149">The following example shows a successful response to the UpdateFolder request.</span></span> <span data-ttu-id="23530-150">この例では、フォルダーの更新されたステータスを反映するために新しいキーの変更が返されます。</span><span class="sxs-lookup"><span data-stu-id="23530-150">In this example, the new change key is returned to reflect the updated status of the folder.</span></span>
  
### <a name="code"></a><span data-ttu-id="23530-151">コード</span><span class="sxs-lookup"><span data-stu-id="23530-151">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <UpdateFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="23530-152">コメント</span><span class="sxs-lookup"><span data-stu-id="23530-152">Comments</span></span>

> [!NOTE]
> <span data-ttu-id="23530-153">フォルダー ID と変更キーは、読みやすさを保持するために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="23530-153">The folder ID and the change key have been shortened to preserve readability.</span></span> 
  
<span data-ttu-id="23530-154">応答で返されたフォルダー ID は、更新されたフォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="23530-154">The folder ID that is returned in the response represents the updated folder.</span></span>
  
### <a name="successful-response-elements"></a><span data-ttu-id="23530-155">正常な応答の要素</span><span class="sxs-lookup"><span data-stu-id="23530-155">Successful response elements</span></span>

<span data-ttu-id="23530-156">次の要素は、応答で使用されます。</span><span class="sxs-lookup"><span data-stu-id="23530-156">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="23530-157">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="23530-157">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="23530-158">UpdateFolderResponse</span><span class="sxs-lookup"><span data-stu-id="23530-158">UpdateFolderResponse</span></span>](updatefolderresponse.md)
    
- [<span data-ttu-id="23530-159">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="23530-159">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="23530-160">UpdateFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="23530-160">UpdateFolderResponseMessage</span></span>](updatefolderresponsemessage.md)
    
- [<span data-ttu-id="23530-161">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="23530-161">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="23530-162">フォルダー</span><span class="sxs-lookup"><span data-stu-id="23530-162">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="23530-163">Folder</span><span class="sxs-lookup"><span data-stu-id="23530-163">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="23530-164">フォルダー Id</span><span class="sxs-lookup"><span data-stu-id="23530-164">FolderId</span></span>](folderid.md)
    
## <a name="updatefolder-error-response-example"></a><span data-ttu-id="23530-165">UpdateFolder エラー応答の例</span><span class="sxs-lookup"><span data-stu-id="23530-165">UpdateFolder Error response example</span></span>

### <a name="description"></a><span data-ttu-id="23530-166">説明</span><span class="sxs-lookup"><span data-stu-id="23530-166">Description</span></span>

<span data-ttu-id="23530-167">UpdateFolder 要求に対するエラー応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="23530-167">The following example shows an error response to an UpdateFolder request.</span></span>
  
### <a name="code"></a><span data-ttu-id="23530-168">コード</span><span class="sxs-lookup"><span data-stu-id="23530-168">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <UpdateFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="23530-169">コメント</span><span class="sxs-lookup"><span data-stu-id="23530-169">Comments</span></span>

<span data-ttu-id="23530-170">この例では、要求に無効な**変更キー**属性が原因で発生するエラー応答を使用します。</span><span class="sxs-lookup"><span data-stu-id="23530-170">This example shows an error response that is caused by an invalid **ChangeKey** attribute in the request.</span></span> 
  
### <a name="error-response-elements"></a><span data-ttu-id="23530-171">エラー応答の要素</span><span class="sxs-lookup"><span data-stu-id="23530-171">Error response elements</span></span>

<span data-ttu-id="23530-172">エラー応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="23530-172">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="23530-173">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="23530-173">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="23530-174">UpdateFolderResponse</span><span class="sxs-lookup"><span data-stu-id="23530-174">UpdateFolderResponse</span></span>](updatefolderresponse.md)
    
- [<span data-ttu-id="23530-175">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="23530-175">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="23530-176">UpdateFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="23530-176">UpdateFolderResponseMessage</span></span>](updatefolderresponsemessage.md)
    
- [<span data-ttu-id="23530-177">MessageText</span><span class="sxs-lookup"><span data-stu-id="23530-177">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="23530-178">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="23530-178">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="23530-179">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="23530-179">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="23530-180">フォルダー</span><span class="sxs-lookup"><span data-stu-id="23530-180">Folders</span></span>](folders-ex15websvcsotherref.md)
    
## <a name="see-also"></a><span data-ttu-id="23530-181">関連項目</span><span class="sxs-lookup"><span data-stu-id="23530-181">See also</span></span>



- [<span data-ttu-id="23530-182">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="23530-182">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

