---
title: CopyItem の操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopyItem
api_type:
- schema
ms.assetid: bcc68f9e-d511-4c29-bba6-ed535524624a
description: CopyItem の操作は、項目をコピーし、別のフォルダーにアイテムを配置します。
ms.openlocfilehash: 95d2371e9185aa25f40eaec37dda54276a54d321
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759783"
---
# <a name="copyitem-operation"></a><span data-ttu-id="01a33-103">CopyItem の操作</span><span class="sxs-lookup"><span data-stu-id="01a33-103">CopyItem operation</span></span>

<span data-ttu-id="01a33-104">**CopyItem**の操作は、項目をコピーし、別のフォルダーにアイテムを配置します。</span><span class="sxs-lookup"><span data-stu-id="01a33-104">The **CopyItem** operation copies items and puts the items in a different folder.</span></span> 
  
## <a name="copyitem-request-example"></a><span data-ttu-id="01a33-105">CopyItem 要求の例</span><span class="sxs-lookup"><span data-stu-id="01a33-105">CopyItem request example</span></span>

### <a name="description"></a><span data-ttu-id="01a33-106">説明</span><span class="sxs-lookup"><span data-stu-id="01a33-106">Description</span></span>

<span data-ttu-id="01a33-107">**CopyItem**要求の次の例では、受信トレイにアイテムをコピーするための要求を作成する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="01a33-107">The following example of a **CopyItem** request shows how to form a request to copy an item to the Inbox.</span></span> 
  
### <a name="code"></a><span data-ttu-id="01a33-108">コード</span><span class="sxs-lookup"><span data-stu-id="01a33-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CopyItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ToFolderId>
        <t:DistinguishedFolderId Id="inbox"/>
      </ToFolderId>
      <ItemIds>
        <t:ItemId Id="AS4AUnV="/>
      </ItemIds>
    </CopyItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="01a33-109">コメント</span><span class="sxs-lookup"><span data-stu-id="01a33-109">Comments</span></span>

> [!NOTE]
> <span data-ttu-id="01a33-110">フォルダー ID と変更キーは、読みやすさを保持するために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="01a33-110">The folder ID and the change key have been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="01a33-111">要素を要求します。</span><span class="sxs-lookup"><span data-stu-id="01a33-111">Request elements</span></span>

<span data-ttu-id="01a33-112">次の要素は、要求で使用されます。</span><span class="sxs-lookup"><span data-stu-id="01a33-112">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="01a33-113">CopyItem</span><span class="sxs-lookup"><span data-stu-id="01a33-113">CopyItem</span></span>](copyitem.md)
    
- [<span data-ttu-id="01a33-114">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="01a33-114">ToFolderId</span></span>](tofolderid.md)
    
- [<span data-ttu-id="01a33-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="01a33-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="01a33-116">Itemid</span><span class="sxs-lookup"><span data-stu-id="01a33-116">ItemIds</span></span>](itemids.md)
    
- [<span data-ttu-id="01a33-117">ItemId</span><span class="sxs-lookup"><span data-stu-id="01a33-117">ItemId</span></span>](itemid.md)
    
> [!NOTE]
> <span data-ttu-id="01a33-118">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="01a33-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span> 
  
<span data-ttu-id="01a33-119">**CopyItem**操作の要求メッセージには、他のオプションを検索するには、スキーマの階層構造を表示します。</span><span class="sxs-lookup"><span data-stu-id="01a33-119">To find other options for the request message of the **CopyItem** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="01a33-120">[CopyItem](copyitem.md)要素から開始します。</span><span class="sxs-lookup"><span data-stu-id="01a33-120">Start at the [CopyItem](copyitem.md) element.</span></span> 
  
## <a name="successful-copyitem-response"></a><span data-ttu-id="01a33-121">CopyItem の正常な応答</span><span class="sxs-lookup"><span data-stu-id="01a33-121">Successful CopyItem Response</span></span>

### <a name="description"></a><span data-ttu-id="01a33-122">説明</span><span class="sxs-lookup"><span data-stu-id="01a33-122">Description</span></span>

<span data-ttu-id="01a33-123">**CopyItem**要求に正常な応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="01a33-123">The following example shows a successful response to the **CopyItem** request.</span></span> 
  
<span data-ttu-id="01a33-124">応答メッセージでは、新しい項目の項目の識別子が返されます。</span><span class="sxs-lookup"><span data-stu-id="01a33-124">The item identifier of the new item is returned in the response message.</span></span> <span data-ttu-id="01a33-125">**CopyItem**のパブリック フォルダーの管理には、間のメールボックスまたはメールボックスの応答に項目の識別子は返されません。</span><span class="sxs-lookup"><span data-stu-id="01a33-125">Item identifiers are not returned in responses for cross-mailbox or mailbox to public folder **CopyItem** operations.</span></span> 
  
### <a name="code"></a><span data-ttu-id="01a33-126">コード</span><span class="sxs-lookup"><span data-stu-id="01a33-126">Code</span></span>

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
    <CopyItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CopyItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Message>
              <t:ItemID Id="AAMkAd" ChangeKey="FwAAABY" />
            </t:Message>
          </m:Items>
        </m:CopyItemResponseMessage>
      </m:ResponseMessages>
    </CopyItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a><span data-ttu-id="01a33-127">正常な応答の要素</span><span class="sxs-lookup"><span data-stu-id="01a33-127">Successful response elements</span></span>

<span data-ttu-id="01a33-128">次の要素は、応答で使用されます。</span><span class="sxs-lookup"><span data-stu-id="01a33-128">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="01a33-129">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="01a33-129">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="01a33-130">CopyItemResponse</span><span class="sxs-lookup"><span data-stu-id="01a33-130">CopyItemResponse</span></span>](copyitemresponse.md)
    
- [<span data-ttu-id="01a33-131">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="01a33-131">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="01a33-132">CopyItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="01a33-132">CopyItemResponseMessage</span></span>](copyitemresponsemessage.md)
    
- [<span data-ttu-id="01a33-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="01a33-133">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="01a33-134">Items</span><span class="sxs-lookup"><span data-stu-id="01a33-134">Items</span></span>](items.md)
    
<span data-ttu-id="01a33-135">**CopyItem**操作の応答メッセージには、他のオプションを検索するには、スキーマの階層構造を表示します。</span><span class="sxs-lookup"><span data-stu-id="01a33-135">To find other options for the response message of the **CopyItem** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="01a33-136">[CopyItemResponse](copyitemresponse.md)要素から開始します。</span><span class="sxs-lookup"><span data-stu-id="01a33-136">Start at the [CopyItemResponse](copyitemresponse.md) element.</span></span> 
  
## <a name="copyitem-error-response"></a><span data-ttu-id="01a33-137">CopyItem エラー応答</span><span class="sxs-lookup"><span data-stu-id="01a33-137">CopyItem error response</span></span>

### <a name="description"></a><span data-ttu-id="01a33-138">説明</span><span class="sxs-lookup"><span data-stu-id="01a33-138">Description</span></span>

<span data-ttu-id="01a33-139">**CopyItem**要求に対してエラー応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="01a33-139">The following example shows an error response to a **CopyItem** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="01a33-140">コード</span><span class="sxs-lookup"><span data-stu-id="01a33-140">Code</span></span>

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
    <CopyItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CopyItemResponseMessage ResponseClass="Error">
          <m:MessageText>Id is malformed.</m:MessageText>
          <m:ResponseCode>ErrorInvalidIdMalformed</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Items />
        </m:CopyItemResponseMessage>
      </m:ResponseMessages>
    </CopyItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="01a33-141">エラー応答の要素</span><span class="sxs-lookup"><span data-stu-id="01a33-141">Error response elements</span></span>

<span data-ttu-id="01a33-142">エラー応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="01a33-142">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="01a33-143">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="01a33-143">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="01a33-144">CopyItemResponse</span><span class="sxs-lookup"><span data-stu-id="01a33-144">CopyItemResponse</span></span>](copyitemresponse.md)
    
- [<span data-ttu-id="01a33-145">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="01a33-145">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="01a33-146">CopyItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="01a33-146">CopyItemResponseMessage</span></span>](copyitemresponsemessage.md)
    
- [<span data-ttu-id="01a33-147">MessageText</span><span class="sxs-lookup"><span data-stu-id="01a33-147">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="01a33-148">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="01a33-148">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="01a33-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="01a33-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="01a33-150">Items</span><span class="sxs-lookup"><span data-stu-id="01a33-150">Items</span></span>](items.md)
    
<span data-ttu-id="01a33-151">**CopyItem**操作の応答のエラー メッセージには、他のオプションを検索するには、スキーマの階層構造を表示します。</span><span class="sxs-lookup"><span data-stu-id="01a33-151">To find other options for the error response message of the **CopyItem** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="01a33-152">[CopyItemResponse](copyitemresponse.md)要素から開始します。</span><span class="sxs-lookup"><span data-stu-id="01a33-152">Start at the [CopyItemResponse](copyitemresponse.md) element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="01a33-153">関連項目</span><span class="sxs-lookup"><span data-stu-id="01a33-153">See also</span></span>



- [<span data-ttu-id="01a33-154">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="01a33-154">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

