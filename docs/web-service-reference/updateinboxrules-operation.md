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
# <a name="updateinboxrules-operation"></a>UpdateInboxRules の操作

Updateinbox Rules 操作は、指定された操作を適用することによって、認証済みのユーザーの受信トレイルールを更新します。 **Updateinbox**ルールは、受信トレイルールを作成したり、受信トレイルールを設定したり、受信トレイルールを削除したりするために使用します。 
  
**Update受信トレイルール**操作を使用すると、Exchange Web サービスによってクライアント側の送信ルールが削除されます。 クライアント側の送信ルールは、クライアントのルールのフォルダー関連情報 (FAI) メッセージにのみ保存されます。 EWS は既定で、このルール FAI メッセージを削除します。これは、Outlook がこれを再作成するという前提に基づいて行われます。 ただし、Outlook で再作成できるのは、拡張ルールとしても存在しているルールです。けれども、クライアント側の送信ルールは拡張ルールとして存在していません。 その結果、これらのルールは失われます。 ソリューションの設計時にこのことを考慮にするようお勧めします。 
  
## <a name="updateinboxrules-create-rule-request-example"></a>Update受信トレイルール (ルールの作成) 要求の例

Exchange Web サービスを使用して、Exchange ストア内のユーザーのメールボックスに受信トレイルールを作成できます。 ルールを作成するには、 [CreateRuleOperation](createruleoperation.md)要素と共に[update受信トレイルール](updateinboxrules.md)要素を使用します。 
  
### <a name="description"></a>Description

クライアントは、要求 XML を構築し、サーバーに送信します。
  
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

この例では、電子メールの件名に "おもしろい" という文字列が含まれている場合に、電子メールメッセージを [迷惑メール] フォルダーに移動するルールを作成します。
  
### <a name="request-elements"></a>Request 要素

**Update受信トレイルール**要求には、次の要素が含まれています。 
  
- [MailboxSmtpAddress](mailboxsmtpaddress.md)
    
- [RemoveOutlookRuleBlob](removeoutlookruleblob.md)
    
- [Operations](operations.md)
    
[操作](operations.md)要素には、ルールを作成するための[CreateRuleOperation](createruleoperation.md)要素が含まれています。 
  
## <a name="updateinboxrules-create-rule-response-example"></a>Update受信トレイルール (作成ルール) の応答の例

### <a name="description"></a>Description

次の簡易オブジェクトアクセスプロトコル (SOAP) 本文の例は、ルールを作成する**Update受信トレイルール**要求に対する正常な応答を示しています。 
  
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
    
- [Update受信トレイルールの応答](updateinboxrulesresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [ResponseCode](responsecode.md)
    
## <a name="updateinboxrules-set-rule-request-example"></a>Update受信トレイルール (Set Rule) 要求の例

Exchange Web サービスを使用して、Exchange ストア内のユーザーのメールボックスの受信トレイルールを変更できます。 ルールを変更するには、 [SetRuleOperation](setruleoperation.md)要素と共に[update受信トレイルール](updateinboxrules.md)要素を使用します。 
  
### <a name="description"></a>Description

クライアントは、要求 XML を構築し、サーバーに送信します。
  
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

次の使用例は、表示名を "(変更) が迷惑メールである" に変更します。
  
> [!NOTE]
> [FolderId](folderid.md)要素の**Id**および**changekey**属性の値は、読みやすくするために短縮されています。 
  
### <a name="request-elements"></a>Request 要素

**Update受信トレイルール**要求には、次の要素が含まれています。 
  
- [MailboxSmtpAddress](mailboxsmtpaddress.md)
    
- [RemoveOutlookRuleBlob](removeoutlookruleblob.md)
    
- [Operations](operations.md)
    
[操作](operations.md)要素には、ルールを変更するための[SetRuleOperation](setruleoperation.md)要素が含まれています。 
  
## <a name="updateinboxrules-set-rule-response-example"></a>Update受信トレイルール (Set Rule) response の例

### <a name="description"></a>Description

次の簡易オブジェクトアクセスプロトコル (SOAP) 本文の例は、ルールを変更する**Update受信トレイルール**要求に対する正常な応答を示しています。 
  
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
    
- [Update受信トレイルールの応答](updateinboxrulesresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [ResponseCode](responsecode.md)
    
## <a name="updateinboxrules-delete-rule-request-example"></a>Update受信トレイルール (デリートルール) 要求の例

Exchange Web サービスを使用して、Exchange ストア内のユーザーのメールボックスの受信トレイルールを削除できます。 ルールを削除するには、 [DeleteRuleOperation](deleteruleoperation.md)要素と共に[Update受信トレイルール](updateinboxrules.md)を使用します。 
  
### <a name="description"></a>Description

クライアントは、要求 XML を構築し、サーバーに送信します。
  
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

この例では、既存の識別されたルールを削除します。
  
### <a name="request-elements"></a>Request 要素

**Update受信トレイルール**要求には、次の要素が含まれています。 
  
- [MailboxSmtpAddress](mailboxsmtpaddress.md)
    
- [RemoveOutlookRuleBlob](removeoutlookruleblob.md)
    
- [Operations](operations.md)
    
[操作](operations.md)要素には、ルールを削除するための[DeleteRuleOperation](deleteruleoperation.md)要素が含まれています。 
  
## <a name="updateinboxrules-delete-rule-response-example"></a>Update受信トレイルール (デリートルール) の応答の例

### <a name="description"></a>Description

次の簡易オブジェクトアクセスプロトコル (SOAP) 本文の例は、ルールを削除する**Update受信トレイルール**要求に対する正常な応答を示しています。 
  
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
    
- [Update受信トレイルールの応答](updateinboxrulesresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [ResponseCode](responsecode.md)
    
## <a name="see-also"></a>関連項目



[GetInboxRules の操作](getinboxrules-operation.md)

