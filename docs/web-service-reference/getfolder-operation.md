---
title: GetFolder の操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetFolder
api_type:
- schema
ms.assetid: 355bcf93-dc71-4493-b177-622afac5fdb9
description: GetFolder の操作は、Exchange ストアからフォルダーを取得します。
ms.openlocfilehash: 1d2806e4febb6059b8a866d585bc70f49befbdef
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760742"
---
# <a name="getfolder-operation"></a><span data-ttu-id="5522b-103">GetFolder の操作</span><span class="sxs-lookup"><span data-stu-id="5522b-103">GetFolder operation</span></span>

<span data-ttu-id="5522b-104">**GetFolder**の操作は、Exchange ストアからフォルダーを取得します。</span><span class="sxs-lookup"><span data-stu-id="5522b-104">The **GetFolder** operation gets folders from the Exchange store.</span></span> 
  
## <a name="getfolder-request-example"></a><span data-ttu-id="5522b-105">GetFolder 要求の例</span><span class="sxs-lookup"><span data-stu-id="5522b-105">GetFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="5522b-106">説明</span><span class="sxs-lookup"><span data-stu-id="5522b-106">Description</span></span>

<span data-ttu-id="5522b-107">**GetFolder**要求の次の例では、フォルダーの識別子を取得、フォルダーの名前、そのフォルダー内の項目の数を子フォルダーの数と未読アイテム数を表示する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="5522b-107">The following example of a **GetFolder** request shows how to obtain a folder identifier, display name, the count of items in that folder, the count of child folders, and the number of unread items in the folder.</span></span> 
  
### <a name="code"></a><span data-ttu-id="5522b-108">コード</span><span class="sxs-lookup"><span data-stu-id="5522b-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
   xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetFolder xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <FolderShape>
        <t:BaseShape>Default</t:BaseShape>
      </FolderShape>
      <FolderIds>
        <t:DistinguishedFolderId Id="inbox"/>
      </FolderIds>
    </GetFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="5522b-109">要素を要求します。</span><span class="sxs-lookup"><span data-stu-id="5522b-109">Request elements</span></span>

<span data-ttu-id="5522b-110">この**GetFolder**要求には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5522b-110">This **GetFolder** request includes the following elements:</span></span> 
  
- [<span data-ttu-id="5522b-111">GetFolder</span><span class="sxs-lookup"><span data-stu-id="5522b-111">GetFolder</span></span>](getfolder.md)
    
- [<span data-ttu-id="5522b-112">FolderShape</span><span class="sxs-lookup"><span data-stu-id="5522b-112">FolderShape</span></span>](foldershape.md)
    
- [<span data-ttu-id="5522b-113">BaseShape</span><span class="sxs-lookup"><span data-stu-id="5522b-113">BaseShape</span></span>](baseshape.md)
    
- [<span data-ttu-id="5522b-114">FolderIds</span><span class="sxs-lookup"><span data-stu-id="5522b-114">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="5522b-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="5522b-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
<span data-ttu-id="5522b-116">**GetFolder**要求を形成するために使用できるその他の要素のスキーマを参照してください。</span><span class="sxs-lookup"><span data-stu-id="5522b-116">See the schema for additional elements that you can use to form a **GetFolder** request.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="5522b-117">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="5522b-117">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span> 
  
## <a name="getfolder-response-example"></a><span data-ttu-id="5522b-118">GetFolder の応答の例</span><span class="sxs-lookup"><span data-stu-id="5522b-118">GetFolder response example</span></span>

### <a name="description"></a><span data-ttu-id="5522b-119">説明</span><span class="sxs-lookup"><span data-stu-id="5522b-119">Description</span></span>

<span data-ttu-id="5522b-120">**GetFolder**要求に正常な応答を Simple Object Access Protocol (SOAP) 本文の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5522b-120">The following Simple Object Access Protocol (SOAP) body example shows a successful response to the **GetFolder** request.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="5522b-121">フォルダー ID と変更キーは、読みやすさを保持するために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="5522b-121">The folder ID and the change key have been shortened to preserve readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="5522b-122">コード</span><span class="sxs-lookup"><span data-stu-id="5522b-122">Code</span></span>

```XML
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="AQApA=" ChangeKey="AQAAAB" />
              <t:DisplayName>Inbox</t:DisplayName>
              <t:TotalCount>2</t:TotalCount>
              <t:ChildFolderCount>0</t:ChildFolderCount>
              <t:UnreadCount>2</t:UnreadCount>
            </t:Folder>
          </m:Folders>
        </m:GetFolderResponseMessage>
      </m:ResponseMessages>
    </GetFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="response-elements"></a><span data-ttu-id="5522b-123">応答の要素</span><span class="sxs-lookup"><span data-stu-id="5522b-123">Response elements</span></span>

<span data-ttu-id="5522b-124">この**GetFolder**の応答には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5522b-124">This **GetFolder** response includes the following elements:</span></span> 
  
- [<span data-ttu-id="5522b-125">GetFolderResponse</span><span class="sxs-lookup"><span data-stu-id="5522b-125">GetFolderResponse</span></span>](getfolderresponse.md)
    
- [<span data-ttu-id="5522b-126">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="5522b-126">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="5522b-127">GetFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="5522b-127">GetFolderResponseMessage</span></span>](getfolderresponsemessage.md)
    
- [<span data-ttu-id="5522b-128">フォルダー</span><span class="sxs-lookup"><span data-stu-id="5522b-128">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="5522b-129">Folder</span><span class="sxs-lookup"><span data-stu-id="5522b-129">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="5522b-130">フォルダー Id</span><span class="sxs-lookup"><span data-stu-id="5522b-130">FolderId</span></span>](folderid.md)
    
- [<span data-ttu-id="5522b-131">表示名 (文字列)</span><span class="sxs-lookup"><span data-stu-id="5522b-131">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="5522b-132">TotalCount</span><span class="sxs-lookup"><span data-stu-id="5522b-132">TotalCount</span></span>](totalcount.md)
    
- [<span data-ttu-id="5522b-133">ChildFolderCount</span><span class="sxs-lookup"><span data-stu-id="5522b-133">ChildFolderCount</span></span>](childfoldercount.md)
    
- [<span data-ttu-id="5522b-134">UnreadCount</span><span class="sxs-lookup"><span data-stu-id="5522b-134">UnreadCount</span></span>](unreadcount.md)
    
## <a name="getfolder-error-response-example"></a><span data-ttu-id="5522b-135">GetFolder エラー応答の例</span><span class="sxs-lookup"><span data-stu-id="5522b-135">GetFolder Error response example</span></span>

### <a name="description"></a><span data-ttu-id="5522b-136">説明</span><span class="sxs-lookup"><span data-stu-id="5522b-136">Description</span></span>

<span data-ttu-id="5522b-137">要求に不正な[フォルダー Id](folderid.md)が原因で発生するエラー応答を SOAP 本文の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5522b-137">The following SOAP body example shows an error response that is caused by an incorrect [FolderId](folderid.md) in the request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="5522b-138">コード</span><span class="sxs-lookup"><span data-stu-id="5522b-138">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetFolderResponseMessage ResponseClass="Error">
          <m:MessageText>Id is malformed.</m:MessageText>
          <m:ResponseCode>ErrorInvalidIdMalformed</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Folders />
        </m:GetFolderResponseMessage>
      </m:ResponseMessages>
    </GetFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="response-elements"></a><span data-ttu-id="5522b-139">応答の要素</span><span class="sxs-lookup"><span data-stu-id="5522b-139">Response elements</span></span>

<span data-ttu-id="5522b-140">この**GetFolder**エラー応答には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5522b-140">This **GetFolder** error response includes the following elements:</span></span> 
  
- [<span data-ttu-id="5522b-141">GetFolderResponse</span><span class="sxs-lookup"><span data-stu-id="5522b-141">GetFolderResponse</span></span>](getfolderresponse.md)
    
- [<span data-ttu-id="5522b-142">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="5522b-142">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="5522b-143">GetFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="5522b-143">GetFolderResponseMessage</span></span>](getfolderresponsemessage.md)
    
- [<span data-ttu-id="5522b-144">MessageText</span><span class="sxs-lookup"><span data-stu-id="5522b-144">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="5522b-145">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="5522b-145">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="5522b-146">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="5522b-146">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="5522b-147">フォルダー</span><span class="sxs-lookup"><span data-stu-id="5522b-147">Folders</span></span>](folders-ex15websvcsotherref.md)
    
## <a name="version-differences"></a><span data-ttu-id="5522b-148">バージョンの相違点</span><span class="sxs-lookup"><span data-stu-id="5522b-148">Version differences</span></span>

<span data-ttu-id="5522b-149">アプリケーションを対象とする Exchange のオンライン、Office 365 の一部として Exchange のオンライン、または、設置型バージョンの Exchange から Exchange 2013 では、フォルダーのアクセス許可は返されません[BaseShape](baseshape.md)の要素に**AllProperties**の値が設定されている場合[GetFolder](getfolder-operation.md)操作要求します。</span><span class="sxs-lookup"><span data-stu-id="5522b-149">For applications that target Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange starting with Exchange 2013, folder permissions are not returned when the [BaseShape](baseshape.md) element has a value of **AllProperties** in the [GetFolder](getfolder-operation.md) operation request.</span></span> <span data-ttu-id="5522b-150">フォルダーのアクセス許可を取得するには、 **GetFolder**要求内の[AdditionalProperties](additionalproperties.md)要素に[PermissionSet (PermissionSetType)](permissionset-permissionsettype.md)の要素を追加します。</span><span class="sxs-lookup"><span data-stu-id="5522b-150">To retrieve folder permissions, add the [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) element to the [AdditionalProperties](additionalproperties.md) element in the **GetFolder** request.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="5522b-151">関連項目</span><span class="sxs-lookup"><span data-stu-id="5522b-151">See also</span></span>



- [<span data-ttu-id="5522b-152">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="5522b-152">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

