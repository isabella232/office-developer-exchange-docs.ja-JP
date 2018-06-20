---
title: ApplyConversationAction 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ApplyConversationAction
api_type:
- schema
ms.assetid: 73d7943d-d361-4f8b-9948-d85f886efa1a
description: ApplyConversationAction 操作では、設定を 1 回だけか、会話内のすべてのアイテムで次の操作をします。 ApplyConversationAction 操作を使用すると、分類、移動、コピー、削除、および会話のすべてのアイテムの読み取り状態を設定できます。 会話で新着メッセージをアクションを設定することもできます。
ms.openlocfilehash: 2a485b84ee87aec2ed807e3f4f0901b83432fa0a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759366"
---
# <a name="applyconversationaction-operation"></a><span data-ttu-id="f0a4d-105">ApplyConversationAction 操作</span><span class="sxs-lookup"><span data-stu-id="f0a4d-105">ApplyConversationAction operation</span></span>

<span data-ttu-id="f0a4d-106">**ApplyConversationAction**操作では、設定を 1 回だけか、会話内のすべてのアイテムで次の操作をします。</span><span class="sxs-lookup"><span data-stu-id="f0a4d-106">The **ApplyConversationAction** operation sets a one-time or follow up action on all the items in a conversation.</span></span> <span data-ttu-id="f0a4d-107">**ApplyConversationAction**操作を使用すると、分類、移動、コピー、削除、および会話のすべてのアイテムの読み取り状態を設定できます。</span><span class="sxs-lookup"><span data-stu-id="f0a4d-107">The **ApplyConversationAction** operation allows you to categorize, move, copy, delete, and set the read state on all items in a conversation.</span></span> <span data-ttu-id="f0a4d-108">会話で新着メッセージをアクションを設定することもできます。</span><span class="sxs-lookup"><span data-stu-id="f0a4d-108">Actions can also be set for new messages in a conversation.</span></span> 
  
## <a name="applyconversationaction-request-example"></a><span data-ttu-id="f0a4d-109">ApplyConversationAction 要求の例</span><span class="sxs-lookup"><span data-stu-id="f0a4d-109">ApplyConversationAction request example</span></span>

### <a name="description"></a><span data-ttu-id="f0a4d-110">説明</span><span class="sxs-lookup"><span data-stu-id="f0a4d-110">Description</span></span>

<span data-ttu-id="f0a4d-111">**ApplyConversationAction**要求の次の例では、指定したスレッドの別のフォルダーにアイテムを移動する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="f0a4d-111">The following example of an **ApplyConversationAction** request shows how to move the items in the specified conversation to another folder.</span></span> <span data-ttu-id="f0a4d-112">会話に追加される項目は、指定したフォルダーにも移動されます。</span><span class="sxs-lookup"><span data-stu-id="f0a4d-112">Items that are added to the conversation will also be moved to the specified folder.</span></span> 
  
### <a name="code"></a><span data-ttu-id="f0a4d-113">コード</span><span class="sxs-lookup"><span data-stu-id="f0a4d-113">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010_SP1" />
  </soap:Header>
  <soap:Body>
    <m:ApplyConversationAction>
      <m:ConversationActions>
        <t:ConversationAction>
          <t:Action>AlwaysMove</t:Action>
          <t:ConversationId Id="AAQkADVkNjM1EH39AWcDUGrnrnJ32hHpdc="/>
          <t:DestinationFolderId>
            <t:FolderId Id="AAMkADVkNjM1ODI3LTEwYTAtNDUBTTT6tWal35iSoKAAAABZZWAAA="/>
          </t:DestinationFolderId>
        </t:ConversationAction>
      </m:ConversationActions>
    </m:ApplyConversationAction>
  </soap:Body>
</soap:Envelope>
```

### <a name="remarks"></a><span data-ttu-id="f0a4d-114">備考</span><span class="sxs-lookup"><span data-stu-id="f0a4d-114">Remarks</span></span>

<span data-ttu-id="f0a4d-115">会話とフォルダーの識別子は、読みやすさを保持するために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="f0a4d-115">The conversation and folder identifiers have been shortened to preserve readability.</span></span>
  
## <a name="applyconversationaction-response-example"></a><span data-ttu-id="f0a4d-116">ApplyConversationAction の応答の例</span><span class="sxs-lookup"><span data-stu-id="f0a4d-116">ApplyConversationAction response example</span></span>

### <a name="description"></a><span data-ttu-id="f0a4d-117">説明</span><span class="sxs-lookup"><span data-stu-id="f0a4d-117">Description</span></span>

<span data-ttu-id="f0a4d-118">**ApplyConversationAction**要求に正常な応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f0a4d-118">The following example shows a successful response to an **ApplyConversationAction** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="f0a4d-119">コード</span><span class="sxs-lookup"><span data-stu-id="f0a4d-119">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="1" 
                         MajorBuildNumber="91" 
                         MinorBuildNumber="0" 
                         Version="Exchange2010_SP1" 
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:ApplyConversationActionResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:ApplyConversationActionResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:ApplyConversationActionResponseMessage>
      </m:ResponseMessages>
    </m:ApplyConversationActionResponse>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="f0a4d-120">関連項目</span><span class="sxs-lookup"><span data-stu-id="f0a4d-120">See also</span></span>

- [<span data-ttu-id="f0a4d-121">ApplyConversationAction 操作</span><span class="sxs-lookup"><span data-stu-id="f0a4d-121">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)
- [<span data-ttu-id="f0a4d-122">Exchange での EWS の操作</span><span class="sxs-lookup"><span data-stu-id="f0a4d-122">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
- [<span data-ttu-id="f0a4d-123">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="f0a4d-123">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="f0a4d-124">EWS での会話</span><span class="sxs-lookup"><span data-stu-id="f0a4d-124">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

