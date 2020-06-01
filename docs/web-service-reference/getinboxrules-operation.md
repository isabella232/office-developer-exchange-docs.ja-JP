---
title: GetInboxRules の操作
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
description: Getinbox Rules 操作は、Exchange Web サービスを使用して、識別されたユーザーのメールボックス内の受信トレイルールを取得します。
ms.openlocfilehash: f4c4c03f55c9f32be4a067024f4387888edd5fe9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457936"
---
# <a name="getinboxrules-operation"></a><span data-ttu-id="92f74-103">GetInboxRules の操作</span><span class="sxs-lookup"><span data-stu-id="92f74-103">GetInboxRules operation</span></span>

<span data-ttu-id="92f74-104">**Getinbox rules**操作は、Exchange Web サービスを使用して、識別されたユーザーのメールボックス内の受信トレイルールを取得します。</span><span class="sxs-lookup"><span data-stu-id="92f74-104">The **GetInboxRules** operation uses Exchange Web Services to retrieve Inbox rules in the identified user's mailbox.</span></span> 
  
## <a name="getinboxrules-request-example"></a><span data-ttu-id="92f74-105">Get受信トレイの要求の例</span><span class="sxs-lookup"><span data-stu-id="92f74-105">GetInboxRules request example</span></span>

### <a name="description"></a><span data-ttu-id="92f74-106">説明</span><span class="sxs-lookup"><span data-stu-id="92f74-106">Description</span></span>

<span data-ttu-id="92f74-107">次の例は、クライアントがサーバーに送信する要求 XML を示しています。</span><span class="sxs-lookup"><span data-stu-id="92f74-107">The following example shows the request XML that the client sends to the server.</span></span> <span data-ttu-id="92f74-108">この要求は、 [MailboxSmtpAddress](mailboxsmtpaddress.md)要素でユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="92f74-108">The request identifies the user in the [MailboxSmtpAddress](mailboxsmtpaddress.md) element.</span></span> <span data-ttu-id="92f74-109">識別されたユーザーのすべての受信トレイルールが応答で返されます。</span><span class="sxs-lookup"><span data-stu-id="92f74-109">All Inbox rules for the identified user are to be returned in the response.</span></span> 
  
### <a name="code"></a><span data-ttu-id="92f74-110">コード</span><span class="sxs-lookup"><span data-stu-id="92f74-110">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
        xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
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

### <a name="request-elements"></a><span data-ttu-id="92f74-111">Request 要素</span><span class="sxs-lookup"><span data-stu-id="92f74-111">Request elements</span></span>

<span data-ttu-id="92f74-112">要求には、次のオプションの要素が含まれます。</span><span class="sxs-lookup"><span data-stu-id="92f74-112">The request includes the following optional element:</span></span>
  
- [<span data-ttu-id="92f74-113">MailboxSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="92f74-113">MailboxSmtpAddress</span></span>](mailboxsmtpaddress.md)
    
## <a name="successful-getinboxrules-response-example"></a><span data-ttu-id="92f74-114">成功した Get受信トレイの応答の例</span><span class="sxs-lookup"><span data-stu-id="92f74-114">Successful GetInboxRules response example</span></span>

### <a name="description"></a><span data-ttu-id="92f74-115">説明</span><span class="sxs-lookup"><span data-stu-id="92f74-115">Description</span></span>

<span data-ttu-id="92f74-116">次の簡易オブジェクトアクセスプロトコル (SOAP) 本文の例は、 **Get受信トレイ**の要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="92f74-116">The following Simple Object Access Protocol (SOAP) body example shows a successful response to the **GetInboxRules** request.</span></span> <span data-ttu-id="92f74-117">この例では、応答に1つのルールが含まれています。</span><span class="sxs-lookup"><span data-stu-id="92f74-117">In this example, the response includes one rule.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="92f74-118">[FolderId](folderid.md)要素の**Id**および**changekey**属性の値は、読みやすさを維持するために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="92f74-118">The values of the **Id** and the **ChangeKey** attributes of the [FolderId](folderid.md) element have been shortened to preserve readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="92f74-119">コード</span><span class="sxs-lookup"><span data-stu-id="92f74-119">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14"
        MinorVersion="1" MajorBuildNumber="139"
        MinorBuildNumber="0"
        Version="Exchange2010_SP1"
        xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
        xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
        xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetInboxRulesResponse ResponseClass="Success"
        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <OutlookRuleBlobExists>true</OutlookRuleBlobExists>
      <InboxRules>
        <Rule xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

### <a name="response-elements"></a><span data-ttu-id="92f74-120">Response 要素</span><span class="sxs-lookup"><span data-stu-id="92f74-120">Response elements</span></span>

<span data-ttu-id="92f74-121">応答には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="92f74-121">The following elements are included in the response:</span></span>
  
- [<span data-ttu-id="92f74-122">Get受信規則の応答</span><span class="sxs-lookup"><span data-stu-id="92f74-122">GetInboxRulesResponse</span></span>](getinboxrulesresponse.md)
    
- [<span data-ttu-id="92f74-123">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="92f74-123">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="92f74-124">OutlookRuleBlobExists</span><span class="sxs-lookup"><span data-stu-id="92f74-124">OutlookRuleBlobExists</span></span>](outlookruleblobexists.md)
    
- [<span data-ttu-id="92f74-125">受信トレイのルール</span><span class="sxs-lookup"><span data-stu-id="92f74-125">InboxRules</span></span>](inboxrules.md)
    
## <a name="see-also"></a><span data-ttu-id="92f74-126">関連項目</span><span class="sxs-lookup"><span data-stu-id="92f74-126">See also</span></span>



[<span data-ttu-id="92f74-127">UpdateInboxRules 操作</span><span class="sxs-lookup"><span data-stu-id="92f74-127">UpdateInboxRules operation</span></span>](updateinboxrules-operation.md)

