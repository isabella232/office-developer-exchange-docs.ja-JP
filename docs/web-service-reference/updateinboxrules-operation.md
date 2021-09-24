---
title: UpdateInboxRules 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- UpdateInboxRules
api_type:
- schema
ms.assetid: f982a237-471e-45c5-a2b5-468cfc53150b
description: UpdateInboxRules 操作は、指定した操作を適用することによって、認証されたユーザーの受信トレイ ルールを更新します。 UpdateInboxRules は、受信トレイ ルールの作成、受信トレイ ルールの設定、受信トレイ ルールの削除に使用されます。
ms.openlocfilehash: 08f46219bcb01f5f1c9d69cfaa8b4934e82ff5bd
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510716"
---
# <a name="updateinboxrules-operation"></a>UpdateInboxRules 操作

UpdateInboxRules 操作は、指定した操作を適用することによって、認証されたユーザーの受信トレイ ルールを更新します。 **UpdateInboxRules は** 、受信トレイ ルールの作成、受信トレイ ルールの設定、受信トレイ ルールの削除に使用されます。 
  
**UpdateInboxRules** 操作を使用すると、Web サービスExchangeクライアント側の送信ルールが削除されます。 クライアント側の送信ルールは、クライアントのルールのフォルダー関連情報 (FAI) メッセージにのみ保存されます。 EWS は既定で、このルール FAI メッセージを削除します。これは、Outlook がこれを再作成するという前提に基づいて行われます。 ただし、Outlook で再作成できるのは、拡張ルールとしても存在しているルールです。けれども、クライアント側の送信ルールは拡張ルールとして存在していません。 その結果、これらのルールは失われます。 ソリューションの設計時にこのことを考慮にするようお勧めします。 
  
## <a name="updateinboxrules-create-rule-request-example"></a>UpdateInboxRules (ルールの作成) 要求の例

Web サービスExchange使用して、ユーザーのメールボックス内に受信トレイ ルールを作成Exchangeできます。 ルールを [作成するには、UpdateInboxRules](updateinboxrules.md) 要素を [CreateRuleOperation](createruleoperation.md) 要素と組み合わせて使用します。 
  
### <a name="description"></a>説明

クライアントは要求 XML を構築し、サーバーに送信します。
  
### <a name="code"></a>コード

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

### <a name="comments"></a>コメント

この例では、電子メール の件名に "興味深い" という文字列が含まれている場合に、電子メール メッセージを迷惑メール フォルダーに移動するルールを作成します。
  
### <a name="request-elements"></a>要求要素

**UpdateInboxRules 要求には**、次の要素が含まれています。 
  
- [MailboxSmtpAddress](mailboxsmtpaddress.md)
    
- [RemoveOutlookRuleBlob](removeoutlookruleblob.md)
    
- [Operations](operations.md)
    
[Operations 要素](operations.md)には、ルールを作成[する CreateRuleOperation](createruleoperation.md)要素が含まれます。 
  
## <a name="updateinboxrules-create-rule-response-example"></a>UpdateInboxRules (ルールの作成) 応答例

### <a name="description"></a>説明

次のSimple Object Access Protocol (SOAP) 本文の例は、ルールを作成する **UpdateInboxRules** 要求に対する正常な応答を示しています。 
  
### <a name="code"></a>コード

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

### <a name="successful-response-elements"></a>成功した応答要素

応答では、次の要素が使用されます。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [UpdateInboxRulesResponse](updateinboxrulesresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [ResponseCode](responsecode.md)
    
## <a name="updateinboxrules-set-rule-request-example"></a>UpdateInboxRules (ルールの設定) 要求の例

Web サービスをExchangeして、メールボックス ストア内のユーザーのメールボックス内の受信トレイ ルールをExchangeできます。 ルールを [変更するには、UpdateInboxRules](updateinboxrules.md) 要素を [SetRuleOperation](setruleoperation.md) 要素と組み合わせて使用します。 
  
### <a name="description"></a>説明

クライアントは要求 XML を構築し、サーバーに送信します。
  
### <a name="code"></a>コード

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

### <a name="comments"></a>コメント

次の使用例は、表示名を "(Modified) This is Junk" に変更します。
  
> [!NOTE]
> [FolderId](folderid.md)要素 **の Id** 属性と **ChangeKey** 属性の値は、読みやすさのために短縮されています。 
  
### <a name="request-elements"></a>要求要素

**UpdateInboxRules 要求には**、次の要素が含まれています。 
  
- [MailboxSmtpAddress](mailboxsmtpaddress.md)
    
- [RemoveOutlookRuleBlob](removeoutlookruleblob.md)
    
- [Operations](operations.md)
    
[Operations 要素](operations.md)には、ルールを変更[する SetRuleOperation](setruleoperation.md)要素が含まれます。 
  
## <a name="updateinboxrules-set-rule-response-example"></a>UpdateInboxRules (ルールの設定) 応答例

### <a name="description"></a>説明

次のSimple Object Access Protocol (SOAP) 本文の例は、ルールを変更する **UpdateInboxRules** 要求に対する正常な応答を示しています。 
  
### <a name="code"></a>コード

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

### <a name="successful-response-elements"></a>成功した応答要素

応答では、次の要素が使用されます。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [UpdateInboxRulesResponse](updateinboxrulesresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [ResponseCode](responsecode.md)
    
## <a name="updateinboxrules-delete-rule-request-example"></a>UpdateInboxRules (ルールの削除) 要求の例

Web サービスExchangeを使用して、ユーザーのメールボックス内の受信トレイ ルールを削除Exchangeできます。 ルールを [削除するには、UpdateInboxRules](updateinboxrules.md) を [DeleteRuleOperation](deleteruleoperation.md) 要素と組み合わせて使用します。 
  
### <a name="description"></a>説明

クライアントは要求 XML を構築し、サーバーに送信します。
  
### <a name="code"></a>コード

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

### <a name="comments"></a>コメント

次の使用例は、既存の識別されたルールを削除します。
  
### <a name="request-elements"></a>要求要素

**UpdateInboxRules 要求には**、次の要素が含まれています。 
  
- [MailboxSmtpAddress](mailboxsmtpaddress.md)
    
- [RemoveOutlookRuleBlob](removeoutlookruleblob.md)
    
- [Operations](operations.md)
    
[Operations 要素](operations.md)には、ルールを削除[する DeleteRuleOperation](deleteruleoperation.md)要素が含まれます。 
  
## <a name="updateinboxrules-delete-rule-response-example"></a>UpdateInboxRules (ルールの削除) 応答例

### <a name="description"></a>説明

次のSimple Object Access Protocol (SOAP) 本文の例は、ルールを削除する **UpdateInboxRules** 要求に対する正常な応答を示しています。 
  
### <a name="code"></a>コード

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

### <a name="successful-response-elements"></a>成功した応答要素

応答では、次の要素が使用されます。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [UpdateInboxRulesResponse](updateinboxrulesresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [ResponseCode](responsecode.md)
    
## <a name="see-also"></a>関連項目



[GetInboxRules の操作](getinboxrules-operation.md)

