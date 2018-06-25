---
title: RemoveImContactFromGroup 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a190bbec-c71b-4e6a-880b-55854c724d8c
description: 操作 RemoveImContactFromGroup EWS についての情報を検索します。
ms.openlocfilehash: 8c9af251014dbddabb439ed5bf5dc35580da6a90
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833099"
---
# <a name="removeimcontactfromgroup-operation"></a><span data-ttu-id="0c9cf-103">RemoveImContactFromGroup 操作</span><span class="sxs-lookup"><span data-stu-id="0c9cf-103">RemoveImContactFromGroup operation</span></span>

<span data-ttu-id="0c9cf-104">**RemoveImContactFromGroup** EWS の操作に関する情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="0c9cf-104">Find information about the **RemoveImContactFromGroup** EWS operation.</span></span> 
  
<span data-ttu-id="0c9cf-105">**RemoveImContactFromGroup**操作では、IM のグループから 1 つの IM 連絡先を削除します。</span><span class="sxs-lookup"><span data-stu-id="0c9cf-105">The **RemoveImContactFromGroup** operation removes a single IM contact from an IM group.</span></span> 
  
<span data-ttu-id="0c9cf-106">この操作は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="0c9cf-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-removeimcontactfromgroup-operation"></a><span data-ttu-id="0c9cf-107">RemoveImContactFromGroup 操作を使用します。</span><span class="sxs-lookup"><span data-stu-id="0c9cf-107">Using the RemoveImContactFromGroup operation</span></span>

<span data-ttu-id="0c9cf-108">**RemoveImContactFromGroup**操作は、2 つの引数をとります: 連絡先アイテムの識別子、および対応するインスタント メッセージング (IM) グループの連絡先を削除します。</span><span class="sxs-lookup"><span data-stu-id="0c9cf-108">The **RemoveImContactFromGroup** operation takes two arguments: a contact item identifier, and the corresponding instant messaging (IM) group from which the contact is removed.</span></span> 
  
### <a name="removeimcontactfromgroup-operation-soap-headers"></a><span data-ttu-id="0c9cf-109">RemoveImContactFromGroup 操作の SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0c9cf-109">RemoveImContactFromGroup operation SOAP headers</span></span>

<span data-ttu-id="0c9cf-110">**RemoveImContactFromGroup**操作は、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="0c9cf-110">The **RemoveImContactFromGroup** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="0c9cf-111">**ヘッダー名**</span><span class="sxs-lookup"><span data-stu-id="0c9cf-111">**Header name**</span></span>|<span data-ttu-id="0c9cf-112">**要素**</span><span class="sxs-lookup"><span data-stu-id="0c9cf-112">**Element**</span></span>|<span data-ttu-id="0c9cf-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="0c9cf-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="0c9cf-114">**偽装**</span><span class="sxs-lookup"><span data-stu-id="0c9cf-114">**Impersonation**</span></span> <br/> |[<span data-ttu-id="0c9cf-115">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="0c9cf-115">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="0c9cf-116">クライアント アプリケーションが偽装するユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="0c9cf-116">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="0c9cf-117">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="0c9cf-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="0c9cf-118">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="0c9cf-118">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="0c9cf-119">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="0c9cf-119">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="0c9cf-120">RFC 3066、」タグの「識別の言語」を使用してメールボックスへのアクセスに定義されているカルチャを識別します。</span><span class="sxs-lookup"><span data-stu-id="0c9cf-120">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="0c9cf-121">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="0c9cf-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="0c9cf-122">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="0c9cf-122">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="0c9cf-123">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="0c9cf-123">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="0c9cf-124">操作要求のスキーマのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="0c9cf-124">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="0c9cf-125">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="0c9cf-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="0c9cf-126">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="0c9cf-126">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="0c9cf-127">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="0c9cf-127">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="0c9cf-128">要求に応答するサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="0c9cf-128">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="0c9cf-129">このヘッダーは、応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="0c9cf-129">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="removeimcontactfromgroup-operation-request-example"></a><span data-ttu-id="0c9cf-130">RemoveImContactFromGroup 操作の要求の例</span><span class="sxs-lookup"><span data-stu-id="0c9cf-130">RemoveImContactFromGroup operation request example</span></span>

<span data-ttu-id="0c9cf-131">**RemoveImContactFromGroup**操作要求の次の例では、IM のグループからの IM の連絡先を削除する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="0c9cf-131">The following example of a **RemoveImContactFromGroup** operation request shows how to remove an IM contact from an IM group.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="0c9cf-132">グループと取引先担当者の識別子は、読みやすさを保持するために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="0c9cf-132">The group and contact identifiers have been shortened to preserve readability.</span></span> 
  
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
      <m:RemoveImContactFromGroup>
         <m:ContactId Id="AAMkAGQ1MjJjMTBkLTcAAAAvcAAA="
                      ChangeKey="EQAAABYAAABtF8oI7iVOQ"/>
         <m:GroupId Id="AAMkAGQ1MjJjMTBkbWAAAAAAQKAAA="
                    ChangeKey="EgAAAA=="/>
      </m:RemoveImContactFromGroup>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="0c9cf-133">要求 SOAP 本体にはには、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0c9cf-133">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="0c9cf-134">RemoveImContactFromGroup</span><span class="sxs-lookup"><span data-stu-id="0c9cf-134">RemoveImContactFromGroup</span></span>](removeimcontactfromgroup.md)
    
- [<span data-ttu-id="0c9cf-135">ContactId</span><span class="sxs-lookup"><span data-stu-id="0c9cf-135">ContactId</span></span>](contactid.md)
    
- [<span data-ttu-id="0c9cf-136">グループ Id</span><span class="sxs-lookup"><span data-stu-id="0c9cf-136">GroupId</span></span>](groupid.md)
    
## <a name="successful-removeimcontactfromgroup-operation-response"></a><span data-ttu-id="0c9cf-137">RemoveImContactFromGroup 操作の成功の応答</span><span class="sxs-lookup"><span data-stu-id="0c9cf-137">Successful RemoveImContactFromGroup operation response</span></span>

<span data-ttu-id="0c9cf-138">成功した要求への応答、 **RemoveImContactFromGroup**操作の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0c9cf-138">The following example shows a successful response to a **RemoveImContactFromGroup** operation request.</span></span> 
  
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
      <RemoveImContactFromGroupResponse ResponseClass="Success" 
                                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </RemoveImContactFromGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="0c9cf-139">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0c9cf-139">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="0c9cf-140">RemoveImContactFromGroupResponse</span><span class="sxs-lookup"><span data-stu-id="0c9cf-140">RemoveImContactFromGroupResponse</span></span>](removeimcontactfromgroupresponse.md)
    
- [<span data-ttu-id="0c9cf-141">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="0c9cf-141">ResponseCode</span></span>](responsecode.md)
    
## <a name="removeimcontactfromgroup-operation-errorinvalidimcontactid-error-response"></a><span data-ttu-id="0c9cf-142">RemoveImContactFromGroup 操作エラー応答の ErrorInvalidImContactId</span><span class="sxs-lookup"><span data-stu-id="0c9cf-142">RemoveImContactFromGroup operation ErrorInvalidImContactId error response</span></span>

<span data-ttu-id="0c9cf-143">**RemoveImContactFromGroup**操作の要求に対してエラー応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0c9cf-143">The following example shows an error response to a **RemoveImContactFromGroup** operation request.</span></span> <span data-ttu-id="0c9cf-144">次のエラー応答は、IM グループに存在しない連絡先アイテムを削除しようとしましたがときに発生します。</span><span class="sxs-lookup"><span data-stu-id="0c9cf-144">The following error response occurs when an attempt is made to remove a contact item that does not exist in the IM group.</span></span> 
  
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
      <RemoveImContactFromGroupResponse ResponseClass="Error" 
                                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified Im Contact Id is invalid.</MessageText>
         <ResponseCode>ErrorInvalidImContactId</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </RemoveImContactFromGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="0c9cf-145">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0c9cf-145">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="0c9cf-146">RemoveImContactFromGroupResponse</span><span class="sxs-lookup"><span data-stu-id="0c9cf-146">RemoveImContactFromGroupResponse</span></span>](removeimcontactfromgroupresponse.md)
    
- [<span data-ttu-id="0c9cf-147">MessageText</span><span class="sxs-lookup"><span data-stu-id="0c9cf-147">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="0c9cf-148">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="0c9cf-148">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="0c9cf-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="0c9cf-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="0c9cf-150">関連項目</span><span class="sxs-lookup"><span data-stu-id="0c9cf-150">See also</span></span>

- [<span data-ttu-id="0c9cf-151">Exchange 内の EWS のユーザーと連絡先</span><span class="sxs-lookup"><span data-stu-id="0c9cf-151">People and contacts in EWS in Exchange</span></span>](http://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [<span data-ttu-id="0c9cf-152">AddDistributionGroupToImList</span><span class="sxs-lookup"><span data-stu-id="0c9cf-152">AddDistributionGroupToImList</span></span>](adddistributiongrouptoimlist-operation.md)
    
- [<span data-ttu-id="0c9cf-153">AddImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="0c9cf-153">AddImContactToGroup</span></span>](addimcontacttogroup-operation.md)
    
- [<span data-ttu-id="0c9cf-154">AddImGroup 操作</span><span class="sxs-lookup"><span data-stu-id="0c9cf-154">AddImGroup operation</span></span>](addimgroup-operation.md)
    
- [<span data-ttu-id="0c9cf-155">AddNewImContactToGroup 操作</span><span class="sxs-lookup"><span data-stu-id="0c9cf-155">AddNewImContactToGroup operation</span></span>](addnewimcontacttogroup-operation.md)
    
- [<span data-ttu-id="0c9cf-156">GetImItemList 操作</span><span class="sxs-lookup"><span data-stu-id="0c9cf-156">GetImItemList operation</span></span>](getimitemlist-operation.md)
    
- [<span data-ttu-id="0c9cf-157">GetImItems</span><span class="sxs-lookup"><span data-stu-id="0c9cf-157">GetImItems</span></span>](getimitems-operation.md)
    
- [<span data-ttu-id="0c9cf-158">RemoveContactFromImList</span><span class="sxs-lookup"><span data-stu-id="0c9cf-158">RemoveContactFromImList</span></span>](removecontactfromimlist-operation.md)
    
- [<span data-ttu-id="0c9cf-159">RemoveDistributionGroupFromImList</span><span class="sxs-lookup"><span data-stu-id="0c9cf-159">RemoveDistributionGroupFromImList</span></span>](removedistributiongroupfromimlist-operation.md)
    
- [<span data-ttu-id="0c9cf-160">RemoveImGroup 操作</span><span class="sxs-lookup"><span data-stu-id="0c9cf-160">RemoveImGroup operation</span></span>](removeimgroup-operation.md)
    
- [<span data-ttu-id="0c9cf-161">SetImGroup 操作</span><span class="sxs-lookup"><span data-stu-id="0c9cf-161">SetImGroup operation</span></span>](setimgroup-operation.md)
    
- [<span data-ttu-id="0c9cf-162">SetImListMigrationCompleted</span><span class="sxs-lookup"><span data-stu-id="0c9cf-162">SetImListMigrationCompleted</span></span>](setimlistmigrationcompleted-operation.md)
    

