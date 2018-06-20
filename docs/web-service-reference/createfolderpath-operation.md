---
title: CreateFolderPath 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5a10aa5e-3f25-4ec3-a0b9-284c30918a1f
description: 操作 CreateFolderPath EWS についての情報を検索します。
ms.openlocfilehash: 22561e5086c144e25d7e04b68ec6674b87c4718d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759819"
---
# <a name="createfolderpath-operation"></a><span data-ttu-id="5770d-103">CreateFolderPath 操作</span><span class="sxs-lookup"><span data-stu-id="5770d-103">CreateFolderPath operation</span></span>

<span data-ttu-id="5770d-104">**CreateFolderPath** EWS の操作に関する情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="5770d-104">Find information about the **CreateFolderPath** EWS operation.</span></span> 
  
<span data-ttu-id="5770d-105">**CreateFolderPath**操作は、フォルダー階層を作成します。</span><span class="sxs-lookup"><span data-stu-id="5770d-105">The **CreateFolderPath** operation creates a folder hierarchy.</span></span> 
  
<span data-ttu-id="5770d-106">この操作は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="5770d-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-createfolderpath-operation"></a><span data-ttu-id="5770d-107">CreateFolderPath 操作を使用します。</span><span class="sxs-lookup"><span data-stu-id="5770d-107">Using the CreateFolderPath operation</span></span>

<span data-ttu-id="5770d-108">**CreateFolderPath**操作の要求は、フォルダーおよび親フォルダーの識別子の配列を受け取るし、配列内のフォルダーの順序に基づいて、フォルダー階層を作成します。</span><span class="sxs-lookup"><span data-stu-id="5770d-108">The **CreateFolderPath** operation request takes an array of folders and a parent folder identifier and creates a folder hierarchy based on the order of the folders in the array.</span></span> 
  
### <a name="createfolderpath-operation-soap-headers"></a><span data-ttu-id="5770d-109">CreateFolderPath 操作の SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5770d-109">CreateFolderPath operation SOAP headers</span></span>

<span data-ttu-id="5770d-110">**CreateFolderPath**操作は、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="5770d-110">The **CreateFolderPath** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="5770d-111">**ヘッダー名**</span><span class="sxs-lookup"><span data-stu-id="5770d-111">**Header name**</span></span>|<span data-ttu-id="5770d-112">**要素**</span><span class="sxs-lookup"><span data-stu-id="5770d-112">**Element**</span></span>|<span data-ttu-id="5770d-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="5770d-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="5770d-114">**偽装**</span><span class="sxs-lookup"><span data-stu-id="5770d-114">**Impersonation**</span></span> <br/> |[<span data-ttu-id="5770d-115">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="5770d-115">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="5770d-116">クライアント アプリケーションが偽装するユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="5770d-116">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="5770d-117">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="5770d-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="5770d-118">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="5770d-118">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="5770d-119">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="5770d-119">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="5770d-120">RFC 3066、」タグの「識別の言語」を使用してメールボックスへのアクセスに定義されているカルチャを識別します。</span><span class="sxs-lookup"><span data-stu-id="5770d-120">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="5770d-121">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="5770d-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="5770d-122">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="5770d-122">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="5770d-123">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="5770d-123">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="5770d-124">操作要求のスキーマのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="5770d-124">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="5770d-125">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="5770d-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="5770d-126">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="5770d-126">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="5770d-127">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="5770d-127">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="5770d-128">要求に応答するサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="5770d-128">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="5770d-129">このヘッダーは、応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="5770d-129">This header is applicable to a response.</span></span>  <br/> |
|<span data-ttu-id="5770d-130">**TimeZoneContext**</span><span class="sxs-lookup"><span data-stu-id="5770d-130">**TimeZoneContext**</span></span> <br/> |[<span data-ttu-id="5770d-131">TimeZoneContext</span><span class="sxs-lookup"><span data-stu-id="5770d-131">TimeZoneContext</span></span>](timezonecontext.md) <br/> |<span data-ttu-id="5770d-132">**日付**プロパティのタイム ゾーンの範囲を識別します。</span><span class="sxs-lookup"><span data-stu-id="5770d-132">Identifies the time zone scope for **DateTime** properties.</span></span> <span data-ttu-id="5770d-133">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="5770d-133">This header is applicable to a request.</span></span>  <br/> |
   
## <a name="createfolderpath-operation-request-example-create-a-folder-hierarchy"></a><span data-ttu-id="5770d-134">CreateFolderPath 操作の要求の例: フォルダーの階層を作成します。</span><span class="sxs-lookup"><span data-stu-id="5770d-134">CreateFolderPath operation request example: Create a folder hierarchy</span></span>

<span data-ttu-id="5770d-135">**CreateFolderPath**操作要求の次の使用例は、3 つのフォルダーは、フォルダー階層を作成する方法を示しています。 既定の受信トレイ フォルダーの深さです。</span><span class="sxs-lookup"><span data-stu-id="5770d-135">The following example of a **CreateFolderPath** operation request shows how to create a folder hierarchy that is three folders deep in the default Inbox folder.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="5770d-136">すべての項目の識別子と変更キーをこの資料では、読みやすさを保持するために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="5770d-136">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
      <t:MailboxCulture>en-US</t:MailboxCulture>
      <t:TimeZoneContext>
         <t:TimeZoneDefinition Id="GMT Standard Time"/>
      </t:TimeZoneContext>
   </soap:Header>
   <soap:Body >
      <m:CreateFolderPath>
         <m:ParentFolderId>
            <t:DistinguishedFolderId Id="inbox"/>
         </m:ParentFolderId>
         <m:RelativeFolderPath>
            <t:Folder>
               <t:DisplayName>MyFirstLevelFolder</t:DisplayName>
            </t:Folder>
            <t:Folder>
               <t:DisplayName>MySecondLevelFolder</t:DisplayName>
            </t:Folder>
            <t:Folder>
               <t:DisplayName>MyThirdLevelFolder</t:DisplayName>
            </t:Folder>
         </m:RelativeFolderPath>
      </m:CreateFolderPath>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="5770d-137">要求 SOAP 本体にはには、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5770d-137">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="5770d-138">CreateFolderPath</span><span class="sxs-lookup"><span data-stu-id="5770d-138">CreateFolderPath</span></span>](createfolderpath.md)
    
- [<span data-ttu-id="5770d-139">ParentFolderId (TargetFolderIdType)</span><span class="sxs-lookup"><span data-stu-id="5770d-139">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md)
    
- [<span data-ttu-id="5770d-140">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="5770d-140">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="5770d-141">RelativeFolderPath</span><span class="sxs-lookup"><span data-stu-id="5770d-141">RelativeFolderPath</span></span>](relativefolderpath.md)
    
- [<span data-ttu-id="5770d-142">Folder</span><span class="sxs-lookup"><span data-stu-id="5770d-142">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="5770d-143">表示名 (文字列)</span><span class="sxs-lookup"><span data-stu-id="5770d-143">DisplayName (string)</span></span>](displayname-string.md)
    
## <a name="successful-createfolderpath-operation-response"></a><span data-ttu-id="5770d-144">CreateFolderPath 操作の成功の応答</span><span class="sxs-lookup"><span data-stu-id="5770d-144">Successful CreateFolderPath operation response</span></span>

<span data-ttu-id="5770d-145">次の使用例は、正常な 3 つの階層のフォルダーにフォルダーを作成する**CreateFolderPath**操作の要求に応答を示しています。 既定の受信トレイ フォルダーの深さです。</span><span class="sxs-lookup"><span data-stu-id="5770d-145">The following example shows a successful response to a **CreateFolderPath** operation request to create a folder hierarchy three folders deep in the default Inbox folder.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="526" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:CreateFolderPathResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:CreateFolderPathResponseMessage ResponseClass="Success">
               <m:ResponseCode>NoError</m:ResponseCode>
               <m:Folders>
                  <t:Folder>
                     <t:FolderId Id="AAMkADEzOTExYisXAAA=" ChangeKey="AQAAABYAABq6Wxb"/>
                     <t:DisplayName>MyFirstLevelFolder</t:DisplayName>
                     <t:TotalCount>0</t:TotalCount>
                     <t:ChildFolderCount>0</t:ChildFolderCount>
                     <t:UnreadCount>0</t:UnreadCount>
                  </t:Folder>
               </m:Folders>
            </m:CreateFolderPathResponseMessage>
            <m:CreateFolderPathResponseMessage ResponseClass="Success">
               <m:ResponseCode>NoError</m:ResponseCode>
               <m:Folders>
                  <t:Folder>
                     <t:FolderId Id="AAMkADEzOTExm4QrAABqxisYAAA=" ChangeKey="AQAAABYAAAm4QrAABq6Wxg"/>
                     <t:DisplayName>MySecondLevelFolder</t:DisplayName>
                     <t:TotalCount>0</t:TotalCount>
                     <t:ChildFolderCount>0</t:ChildFolderCount>
                     <t:UnreadCount>0</t:UnreadCount>
                  </t:Folder>
               </m:Folders>
            </m:CreateFolderPathResponseMessage>
            <m:CreateFolderPathResponseMessage ResponseClass="Success">
               <m:ResponseCode>NoError</m:ResponseCode>
               <m:Folders>
                  <t:Folder>
                     <t:FolderId Id="AAMkADEzOTAABqxisZAAA=" ChangeKey="AQAAABYAA6Wxl"/>
                     <t:DisplayName>MyThirdLevelFolder</t:DisplayName>
                     <t:TotalCount>0</t:TotalCount>
                     <t:ChildFolderCount>0</t:ChildFolderCount>
                     <t:UnreadCount>0</t:UnreadCount>
                  </t:Folder>
               </m:Folders>
            </m:CreateFolderPathResponseMessage>
         </m:ResponseMessages>
      </m:CreateFolderPathResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="5770d-146">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5770d-146">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="5770d-147">CreateFolderPathResponse</span><span class="sxs-lookup"><span data-stu-id="5770d-147">CreateFolderPathResponse</span></span>](createfolderpathresponse.md)
    
- [<span data-ttu-id="5770d-148">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="5770d-148">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="5770d-149">CreateFolderPathResponseMessage</span><span class="sxs-lookup"><span data-stu-id="5770d-149">CreateFolderPathResponseMessage</span></span>](createfolderpathresponsemessage.md)
    
- [<span data-ttu-id="5770d-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="5770d-150">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="5770d-151">フォルダー</span><span class="sxs-lookup"><span data-stu-id="5770d-151">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="5770d-152">Folder</span><span class="sxs-lookup"><span data-stu-id="5770d-152">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="5770d-153">フォルダー Id</span><span class="sxs-lookup"><span data-stu-id="5770d-153">FolderId</span></span>](folderid.md)
    
- [<span data-ttu-id="5770d-154">表示名 (文字列)</span><span class="sxs-lookup"><span data-stu-id="5770d-154">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="5770d-155">TotalCount</span><span class="sxs-lookup"><span data-stu-id="5770d-155">TotalCount</span></span>](totalcount.md)
    
- [<span data-ttu-id="5770d-156">ChildFolderCount</span><span class="sxs-lookup"><span data-stu-id="5770d-156">ChildFolderCount</span></span>](childfoldercount.md)
    
- [<span data-ttu-id="5770d-157">UnreadCount</span><span class="sxs-lookup"><span data-stu-id="5770d-157">UnreadCount</span></span>](unreadcount.md)
    
## <a name="createfolderpath-operation-error-response"></a><span data-ttu-id="5770d-158">CreateFolderPath 操作のエラー応答</span><span class="sxs-lookup"><span data-stu-id="5770d-158">CreateFolderPath operation error response</span></span>

<span data-ttu-id="5770d-159">**CreateFolderPath**操作の要求に対してエラー応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5770d-159">The following example shows an error response to a **CreateFolderPath** operation request.</span></span> <span data-ttu-id="5770d-160">これは、最初のうちに設定された表示名のプロパティの種類がない 2 つのフォルダーを作成する要求に応答します。</span><span class="sxs-lookup"><span data-stu-id="5770d-160">This is a response to a request to create two folders, the first of which does not have a display name property set.</span></span> <span data-ttu-id="5770d-161">せず、表示名のプロパティでは、階層内の最初のフォルダーを作成することはできませんし、階層内の親フォルダーが作成されなかったために、2 番目のフォルダーを作成できません。</span><span class="sxs-lookup"><span data-stu-id="5770d-161">The first folder in the hierarchy cannot be created without a display name property, and the second folder cannot be created because the parent folder in the hierarchy was not created.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="14" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:CreateFolderPathResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:CreateFolderPathResponseMessage ResponseClass="Error">
               <m:MessageText>The folder save operation failed due to invalid property values.</m:MessageText>
               <m:ResponseCode>ErrorFolderSavePropertyError</m:ResponseCode>
               <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
               <m:MessageXml>
                  <t:FieldURI FieldURI="folder:DisplayName"/>
               </m:MessageXml>
               <m:Folders/>
            </m:CreateFolderPathResponseMessage>
            <m:CreateFolderPathResponseMessage ResponseClass="Error">
               <m:MessageText>The specified parent folder could not be found.</m:MessageText>
               <m:ResponseCode>ErrorParentFolderNotFound</m:ResponseCode>
               <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
               <m:Folders/>
            </m:CreateFolderPathResponseMessage>
         </m:ResponseMessages>
      </m:CreateFolderPathResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="5770d-162">エラー応答 SOAP 本体にはには、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5770d-162">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="5770d-163">CreateFolderPathResponse</span><span class="sxs-lookup"><span data-stu-id="5770d-163">CreateFolderPathResponse</span></span>](createfolderpathresponse.md)
    
- [<span data-ttu-id="5770d-164">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="5770d-164">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="5770d-165">CreateFolderPathResponseMessage</span><span class="sxs-lookup"><span data-stu-id="5770d-165">CreateFolderPathResponseMessage</span></span>](createfolderpathresponsemessage.md)
    
- [<span data-ttu-id="5770d-166">MessageText</span><span class="sxs-lookup"><span data-stu-id="5770d-166">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="5770d-167">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="5770d-167">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="5770d-168">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="5770d-168">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="5770d-169">MessageXml</span><span class="sxs-lookup"><span data-stu-id="5770d-169">MessageXml</span></span>](messagexml.md)
    
- [<span data-ttu-id="5770d-170">FieldURI</span><span class="sxs-lookup"><span data-stu-id="5770d-170">FieldURI</span></span>](fielduri.md)
    
- [<span data-ttu-id="5770d-171">フォルダー</span><span class="sxs-lookup"><span data-stu-id="5770d-171">Folders</span></span>](folders-ex15websvcsotherref.md)
    
<span data-ttu-id="5770d-172">EWS を汎用的なこの操作に固有のエラー コードは、 [ResponseCode](responsecode.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5770d-172">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="5770d-173">関連項目</span><span class="sxs-lookup"><span data-stu-id="5770d-173">See also</span></span>

- [<span data-ttu-id="5770d-174">Exchange での EWS の操作</span><span class="sxs-lookup"><span data-stu-id="5770d-174">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- <span data-ttu-id="5770d-175">
  [FindFolder 操作](findfolder-operation.md)</span><span class="sxs-lookup"><span data-stu-id="5770d-175">[FindFolder operation](findfolder-operation.md)</span></span>
    

