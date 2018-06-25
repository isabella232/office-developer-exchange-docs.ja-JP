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
description: FindFolder 操作は、Exchange Web サービスを使用して識別されたフォルダーのサブフォルダーを検索し、サブフォルダーの設定を記述するプロパティのセットを返します。
ms.openlocfilehash: 655455b46d4a3192b294bee9d85352d95ded49ae
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760502"
---
# <a name="findfolder-operation"></a><span data-ttu-id="ab036-103">FindFolder 操作</span><span class="sxs-lookup"><span data-stu-id="ab036-103">FindFolder operation</span></span>

<span data-ttu-id="ab036-104">**FindFolder**操作は、Exchange Web サービスを使用して識別されたフォルダーのサブフォルダーを検索し、サブフォルダーの設定を記述するプロパティのセットを返します。</span><span class="sxs-lookup"><span data-stu-id="ab036-104">The **FindFolder** operation uses Exchange Web Services to find subfolders of an identified folder and returns a set of properties that describe the set of subfolders.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="ab036-105">備考</span><span class="sxs-lookup"><span data-stu-id="ab036-105">Remarks</span></span>

<span data-ttu-id="ab036-106">FindFolder は、ストリーム再生可能なプロパティの最初の 512 バイトのみを返します。</span><span class="sxs-lookup"><span data-stu-id="ab036-106">FindFolder returns only the first 512 bytes of any streamable property.</span></span> <span data-ttu-id="ab036-107">Unicode では、null で終わる Unicode 文字列を使用して、最初の 255 文字を返します。</span><span class="sxs-lookup"><span data-stu-id="ab036-107">For Unicode, it returns the first 255 characters by using a null-terminated Unicode string.</span></span>
  
<span data-ttu-id="ab036-108">パブリック フォルダーの深い階層にわたるクエリを実行できません。</span><span class="sxs-lookup"><span data-stu-id="ab036-108">Deep traversal queries cannot be performed on public folders.</span></span>
  
<span data-ttu-id="ab036-109">制限は、許可およびのみ、フォルダーのプロパティ、項目のプロパティではなくを使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ab036-109">Restrictions are permitted and should use only the folder properties, not the item properties.</span></span> <span data-ttu-id="ab036-110">並べ替え機能では、 **FindFolder**応答を使用できません。</span><span class="sxs-lookup"><span data-stu-id="ab036-110">Sorting functionality is not available for **FindFolder** responses.</span></span> <span data-ttu-id="ab036-111">**FindFolder**クエリのクエリをグループ化することはできません。</span><span class="sxs-lookup"><span data-stu-id="ab036-111">Grouped queries are not available for **FindFolder** queries.</span></span> 
  
 <span data-ttu-id="ab036-112">**メモ****FindFolder**操作は、管理対象のフォルダーを検索するのにも使用されます。</span><span class="sxs-lookup"><span data-stu-id="ab036-112">**Note** The **FindFolder** operation is also used to find managed folders.</span></span> 
  
### <a name="soap-headers"></a><span data-ttu-id="ab036-113">SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ab036-113">SOAP Headers</span></span>

<span data-ttu-id="ab036-114">**FindFolder**操作が一覧表示され、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="ab036-114">The **FindFolder** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="ab036-115">**Header**</span><span class="sxs-lookup"><span data-stu-id="ab036-115">**Header**</span></span>|<span data-ttu-id="ab036-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="ab036-116">**Element**</span></span>|<span data-ttu-id="ab036-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="ab036-117">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="ab036-118">偽装</span><span class="sxs-lookup"><span data-stu-id="ab036-118">Impersonation</span></span>  <br/> |[<span data-ttu-id="ab036-119">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="ab036-119">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="ab036-120">クライアント アプリケーションが偽装するユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="ab036-120">Identifies the user whom the client application is impersonating.</span></span>  <br/> |
|<span data-ttu-id="ab036-121">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="ab036-121">MailboxCulture</span></span>  <br/> |[<span data-ttu-id="ab036-122">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="ab036-122">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="ab036-123">RFC3066 カルチャを使用してメールボックスへのアクセスを識別します。</span><span class="sxs-lookup"><span data-stu-id="ab036-123">Identifies the RFC3066 culture to be used to access the mailbox.</span></span>  <br/> |
|<span data-ttu-id="ab036-124">RequestVersion</span><span class="sxs-lookup"><span data-stu-id="ab036-124">RequestVersion</span></span>  <br/> |[<span data-ttu-id="ab036-125">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="ab036-125">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="ab036-126">操作要求のスキーマのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="ab036-126">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="ab036-127">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="ab036-127">ServerVersion</span></span>  <br/> |[<span data-ttu-id="ab036-128">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="ab036-128">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="ab036-129">要求に応答するサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="ab036-129">Identifies the version of the server that responded to the request.</span></span>  <br/> |
|<span data-ttu-id="ab036-130">TimeZoneContext</span><span class="sxs-lookup"><span data-stu-id="ab036-130">TimeZoneContext</span></span>  <br/> |[<span data-ttu-id="ab036-131">TimeZoneContext</span><span class="sxs-lookup"><span data-stu-id="ab036-131">TimeZoneContext</span></span>](timezonecontext.md) <br/> |<span data-ttu-id="ab036-132">サーバーからのすべての応答に使用するタイム ゾーンを識別します。</span><span class="sxs-lookup"><span data-stu-id="ab036-132">Identifies the time zone to be used for all responses from the server.</span></span>  <br/> |
   
## <a name="findfolder-request-example"></a><span data-ttu-id="ab036-133">FindFolder 要求の例</span><span class="sxs-lookup"><span data-stu-id="ab036-133">FindFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="ab036-134">説明</span><span class="sxs-lookup"><span data-stu-id="ab036-134">Description</span></span>

<span data-ttu-id="ab036-135">**FindFolder**要求の次の例では、受信トレイ内にあるすべてのフォルダーを検索する要求を作成する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="ab036-135">The following example of a **FindFolder** request shows how to form a request to find all the folders located in an Inbox.</span></span> 
  
### <a name="code"></a><span data-ttu-id="ab036-136">コード</span><span class="sxs-lookup"><span data-stu-id="ab036-136">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindFolder Traversal="Shallow" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="ab036-137">コメント</span><span class="sxs-lookup"><span data-stu-id="ab036-137">Comments</span></span>

<span data-ttu-id="ab036-138">[BaseShape](baseshape.md)の既定値を使用して、応答は、フォルダー名、フォルダー ID では、サブフォルダー、フォルダー、および未読アイテム数内の子フォルダーの数の数を返します。</span><span class="sxs-lookup"><span data-stu-id="ab036-138">Using the Default value for the [BaseShape](baseshape.md), the response returns the folder name, the folder ID, the number of subfolders, the number of child folders found in the folder, and the count of unread items.</span></span>
  
### <a name="request-elements"></a><span data-ttu-id="ab036-139">要素を要求します。</span><span class="sxs-lookup"><span data-stu-id="ab036-139">Request elements</span></span>

<span data-ttu-id="ab036-140">**FindFolder**要求には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ab036-140">This **FindFolder** request includes the following elements:</span></span> 
  
- [<span data-ttu-id="ab036-141">FindFolder</span><span class="sxs-lookup"><span data-stu-id="ab036-141">FindFolder</span></span>](findfolder.md)
    
- [<span data-ttu-id="ab036-142">FolderShape</span><span class="sxs-lookup"><span data-stu-id="ab036-142">FolderShape</span></span>](foldershape.md)
    
- [<span data-ttu-id="ab036-143">BaseShape</span><span class="sxs-lookup"><span data-stu-id="ab036-143">BaseShape</span></span>](baseshape.md)
    
- [<span data-ttu-id="ab036-144">ParentFolderIds</span><span class="sxs-lookup"><span data-stu-id="ab036-144">ParentFolderIds</span></span>](parentfolderids.md)
    
- [<span data-ttu-id="ab036-145">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="ab036-145">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
 <span data-ttu-id="ab036-146">**FindFolder**要求の追加の要素は、スキーマを参照してください。</span><span class="sxs-lookup"><span data-stu-id="ab036-146">For additional **FindFolder** request elements, see the schema.</span></span> 
  
## <a name="findfolder-response-example"></a><span data-ttu-id="ab036-147">FindFolder 応答の例</span><span class="sxs-lookup"><span data-stu-id="ab036-147">FindFolder response example</span></span>

### <a name="description"></a><span data-ttu-id="ab036-148">説明</span><span class="sxs-lookup"><span data-stu-id="ab036-148">Description</span></span>

<span data-ttu-id="ab036-149">**FindFolder**要求に正常な応答を Simple Object Access Protocol (SOAP) 本文の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ab036-149">The following Simple Object Access Protocol (SOAP) body example shows a successful response to the **FindFolder** request.</span></span> <span data-ttu-id="ab036-150">応答には、 [BaseShape](baseshape.md)の既定値が使用されるときに返される要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ab036-150">The response contains the elements that are returned when the Default value for the [BaseShape](baseshape.md) is used.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="ab036-151">フォルダー ID と変更キーは、読みやすさを保持するために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="ab036-151">The folder ID and the change key have been shortened to preserve readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="ab036-152">コード</span><span class="sxs-lookup"><span data-stu-id="ab036-152">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="652" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="response-elements"></a><span data-ttu-id="ab036-153">応答の要素</span><span class="sxs-lookup"><span data-stu-id="ab036-153">Response elements</span></span>

<span data-ttu-id="ab036-154">応答で返されるプロパティは、使用される場合に、 [BaseShape](baseshape.md)と[AdditionalProperties](additionalproperties.md)によって決定されます。</span><span class="sxs-lookup"><span data-stu-id="ab036-154">The properties that are returned in the response are determined by the [BaseShape](baseshape.md) and the [AdditionalProperties](additionalproperties.md) if they are used.</span></span> <span data-ttu-id="ab036-155">**FindFolder**の正常な応答には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ab036-155">A successful **FindFolder** response includes the following elements:</span></span> 
  
- [<span data-ttu-id="ab036-156">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="ab036-156">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="ab036-157">FindFolderResponse</span><span class="sxs-lookup"><span data-stu-id="ab036-157">FindFolderResponse</span></span>](findfolderresponse.md)
    
- [<span data-ttu-id="ab036-158">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="ab036-158">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="ab036-159">FindFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ab036-159">FindFolderResponseMessage</span></span>](findfolderresponsemessage.md)
    
- [<span data-ttu-id="ab036-160">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="ab036-160">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="ab036-161">RootFolder (FindItemResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="ab036-161">RootFolder (FindItemResponseMessage)</span></span>](rootfolder-finditemresponsemessage.md)
    
- [<span data-ttu-id="ab036-162">フォルダー</span><span class="sxs-lookup"><span data-stu-id="ab036-162">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="ab036-163">Folder</span><span class="sxs-lookup"><span data-stu-id="ab036-163">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="ab036-164">フォルダー Id</span><span class="sxs-lookup"><span data-stu-id="ab036-164">FolderId</span></span>](folderid.md)
    
- [<span data-ttu-id="ab036-165">表示名 (文字列)</span><span class="sxs-lookup"><span data-stu-id="ab036-165">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="ab036-166">TotalCount</span><span class="sxs-lookup"><span data-stu-id="ab036-166">TotalCount</span></span>](totalcount.md)
    
- [<span data-ttu-id="ab036-167">ChildFolderCount</span><span class="sxs-lookup"><span data-stu-id="ab036-167">ChildFolderCount</span></span>](childfoldercount.md)
    
- [<span data-ttu-id="ab036-168">UnreadCount</span><span class="sxs-lookup"><span data-stu-id="ab036-168">UnreadCount</span></span>](unreadcount.md)
    
### <a name="comments"></a><span data-ttu-id="ab036-169">コメント</span><span class="sxs-lookup"><span data-stu-id="ab036-169">Comments</span></span>

 <span data-ttu-id="ab036-170">[TotalCount](totalcount.md)とパブリック フォルダーの検索の[UnreadCount](unreadcount.md)要素、 **FindFolder** **AllProperties**応答の形をした要求の応答は返されません。</span><span class="sxs-lookup"><span data-stu-id="ab036-170">**FindFolder** responses to a request with the **AllProperties** response shape will not return the [TotalCount](totalcount.md) and [UnreadCount](unreadcount.md) elements for public folder searches.</span></span> 
  
## <a name="findfolder-error-response-example"></a><span data-ttu-id="ab036-171">FindFolder エラー応答の例</span><span class="sxs-lookup"><span data-stu-id="ab036-171">FindFolder Error response example</span></span>

### <a name="description"></a><span data-ttu-id="ab036-172">説明</span><span class="sxs-lookup"><span data-stu-id="ab036-172">Description</span></span>

<span data-ttu-id="ab036-173">不正なフォルダー id で識別されているフォルダーを検索するときに発生するエラー応答を SOAP 本文の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ab036-173">The following SOAP body example shows an error response that occurs when you search for a folder that is identified by a malformed folder identifier.</span></span>
  
### <a name="code"></a><span data-ttu-id="ab036-174">コード</span><span class="sxs-lookup"><span data-stu-id="ab036-174">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
                 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                 xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="652" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="error-response-elements"></a><span data-ttu-id="ab036-175">エラー応答の要素</span><span class="sxs-lookup"><span data-stu-id="ab036-175">Error response elements</span></span>

<span data-ttu-id="ab036-176">**FindFolder**エラー応答には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ab036-176">The **FindFolder** error response includes the following elements:</span></span> 
  
- [<span data-ttu-id="ab036-177">FindFolderResponse</span><span class="sxs-lookup"><span data-stu-id="ab036-177">FindFolderResponse</span></span>](findfolderresponse.md)
    
- [<span data-ttu-id="ab036-178">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="ab036-178">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="ab036-179">MessageText</span><span class="sxs-lookup"><span data-stu-id="ab036-179">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="ab036-180">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="ab036-180">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="ab036-181">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="ab036-181">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="additional-information"></a><span data-ttu-id="ab036-182">その他の情報</span><span class="sxs-lookup"><span data-stu-id="ab036-182">Additional Information</span></span>

- <span data-ttu-id="ab036-183">フォルダーの[表示名 (文字列)](displayname-string.md)の要素は常に既定の図形に含まれます。</span><span class="sxs-lookup"><span data-stu-id="ab036-183">The folder [DisplayName (string)](displayname-string.md) element is always included in the default shape.</span></span> 
    
- <span data-ttu-id="ab036-184">仕事リストとメモのフォルダーの[UnreadCount](unreadcount.md)要素が含まれます。</span><span class="sxs-lookup"><span data-stu-id="ab036-184">The [UnreadCount](unreadcount.md) element is included in Tasks and Notes folders.</span></span> 
    
- <span data-ttu-id="ab036-185">[ExtendedFieldURI](extendedfielduri.md)要素を使用して管理対象のフォルダーを識別するのに**整数**のプロパティの種類と 0x672D の**PropertyTag**値を使用します。</span><span class="sxs-lookup"><span data-stu-id="ab036-185">Use the **PropertyTag** value of 0x672D with a property type of **Integer** to identify a managed folder by using the [ExtendedFieldURI](extendedfielduri.md) element.</span></span> 
    
## <a name="see-also"></a><span data-ttu-id="ab036-186">関連項目</span><span class="sxs-lookup"><span data-stu-id="ab036-186">See also</span></span>



[<span data-ttu-id="ab036-187">フォルダーを検索します。</span><span class="sxs-lookup"><span data-stu-id="ab036-187">Finding Folders</span></span>](http://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)

