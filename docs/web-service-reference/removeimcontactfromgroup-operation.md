---
title: RemoveImContactFromGroup 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a190bbec-c71b-4e6a-880b-55854c724d8c
description: RemoveImContactFromGroup EWS 操作についての情報を検索します。
ms.openlocfilehash: 4750ef57794c3da540ac36baa8ef6ef093939ea1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466970"
---
# <a name="removeimcontactfromgroup-operation"></a><span data-ttu-id="3ab50-103">RemoveImContactFromGroup 操作</span><span class="sxs-lookup"><span data-stu-id="3ab50-103">RemoveImContactFromGroup operation</span></span>

<span data-ttu-id="3ab50-104">**Removeimcontactfromgroup** EWS 操作についての情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="3ab50-104">Find information about the **RemoveImContactFromGroup** EWS operation.</span></span> 
  
<span data-ttu-id="3ab50-105">**Removeimcontactfromgroup**操作は、im グループから1つの im 連絡先を削除します。</span><span class="sxs-lookup"><span data-stu-id="3ab50-105">The **RemoveImContactFromGroup** operation removes a single IM contact from an IM group.</span></span> 
  
<span data-ttu-id="3ab50-106">この操作は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="3ab50-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-removeimcontactfromgroup-operation"></a><span data-ttu-id="3ab50-107">RemoveImContactFromGroup 操作の使用</span><span class="sxs-lookup"><span data-stu-id="3ab50-107">Using the RemoveImContactFromGroup operation</span></span>

<span data-ttu-id="3ab50-108">**Removeimcontactfromgroup**操作では、連絡先アイテムの識別子と、対応するインスタントメッセージング (IM) グループ (連絡先が削除される) の2つの引数を取ります。</span><span class="sxs-lookup"><span data-stu-id="3ab50-108">The **RemoveImContactFromGroup** operation takes two arguments: a contact item identifier, and the corresponding instant messaging (IM) group from which the contact is removed.</span></span> 
  
### <a name="removeimcontactfromgroup-operation-soap-headers"></a><span data-ttu-id="3ab50-109">RemoveImContactFromGroup 操作 SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3ab50-109">RemoveImContactFromGroup operation SOAP headers</span></span>

<span data-ttu-id="3ab50-110">**Removeimcontactfromgroup**操作では、次の表に示す SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="3ab50-110">The **RemoveImContactFromGroup** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="3ab50-111">**ヘッダー名**</span><span class="sxs-lookup"><span data-stu-id="3ab50-111">**Header name**</span></span>|<span data-ttu-id="3ab50-112">**要素**</span><span class="sxs-lookup"><span data-stu-id="3ab50-112">**Element**</span></span>|<span data-ttu-id="3ab50-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="3ab50-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="3ab50-114">**偽装**</span><span class="sxs-lookup"><span data-stu-id="3ab50-114">**Impersonation**</span></span> <br/> |[<span data-ttu-id="3ab50-115">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="3ab50-115">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="3ab50-116">クライアントアプリケーションが偽装しているユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="3ab50-116">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="3ab50-117">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="3ab50-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="3ab50-118">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="3ab50-118">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="3ab50-119">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="3ab50-119">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="3ab50-120">RFC 3066 で定義されているように、メールボックスへのアクセスに使用されるカルチャ (言語の識別用のタグ) を識別します。</span><span class="sxs-lookup"><span data-stu-id="3ab50-120">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="3ab50-121">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="3ab50-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="3ab50-122">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="3ab50-122">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="3ab50-123">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="3ab50-123">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="3ab50-124">操作要求のスキーマバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="3ab50-124">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="3ab50-125">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="3ab50-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="3ab50-126">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="3ab50-126">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="3ab50-127">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="3ab50-127">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="3ab50-128">要求に応答したサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="3ab50-128">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="3ab50-129">このヘッダーは応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="3ab50-129">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="removeimcontactfromgroup-operation-request-example"></a><span data-ttu-id="3ab50-130">RemoveImContactFromGroup 操作要求の例</span><span class="sxs-lookup"><span data-stu-id="3ab50-130">RemoveImContactFromGroup operation request example</span></span>

<span data-ttu-id="3ab50-131">次の例は、 **Removeimcontactfromgroup**操作要求の例で、im グループから im 連絡先を削除する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="3ab50-131">The following example of a **RemoveImContactFromGroup** operation request shows how to remove an IM contact from an IM group.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="3ab50-132">読みやすくするために、グループと連絡先の識別子が短縮されています。</span><span class="sxs-lookup"><span data-stu-id="3ab50-132">The group and contact identifiers have been shortened to preserve readability.</span></span> 
  
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
      <m:RemoveImContactFromGroup>
         <m:ContactId Id="AAMkAGQ1MjJjMTBkLTcAAAAvcAAA="
                      ChangeKey="EQAAABYAAABtF8oI7iVOQ"/>
         <m:GroupId Id="AAMkAGQ1MjJjMTBkbWAAAAAAQKAAA="
                    ChangeKey="EgAAAA=="/>
      </m:RemoveImContactFromGroup>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="3ab50-133">要求 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="3ab50-133">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="3ab50-134">RemoveImContactFromGroup</span><span class="sxs-lookup"><span data-stu-id="3ab50-134">RemoveImContactFromGroup</span></span>](removeimcontactfromgroup.md)
    
- [<span data-ttu-id="3ab50-135">ContactId</span><span class="sxs-lookup"><span data-stu-id="3ab50-135">ContactId</span></span>](contactid.md)
    
- [<span data-ttu-id="3ab50-136">GroupId</span><span class="sxs-lookup"><span data-stu-id="3ab50-136">GroupId</span></span>](groupid.md)
    
## <a name="successful-removeimcontactfromgroup-operation-response"></a><span data-ttu-id="3ab50-137">RemoveImContactFromGroup 操作の応答が正常に行われる</span><span class="sxs-lookup"><span data-stu-id="3ab50-137">Successful RemoveImContactFromGroup operation response</span></span>

<span data-ttu-id="3ab50-138">次の例は、 **Removeimcontactfromgroup**操作要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="3ab50-138">The following example shows a successful response to a **RemoveImContactFromGroup** operation request.</span></span> 
  
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
      <RemoveImContactFromGroupResponse ResponseClass="Success" 
                                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </RemoveImContactFromGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="3ab50-139">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="3ab50-139">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="3ab50-140">RemoveImContactFromGroupResponse</span><span class="sxs-lookup"><span data-stu-id="3ab50-140">RemoveImContactFromGroupResponse</span></span>](removeimcontactfromgroupresponse.md)
    
- [<span data-ttu-id="3ab50-141">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="3ab50-141">ResponseCode</span></span>](responsecode.md)
    
## <a name="removeimcontactfromgroup-operation-errorinvalidimcontactid-error-response"></a><span data-ttu-id="3ab50-142">RemoveImContactFromGroup 操作 ErrorInvalidImContactId エラー応答</span><span class="sxs-lookup"><span data-stu-id="3ab50-142">RemoveImContactFromGroup operation ErrorInvalidImContactId error response</span></span>

<span data-ttu-id="3ab50-143">次の例は、 **Removeimcontactfromgroup**操作要求へのエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="3ab50-143">The following example shows an error response to a **RemoveImContactFromGroup** operation request.</span></span> <span data-ttu-id="3ab50-144">IM グループに存在しない連絡先アイテムを削除しようとすると、次のエラー応答が発生します。</span><span class="sxs-lookup"><span data-stu-id="3ab50-144">The following error response occurs when an attempt is made to remove a contact item that does not exist in the IM group.</span></span> 
  
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
      <RemoveImContactFromGroupResponse ResponseClass="Error" 
                                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified Im Contact Id is invalid.</MessageText>
         <ResponseCode>ErrorInvalidImContactId</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </RemoveImContactFromGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="3ab50-145">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="3ab50-145">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="3ab50-146">RemoveImContactFromGroupResponse</span><span class="sxs-lookup"><span data-stu-id="3ab50-146">RemoveImContactFromGroupResponse</span></span>](removeimcontactfromgroupresponse.md)
    
- [<span data-ttu-id="3ab50-147">MessageText</span><span class="sxs-lookup"><span data-stu-id="3ab50-147">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="3ab50-148">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="3ab50-148">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="3ab50-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="3ab50-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="3ab50-150">関連項目</span><span class="sxs-lookup"><span data-stu-id="3ab50-150">See also</span></span>

- [<span data-ttu-id="3ab50-151">Exchange 内の EWS のユーザーと連絡先</span><span class="sxs-lookup"><span data-stu-id="3ab50-151">People and contacts in EWS in Exchange</span></span>](https://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [<span data-ttu-id="3ab50-152">AddDistributionGroupToImList</span><span class="sxs-lookup"><span data-stu-id="3ab50-152">AddDistributionGroupToImList</span></span>](adddistributiongrouptoimlist-operation.md)
    
- [<span data-ttu-id="3ab50-153">AddImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="3ab50-153">AddImContactToGroup</span></span>](addimcontacttogroup-operation.md)
    
- [<span data-ttu-id="3ab50-154">AddImGroup 操作</span><span class="sxs-lookup"><span data-stu-id="3ab50-154">AddImGroup operation</span></span>](addimgroup-operation.md)
    
- [<span data-ttu-id="3ab50-155">AddNewImContactToGroup 操作</span><span class="sxs-lookup"><span data-stu-id="3ab50-155">AddNewImContactToGroup operation</span></span>](addnewimcontacttogroup-operation.md)
    
- [<span data-ttu-id="3ab50-156">GetImItemList 操作</span><span class="sxs-lookup"><span data-stu-id="3ab50-156">GetImItemList operation</span></span>](getimitemlist-operation.md)
    
- [<span data-ttu-id="3ab50-157">GetImItems</span><span class="sxs-lookup"><span data-stu-id="3ab50-157">GetImItems</span></span>](getimitems-operation.md)
    
- [<span data-ttu-id="3ab50-158">RemoveContactFromImList</span><span class="sxs-lookup"><span data-stu-id="3ab50-158">RemoveContactFromImList</span></span>](removecontactfromimlist-operation.md)
    
- [<span data-ttu-id="3ab50-159">RemoveDistributionGroupFromImList</span><span class="sxs-lookup"><span data-stu-id="3ab50-159">RemoveDistributionGroupFromImList</span></span>](removedistributiongroupfromimlist-operation.md)
    
- [<span data-ttu-id="3ab50-160">RemoveImGroup 操作</span><span class="sxs-lookup"><span data-stu-id="3ab50-160">RemoveImGroup operation</span></span>](removeimgroup-operation.md)
    
- [<span data-ttu-id="3ab50-161">SetImGroup 操作</span><span class="sxs-lookup"><span data-stu-id="3ab50-161">SetImGroup operation</span></span>](setimgroup-operation.md)
    
- [<span data-ttu-id="3ab50-162">SetImListMigrationCompleted</span><span class="sxs-lookup"><span data-stu-id="3ab50-162">SetImListMigrationCompleted</span></span>](setimlistmigrationcompleted-operation.md)
    

