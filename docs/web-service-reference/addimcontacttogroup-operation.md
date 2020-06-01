---
title: AddImContactToGroup 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 376acc42-2684-4596-aca1-82a4a10865c9
description: AddImContactToGroup EWS 操作に関する情報を検索します。
ms.openlocfilehash: a69ee0b355e78e1249383cab612a75bcda8d9e8a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458412"
---
# <a name="addimcontacttogroup-operation"></a><span data-ttu-id="0ce0d-103">AddImContactToGroup 操作</span><span class="sxs-lookup"><span data-stu-id="0ce0d-103">AddImContactToGroup operation</span></span>

<span data-ttu-id="0ce0d-104">**Addimcontacttogroup** EWS 操作に関する情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="0ce0d-104">Find information about the **AddImContactToGroup** EWS operation.</span></span> 
  
<span data-ttu-id="0ce0d-105">**Addimcontacttogroup** Exchange Web サービス (EWS) 操作は、既存のインスタントメッセージング (IM) 連絡先をグループに追加します。</span><span class="sxs-lookup"><span data-stu-id="0ce0d-105">The **AddImContactToGroup** Exchange Web Services (EWS) operation adds an existing instant messaging (IM) contact to a group.</span></span> 
  
<span data-ttu-id="0ce0d-106">この操作は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="0ce0d-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-addimcontacttogroup-operation"></a><span data-ttu-id="0ce0d-107">AddImContactToGroup 操作の使用</span><span class="sxs-lookup"><span data-stu-id="0ce0d-107">Using the AddImContactToGroup operation</span></span>

<span data-ttu-id="0ce0d-108">**Addimcontacttogroup**操作では、IM の連絡先のみを受け入れることができます。</span><span class="sxs-lookup"><span data-stu-id="0ce0d-108">The **AddImContactToGroup** operation can only accept IM contacts.</span></span> <span data-ttu-id="0ce0d-109">新しい IM 連絡先を統合連絡先ストアに追加する場合は、 [AddNewImContactToGroup](addnewimcontacttogroup-operation.md)操作を使用します。</span><span class="sxs-lookup"><span data-stu-id="0ce0d-109">If you want to add a new IM contact to the Unified Contact Store, use the [AddNewImContactToGroup](addnewimcontacttogroup-operation.md) operation.</span></span> 
  
<span data-ttu-id="0ce0d-110">**Addimcontacttogroup**操作では、次の表に示す SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="0ce0d-110">The **AddImContactToGroup** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
<span data-ttu-id="0ce0d-111">**表1AddImContactToGroup 操作 SOAP ヘッダー**</span><span class="sxs-lookup"><span data-stu-id="0ce0d-111">**Table 1. AddImContactToGroup operation SOAP headers**</span></span>

|<span data-ttu-id="0ce0d-112">**ヘッダー名**</span><span class="sxs-lookup"><span data-stu-id="0ce0d-112">**Header name**</span></span>|<span data-ttu-id="0ce0d-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="0ce0d-113">**Element**</span></span>|<span data-ttu-id="0ce0d-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="0ce0d-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="0ce0d-115">**偽装**</span><span class="sxs-lookup"><span data-stu-id="0ce0d-115">**Impersonation**</span></span> <br/> |[<span data-ttu-id="0ce0d-116">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="0ce0d-116">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="0ce0d-117">クライアントアプリケーションが偽装しているユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="0ce0d-117">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="0ce0d-118">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="0ce0d-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="0ce0d-119">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="0ce0d-119">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="0ce0d-120">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="0ce0d-120">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="0ce0d-121">RFC 3066 で定義されているように、メールボックスへのアクセスに使用されるカルチャ (言語の識別用のタグ) を識別します。</span><span class="sxs-lookup"><span data-stu-id="0ce0d-121">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="0ce0d-122">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="0ce0d-122">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="0ce0d-123">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="0ce0d-123">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="0ce0d-124">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="0ce0d-124">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="0ce0d-125">操作要求のスキーマバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="0ce0d-125">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="0ce0d-126">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="0ce0d-126">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="0ce0d-127">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="0ce0d-127">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="0ce0d-128">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="0ce0d-128">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="0ce0d-129">要求に応答したサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="0ce0d-129">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="0ce0d-130">このヘッダーは応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="0ce0d-130">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="addimcontacttogroup-operation-request-example-add-an-existing-im-contact-to-an-im-group"></a><span data-ttu-id="0ce0d-131">AddImContactToGroup 操作要求の例: 既存の IM 連絡先を IM グループに追加します。</span><span class="sxs-lookup"><span data-stu-id="0ce0d-131">AddImContactToGroup operation request example: Add an existing IM contact to an IM group</span></span>

<span data-ttu-id="0ce0d-132">**Addimcontacttogroup**操作要求の次の例は、既存の im 連絡先を im グループに追加する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="0ce0d-132">The following example of an **AddImContactToGroup** operation request shows how to add an existing IM contact an IM group.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

<span data-ttu-id="0ce0d-133">要求 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0ce0d-133">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="0ce0d-134">AddImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="0ce0d-134">AddImContactToGroup</span></span>](addimcontacttogroup.md)
    
- [<span data-ttu-id="0ce0d-135">ContactId</span><span class="sxs-lookup"><span data-stu-id="0ce0d-135">ContactId</span></span>](contactid.md)
    
- [<span data-ttu-id="0ce0d-136">GroupId</span><span class="sxs-lookup"><span data-stu-id="0ce0d-136">GroupId</span></span>](groupid.md)
    
## <a name="successful-addimcontacttogroup-operation-response"></a><span data-ttu-id="0ce0d-137">正常な AddImContactToGroup 操作の応答</span><span class="sxs-lookup"><span data-stu-id="0ce0d-137">Successful AddImContactToGroup operation response</span></span>

<span data-ttu-id="0ce0d-138">次の例は、 **Addimcontacttogroup**操作要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="0ce0d-138">The following example shows a successful response to an **AddImContactToGroup** operation request.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="349" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <AddImContactToGroupResponse ResponseClass="Success" 
                                   xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </AddImContactToGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="0ce0d-139">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0ce0d-139">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="0ce0d-140">AddImContactToGroupResponse</span><span class="sxs-lookup"><span data-stu-id="0ce0d-140">AddImContactToGroupResponse</span></span>](addimcontacttogroupresponse.md)
    
- [<span data-ttu-id="0ce0d-141">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="0ce0d-141">ResponseCode</span></span>](responsecode.md)
    
## <a name="addimcontacttogroup-operation-errorinvalidimcontactid-error-response"></a><span data-ttu-id="0ce0d-142">AddImContactToGroup 操作 ErrorInvalidImContactId エラー応答</span><span class="sxs-lookup"><span data-stu-id="0ce0d-142">AddImContactToGroup operation ErrorInvalidImContactId error response</span></span>

<span data-ttu-id="0ce0d-143">次の例は、 **Addimcontacttogroup**操作要求へのエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="0ce0d-143">The following example shows an error response to an **AddImContactToGroup** operation request.</span></span> <span data-ttu-id="0ce0d-144">IM 連絡先ではない連絡先を追加しようとすると、次のエラー応答が発生します。</span><span class="sxs-lookup"><span data-stu-id="0ce0d-144">The following error response occurs when an attempt is made to add a contact that is not an IM contact.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15"
                           MinorVersion="0" 
                           MajorBuildNumber="349" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <AddImContactToGroupResponse ResponseClass="Error" 
                                   xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified Im Contact Id is invalid.</MessageText>
         <ResponseCode>ErrorInvalidImContactId</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
         </AddImContactToGroupResponse>
      </s:Body>
</s:Envelope>
```

<span data-ttu-id="0ce0d-145">エラー応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0ce0d-145">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="0ce0d-146">AddImContactToGroupResponse</span><span class="sxs-lookup"><span data-stu-id="0ce0d-146">AddImContactToGroupResponse</span></span>](addimcontacttogroupresponse.md)
    
- [<span data-ttu-id="0ce0d-147">MessageText</span><span class="sxs-lookup"><span data-stu-id="0ce0d-147">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="0ce0d-148">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="0ce0d-148">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="0ce0d-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="0ce0d-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="0ce0d-150">関連項目</span><span class="sxs-lookup"><span data-stu-id="0ce0d-150">See also</span></span>

- [<span data-ttu-id="0ce0d-151">AddImGroup 操作</span><span class="sxs-lookup"><span data-stu-id="0ce0d-151">AddImGroup operation</span></span>](addimgroup-operation.md)
    
- [<span data-ttu-id="0ce0d-152">AddNewImContactToGroup 操作</span><span class="sxs-lookup"><span data-stu-id="0ce0d-152">AddNewImContactToGroup operation</span></span>](addnewimcontacttogroup-operation.md)
    
- [<span data-ttu-id="0ce0d-153">SetImGroup 操作</span><span class="sxs-lookup"><span data-stu-id="0ce0d-153">SetImGroup operation</span></span>](setimgroup-operation.md)
    
- [<span data-ttu-id="0ce0d-154">RemoveImGroup 操作</span><span class="sxs-lookup"><span data-stu-id="0ce0d-154">RemoveImGroup operation</span></span>](removeimgroup-operation.md)
    
- [<span data-ttu-id="0ce0d-155">GetImItemList 操作</span><span class="sxs-lookup"><span data-stu-id="0ce0d-155">GetImItemList operation</span></span>](getimitemlist-operation.md)
    
- [<span data-ttu-id="0ce0d-156">Exchange 内の EWS のユーザーと連絡先</span><span class="sxs-lookup"><span data-stu-id="0ce0d-156">People and contacts in EWS in Exchange</span></span>](https://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    

