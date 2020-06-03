---
title: GetFolder 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
api_name:
- GetFolder
api_type:
- schema
ms.assetid: 355bcf93-dc71-4493-b177-622afac5fdb9
description: GetFolder 操作は、Exchange ストアからフォルダーを取得します。
localization_priority: Priority
ms.openlocfilehash: 9d511f309b9210fd9b5a49ff6c60bc7982992973
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459182"
---
# <a name="getfolder-operation"></a><span data-ttu-id="a4354-103">GetFolder 操作</span><span class="sxs-lookup"><span data-stu-id="a4354-103">GetFolder operation</span></span>

<span data-ttu-id="a4354-104">**Getfolder**操作は、Exchange ストアからフォルダーを取得します。</span><span class="sxs-lookup"><span data-stu-id="a4354-104">The **GetFolder** operation gets folders from the Exchange store.</span></span> 
  
## <a name="getfolder-request-example"></a><span data-ttu-id="a4354-105">GetFolder 要求の例</span><span class="sxs-lookup"><span data-stu-id="a4354-105">GetFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="a4354-106">Description</span><span class="sxs-lookup"><span data-stu-id="a4354-106">Description</span></span>

<span data-ttu-id="a4354-107">次の**Getfolder**要求の例は、フォルダー識別子、表示名、そのフォルダー内のアイテム数、子フォルダーの数、およびフォルダー内の未読アイテム数を取得する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="a4354-107">The following example of a **GetFolder** request shows how to obtain a folder identifier, display name, the count of items in that folder, the count of child folders, and the number of unread items in the folder.</span></span> 
  
### <a name="code"></a><span data-ttu-id="a4354-108">コード</span><span class="sxs-lookup"><span data-stu-id="a4354-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
   xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetFolder xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

### <a name="request-elements"></a><span data-ttu-id="a4354-109">Request 要素</span><span class="sxs-lookup"><span data-stu-id="a4354-109">Request elements</span></span>

<span data-ttu-id="a4354-110">この**Getfolder**要求には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a4354-110">This **GetFolder** request includes the following elements:</span></span> 
  
- [<span data-ttu-id="a4354-111">GetFolder</span><span class="sxs-lookup"><span data-stu-id="a4354-111">GetFolder</span></span>](getfolder.md)
    
- [<span data-ttu-id="a4354-112">FolderShape</span><span class="sxs-lookup"><span data-stu-id="a4354-112">FolderShape</span></span>](foldershape.md)
    
- [<span data-ttu-id="a4354-113">BaseShape</span><span class="sxs-lookup"><span data-stu-id="a4354-113">BaseShape</span></span>](baseshape.md)
    
- [<span data-ttu-id="a4354-114">FolderIds</span><span class="sxs-lookup"><span data-stu-id="a4354-114">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="a4354-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="a4354-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
<span data-ttu-id="a4354-116">**Getfolder**要求の形成に使用できるその他の要素については、スキーマを参照してください。</span><span class="sxs-lookup"><span data-stu-id="a4354-116">See the schema for additional elements that you can use to form a **GetFolder** request.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="a4354-117">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="a4354-117">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span> 
  
## <a name="getfolder-response-example"></a><span data-ttu-id="a4354-118">GetFolder 応答の例</span><span class="sxs-lookup"><span data-stu-id="a4354-118">GetFolder response example</span></span>

### <a name="description"></a><span data-ttu-id="a4354-119">Description</span><span class="sxs-lookup"><span data-stu-id="a4354-119">Description</span></span>

<span data-ttu-id="a4354-120">次の簡易オブジェクトアクセスプロトコル (SOAP) 本文の例は、 **Getfolder**要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="a4354-120">The following Simple Object Access Protocol (SOAP) body example shows a successful response to the **GetFolder** request.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="a4354-121">読みやすくするために、フォルダー ID と変更キーが短縮されています。</span><span class="sxs-lookup"><span data-stu-id="a4354-121">The folder ID and the change key have been shortened to preserve readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="a4354-122">コード</span><span class="sxs-lookup"><span data-stu-id="a4354-122">Code</span></span>

```XML
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="response-elements"></a><span data-ttu-id="a4354-123">Response 要素</span><span class="sxs-lookup"><span data-stu-id="a4354-123">Response elements</span></span>

<span data-ttu-id="a4354-124">この**Getfolder**応答には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a4354-124">This **GetFolder** response includes the following elements:</span></span> 
  
- [<span data-ttu-id="a4354-125">GetFolderResponse</span><span class="sxs-lookup"><span data-stu-id="a4354-125">GetFolderResponse</span></span>](getfolderresponse.md)
    
- [<span data-ttu-id="a4354-126">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="a4354-126">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="a4354-127">GetFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="a4354-127">GetFolderResponseMessage</span></span>](getfolderresponsemessage.md)
    
- [<span data-ttu-id="a4354-128">フォルダー</span><span class="sxs-lookup"><span data-stu-id="a4354-128">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="a4354-129">Folder</span><span class="sxs-lookup"><span data-stu-id="a4354-129">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="a4354-130">FolderId</span><span class="sxs-lookup"><span data-stu-id="a4354-130">FolderId</span></span>](folderid.md)
    
- [<span data-ttu-id="a4354-131">DisplayName (文字列)</span><span class="sxs-lookup"><span data-stu-id="a4354-131">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="a4354-132">TotalCount</span><span class="sxs-lookup"><span data-stu-id="a4354-132">TotalCount</span></span>](totalcount.md)
    
- [<span data-ttu-id="a4354-133">ChildFolderCount</span><span class="sxs-lookup"><span data-stu-id="a4354-133">ChildFolderCount</span></span>](childfoldercount.md)
    
- [<span data-ttu-id="a4354-134">UnreadCount</span><span class="sxs-lookup"><span data-stu-id="a4354-134">UnreadCount</span></span>](unreadcount.md)
    
## <a name="getfolder-error-response-example"></a><span data-ttu-id="a4354-135">GetFolder エラー応答の例</span><span class="sxs-lookup"><span data-stu-id="a4354-135">GetFolder Error response example</span></span>

### <a name="description"></a><span data-ttu-id="a4354-136">Description</span><span class="sxs-lookup"><span data-stu-id="a4354-136">Description</span></span>

<span data-ttu-id="a4354-137">次の SOAP 本文の例は、要求の[FolderId](folderid.md)が正しくないことが原因で発生するエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="a4354-137">The following SOAP body example shows an error response that is caused by an incorrect [FolderId](folderid.md) in the request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="a4354-138">コード</span><span class="sxs-lookup"><span data-stu-id="a4354-138">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="response-elements"></a><span data-ttu-id="a4354-139">Response 要素</span><span class="sxs-lookup"><span data-stu-id="a4354-139">Response elements</span></span>

<span data-ttu-id="a4354-140">この**Getfolder**エラー応答には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a4354-140">This **GetFolder** error response includes the following elements:</span></span> 
  
- [<span data-ttu-id="a4354-141">GetFolderResponse</span><span class="sxs-lookup"><span data-stu-id="a4354-141">GetFolderResponse</span></span>](getfolderresponse.md)
    
- [<span data-ttu-id="a4354-142">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="a4354-142">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="a4354-143">GetFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="a4354-143">GetFolderResponseMessage</span></span>](getfolderresponsemessage.md)
    
- [<span data-ttu-id="a4354-144">MessageText</span><span class="sxs-lookup"><span data-stu-id="a4354-144">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="a4354-145">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="a4354-145">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="a4354-146">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="a4354-146">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="a4354-147">フォルダー</span><span class="sxs-lookup"><span data-stu-id="a4354-147">Folders</span></span>](folders-ex15websvcsotherref.md)
    
## <a name="version-differences"></a><span data-ttu-id="a4354-148">バージョンの相違点</span><span class="sxs-lookup"><span data-stu-id="a4354-148">Version differences</span></span>

<span data-ttu-id="a4354-149">Exchange Online を対象とするアプリケーション、Office 365 の一部としての Exchange Online、または exchange 2013 以降のオンプレミスバージョンの Exchange の場合、フォルダーのアクセス許可は、 [Baseshape](baseshape.md)要素の値が[getfolder](getfolder-operation.md)操作要求で**allproperties**の値になっている場合は返されません。</span><span class="sxs-lookup"><span data-stu-id="a4354-149">For applications that target Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange starting with Exchange 2013, folder permissions are not returned when the [BaseShape](baseshape.md) element has a value of **AllProperties** in the [GetFolder](getfolder-operation.md) operation request.</span></span> <span data-ttu-id="a4354-150">フォルダーのアクセス許可を取得するには、 [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md)要素を、 **Getfolder**要求の[additionalproperties](additionalproperties.md)要素に追加します。</span><span class="sxs-lookup"><span data-stu-id="a4354-150">To retrieve folder permissions, add the [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) element to the [AdditionalProperties](additionalproperties.md) element in the **GetFolder** request.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="a4354-151">関連項目</span><span class="sxs-lookup"><span data-stu-id="a4354-151">See also</span></span>



- [<span data-ttu-id="a4354-152">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="a4354-152">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

