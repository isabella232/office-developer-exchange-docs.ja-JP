---
title: UpdateInboxRules の操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateInboxRules
api_type:
- schema
ms.assetid: f982a237-471e-45c5-a2b5-468cfc53150b
description: Updateinbox Rules 操作は、指定された操作を適用することによって、認証済みのユーザーの受信トレイルールを更新します。 Updateinbox ルールは、受信トレイルールを作成したり、受信トレイルールを設定したり、受信トレイルールを削除したりするために使用します。
ms.openlocfilehash: a6ced4be25c6fe4649ad649ba01194791548bf67
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44531001"
---
# <a name="updateinboxrules-operation"></a><span data-ttu-id="5009a-104">UpdateInboxRules の操作</span><span class="sxs-lookup"><span data-stu-id="5009a-104">UpdateInboxRules operation</span></span>

<span data-ttu-id="5009a-105">Updateinbox Rules 操作は、指定された操作を適用することによって、認証済みのユーザーの受信トレイルールを更新します。</span><span class="sxs-lookup"><span data-stu-id="5009a-105">The UpdateInboxRules operation updates the authenticated user's Inbox rules by applying the specified operations.</span></span> <span data-ttu-id="5009a-106">**Updateinbox**ルールは、受信トレイルールを作成したり、受信トレイルールを設定したり、受信トレイルールを削除したりするために使用します。</span><span class="sxs-lookup"><span data-stu-id="5009a-106">**UpdateInboxRules** is used to create an Inbox rule, to set an Inbox rule, or to delete an Inbox rule.</span></span> 
  
<span data-ttu-id="5009a-107">**Update受信トレイルール**操作を使用すると、Exchange Web サービスによってクライアント側の送信ルールが削除されます。</span><span class="sxs-lookup"><span data-stu-id="5009a-107">When you use the **UpdateInboxRules** operation, Exchange Web Services deletes client-side send rules.</span></span> <span data-ttu-id="5009a-108">クライアント側の送信ルールは、クライアントのルールのフォルダー関連情報 (FAI) メッセージにのみ保存されます。</span><span class="sxs-lookup"><span data-stu-id="5009a-108">Client-side send rules are stored on the client in the rule Folder Associated Information (FAI) Message and nowhere else.</span></span> <span data-ttu-id="5009a-109">EWS は既定で、このルール FAI メッセージを削除します。これは、Outlook がこれを再作成するという前提に基づいて行われます。</span><span class="sxs-lookup"><span data-stu-id="5009a-109">EWS deletes this rule FAI message by default, based on the expectation that Outlook will recreate it.</span></span> <span data-ttu-id="5009a-110">ただし、Outlook で再作成できるのは、拡張ルールとしても存在しているルールです。けれども、クライアント側の送信ルールは拡張ルールとして存在していません。</span><span class="sxs-lookup"><span data-stu-id="5009a-110">However, Outlook can't recreate rules that don't also exist as an extended rule, and client-side send rules don't exist as extended rules.</span></span> <span data-ttu-id="5009a-111">その結果、これらのルールは失われます。</span><span class="sxs-lookup"><span data-stu-id="5009a-111">As a result, these rules are lost.</span></span> <span data-ttu-id="5009a-112">ソリューションの設計時にこのことを考慮にするようお勧めします。</span><span class="sxs-lookup"><span data-stu-id="5009a-112">We suggest you consider this when designing your solution.</span></span> 
  
## <a name="updateinboxrules-create-rule-request-example"></a><span data-ttu-id="5009a-113">Update受信トレイルール (ルールの作成) 要求の例</span><span class="sxs-lookup"><span data-stu-id="5009a-113">UpdateInboxRules (Create Rule) request example</span></span>

<span data-ttu-id="5009a-114">Exchange Web サービスを使用して、Exchange ストア内のユーザーのメールボックスに受信トレイルールを作成できます。</span><span class="sxs-lookup"><span data-stu-id="5009a-114">You can use Exchange Web Services to create an Inbox rule in a user's mailbox in the Exchange store.</span></span> <span data-ttu-id="5009a-115">ルールを作成するには、 [CreateRuleOperation](createruleoperation.md)要素と共に[update受信トレイルール](updateinboxrules.md)要素を使用します。</span><span class="sxs-lookup"><span data-stu-id="5009a-115">Use the [UpdateInboxRules](updateinboxrules.md) element in conjunction with the [CreateRuleOperation](createruleoperation.md) element to create a rule.</span></span> 
  
### <a name="description"></a><span data-ttu-id="5009a-116">Description</span><span class="sxs-lookup"><span data-stu-id="5009a-116">Description</span></span>

<span data-ttu-id="5009a-117">クライアントは、要求 XML を構築し、サーバーに送信します。</span><span class="sxs-lookup"><span data-stu-id="5009a-117">The client constructs the request XML and sends it to the server.</span></span>
  
### <a name="code"></a><span data-ttu-id="5009a-118">コード</span><span class="sxs-lookup"><span data-stu-id="5009a-118">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version ="Exchange2010_SP1"/>
  </soap:Header>
  <soap:Body>
      <m:UpdateInboxRules>
        <m:RemoveOutlookRuleBlob>true</m:RemoveOutlookRuleBlob>
        <m:Operations>
          <t:CreateRuleOperation>
            <t:Rule>
              <t:DisplayName>MoveInterestingToJunk</t:DisplayName>
              <t:Priority>1</t:Priority>
              <t:IsEnabled>true</t:IsEnabled>
              <t:Conditions>
                <t:ContainsSubjectStrings>
                  <t:String>Interesting</t:String>
                </t:ContainsSubjectStrings>
              </t:Conditions>
              <t:Exceptions />
              <t:Actions>
                <t:MoveToFolder>
                  <t:DistinguishedFolderId Id="junkemail" />
                </t:MoveToFolder>
              </t:Actions>
            </t:Rule>
          </t:CreateRuleOperation>
        </m:Operations>
      </m:UpdateInboxRules>
  </soap:Body>
</soap:Envelope>

```

### <a name="comments"></a><span data-ttu-id="5009a-119">コメント</span><span class="sxs-lookup"><span data-stu-id="5009a-119">Comments</span></span>

<span data-ttu-id="5009a-120">この例では、電子メールの件名に "おもしろい" という文字列が含まれている場合に、電子メールメッセージを [迷惑メール] フォルダーに移動するルールを作成します。</span><span class="sxs-lookup"><span data-stu-id="5009a-120">This example builds a rule that will move an e-mail message to the Junk E-mail folder if the e-mail subject contains a string that equals "Interesting".</span></span>
  
### <a name="request-elements"></a><span data-ttu-id="5009a-121">Request 要素</span><span class="sxs-lookup"><span data-stu-id="5009a-121">Request elements</span></span>

<span data-ttu-id="5009a-122">**Update受信トレイルール**要求には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5009a-122">The **UpdateInboxRules** request includes the following elements:</span></span> 
  
- [<span data-ttu-id="5009a-123">MailboxSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="5009a-123">MailboxSmtpAddress</span></span>](mailboxsmtpaddress.md)
    
- [<span data-ttu-id="5009a-124">RemoveOutlookRuleBlob</span><span class="sxs-lookup"><span data-stu-id="5009a-124">RemoveOutlookRuleBlob</span></span>](removeoutlookruleblob.md)
    
- [<span data-ttu-id="5009a-125">Operations</span><span class="sxs-lookup"><span data-stu-id="5009a-125">Operations</span></span>](operations.md)
    
<span data-ttu-id="5009a-126">[操作](operations.md)要素には、ルールを作成するための[CreateRuleOperation](createruleoperation.md)要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5009a-126">The [Operations](operations.md) element contains the [CreateRuleOperation](createruleoperation.md) element to create a rule.</span></span> 
  
## <a name="updateinboxrules-create-rule-response-example"></a><span data-ttu-id="5009a-127">Update受信トレイルール (作成ルール) の応答の例</span><span class="sxs-lookup"><span data-stu-id="5009a-127">UpdateInboxRules (Create Rule) response example</span></span>

### <a name="description"></a><span data-ttu-id="5009a-128">Description</span><span class="sxs-lookup"><span data-stu-id="5009a-128">Description</span></span>

<span data-ttu-id="5009a-129">次の簡易オブジェクトアクセスプロトコル (SOAP) 本文の例は、ルールを作成する**Update受信トレイルール**要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="5009a-129">The following Simple Object Access Protocol (SOAP) body example shows a successful response to the **UpdateInboxRules** request that creates a rule.</span></span> 
  
### <a name="code"></a><span data-ttu-id="5009a-130">コード</span><span class="sxs-lookup"><span data-stu-id="5009a-130">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
        MinorVersion="1" 
        MajorBuildNumber="139" 
        MinorBuildNumber="0" Version="Exchange2010_SP1" 
        xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <UpdateInboxRulesResponse 
         ResponseClass="Success" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
    </UpdateInboxRulesResponse>
  </s:Body>
</s:Envelope>

```

### <a name="successful-response-elements"></a><span data-ttu-id="5009a-131">成功した応答要素</span><span class="sxs-lookup"><span data-stu-id="5009a-131">Successful response elements</span></span>

<span data-ttu-id="5009a-132">応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="5009a-132">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="5009a-133">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="5009a-133">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="5009a-134">Update受信トレイルールの応答</span><span class="sxs-lookup"><span data-stu-id="5009a-134">UpdateInboxRulesResponse</span></span>](updateinboxrulesresponse.md)
    
- [<span data-ttu-id="5009a-135">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="5009a-135">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="5009a-136">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="5009a-136">ResponseCode</span></span>](responsecode.md)
    
## <a name="updateinboxrules-set-rule-request-example"></a><span data-ttu-id="5009a-137">Update受信トレイルール (Set Rule) 要求の例</span><span class="sxs-lookup"><span data-stu-id="5009a-137">UpdateInboxRules (Set Rule) request example</span></span>

<span data-ttu-id="5009a-138">Exchange Web サービスを使用して、Exchange ストア内のユーザーのメールボックスの受信トレイルールを変更できます。</span><span class="sxs-lookup"><span data-stu-id="5009a-138">You can use Exchange Web Services to modify an Inbox rule in a user's mailbox in the Exchange store.</span></span> <span data-ttu-id="5009a-139">ルールを変更するには、 [SetRuleOperation](setruleoperation.md)要素と共に[update受信トレイルール](updateinboxrules.md)要素を使用します。</span><span class="sxs-lookup"><span data-stu-id="5009a-139">Use the [UpdateInboxRules](updateinboxrules.md) element in conjunction with the [SetRuleOperation](setruleoperation.md) element to modify a rule.</span></span> 
  
### <a name="description"></a><span data-ttu-id="5009a-140">Description</span><span class="sxs-lookup"><span data-stu-id="5009a-140">Description</span></span>

<span data-ttu-id="5009a-141">クライアントは、要求 XML を構築し、サーバーに送信します。</span><span class="sxs-lookup"><span data-stu-id="5009a-141">The client constructs the request XML and sends it to the server.</span></span>
  
### <a name="code"></a><span data-ttu-id="5009a-142">コード</span><span class="sxs-lookup"><span data-stu-id="5009a-142">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version ="Exchange2010_SP1"/>
  </soap:Header>
  <soap:Body>
      <m:UpdateInboxRules>
        <m:RemoveOutlookRuleBlob>true</m:RemoveOutlookRuleBlob>
        <Operations xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
          <SetRuleOperation xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
            <Rule>
              <RuleId>Nh8AAAAwW/w=</RuleId>
              <DisplayName>(Modified) This is Junk</DisplayName>
              <Priority>1</Priority>
              <IsEnabled>true</IsEnabled>
              <Conditions>
                <ContainsSubjectStrings>
                  <String>Interesting</String>
                </ContainsSubjectStrings>
              </Conditions>
              <Actions>
                <MoveToFolder>
                  <FolderId Id="AAMkADQ1YTE1" ChangeKey="AQAAAA==" />
                </MoveToFolder>
              </Actions>
            </Rule>
          </SetRuleOperation>
        </Operations>
      </m:UpdateInboxRules>
  </soap:Body>
</soap:Envelope>

```

### <a name="comments"></a><span data-ttu-id="5009a-143">コメント</span><span class="sxs-lookup"><span data-stu-id="5009a-143">Comments</span></span>

<span data-ttu-id="5009a-144">次の使用例は、表示名を "(変更) が迷惑メールである" に変更します。</span><span class="sxs-lookup"><span data-stu-id="5009a-144">This example changes the display name to "(Modified) This is Junk".</span></span>
  
> [!NOTE]
> <span data-ttu-id="5009a-145">[FolderId](folderid.md)要素の**Id**および**changekey**属性の値は、読みやすくするために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="5009a-145">The values of the **Id** and **ChangeKey** attributes of the [FolderId](folderid.md) element have been shortened for readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="5009a-146">Request 要素</span><span class="sxs-lookup"><span data-stu-id="5009a-146">Request elements</span></span>

<span data-ttu-id="5009a-147">**Update受信トレイルール**要求には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5009a-147">The **UpdateInboxRules** request includes the following elements:</span></span> 
  
- [<span data-ttu-id="5009a-148">MailboxSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="5009a-148">MailboxSmtpAddress</span></span>](mailboxsmtpaddress.md)
    
- [<span data-ttu-id="5009a-149">RemoveOutlookRuleBlob</span><span class="sxs-lookup"><span data-stu-id="5009a-149">RemoveOutlookRuleBlob</span></span>](removeoutlookruleblob.md)
    
- [<span data-ttu-id="5009a-150">Operations</span><span class="sxs-lookup"><span data-stu-id="5009a-150">Operations</span></span>](operations.md)
    
<span data-ttu-id="5009a-151">[操作](operations.md)要素には、ルールを変更するための[SetRuleOperation](setruleoperation.md)要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5009a-151">The [Operations](operations.md) element contains the [SetRuleOperation](setruleoperation.md) element to modify a rule.</span></span> 
  
## <a name="updateinboxrules-set-rule-response-example"></a><span data-ttu-id="5009a-152">Update受信トレイルール (Set Rule) response の例</span><span class="sxs-lookup"><span data-stu-id="5009a-152">UpdateInboxRules (Set Rule) response example</span></span>

### <a name="description"></a><span data-ttu-id="5009a-153">Description</span><span class="sxs-lookup"><span data-stu-id="5009a-153">Description</span></span>

<span data-ttu-id="5009a-154">次の簡易オブジェクトアクセスプロトコル (SOAP) 本文の例は、ルールを変更する**Update受信トレイルール**要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="5009a-154">The following Simple Object Access Protocol (SOAP) body example shows a successful response to the **UpdateInboxRules** request that modifies a rule.</span></span> 
  
### <a name="code"></a><span data-ttu-id="5009a-155">コード</span><span class="sxs-lookup"><span data-stu-id="5009a-155">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
        MinorVersion="1" 
        MajorBuildNumber="139" 
        MinorBuildNumber="0" 
        Version="Exchange2010_SP1" 
        xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <UpdateInboxRulesResponse 
          ResponseClass="Success" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
    </UpdateInboxRulesResponse>
  </s:Body>
</s:Envelope>

```

### <a name="successful-response-elements"></a><span data-ttu-id="5009a-156">成功した応答要素</span><span class="sxs-lookup"><span data-stu-id="5009a-156">Successful response elements</span></span>

<span data-ttu-id="5009a-157">応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="5009a-157">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="5009a-158">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="5009a-158">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="5009a-159">Update受信トレイルールの応答</span><span class="sxs-lookup"><span data-stu-id="5009a-159">UpdateInboxRulesResponse</span></span>](updateinboxrulesresponse.md)
    
- [<span data-ttu-id="5009a-160">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="5009a-160">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="5009a-161">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="5009a-161">ResponseCode</span></span>](responsecode.md)
    
## <a name="updateinboxrules-delete-rule-request-example"></a><span data-ttu-id="5009a-162">Update受信トレイルール (デリートルール) 要求の例</span><span class="sxs-lookup"><span data-stu-id="5009a-162">UpdateInboxRules (Delete Rule) request example</span></span>

<span data-ttu-id="5009a-163">Exchange Web サービスを使用して、Exchange ストア内のユーザーのメールボックスの受信トレイルールを削除できます。</span><span class="sxs-lookup"><span data-stu-id="5009a-163">You can use Exchange Web Services to delete an Inbox rule in a user's mailbox in the Exchange store.</span></span> <span data-ttu-id="5009a-164">ルールを削除するには、 [DeleteRuleOperation](deleteruleoperation.md)要素と共に[Update受信トレイルール](updateinboxrules.md)を使用します。</span><span class="sxs-lookup"><span data-stu-id="5009a-164">Use the [UpdateInboxRules](updateinboxrules.md) in conjunction with the [DeleteRuleOperation](deleteruleoperation.md) element to delete a rule.</span></span> 
  
### <a name="description"></a><span data-ttu-id="5009a-165">Description</span><span class="sxs-lookup"><span data-stu-id="5009a-165">Description</span></span>

<span data-ttu-id="5009a-166">クライアントは、要求 XML を構築し、サーバーに送信します。</span><span class="sxs-lookup"><span data-stu-id="5009a-166">The client constructs the request XML and sends it to the server.</span></span>
  
### <a name="code"></a><span data-ttu-id="5009a-167">コード</span><span class="sxs-lookup"><span data-stu-id="5009a-167">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version ="Exchange2010_SP1"/>
  </soap:Header>
  <soap:Body>
      <m:UpdateInboxRules>
        <m:RemoveOutlookRuleBlob>true</m:RemoveOutlookRuleBlob>
        <m:Operations>
          <t:DeleteRuleOperation>
            <t:RuleId>Nh8AAAAwW/U=</t:RuleId>
          </t:DeleteRuleOperation>
        </m:Operations>
      </m:UpdateInboxRules>
  </soap:Body>
</soap:Envelope>

```

### <a name="comments"></a><span data-ttu-id="5009a-168">コメント</span><span class="sxs-lookup"><span data-stu-id="5009a-168">Comments</span></span>

<span data-ttu-id="5009a-169">この例では、既存の識別されたルールを削除します。</span><span class="sxs-lookup"><span data-stu-id="5009a-169">This example deletes the existing identified rule.</span></span>
  
### <a name="request-elements"></a><span data-ttu-id="5009a-170">Request 要素</span><span class="sxs-lookup"><span data-stu-id="5009a-170">Request elements</span></span>

<span data-ttu-id="5009a-171">**Update受信トレイルール**要求には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5009a-171">The **UpdateInboxRules** request includes the following elements:</span></span> 
  
- [<span data-ttu-id="5009a-172">MailboxSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="5009a-172">MailboxSmtpAddress</span></span>](mailboxsmtpaddress.md)
    
- [<span data-ttu-id="5009a-173">RemoveOutlookRuleBlob</span><span class="sxs-lookup"><span data-stu-id="5009a-173">RemoveOutlookRuleBlob</span></span>](removeoutlookruleblob.md)
    
- [<span data-ttu-id="5009a-174">Operations</span><span class="sxs-lookup"><span data-stu-id="5009a-174">Operations</span></span>](operations.md)
    
<span data-ttu-id="5009a-175">[操作](operations.md)要素には、ルールを削除するための[DeleteRuleOperation](deleteruleoperation.md)要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5009a-175">The [Operations](operations.md) element contains the [DeleteRuleOperation](deleteruleoperation.md) element to delete a rule.</span></span> 
  
## <a name="updateinboxrules-delete-rule-response-example"></a><span data-ttu-id="5009a-176">Update受信トレイルール (デリートルール) の応答の例</span><span class="sxs-lookup"><span data-stu-id="5009a-176">UpdateInboxRules (Delete Rule) response example</span></span>

### <a name="description"></a><span data-ttu-id="5009a-177">Description</span><span class="sxs-lookup"><span data-stu-id="5009a-177">Description</span></span>

<span data-ttu-id="5009a-178">次の簡易オブジェクトアクセスプロトコル (SOAP) 本文の例は、ルールを削除する**Update受信トレイルール**要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="5009a-178">The following Simple Object Access Protocol (SOAP) body example shows a successful response to the **UpdateInboxRules** request that deletes a rule.</span></span> 
  
### <a name="code"></a><span data-ttu-id="5009a-179">コード</span><span class="sxs-lookup"><span data-stu-id="5009a-179">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
        MinorVersion="1" 
        MajorBuildNumber="139" 
        MinorBuildNumber="0" 
        Version="Exchange2010_SP1" 
        xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <UpdateInboxRulesResponse ResponseClass="Success" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
    </UpdateInboxRulesResponse>
  </s:Body>
</s:Envelope>

```

### <a name="successful-response-elements"></a><span data-ttu-id="5009a-180">成功した応答要素</span><span class="sxs-lookup"><span data-stu-id="5009a-180">Successful response elements</span></span>

<span data-ttu-id="5009a-181">応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="5009a-181">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="5009a-182">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="5009a-182">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="5009a-183">Update受信トレイルールの応答</span><span class="sxs-lookup"><span data-stu-id="5009a-183">UpdateInboxRulesResponse</span></span>](updateinboxrulesresponse.md)
    
- [<span data-ttu-id="5009a-184">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="5009a-184">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="5009a-185">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="5009a-185">ResponseCode</span></span>](responsecode.md)
    
## <a name="see-also"></a><span data-ttu-id="5009a-186">関連項目</span><span class="sxs-lookup"><span data-stu-id="5009a-186">See also</span></span>



[<span data-ttu-id="5009a-187">GetInboxRules の操作</span><span class="sxs-lookup"><span data-stu-id="5009a-187">GetInboxRules operation</span></span>](getinboxrules-operation.md)

