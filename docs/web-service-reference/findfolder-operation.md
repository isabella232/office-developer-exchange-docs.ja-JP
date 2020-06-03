---
title: FindFolder 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindFolder
api_type:
- schema
ms.assetid: 7a9855aa-06cc-45ba-ad2a-645c15b7d031
description: FindFolder 操作は、Exchange Web サービスを使用して、識別されたフォルダーのサブフォルダーを検索し、一連のサブフォルダーを記述する一連のプロパティを返します。
ms.openlocfilehash: f1cc199bdaf684d8d74687ed7f064eb66fee48ff
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462585"
---
# <a name="findfolder-operation"></a><span data-ttu-id="a53ff-103">FindFolder 操作</span><span class="sxs-lookup"><span data-stu-id="a53ff-103">FindFolder operation</span></span>

<span data-ttu-id="a53ff-104">**Findfolder**操作は、Exchange Web サービスを使用して、識別されたフォルダーのサブフォルダーを検索し、一連のサブフォルダーを記述する一連のプロパティを返します。</span><span class="sxs-lookup"><span data-stu-id="a53ff-104">The **FindFolder** operation uses Exchange Web Services to find subfolders of an identified folder and returns a set of properties that describe the set of subfolders.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="a53ff-105">注釈</span><span class="sxs-lookup"><span data-stu-id="a53ff-105">Remarks</span></span>

<span data-ttu-id="a53ff-106">FindFolder は、任意のストリーミング可能なプロパティの最初の 512 バイトだけを返します。</span><span class="sxs-lookup"><span data-stu-id="a53ff-106">FindFolder returns only the first 512 bytes of any streamable property.</span></span> <span data-ttu-id="a53ff-107">Unicode の場合は、Null 終了の Unicode 文字列を使用して最初の 255 文字を返します。</span><span class="sxs-lookup"><span data-stu-id="a53ff-107">For Unicode, it returns the first 255 characters by using a null-terminated Unicode string.</span></span>
  
<span data-ttu-id="a53ff-108">ディープトラバースクエリは、パブリックフォルダーでは実行できません。</span><span class="sxs-lookup"><span data-stu-id="a53ff-108">Deep traversal queries cannot be performed on public folders.</span></span>
  
<span data-ttu-id="a53ff-109">制限は許可され、アイテムのプロパティではなく、フォルダーのプロパティのみを使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a53ff-109">Restrictions are permitted and should use only the folder properties, not the item properties.</span></span> <span data-ttu-id="a53ff-110">**Findfolder**応答では、並べ替え機能を使用できません。</span><span class="sxs-lookup"><span data-stu-id="a53ff-110">Sorting functionality is not available for **FindFolder** responses.</span></span> <span data-ttu-id="a53ff-111">グループ化されたクエリは、 **Findfolder**クエリでは使用できません。</span><span class="sxs-lookup"><span data-stu-id="a53ff-111">Grouped queries are not available for **FindFolder** queries.</span></span> 
  
 <span data-ttu-id="a53ff-112">**メモ\*\*\*\*Findfolder**操作は、管理フォルダーを検索するためにも使用されます。</span><span class="sxs-lookup"><span data-stu-id="a53ff-112">**Note** The **FindFolder** operation is also used to find managed folders.</span></span> 
  
### <a name="soap-headers"></a><span data-ttu-id="a53ff-113">SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a53ff-113">SOAP Headers</span></span>

<span data-ttu-id="a53ff-114">**Findfolder**操作では、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="a53ff-114">The **FindFolder** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="a53ff-115">**Header**</span><span class="sxs-lookup"><span data-stu-id="a53ff-115">**Header**</span></span>|<span data-ttu-id="a53ff-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="a53ff-116">**Element**</span></span>|<span data-ttu-id="a53ff-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="a53ff-117">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="a53ff-118">偽装</span><span class="sxs-lookup"><span data-stu-id="a53ff-118">Impersonation</span></span>  <br/> |[<span data-ttu-id="a53ff-119">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="a53ff-119">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="a53ff-120">クライアントアプリケーションが偽装しているユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="a53ff-120">Identifies the user whom the client application is impersonating.</span></span>  <br/> |
|<span data-ttu-id="a53ff-121">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="a53ff-121">MailboxCulture</span></span>  <br/> |[<span data-ttu-id="a53ff-122">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="a53ff-122">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="a53ff-123">メールボックスへのアクセスに使用する RFC3066 カルチャを指定します。</span><span class="sxs-lookup"><span data-stu-id="a53ff-123">Identifies the RFC3066 culture to be used to access the mailbox.</span></span>  <br/> |
|<span data-ttu-id="a53ff-124">RequestVersion</span><span class="sxs-lookup"><span data-stu-id="a53ff-124">RequestVersion</span></span>  <br/> |[<span data-ttu-id="a53ff-125">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="a53ff-125">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="a53ff-126">操作要求のスキーマバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="a53ff-126">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="a53ff-127">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="a53ff-127">ServerVersion</span></span>  <br/> |[<span data-ttu-id="a53ff-128">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="a53ff-128">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="a53ff-129">要求に応答したサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="a53ff-129">Identifies the version of the server that responded to the request.</span></span>  <br/> |
|<span data-ttu-id="a53ff-130">TimeZoneContext</span><span class="sxs-lookup"><span data-stu-id="a53ff-130">TimeZoneContext</span></span>  <br/> |[<span data-ttu-id="a53ff-131">TimeZoneContext</span><span class="sxs-lookup"><span data-stu-id="a53ff-131">TimeZoneContext</span></span>](timezonecontext.md) <br/> |<span data-ttu-id="a53ff-132">サーバーからのすべての応答に使用するタイムゾーンを指定します。</span><span class="sxs-lookup"><span data-stu-id="a53ff-132">Identifies the time zone to be used for all responses from the server.</span></span>  <br/> |
   
## <a name="findfolder-request-example"></a><span data-ttu-id="a53ff-133">FindFolder 要求の例</span><span class="sxs-lookup"><span data-stu-id="a53ff-133">FindFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="a53ff-134">Description</span><span class="sxs-lookup"><span data-stu-id="a53ff-134">Description</span></span>

<span data-ttu-id="a53ff-135">**Findfolder**要求の次の例は、受信トレイ内のすべてのフォルダーを検索するための要求を形成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="a53ff-135">The following example of a **FindFolder** request shows how to form a request to find all the folders located in an Inbox.</span></span> 
  
### <a name="code"></a><span data-ttu-id="a53ff-136">コード</span><span class="sxs-lookup"><span data-stu-id="a53ff-136">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindFolder Traversal="Shallow" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <FolderShape>
        <t:BaseShape>Default</t:BaseShape>
      </FolderShape>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox"/>
      </ParentFolderIds>
    </FindFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="a53ff-137">コメント</span><span class="sxs-lookup"><span data-stu-id="a53ff-137">Comments</span></span>

<span data-ttu-id="a53ff-138">[Baseshape](baseshape.md)の既定値を使用すると、応答はフォルダー名、フォルダー ID、サブフォルダー数、フォルダー内で見つかった子フォルダーの数、未読アイテムの数を返します。</span><span class="sxs-lookup"><span data-stu-id="a53ff-138">Using the Default value for the [BaseShape](baseshape.md), the response returns the folder name, the folder ID, the number of subfolders, the number of child folders found in the folder, and the count of unread items.</span></span>
  
### <a name="request-elements"></a><span data-ttu-id="a53ff-139">Request 要素</span><span class="sxs-lookup"><span data-stu-id="a53ff-139">Request elements</span></span>

<span data-ttu-id="a53ff-140">この**Findfolder**要求には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a53ff-140">This **FindFolder** request includes the following elements:</span></span> 
  
- [<span data-ttu-id="a53ff-141">FindFolder</span><span class="sxs-lookup"><span data-stu-id="a53ff-141">FindFolder</span></span>](findfolder.md)
    
- [<span data-ttu-id="a53ff-142">FolderShape</span><span class="sxs-lookup"><span data-stu-id="a53ff-142">FolderShape</span></span>](foldershape.md)
    
- [<span data-ttu-id="a53ff-143">BaseShape</span><span class="sxs-lookup"><span data-stu-id="a53ff-143">BaseShape</span></span>](baseshape.md)
    
- [<span data-ttu-id="a53ff-144">ParentFolderIds</span><span class="sxs-lookup"><span data-stu-id="a53ff-144">ParentFolderIds</span></span>](parentfolderids.md)
    
- [<span data-ttu-id="a53ff-145">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="a53ff-145">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
 <span data-ttu-id="a53ff-146">**Findfolder**要求の追加要素については、スキーマを参照してください。</span><span class="sxs-lookup"><span data-stu-id="a53ff-146">For additional **FindFolder** request elements, see the schema.</span></span> 
  
## <a name="findfolder-response-example"></a><span data-ttu-id="a53ff-147">FindFolder 応答の例</span><span class="sxs-lookup"><span data-stu-id="a53ff-147">FindFolder response example</span></span>

### <a name="description"></a><span data-ttu-id="a53ff-148">Description</span><span class="sxs-lookup"><span data-stu-id="a53ff-148">Description</span></span>

<span data-ttu-id="a53ff-149">次の簡易オブジェクトアクセスプロトコル (SOAP) 本文の例は、 **Findfolder**要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="a53ff-149">The following Simple Object Access Protocol (SOAP) body example shows a successful response to the **FindFolder** request.</span></span> <span data-ttu-id="a53ff-150">応答には、 [Baseshape](baseshape.md)の既定値が使用されたときに返される要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a53ff-150">The response contains the elements that are returned when the Default value for the [BaseShape](baseshape.md) is used.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="a53ff-151">読みやすくするために、フォルダー ID と変更キーが短縮されています。</span><span class="sxs-lookup"><span data-stu-id="a53ff-151">The folder ID and the change key have been shortened to preserve readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="a53ff-152">コード</span><span class="sxs-lookup"><span data-stu-id="a53ff-152">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="652" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:FindFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder TotalItemsInView="1" IncludesLastItemInRange="true">
            <t:Folders>
              <t:Folder>
                <t:FolderId Id="AQAnAH" ChangeKey="AQAAABY" />
                <t:DisplayName>TestFolder</t:DisplayName>
                <t:TotalCount>0</t:TotalCount>
                <t:ChildFolderCount>0</t:ChildFolderCount>
                <t:UnreadCount>0</t:UnreadCount>
              </t:Folder>
            </t:Folders>
          </m:RootFolder>
        </m:FindFolderResponseMessage>
      </m:ResponseMessages>
    </FindFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="response-elements"></a><span data-ttu-id="a53ff-153">Response 要素</span><span class="sxs-lookup"><span data-stu-id="a53ff-153">Response elements</span></span>

<span data-ttu-id="a53ff-154">応答で返されるプロパティは、使用されている場合は[Baseshape](baseshape.md)および[additionalproperties](additionalproperties.md)によって決まります。</span><span class="sxs-lookup"><span data-stu-id="a53ff-154">The properties that are returned in the response are determined by the [BaseShape](baseshape.md) and the [AdditionalProperties](additionalproperties.md) if they are used.</span></span> <span data-ttu-id="a53ff-155">正常な**Findfolder**応答には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a53ff-155">A successful **FindFolder** response includes the following elements:</span></span> 
  
- [<span data-ttu-id="a53ff-156">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="a53ff-156">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="a53ff-157">FindFolderResponse</span><span class="sxs-lookup"><span data-stu-id="a53ff-157">FindFolderResponse</span></span>](findfolderresponse.md)
    
- [<span data-ttu-id="a53ff-158">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="a53ff-158">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="a53ff-159">FindFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="a53ff-159">FindFolderResponseMessage</span></span>](findfolderresponsemessage.md)
    
- [<span data-ttu-id="a53ff-160">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="a53ff-160">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="a53ff-161">RootFolder (FindItemResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="a53ff-161">RootFolder (FindItemResponseMessage)</span></span>](rootfolder-finditemresponsemessage.md)
    
- [<span data-ttu-id="a53ff-162">フォルダー</span><span class="sxs-lookup"><span data-stu-id="a53ff-162">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="a53ff-163">Folder</span><span class="sxs-lookup"><span data-stu-id="a53ff-163">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="a53ff-164">FolderId</span><span class="sxs-lookup"><span data-stu-id="a53ff-164">FolderId</span></span>](folderid.md)
    
- [<span data-ttu-id="a53ff-165">DisplayName (文字列)</span><span class="sxs-lookup"><span data-stu-id="a53ff-165">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="a53ff-166">TotalCount</span><span class="sxs-lookup"><span data-stu-id="a53ff-166">TotalCount</span></span>](totalcount.md)
    
- [<span data-ttu-id="a53ff-167">ChildFolderCount</span><span class="sxs-lookup"><span data-stu-id="a53ff-167">ChildFolderCount</span></span>](childfoldercount.md)
    
- [<span data-ttu-id="a53ff-168">UnreadCount</span><span class="sxs-lookup"><span data-stu-id="a53ff-168">UnreadCount</span></span>](unreadcount.md)
    
### <a name="comments"></a><span data-ttu-id="a53ff-169">コメント</span><span class="sxs-lookup"><span data-stu-id="a53ff-169">Comments</span></span>

 <span data-ttu-id="a53ff-170">**Allproperties**応答図形を使用した要求に対する**findfolder**応答では、パブリックフォルダー検索の[totalcount](totalcount.md)要素と[UnreadCount](unreadcount.md)要素は返されません。</span><span class="sxs-lookup"><span data-stu-id="a53ff-170">**FindFolder** responses to a request with the **AllProperties** response shape will not return the [TotalCount](totalcount.md) and [UnreadCount](unreadcount.md) elements for public folder searches.</span></span> 
  
## <a name="findfolder-error-response-example"></a><span data-ttu-id="a53ff-171">FindFolder エラー応答の例</span><span class="sxs-lookup"><span data-stu-id="a53ff-171">FindFolder Error response example</span></span>

### <a name="description"></a><span data-ttu-id="a53ff-172">Description</span><span class="sxs-lookup"><span data-stu-id="a53ff-172">Description</span></span>

<span data-ttu-id="a53ff-173">次の SOAP 本文の例は、無効なフォルダーの識別子によって識別されるフォルダーを検索すると発生するエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="a53ff-173">The following SOAP body example shows an error response that occurs when you search for a folder that is identified by a malformed folder identifier.</span></span>
  
### <a name="code"></a><span data-ttu-id="a53ff-174">コード</span><span class="sxs-lookup"><span data-stu-id="a53ff-174">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
                 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                 xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="652" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:FindFolderResponseMessage ResponseClass="Error">
          <m:MessageText>Id is malformed.</m:MessageText>
          <m:ResponseCode>ErrorInvalidIdMalformed</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:FindFolderResponseMessage>
      </m:ResponseMessages>
    </FindFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="a53ff-175">エラー応答要素</span><span class="sxs-lookup"><span data-stu-id="a53ff-175">Error response elements</span></span>

<span data-ttu-id="a53ff-176">**Findfolder**エラー応答には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a53ff-176">The **FindFolder** error response includes the following elements:</span></span> 
  
- [<span data-ttu-id="a53ff-177">FindFolderResponse</span><span class="sxs-lookup"><span data-stu-id="a53ff-177">FindFolderResponse</span></span>](findfolderresponse.md)
    
- [<span data-ttu-id="a53ff-178">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="a53ff-178">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="a53ff-179">MessageText</span><span class="sxs-lookup"><span data-stu-id="a53ff-179">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="a53ff-180">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="a53ff-180">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="a53ff-181">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="a53ff-181">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="additional-information"></a><span data-ttu-id="a53ff-182">追加情報</span><span class="sxs-lookup"><span data-stu-id="a53ff-182">Additional Information</span></span>

- <span data-ttu-id="a53ff-183">Folder [DisplayName (string)](displayname-string.md)要素は、常に既定の図形に含まれています。</span><span class="sxs-lookup"><span data-stu-id="a53ff-183">The folder [DisplayName (string)](displayname-string.md) element is always included in the default shape.</span></span> 
    
- <span data-ttu-id="a53ff-184">[UnreadCount](unreadcount.md)要素は、タスクフォルダーとメモフォルダーに含まれています。</span><span class="sxs-lookup"><span data-stu-id="a53ff-184">The [UnreadCount](unreadcount.md) element is included in Tasks and Notes folders.</span></span> 
    
- <span data-ttu-id="a53ff-185">[ExtendedFieldURI](extendedfielduri.md)要素を使用して、管理フォルダーを識別するには、プロパティの種類が**Integer**の**Propertytag**の値0x672d を使用します。</span><span class="sxs-lookup"><span data-stu-id="a53ff-185">Use the **PropertyTag** value of 0x672D with a property type of **Integer** to identify a managed folder by using the [ExtendedFieldURI](extendedfielduri.md) element.</span></span> 
    
## <a name="see-also"></a><span data-ttu-id="a53ff-186">関連項目</span><span class="sxs-lookup"><span data-stu-id="a53ff-186">See also</span></span>



[<span data-ttu-id="a53ff-187">フォルダーの検索</span><span class="sxs-lookup"><span data-stu-id="a53ff-187">Finding Folders</span></span>](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)

