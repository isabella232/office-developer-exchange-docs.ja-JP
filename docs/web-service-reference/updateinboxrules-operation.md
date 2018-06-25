---
title: UpdateInboxRules 操作
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
description: UpdateInboxRules 操作は、指定した操作を適用することによって認証されたユーザーの受信トレイ ルールを更新します。 UpdateInboxRules を使用して、または受信トレイ ルールを削除するのには、受信トレイ ルールを設定するのには、受信トレイのルールを作成します。
ms.openlocfilehash: 6e979421d619fed6625fe05db86c1f8c6a7418c9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839855"
---
# <a name="updateinboxrules-operation"></a><span data-ttu-id="44a3f-104">UpdateInboxRules 操作</span><span class="sxs-lookup"><span data-stu-id="44a3f-104">UpdateInboxRules operation</span></span>

<span data-ttu-id="44a3f-105">UpdateInboxRules 操作は、指定した操作を適用することによって認証されたユーザーの受信トレイ ルールを更新します。</span><span class="sxs-lookup"><span data-stu-id="44a3f-105">The UpdateInboxRules operation updates the authenticated user's Inbox rules by applying the specified operations.</span></span> <span data-ttu-id="44a3f-106">**UpdateInboxRules**を使用して、または受信トレイ ルールを削除するのには、受信トレイ ルールを設定するのには、受信トレイのルールを作成します。</span><span class="sxs-lookup"><span data-stu-id="44a3f-106">**UpdateInboxRules** is used to create an Inbox rule, to set an Inbox rule, or to delete an Inbox rule.</span></span> 
  
<span data-ttu-id="44a3f-107">**UpdateInboxRules**操作を使用する場合、Exchange Web サービスは、クライアント側の送信規則を削除します。</span><span class="sxs-lookup"><span data-stu-id="44a3f-107">When you use the **UpdateInboxRules** operation, Exchange Web Services deletes client-side send rules.</span></span> <span data-ttu-id="44a3f-108">フォルダー関連情報 (FAI) メッセージのルールでクライアントと他の場所では、クライアント側の送信規則が格納されます。</span><span class="sxs-lookup"><span data-stu-id="44a3f-108">Client-side send rules are stored on the client in the rule Folder Associated Information (FAI) Message and nowhere else.</span></span> <span data-ttu-id="44a3f-109">EWS では、既定では、Outlook は、再作成を前提に基づく FAI メッセージ ルールを削除します。</span><span class="sxs-lookup"><span data-stu-id="44a3f-109">EWS deletes this rule FAI message by default, based on the expectation that Outlook will recreate it.</span></span> <span data-ttu-id="44a3f-110">ただし、Outlook は、拡張のルールとしても存在しないルールを再作成できません、拡張ルールとクライアント側の送信規則が存在しません。</span><span class="sxs-lookup"><span data-stu-id="44a3f-110">However, Outlook can't recreate rules that don't also exist as an extended rule, and client-side send rules don't exist as extended rules.</span></span> <span data-ttu-id="44a3f-111">その結果、これらのルールは失われます。</span><span class="sxs-lookup"><span data-stu-id="44a3f-111">As a result, these rules are lost.</span></span> <span data-ttu-id="44a3f-112">ソリューションを設計するときこれを考慮することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="44a3f-112">We suggest you consider this when designing your solution.</span></span> 
  
## <a name="updateinboxrules-create-rule-request-example"></a><span data-ttu-id="44a3f-113">UpdateInboxRules (ルールの作成) の要求の例</span><span class="sxs-lookup"><span data-stu-id="44a3f-113">UpdateInboxRules (Create Rule) request example</span></span>

<span data-ttu-id="44a3f-114">Exchange Web サービスを使用すると、Exchange ストア内のユーザーのメールボックスで受信トレイ ルールを作成します。</span><span class="sxs-lookup"><span data-stu-id="44a3f-114">You can use Exchange Web Services to create an Inbox rule in a user's mailbox in the Exchange store.</span></span> <span data-ttu-id="44a3f-115">[CreateRuleOperation](createruleoperation.md)要素と組み合わせて[UpdateInboxRules](updateinboxrules.md)要素を使用して、ルールを作成します。</span><span class="sxs-lookup"><span data-stu-id="44a3f-115">Use the [UpdateInboxRules](updateinboxrules.md) element in conjunction with the [CreateRuleOperation](createruleoperation.md) element to create a rule.</span></span> 
  
### <a name="description"></a><span data-ttu-id="44a3f-116">説明</span><span class="sxs-lookup"><span data-stu-id="44a3f-116">Description</span></span>

<span data-ttu-id="44a3f-117">クライアントは、要求の XML を構築し、サーバーに送信します。</span><span class="sxs-lookup"><span data-stu-id="44a3f-117">The client constructs the request XML and sends it to the server.</span></span>
  
### <a name="code"></a><span data-ttu-id="44a3f-118">コード</span><span class="sxs-lookup"><span data-stu-id="44a3f-118">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="44a3f-119">コメント</span><span class="sxs-lookup"><span data-stu-id="44a3f-119">Comments</span></span>

<span data-ttu-id="44a3f-120">次の使用例は、電子メールの件名に「おもしろい」に相当する文字列が含まれている場合、[迷惑メール] フォルダーに電子メール メッセージを移動するルールを作成します。</span><span class="sxs-lookup"><span data-stu-id="44a3f-120">This example builds a rule that will move an e-mail message to the Junk E-mail folder if the e-mail subject contains a string that equals "Interesting".</span></span>
  
### <a name="request-elements"></a><span data-ttu-id="44a3f-121">要素を要求します。</span><span class="sxs-lookup"><span data-stu-id="44a3f-121">Request elements</span></span>

<span data-ttu-id="44a3f-122">**UpdateInboxRules**要求には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="44a3f-122">The **UpdateInboxRules** request includes the following elements:</span></span> 
  
- [<span data-ttu-id="44a3f-123">MailboxSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="44a3f-123">MailboxSmtpAddress</span></span>](mailboxsmtpaddress.md)
    
- [<span data-ttu-id="44a3f-124">RemoveOutlookRuleBlob</span><span class="sxs-lookup"><span data-stu-id="44a3f-124">RemoveOutlookRuleBlob</span></span>](removeoutlookruleblob.md)
    
- [<span data-ttu-id="44a3f-125">Operations</span><span class="sxs-lookup"><span data-stu-id="44a3f-125">Operations</span></span>](operations.md)
    
<span data-ttu-id="44a3f-126">[操作](operations.md)要素には、ルールを作成する[CreateRuleOperation](createruleoperation.md)要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="44a3f-126">The [Operations](operations.md) element contains the [CreateRuleOperation](createruleoperation.md) element to create a rule.</span></span> 
  
## <a name="updateinboxrules-create-rule-response-example"></a><span data-ttu-id="44a3f-127">UpdateInboxRules (ルールの作成) の応答の例</span><span class="sxs-lookup"><span data-stu-id="44a3f-127">UpdateInboxRules (Create Rule) response example</span></span>

### <a name="description"></a><span data-ttu-id="44a3f-128">説明</span><span class="sxs-lookup"><span data-stu-id="44a3f-128">Description</span></span>

<span data-ttu-id="44a3f-129">Simple Object Access Protocol (SOAP) 本文の次の使用例は、ルールを作成する**UpdateInboxRules**要求に正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="44a3f-129">The following Simple Object Access Protocol (SOAP) body example shows a successful response to the **UpdateInboxRules** request that creates a rule.</span></span> 
  
### <a name="code"></a><span data-ttu-id="44a3f-130">コード</span><span class="sxs-lookup"><span data-stu-id="44a3f-130">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
        MinorVersion="1" 
        MajorBuildNumber="139" 
        MinorBuildNumber="0" Version="Exchange2010_SP1" 
        xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <UpdateInboxRulesResponse 
         ResponseClass="Success" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
    </UpdateInboxRulesResponse>
  </s:Body>
</s:Envelope>

```

### <a name="successful-response-elements"></a><span data-ttu-id="44a3f-131">正常な応答の要素</span><span class="sxs-lookup"><span data-stu-id="44a3f-131">Successful response elements</span></span>

<span data-ttu-id="44a3f-132">次の要素は、応答で使用されます。</span><span class="sxs-lookup"><span data-stu-id="44a3f-132">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="44a3f-133">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="44a3f-133">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="44a3f-134">UpdateInboxRulesResponse</span><span class="sxs-lookup"><span data-stu-id="44a3f-134">UpdateInboxRulesResponse</span></span>](updateinboxrulesresponse.md)
    
- [<span data-ttu-id="44a3f-135">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="44a3f-135">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="44a3f-136">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="44a3f-136">ResponseCode</span></span>](responsecode.md)
    
## <a name="updateinboxrules-set-rule-request-example"></a><span data-ttu-id="44a3f-137">UpdateInboxRules (ルールのセット) の要求の例</span><span class="sxs-lookup"><span data-stu-id="44a3f-137">UpdateInboxRules (Set Rule) request example</span></span>

<span data-ttu-id="44a3f-138">Exchange ストア内のユーザーのメールボックスの受信トレイのルールを変更するのには Exchange Web サービスを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="44a3f-138">You can use Exchange Web Services to modify an Inbox rule in a user's mailbox in the Exchange store.</span></span> <span data-ttu-id="44a3f-139">[SetRuleOperation](setruleoperation.md)要素と組み合わせて[UpdateInboxRules](updateinboxrules.md)要素を使用して、ルールを変更します。</span><span class="sxs-lookup"><span data-stu-id="44a3f-139">Use the [UpdateInboxRules](updateinboxrules.md) element in conjunction with the [SetRuleOperation](setruleoperation.md) element to modify a rule.</span></span> 
  
### <a name="description"></a><span data-ttu-id="44a3f-140">説明</span><span class="sxs-lookup"><span data-stu-id="44a3f-140">Description</span></span>

<span data-ttu-id="44a3f-141">クライアントは、要求の XML を構築し、サーバーに送信します。</span><span class="sxs-lookup"><span data-stu-id="44a3f-141">The client constructs the request XML and sends it to the server.</span></span>
  
### <a name="code"></a><span data-ttu-id="44a3f-142">コード</span><span class="sxs-lookup"><span data-stu-id="44a3f-142">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version ="Exchange2010_SP1"/>
  </soap:Header>
  <soap:Body>
      <m:UpdateInboxRules>
        <m:RemoveOutlookRuleBlob>true</m:RemoveOutlookRuleBlob>
        <Operations xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
          <SetRuleOperation xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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

### <a name="comments"></a><span data-ttu-id="44a3f-143">コメント</span><span class="sxs-lookup"><span data-stu-id="44a3f-143">Comments</span></span>

<span data-ttu-id="44a3f-144">この例で表示名を変更 (更新) これは、迷惑メールです。</span><span class="sxs-lookup"><span data-stu-id="44a3f-144">This example changes the display name to "(Modified) This is Junk".</span></span>
  
> [!NOTE]
> <span data-ttu-id="44a3f-145">[フォルダー Id](folderid.md)要素の属性を**変更キー**と**Id**の値は、読みやすさに短縮されています。</span><span class="sxs-lookup"><span data-stu-id="44a3f-145">The values of the **Id** and **ChangeKey** attributes of the [FolderId](folderid.md) element have been shortened for readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="44a3f-146">要素を要求します。</span><span class="sxs-lookup"><span data-stu-id="44a3f-146">Request elements</span></span>

<span data-ttu-id="44a3f-147">**UpdateInboxRules**要求には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="44a3f-147">The **UpdateInboxRules** request includes the following elements:</span></span> 
  
- [<span data-ttu-id="44a3f-148">MailboxSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="44a3f-148">MailboxSmtpAddress</span></span>](mailboxsmtpaddress.md)
    
- [<span data-ttu-id="44a3f-149">RemoveOutlookRuleBlob</span><span class="sxs-lookup"><span data-stu-id="44a3f-149">RemoveOutlookRuleBlob</span></span>](removeoutlookruleblob.md)
    
- [<span data-ttu-id="44a3f-150">Operations</span><span class="sxs-lookup"><span data-stu-id="44a3f-150">Operations</span></span>](operations.md)
    
<span data-ttu-id="44a3f-151">[操作](operations.md)要素には、ルールを変更する[SetRuleOperation](setruleoperation.md)要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="44a3f-151">The [Operations](operations.md) element contains the [SetRuleOperation](setruleoperation.md) element to modify a rule.</span></span> 
  
## <a name="updateinboxrules-set-rule-response-example"></a><span data-ttu-id="44a3f-152">UpdateInboxRules (ルールを設定する) 応答の例</span><span class="sxs-lookup"><span data-stu-id="44a3f-152">UpdateInboxRules (Set Rule) response example</span></span>

### <a name="description"></a><span data-ttu-id="44a3f-153">説明</span><span class="sxs-lookup"><span data-stu-id="44a3f-153">Description</span></span>

<span data-ttu-id="44a3f-154">Simple Object Access Protocol (SOAP) 本文の次の使用例は、ルールを変更する**UpdateInboxRules**要求に正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="44a3f-154">The following Simple Object Access Protocol (SOAP) body example shows a successful response to the **UpdateInboxRules** request that modifies a rule.</span></span> 
  
### <a name="code"></a><span data-ttu-id="44a3f-155">コード</span><span class="sxs-lookup"><span data-stu-id="44a3f-155">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
        MinorVersion="1" 
        MajorBuildNumber="139" 
        MinorBuildNumber="0" 
        Version="Exchange2010_SP1" 
        xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <UpdateInboxRulesResponse 
          ResponseClass="Success" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
    </UpdateInboxRulesResponse>
  </s:Body>
</s:Envelope>

```

### <a name="successful-response-elements"></a><span data-ttu-id="44a3f-156">正常な応答の要素</span><span class="sxs-lookup"><span data-stu-id="44a3f-156">Successful response elements</span></span>

<span data-ttu-id="44a3f-157">次の要素は、応答で使用されます。</span><span class="sxs-lookup"><span data-stu-id="44a3f-157">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="44a3f-158">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="44a3f-158">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="44a3f-159">UpdateInboxRulesResponse</span><span class="sxs-lookup"><span data-stu-id="44a3f-159">UpdateInboxRulesResponse</span></span>](updateinboxrulesresponse.md)
    
- [<span data-ttu-id="44a3f-160">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="44a3f-160">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="44a3f-161">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="44a3f-161">ResponseCode</span></span>](responsecode.md)
    
## <a name="updateinboxrules-delete-rule-request-example"></a><span data-ttu-id="44a3f-162">UpdateInboxRules (ルールの削除) の要求の例</span><span class="sxs-lookup"><span data-stu-id="44a3f-162">UpdateInboxRules (Delete Rule) request example</span></span>

<span data-ttu-id="44a3f-163">Exchange Web サービスを使用すると、Exchange ストア内のユーザーのメールボックスの受信トレイ ルールを削除します。</span><span class="sxs-lookup"><span data-stu-id="44a3f-163">You can use Exchange Web Services to delete an Inbox rule in a user's mailbox in the Exchange store.</span></span> <span data-ttu-id="44a3f-164">[DeleteRuleOperation](deleteruleoperation.md)要素と連携して動作規則を削除するのには[UpdateInboxRules](updateinboxrules.md)を使用します。</span><span class="sxs-lookup"><span data-stu-id="44a3f-164">Use the [UpdateInboxRules](updateinboxrules.md) in conjunction with the [DeleteRuleOperation](deleteruleoperation.md) element to delete a rule.</span></span> 
  
### <a name="description"></a><span data-ttu-id="44a3f-165">説明</span><span class="sxs-lookup"><span data-stu-id="44a3f-165">Description</span></span>

<span data-ttu-id="44a3f-166">クライアントは、要求の XML を構築し、サーバーに送信します。</span><span class="sxs-lookup"><span data-stu-id="44a3f-166">The client constructs the request XML and sends it to the server.</span></span>
  
### <a name="code"></a><span data-ttu-id="44a3f-167">コード</span><span class="sxs-lookup"><span data-stu-id="44a3f-167">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="44a3f-168">コメント</span><span class="sxs-lookup"><span data-stu-id="44a3f-168">Comments</span></span>

<span data-ttu-id="44a3f-169">この例では、既存の特定の規則を削除します。</span><span class="sxs-lookup"><span data-stu-id="44a3f-169">This example deletes the existing identified rule.</span></span>
  
### <a name="request-elements"></a><span data-ttu-id="44a3f-170">要素を要求します。</span><span class="sxs-lookup"><span data-stu-id="44a3f-170">Request elements</span></span>

<span data-ttu-id="44a3f-171">**UpdateInboxRules**要求には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="44a3f-171">The **UpdateInboxRules** request includes the following elements:</span></span> 
  
- [<span data-ttu-id="44a3f-172">MailboxSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="44a3f-172">MailboxSmtpAddress</span></span>](mailboxsmtpaddress.md)
    
- [<span data-ttu-id="44a3f-173">RemoveOutlookRuleBlob</span><span class="sxs-lookup"><span data-stu-id="44a3f-173">RemoveOutlookRuleBlob</span></span>](removeoutlookruleblob.md)
    
- [<span data-ttu-id="44a3f-174">Operations</span><span class="sxs-lookup"><span data-stu-id="44a3f-174">Operations</span></span>](operations.md)
    
<span data-ttu-id="44a3f-175">[操作](operations.md)要素には、ルールを削除する[DeleteRuleOperation](deleteruleoperation.md)要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="44a3f-175">The [Operations](operations.md) element contains the [DeleteRuleOperation](deleteruleoperation.md) element to delete a rule.</span></span> 
  
## <a name="updateinboxrules-delete-rule-response-example"></a><span data-ttu-id="44a3f-176">UpdateInboxRules (ルールの削除) 応答の例</span><span class="sxs-lookup"><span data-stu-id="44a3f-176">UpdateInboxRules (Delete Rule) response example</span></span>

### <a name="description"></a><span data-ttu-id="44a3f-177">説明</span><span class="sxs-lookup"><span data-stu-id="44a3f-177">Description</span></span>

<span data-ttu-id="44a3f-178">Simple Object Access Protocol (SOAP) 本文の次の使用例は、ルールを削除する**UpdateInboxRules**要求に正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="44a3f-178">The following Simple Object Access Protocol (SOAP) body example shows a successful response to the **UpdateInboxRules** request that deletes a rule.</span></span> 
  
### <a name="code"></a><span data-ttu-id="44a3f-179">コード</span><span class="sxs-lookup"><span data-stu-id="44a3f-179">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
        MinorVersion="1" 
        MajorBuildNumber="139" 
        MinorBuildNumber="0" 
        Version="Exchange2010_SP1" 
        xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <UpdateInboxRulesResponse ResponseClass="Success" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
    </UpdateInboxRulesResponse>
  </s:Body>
</s:Envelope>

```

### <a name="successful-response-elements"></a><span data-ttu-id="44a3f-180">正常な応答の要素</span><span class="sxs-lookup"><span data-stu-id="44a3f-180">Successful response elements</span></span>

<span data-ttu-id="44a3f-181">次の要素は、応答で使用されます。</span><span class="sxs-lookup"><span data-stu-id="44a3f-181">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="44a3f-182">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="44a3f-182">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="44a3f-183">UpdateInboxRulesResponse</span><span class="sxs-lookup"><span data-stu-id="44a3f-183">UpdateInboxRulesResponse</span></span>](updateinboxrulesresponse.md)
    
- [<span data-ttu-id="44a3f-184">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="44a3f-184">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="44a3f-185">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="44a3f-185">ResponseCode</span></span>](responsecode.md)
    
## <a name="see-also"></a><span data-ttu-id="44a3f-186">関連項目</span><span class="sxs-lookup"><span data-stu-id="44a3f-186">See also</span></span>



[<span data-ttu-id="44a3f-187">GetInboxRules の操作</span><span class="sxs-lookup"><span data-stu-id="44a3f-187">GetInboxRules operation</span></span>](getinboxrules-operation.md)

