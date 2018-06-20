---
title: GetInboxRules 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetInboxRules
api_type:
- schema
ms.assetid: b4b2701a-4a23-4acc-8c75-19f7955ad7ae
description: GetInboxRules 操作は、識別されたユーザーのメールボックスの受信トレイ ルールを取得するために、Exchange Web サービスを使用します。
ms.openlocfilehash: f8a5068b1f189cc6fd5feef6dfec29204a0b8887
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760756"
---
# <a name="getinboxrules-operation"></a><span data-ttu-id="fc762-103">GetInboxRules 操作</span><span class="sxs-lookup"><span data-stu-id="fc762-103">GetInboxRules operation</span></span>

<span data-ttu-id="fc762-104">**GetInboxRules**操作は、識別されたユーザーのメールボックスの受信トレイ ルールを取得するために、Exchange Web サービスを使用します。</span><span class="sxs-lookup"><span data-stu-id="fc762-104">The **GetInboxRules** operation uses Exchange Web Services to retrieve Inbox rules in the identified user's mailbox.</span></span> 
  
## <a name="getinboxrules-request-example"></a><span data-ttu-id="fc762-105">GetInboxRules 要求の例</span><span class="sxs-lookup"><span data-stu-id="fc762-105">GetInboxRules request example</span></span>

### <a name="description"></a><span data-ttu-id="fc762-106">説明</span><span class="sxs-lookup"><span data-stu-id="fc762-106">Description</span></span>

<span data-ttu-id="fc762-107">要求クライアントがサーバーに送信する XML の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fc762-107">The following example shows the request XML that the client sends to the server.</span></span> <span data-ttu-id="fc762-108">要求は、 [MailboxSmtpAddress](mailboxsmtpaddress.md)要素内でユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="fc762-108">The request identifies the user in the [MailboxSmtpAddress](mailboxsmtpaddress.md) element.</span></span> <span data-ttu-id="fc762-109">識別されたユーザーのすべての受信トレイのルールでは、応答で返されます。</span><span class="sxs-lookup"><span data-stu-id="fc762-109">All Inbox rules for the identified user are to be returned in the response.</span></span> 
  
### <a name="code"></a><span data-ttu-id="fc762-110">コード</span><span class="sxs-lookup"><span data-stu-id="fc762-110">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
        xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
        xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010_SP1" />
  </soap:Header>
  <soap:Body>
    <m:GetInboxRules>
      <m:MailboxSmtpAddress>User1@Contoso.com</m:MailboxSmtpAddress>
    </m:GetInboxRules>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="fc762-111">要素を要求します。</span><span class="sxs-lookup"><span data-stu-id="fc762-111">Request elements</span></span>

<span data-ttu-id="fc762-112">要求には、次の省略可能な要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="fc762-112">The request includes the following optional element:</span></span>
  
- [<span data-ttu-id="fc762-113">MailboxSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="fc762-113">MailboxSmtpAddress</span></span>](mailboxsmtpaddress.md)
    
## <a name="successful-getinboxrules-response-example"></a><span data-ttu-id="fc762-114">成功した GetInboxRules の応答の例</span><span class="sxs-lookup"><span data-stu-id="fc762-114">Successful GetInboxRules response example</span></span>

### <a name="description"></a><span data-ttu-id="fc762-115">説明</span><span class="sxs-lookup"><span data-stu-id="fc762-115">Description</span></span>

<span data-ttu-id="fc762-116">Simple Object Access Protocol (SOAP) 本文の次の使用例は、 **GetInboxRules**要求に正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="fc762-116">The following Simple Object Access Protocol (SOAP) body example shows a successful response to the **GetInboxRules** request.</span></span> <span data-ttu-id="fc762-117">この例では、応答には、1 つのルールが含まれています。</span><span class="sxs-lookup"><span data-stu-id="fc762-117">In this example, the response includes one rule.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="fc762-118">[フォルダー Id](folderid.md)の要素の**変更キー**属性と**Id**の値は、読みやすさを保持するために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="fc762-118">The values of the **Id** and the **ChangeKey** attributes of the [FolderId](folderid.md) element have been shortened to preserve readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="fc762-119">コード</span><span class="sxs-lookup"><span data-stu-id="fc762-119">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14"
        MinorVersion="1" MajorBuildNumber="139"
        MinorBuildNumber="0"
        Version="Exchange2010_SP1"
        xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
        xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
        xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetInboxRulesResponse ResponseClass="Success"
        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <OutlookRuleBlobExists>true</OutlookRuleBlobExists>
      <InboxRules>
        <Rule xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <RuleId>dCsAAABjzvA=</RuleId>
          <DisplayName>MoveInterestingToJunk</DisplayName>
          <Priority>1</Priority>
          <IsEnabled>true</IsEnabled>
          <Conditions>
            <ContainsSubjectStrings>
              <String>Interesting</String>
            </ContainsSubjectStrings>
          </Conditions>
          <Actions>
            <MoveToFolder>
              <FolderId ChangeKey="AQAAAA==" Id="AAMkAGYzZjZm" />
            </MoveToFolder>
          </Actions>
        </Rule>
      </InboxRules>
    </GetInboxRulesResponse>
  </s:Body>
</s:Envelope>
```

### <a name="response-elements"></a><span data-ttu-id="fc762-120">応答の要素</span><span class="sxs-lookup"><span data-stu-id="fc762-120">Response elements</span></span>

<span data-ttu-id="fc762-121">応答では、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="fc762-121">The following elements are included in the response:</span></span>
  
- [<span data-ttu-id="fc762-122">GetInboxRulesResponse</span><span class="sxs-lookup"><span data-stu-id="fc762-122">GetInboxRulesResponse</span></span>](getinboxrulesresponse.md)
    
- [<span data-ttu-id="fc762-123">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="fc762-123">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="fc762-124">OutlookRuleBlobExists</span><span class="sxs-lookup"><span data-stu-id="fc762-124">OutlookRuleBlobExists</span></span>](outlookruleblobexists.md)
    
- [<span data-ttu-id="fc762-125">InboxRules</span><span class="sxs-lookup"><span data-stu-id="fc762-125">InboxRules</span></span>](inboxrules.md)
    
## <a name="see-also"></a><span data-ttu-id="fc762-126">関連項目</span><span class="sxs-lookup"><span data-stu-id="fc762-126">See also</span></span>



[<span data-ttu-id="fc762-127">UpdateInboxRules の操作</span><span class="sxs-lookup"><span data-stu-id="fc762-127">UpdateInboxRules operation</span></span>](updateinboxrules-operation.md)

