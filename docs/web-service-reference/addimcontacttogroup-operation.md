---
title: AddImContactToGroup 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 376acc42-2684-4596-aca1-82a4a10865c9
description: 操作 AddImContactToGroup EWS についての情報を検索します。
ms.openlocfilehash: 669d798b6cabc1cab1fc057a3e18c565467440f7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759278"
---
# <a name="addimcontacttogroup-operation"></a><span data-ttu-id="1fc07-103">AddImContactToGroup 操作</span><span class="sxs-lookup"><span data-stu-id="1fc07-103">AddImContactToGroup operation</span></span>

<span data-ttu-id="1fc07-104">**AddImContactToGroup** EWS の操作に関する情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="1fc07-104">Find information about the **AddImContactToGroup** EWS operation.</span></span> 
  
<span data-ttu-id="1fc07-105">**AddImContactToGroup** Exchange Web サービス (EWS) 操作では、インスタント メッセージング (IM) の既存の連絡先をグループに追加します。</span><span class="sxs-lookup"><span data-stu-id="1fc07-105">The **AddImContactToGroup** Exchange Web Services (EWS) operation adds an existing instant messaging (IM) contact to a group.</span></span> 
  
<span data-ttu-id="1fc07-106">この操作は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="1fc07-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-addimcontacttogroup-operation"></a><span data-ttu-id="1fc07-107">AddImContactToGroup 操作を使用します。</span><span class="sxs-lookup"><span data-stu-id="1fc07-107">Using the AddImContactToGroup operation</span></span>

<span data-ttu-id="1fc07-108">**AddImContactToGroup**操作には、IM の連絡先のみを受け入れることができます。</span><span class="sxs-lookup"><span data-stu-id="1fc07-108">The **AddImContactToGroup** operation can only accept IM contacts.</span></span> <span data-ttu-id="1fc07-109">統合連絡先ストアに新しい IM の連絡先を追加する場合は、 [AddNewImContactToGroup](addnewimcontacttogroup-operation.md)操作を使用します。</span><span class="sxs-lookup"><span data-stu-id="1fc07-109">If you want to add a new IM contact to the Unified Contact Store, use the [AddNewImContactToGroup](addnewimcontacttogroup-operation.md) operation.</span></span> 
  
<span data-ttu-id="1fc07-110">**AddImContactToGroup**操作は、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="1fc07-110">The **AddImContactToGroup** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
<span data-ttu-id="1fc07-111">**表 1 です。AddImContactToGroup 操作の SOAP ヘッダー**</span><span class="sxs-lookup"><span data-stu-id="1fc07-111">**Table 1. AddImContactToGroup operation SOAP headers**</span></span>

|<span data-ttu-id="1fc07-112">**ヘッダー名**</span><span class="sxs-lookup"><span data-stu-id="1fc07-112">**Header name**</span></span>|<span data-ttu-id="1fc07-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="1fc07-113">**Element**</span></span>|<span data-ttu-id="1fc07-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="1fc07-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="1fc07-115">**偽装**</span><span class="sxs-lookup"><span data-stu-id="1fc07-115">**Impersonation**</span></span> <br/> |[<span data-ttu-id="1fc07-116">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="1fc07-116">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="1fc07-117">クライアント アプリケーションが偽装するユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="1fc07-117">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="1fc07-118">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="1fc07-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="1fc07-119">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="1fc07-119">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="1fc07-120">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="1fc07-120">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="1fc07-121">RFC 3066、」タグの「識別の言語」を使用してメールボックスへのアクセスに定義されているカルチャを識別します。</span><span class="sxs-lookup"><span data-stu-id="1fc07-121">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="1fc07-122">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="1fc07-122">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="1fc07-123">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="1fc07-123">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="1fc07-124">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="1fc07-124">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="1fc07-125">操作要求のスキーマのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="1fc07-125">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="1fc07-126">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="1fc07-126">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="1fc07-127">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="1fc07-127">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="1fc07-128">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="1fc07-128">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="1fc07-129">要求に応答するサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="1fc07-129">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="1fc07-130">このヘッダーは、応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="1fc07-130">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="addimcontacttogroup-operation-request-example-add-an-existing-im-contact-to-an-im-group"></a><span data-ttu-id="1fc07-131">AddImContactToGroup 操作の要求の例: 既存の IM の IM のグループに連絡先追加</span><span class="sxs-lookup"><span data-stu-id="1fc07-131">AddImContactToGroup operation request example: Add an existing IM contact to an IM group</span></span>

<span data-ttu-id="1fc07-132">**AddImContactToGroup**操作要求の次の使用例は、IM グループの既存の IM 連絡先を追加する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="1fc07-132">The following example of an **AddImContactToGroup** operation request shows how to add an existing IM contact an IM group.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
      <t:MailboxCulture>en-US</t:MailboxCulture>
   </soap:Header>
   <soap:Body >
      <m:AddImContactToGroup>
         <m:ContactId Id="AAMkAGQ1MjJjMTBkLTc4Y2AA="
                      ChangeKey="EQAAABYAAABtF8oI7i"/>
         <m:GroupId Id="AAMkAGQ1MjJjMTBkzzAAAQKAAA="
                    ChangeKey="EgAAAA=="/>
      </m:AddImContactToGroup>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="1fc07-133">要求 SOAP 本体にはには、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1fc07-133">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="1fc07-134">AddImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="1fc07-134">AddImContactToGroup</span></span>](addimcontacttogroup.md)
    
- [<span data-ttu-id="1fc07-135">ContactId</span><span class="sxs-lookup"><span data-stu-id="1fc07-135">ContactId</span></span>](contactid.md)
    
- [<span data-ttu-id="1fc07-136">グループ Id</span><span class="sxs-lookup"><span data-stu-id="1fc07-136">GroupId</span></span>](groupid.md)
    
## <a name="successful-addimcontacttogroup-operation-response"></a><span data-ttu-id="1fc07-137">AddImContactToGroup 操作の成功の応答</span><span class="sxs-lookup"><span data-stu-id="1fc07-137">Successful AddImContactToGroup operation response</span></span>

<span data-ttu-id="1fc07-138">**AddImContactToGroup**操作の要求に正常な応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1fc07-138">The following example shows a successful response to an **AddImContactToGroup** operation request.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="349" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <AddImContactToGroupResponse ResponseClass="Success" 
                                   xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </AddImContactToGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="1fc07-139">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1fc07-139">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="1fc07-140">AddImContactToGroupResponse</span><span class="sxs-lookup"><span data-stu-id="1fc07-140">AddImContactToGroupResponse</span></span>](addimcontacttogroupresponse.md)
    
- [<span data-ttu-id="1fc07-141">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="1fc07-141">ResponseCode</span></span>](responsecode.md)
    
## <a name="addimcontacttogroup-operation-errorinvalidimcontactid-error-response"></a><span data-ttu-id="1fc07-142">AddImContactToGroup 操作エラー応答の ErrorInvalidImContactId</span><span class="sxs-lookup"><span data-stu-id="1fc07-142">AddImContactToGroup operation ErrorInvalidImContactId error response</span></span>

<span data-ttu-id="1fc07-143">**AddImContactToGroup**操作要求に対するエラー応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1fc07-143">The following example shows an error response to an **AddImContactToGroup** operation request.</span></span> <span data-ttu-id="1fc07-144">次のエラー応答は、IM の連絡先ではない連絡先を追加しようとしましたがときに発生します。</span><span class="sxs-lookup"><span data-stu-id="1fc07-144">The following error response occurs when an attempt is made to add a contact that is not an IM contact.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15"
                           MinorVersion="0" 
                           MajorBuildNumber="349" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <AddImContactToGroupResponse ResponseClass="Error" 
                                   xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified Im Contact Id is invalid.</MessageText>
         <ResponseCode>ErrorInvalidImContactId</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
         </AddImContactToGroupResponse>
      </s:Body>
</s:Envelope>
```

<span data-ttu-id="1fc07-145">エラー応答 SOAP 本体にはには、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1fc07-145">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="1fc07-146">AddImContactToGroupResponse</span><span class="sxs-lookup"><span data-stu-id="1fc07-146">AddImContactToGroupResponse</span></span>](addimcontacttogroupresponse.md)
    
- [<span data-ttu-id="1fc07-147">MessageText</span><span class="sxs-lookup"><span data-stu-id="1fc07-147">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="1fc07-148">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="1fc07-148">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="1fc07-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="1fc07-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="1fc07-150">関連項目</span><span class="sxs-lookup"><span data-stu-id="1fc07-150">See also</span></span>

- [<span data-ttu-id="1fc07-151">AddImGroup 操作</span><span class="sxs-lookup"><span data-stu-id="1fc07-151">AddImGroup operation</span></span>](addimgroup-operation.md)
    
- [<span data-ttu-id="1fc07-152">AddNewImContactToGroup 操作</span><span class="sxs-lookup"><span data-stu-id="1fc07-152">AddNewImContactToGroup operation</span></span>](addnewimcontacttogroup-operation.md)
    
- [<span data-ttu-id="1fc07-153">SetImGroup 操作</span><span class="sxs-lookup"><span data-stu-id="1fc07-153">SetImGroup operation</span></span>](setimgroup-operation.md)
    
- [<span data-ttu-id="1fc07-154">RemoveImGroup 操作</span><span class="sxs-lookup"><span data-stu-id="1fc07-154">RemoveImGroup operation</span></span>](removeimgroup-operation.md)
    
- [<span data-ttu-id="1fc07-155">GetImItemList 操作</span><span class="sxs-lookup"><span data-stu-id="1fc07-155">GetImItemList operation</span></span>](getimitemlist-operation.md)
    
- [<span data-ttu-id="1fc07-156">Exchange 内の EWS のユーザーと連絡先</span><span class="sxs-lookup"><span data-stu-id="1fc07-156">People and contacts in EWS in Exchange</span></span>](http://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    

