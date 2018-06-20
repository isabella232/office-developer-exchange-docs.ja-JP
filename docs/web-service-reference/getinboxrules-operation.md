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
# <a name="getinboxrules-operation"></a>GetInboxRules 操作

**GetInboxRules**操作は、識別されたユーザーのメールボックスの受信トレイ ルールを取得するために、Exchange Web サービスを使用します。 
  
## <a name="getinboxrules-request-example"></a>GetInboxRules 要求の例

### <a name="description"></a>説明

要求クライアントがサーバーに送信する XML の例を次に示します。 要求は、 [MailboxSmtpAddress](mailboxsmtpaddress.md)要素内でユーザーを識別します。 識別されたユーザーのすべての受信トレイのルールでは、応答で返されます。 
  
### <a name="code"></a>コード

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

### <a name="request-elements"></a>要素を要求します。

要求には、次の省略可能な要素が含まれています。
  
- [MailboxSmtpAddress](mailboxsmtpaddress.md)
    
## <a name="successful-getinboxrules-response-example"></a>成功した GetInboxRules の応答の例

### <a name="description"></a>説明

Simple Object Access Protocol (SOAP) 本文の次の使用例は、 **GetInboxRules**要求に正常な応答を示しています。 この例では、応答には、1 つのルールが含まれています。 
  
> [!NOTE]
> [フォルダー Id](folderid.md)の要素の**変更キー**属性と**Id**の値は、読みやすさを保持するために短縮されています。 
  
### <a name="code"></a>コード

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

### <a name="response-elements"></a>応答の要素

応答では、次の要素が含まれています。
  
- [GetInboxRulesResponse](getinboxrulesresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [OutlookRuleBlobExists](outlookruleblobexists.md)
    
- [InboxRules](inboxrules.md)
    
## <a name="see-also"></a>関連項目



[UpdateInboxRules の操作](updateinboxrules-operation.md)

