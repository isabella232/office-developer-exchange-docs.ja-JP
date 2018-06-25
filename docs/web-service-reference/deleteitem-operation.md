---
title: DeleteItem の操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteItem
api_type:
- schema
ms.assetid: 3e26c416-fa12-476e-bfd2-5c1f4bb7b348
description: DeleteItem 操作は、Exchange ストア内の項目を削除します。
ms.openlocfilehash: 87d7853daa5db0cd87b3f6469c228a584b4d9caf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759985"
---
# <a name="deleteitem-operation"></a><span data-ttu-id="5068f-103">DeleteItem の操作</span><span class="sxs-lookup"><span data-stu-id="5068f-103">DeleteItem operation</span></span>

<span data-ttu-id="5068f-104">**DeleteItem**操作は、Exchange ストア内の項目を削除します。</span><span class="sxs-lookup"><span data-stu-id="5068f-104">The **DeleteItem** operation deletes items in the Exchange store.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="5068f-105">デリゲートは、DisposalType を MoveToDeletedItems に設定することによって、プリンシパルのメールボックス内のアイテムを削除するのにはしようとすると、 **DeleteItem**操作の ErrorCannotDeleteObject のエラー コードが含まれるエラー応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="5068f-105">An error response that includes the ErrorCannotDeleteObject error code will be returned for a **DeleteItem** operation when a delegate tries to delete an item in the principal's mailbox by setting the DisposalType to MoveToDeletedItems.</span></span> <span data-ttu-id="5068f-106">アイテムを削除するには、削除済みアイテム フォルダーに移動すること、代理人は[MoveItem 操作](moveitem-operation.md)を使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="5068f-106">To delete an item by moving it to the Deleted Items folder, a delegate must use the [MoveItem operation](moveitem-operation.md).</span></span> 
  
## <a name="deleteitem-request-example"></a><span data-ttu-id="5068f-107">DeleteItem 要求の例</span><span class="sxs-lookup"><span data-stu-id="5068f-107">DeleteItem request example</span></span>

### <a name="description"></a><span data-ttu-id="5068f-108">説明</span><span class="sxs-lookup"><span data-stu-id="5068f-108">Description</span></span>

<span data-ttu-id="5068f-109">**DeleteItem**要求の次の例では、メールボックスからアイテムを削除してハードを実行する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="5068f-109">The following example of a **DeleteItem** request shows how to perform a hard delete of an item from a mailbox.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="5068f-110">品目 ID が小さすぎると読みやすさを維持します。</span><span class="sxs-lookup"><span data-stu-id="5068f-110">The item ID has been shortened to preserve readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="5068f-111">コード</span><span class="sxs-lookup"><span data-stu-id="5068f-111">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <DeleteItem DeleteType="HardDelete" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemIds>
        <t:ItemId Id="AS4AUn=="/>
      </ItemIds>
    </DeleteItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="5068f-112">要素を要求します。</span><span class="sxs-lookup"><span data-stu-id="5068f-112">Request elements</span></span>

<span data-ttu-id="5068f-113">次の要素は、要求で使用されます。</span><span class="sxs-lookup"><span data-stu-id="5068f-113">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="5068f-114">DeleteItem</span><span class="sxs-lookup"><span data-stu-id="5068f-114">DeleteItem</span></span>](deleteitem.md)
    
- [<span data-ttu-id="5068f-115">Itemid</span><span class="sxs-lookup"><span data-stu-id="5068f-115">ItemIds</span></span>](itemids.md)
    
- [<span data-ttu-id="5068f-116">ItemId</span><span class="sxs-lookup"><span data-stu-id="5068f-116">ItemId</span></span>](itemid.md)
    
<span data-ttu-id="5068f-117">**DeleteItem**操作の要求メッセージには、他のオプションを検索するには、スキーマの階層構造を表示します。</span><span class="sxs-lookup"><span data-stu-id="5068f-117">To find other options for the request message of the **DeleteItem** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="5068f-118">[DeleteItem](deleteitem.md)要素から開始します。</span><span class="sxs-lookup"><span data-stu-id="5068f-118">Start at the [DeleteItem](deleteitem.md) element.</span></span> 
  
## <a name="successful-deleteitem-response"></a><span data-ttu-id="5068f-119">DeleteItem の正常な応答</span><span class="sxs-lookup"><span data-stu-id="5068f-119">Successful DeleteItem response</span></span>

### <a name="description"></a><span data-ttu-id="5068f-120">説明</span><span class="sxs-lookup"><span data-stu-id="5068f-120">Description</span></span>

<span data-ttu-id="5068f-121">**DeleteItem**要求に正常な応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5068f-121">The following example shows a successful response to the **DeleteItem** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="5068f-122">コード</span><span class="sxs-lookup"><span data-stu-id="5068f-122">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <DeleteItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:DeleteItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:DeleteItemResponseMessage>
      </m:ResponseMessages>
    </DeleteItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a><span data-ttu-id="5068f-123">正常な応答の要素</span><span class="sxs-lookup"><span data-stu-id="5068f-123">Successful response elements</span></span>

<span data-ttu-id="5068f-124">次の要素は、応答で使用されます。</span><span class="sxs-lookup"><span data-stu-id="5068f-124">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="5068f-125">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="5068f-125">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="5068f-126">DeleteItemResponse</span><span class="sxs-lookup"><span data-stu-id="5068f-126">DeleteItemResponse</span></span>](deleteitemresponse.md)
    
- [<span data-ttu-id="5068f-127">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="5068f-127">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="5068f-128">DeleteItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="5068f-128">DeleteItemResponseMessage</span></span>](deleteitemresponsemessage.md)
    
- [<span data-ttu-id="5068f-129">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="5068f-129">ResponseCode</span></span>](responsecode.md)
    
<span data-ttu-id="5068f-130">**DeleteItem**操作の応答メッセージには、他のオプションを検索するには、スキーマの階層構造を表示します。</span><span class="sxs-lookup"><span data-stu-id="5068f-130">To find other options for the response message of the **DeleteItem** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="5068f-131">[DeleteItemResponse](deleteitemresponse.md)要素から開始します。</span><span class="sxs-lookup"><span data-stu-id="5068f-131">Start at the [DeleteItemResponse](deleteitemresponse.md) element.</span></span> 
  
## <a name="deleteitem-error-response"></a><span data-ttu-id="5068f-132">DeleteItem エラー応答</span><span class="sxs-lookup"><span data-stu-id="5068f-132">DeleteItem error response</span></span>

### <a name="description"></a><span data-ttu-id="5068f-133">説明</span><span class="sxs-lookup"><span data-stu-id="5068f-133">Description</span></span>

<span data-ttu-id="5068f-134">**DeleteItem**要求に対してエラー応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5068f-134">The following example shows an error response to a **DeleteItem** request.</span></span> <span data-ttu-id="5068f-135">操作がないアイテムを削除しようとしたため、エラーが作成された Exchange ストアにします。</span><span class="sxs-lookup"><span data-stu-id="5068f-135">The error was created because the operation tried to delete an item that was not found in the Exchange store.</span></span> 
  
### <a name="code"></a><span data-ttu-id="5068f-136">コード</span><span class="sxs-lookup"><span data-stu-id="5068f-136">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <DeleteItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:DeleteItemResponseMessage ResponseClass="Error">
          <m:MessageText>The specified object was not found in the store.</m:MessageText>
          <m:ResponseCode>ErrorItemNotFound</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:DeleteItemResponseMessage>
      </m:ResponseMessages>
    </DeleteItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="5068f-137">エラー応答の要素</span><span class="sxs-lookup"><span data-stu-id="5068f-137">Error response elements</span></span>

<span data-ttu-id="5068f-138">エラー応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="5068f-138">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="5068f-139">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="5068f-139">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="5068f-140">DeleteItemResponse</span><span class="sxs-lookup"><span data-stu-id="5068f-140">DeleteItemResponse</span></span>](deleteitemresponse.md)
    
- [<span data-ttu-id="5068f-141">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="5068f-141">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="5068f-142">DeleteItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="5068f-142">DeleteItemResponseMessage</span></span>](deleteitemresponsemessage.md)
    
- [<span data-ttu-id="5068f-143">MessageText</span><span class="sxs-lookup"><span data-stu-id="5068f-143">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="5068f-144">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="5068f-144">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="5068f-145">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="5068f-145">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="5068f-146">**DeleteItem**操作の応答のエラー メッセージには、他のオプションを検索するには、スキーマの階層構造を表示します。</span><span class="sxs-lookup"><span data-stu-id="5068f-146">To find other options for the error response message of the **DeleteItem** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="5068f-147">[DeleteItemResponse](deleteitemresponse.md)要素から開始します。</span><span class="sxs-lookup"><span data-stu-id="5068f-147">Start at the [DeleteItemResponse](deleteitemresponse.md) element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="5068f-148">関連項目</span><span class="sxs-lookup"><span data-stu-id="5068f-148">See also</span></span>

- [<span data-ttu-id="5068f-149">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="5068f-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="5068f-150">連絡先を削除します。</span><span class="sxs-lookup"><span data-stu-id="5068f-150">Deleting Contacts</span></span>](http://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)  
- [<span data-ttu-id="5068f-151">電子メール メッセージを削除します。</span><span class="sxs-lookup"><span data-stu-id="5068f-151">Deleting E-mail Messages</span></span>](http://msdn.microsoft.com/library/c40f2f0b-dae0-412f-b716-727e8c0949b4%28Office.15%29.aspx) 
- [<span data-ttu-id="5068f-152">タスクを削除します。</span><span class="sxs-lookup"><span data-stu-id="5068f-152">Deleting Tasks</span></span>](http://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

