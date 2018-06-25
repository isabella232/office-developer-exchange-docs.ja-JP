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
# <a name="updateinboxrules-operation"></a>UpdateInboxRules 操作

UpdateInboxRules 操作は、指定した操作を適用することによって認証されたユーザーの受信トレイ ルールを更新します。 **UpdateInboxRules**を使用して、または受信トレイ ルールを削除するのには、受信トレイ ルールを設定するのには、受信トレイのルールを作成します。 
  
**UpdateInboxRules**操作を使用する場合、Exchange Web サービスは、クライアント側の送信規則を削除します。 フォルダー関連情報 (FAI) メッセージのルールでクライアントと他の場所では、クライアント側の送信規則が格納されます。 EWS では、既定では、Outlook は、再作成を前提に基づく FAI メッセージ ルールを削除します。 ただし、Outlook は、拡張のルールとしても存在しないルールを再作成できません、拡張ルールとクライアント側の送信規則が存在しません。 その結果、これらのルールは失われます。 ソリューションを設計するときこれを考慮することをお勧めします。 
  
## <a name="updateinboxrules-create-rule-request-example"></a>UpdateInboxRules (ルールの作成) の要求の例

Exchange Web サービスを使用すると、Exchange ストア内のユーザーのメールボックスで受信トレイ ルールを作成します。 [CreateRuleOperation](createruleoperation.md)要素と組み合わせて[UpdateInboxRules](updateinboxrules.md)要素を使用して、ルールを作成します。 
  
### <a name="description"></a>説明

クライアントは、要求の XML を構築し、サーバーに送信します。
  
### <a name="code"></a>コード

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

### <a name="comments"></a>コメント

次の使用例は、電子メールの件名に「おもしろい」に相当する文字列が含まれている場合、[迷惑メール] フォルダーに電子メール メッセージを移動するルールを作成します。
  
### <a name="request-elements"></a>要素を要求します。

**UpdateInboxRules**要求には、次の要素が含まれています。 
  
- [MailboxSmtpAddress](mailboxsmtpaddress.md)
    
- [RemoveOutlookRuleBlob](removeoutlookruleblob.md)
    
- [Operations](operations.md)
    
[操作](operations.md)要素には、ルールを作成する[CreateRuleOperation](createruleoperation.md)要素が含まれています。 
  
## <a name="updateinboxrules-create-rule-response-example"></a>UpdateInboxRules (ルールの作成) の応答の例

### <a name="description"></a>説明

Simple Object Access Protocol (SOAP) 本文の次の使用例は、ルールを作成する**UpdateInboxRules**要求に正常な応答を示しています。 
  
### <a name="code"></a>コード

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

### <a name="successful-response-elements"></a>正常な応答の要素

次の要素は、応答で使用されます。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [UpdateInboxRulesResponse](updateinboxrulesresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [ResponseCode](responsecode.md)
    
## <a name="updateinboxrules-set-rule-request-example"></a>UpdateInboxRules (ルールのセット) の要求の例

Exchange ストア内のユーザーのメールボックスの受信トレイのルールを変更するのには Exchange Web サービスを使用することができます。 [SetRuleOperation](setruleoperation.md)要素と組み合わせて[UpdateInboxRules](updateinboxrules.md)要素を使用して、ルールを変更します。 
  
### <a name="description"></a>説明

クライアントは、要求の XML を構築し、サーバーに送信します。
  
### <a name="code"></a>コード

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

### <a name="comments"></a>コメント

この例で表示名を変更 (更新) これは、迷惑メールです。
  
> [!NOTE]
> [フォルダー Id](folderid.md)要素の属性を**変更キー**と**Id**の値は、読みやすさに短縮されています。 
  
### <a name="request-elements"></a>要素を要求します。

**UpdateInboxRules**要求には、次の要素が含まれています。 
  
- [MailboxSmtpAddress](mailboxsmtpaddress.md)
    
- [RemoveOutlookRuleBlob](removeoutlookruleblob.md)
    
- [Operations](operations.md)
    
[操作](operations.md)要素には、ルールを変更する[SetRuleOperation](setruleoperation.md)要素が含まれています。 
  
## <a name="updateinboxrules-set-rule-response-example"></a>UpdateInboxRules (ルールを設定する) 応答の例

### <a name="description"></a>説明

Simple Object Access Protocol (SOAP) 本文の次の使用例は、ルールを変更する**UpdateInboxRules**要求に正常な応答を示しています。 
  
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

### <a name="successful-response-elements"></a>正常な応答の要素

次の要素は、応答で使用されます。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [UpdateInboxRulesResponse](updateinboxrulesresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [ResponseCode](responsecode.md)
    
## <a name="updateinboxrules-delete-rule-request-example"></a>UpdateInboxRules (ルールの削除) の要求の例

Exchange Web サービスを使用すると、Exchange ストア内のユーザーのメールボックスの受信トレイ ルールを削除します。 [DeleteRuleOperation](deleteruleoperation.md)要素と連携して動作規則を削除するのには[UpdateInboxRules](updateinboxrules.md)を使用します。 
  
### <a name="description"></a>説明

クライアントは、要求の XML を構築し、サーバーに送信します。
  
### <a name="code"></a>コード

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

### <a name="comments"></a>コメント

この例では、既存の特定の規則を削除します。
  
### <a name="request-elements"></a>要素を要求します。

**UpdateInboxRules**要求には、次の要素が含まれています。 
  
- [MailboxSmtpAddress](mailboxsmtpaddress.md)
    
- [RemoveOutlookRuleBlob](removeoutlookruleblob.md)
    
- [Operations](operations.md)
    
[操作](operations.md)要素には、ルールを削除する[DeleteRuleOperation](deleteruleoperation.md)要素が含まれています。 
  
## <a name="updateinboxrules-delete-rule-response-example"></a>UpdateInboxRules (ルールの削除) 応答の例

### <a name="description"></a>説明

Simple Object Access Protocol (SOAP) 本文の次の使用例は、ルールを削除する**UpdateInboxRules**要求に正常な応答を示しています。 
  
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

### <a name="successful-response-elements"></a>正常な応答の要素

次の要素は、応答で使用されます。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [UpdateInboxRulesResponse](updateinboxrulesresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [ResponseCode](responsecode.md)
    
## <a name="see-also"></a>関連項目



[GetInboxRules の操作](getinboxrules-operation.md)

