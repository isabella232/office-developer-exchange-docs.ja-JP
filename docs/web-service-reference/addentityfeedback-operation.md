---
title: AddEntityFeedback 操作
manager: luken
ms.date: 4/18/2016
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 00e40197-5794-4268-b937-bd65aa044890
description: AddEntityFeedback 操作は、サーバー側の問題に対応するエラー情報を返します。
ms.openlocfilehash: a1027a0a1ee06cf3e83833b1d84c13d77b07c0b9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458440"
---
# <a name="addentityfeedback-operation"></a>AddEntityFeedback 操作

**Addentityfeedback**操作は、サーバー側の問題に対応するエラー情報を返します。 
  
この操作では、ログに記録されるイベントの種類に依存します。 最も重要なイベントの1つは、選択されているエンティティに対応する**Entityadded が追加**されたことです。 この操作はバッチであるため、1回の要求でエントリのバッチをログに記録するために使用できます。 
  
## <a name="findpeople-request-examples"></a>FindPeople 要求の例

**Addentityfeedback**操作は、クライアントがサービスによって返されるエンティティとの対話の詳細をログに記録する方法を提供します。 これは、クライアントごとに、シーンの背後で関連性を向上させるための信号として使用できます。 例: クライアントは、この操作を使用して、 **findpeople**から返された人物エンティティについてのフィードバックを提供できます。
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
                             xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                             xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:AddEntityFeedback>
            <m:EntityFeedbackEntries>
                  <t:EntityFeedbackEntry>
                        <t:ClientEventTimeUTC> 2015-07-05T22:16:18+00:00</t:ClientEventTimeUTC>
                        <t:ClientEventTimeLocal> 2015-07-05T22:16:18+00:00</t:ClientEventTimeLocal>
                        <t:ClientSessionId>00000000-0000-0000-0000-000000000012</t:ClientSessionId>
                        <t:ClientVersion>15.01.0101.01</t:ClientVersion>
                        <t:ClientId>Web</t:ClientId>
                        <t:TransactionId>123456789</t:TransactionId>
                        <t:EventType>EntityAdded</t:EventType>
                        <t:TargetEntityList>["a","b","c"]</t:TargetEntityList>
                        <t:SourceOfEntityAdded></t:SourceOfEntityAdded>
                        <t:JSONPropertyBag></t:JSONPropertyBag>
                  </t:EntityFeedbackEntry>
                  <t:EntityFeedbackEntry>
                  …
                  </t:EntityFeedbackEntry>
            </m:EntityFeedbackEntries>
      </m:AddEntityFeedback>
   </soap:Body>
</soap:Envelope>

```

### <a name="the-request-soap-body-contents"></a>要求 SOAP 本文のコンテンツ

Soap 要求には、1つの要素の**エンティティフィードのバックエントリ**が含まれています。 これには、 **Entityフィードバック entry**オブジェクトの配列が含まれています。 配列内の各エントリには、次の要素を含めることができます。 
  
|**要求のパラメータ**|**必須**|**説明**|**型**|
|:-----|:-----|:-----|:-----|
|**ClientEventTimeUtc** <br/> |はい  <br/> |クライアント側でイベントが発生した UTC 時間。  <br/> |DateTime
  <br/> |
|**ClientEventTimeLocal** <br/> |はい  <br/> |クライアント側でイベントが発生したローカル時刻。  <br/> |DateTime
  <br/> |
|**ClientId** <br/> |はい  <br/> |クライアントの種類 (Outlook、OWA など)。  <br/> |ClientIDType 列挙型  <br/> |
|**ClientSessionId** <br/> |はい  <br/> |セッション ID を識別する GUID。 クライアントで生成されます。  <br/> |GUID  <br/> |
|**ClientVersion** <br/> |はい  <br/> |クライアントのバージョン (例: 15.01.0101.000)。  <br/> |文字列  <br/> |
|**EntityAddSource** <br/> |いいえ  <br/> |移行元のエンティティ (EntityRelevanceAPI、型、貼り付けなど)。  <br/> |EntityAddSource 列挙  <br/> |
|**EntrySequenceNumber** <br/> |はい  <br/> |クライアントセッションあたりの増分整数。 データ損失を検出するために使用されます。  <br/> |Int  <br/> |
|**EventType** <br/> |はい  <br/> |イベントの種類 (たとえば、エンティティが追加され、エンティティが削除された場合)。  <br/> |文字列  <br/> |
|**JSONPropertyBag** <br/> |いいえ  <br/> |イベント (キー/値のペアの JSON blob) に関連付けられている追加のプロパティ。  <br/> |JSON Blob  <br/> |
|**TargetEntityList** <br/> |いいえ  <br/> |イベントに関連付けられているエンティティのリスト。  <br/> |JSON 文字列  <br/> |
|**TransactionId** <br/> |いいえ  <br/> |Id (GUID) は、クエリログの ID を関連付けます。  <br/> |文字列  <br/> |
   
### <a name="successful-addentityfeedback-operation-response"></a>AddEntityFeedback 操作の成功応答

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
    <s:Header>
        <h:ServerVersionInfo MajorVersion="15" 
                                MinorVersion="1" 
                                MajorBuildNumber="228" 
                                MinorBuildNumber="0" 
                                Version="V2_49" 
                                xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                                xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                                xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
    </s:Header>
    <s:Body>
        <AddEntityFeedbackResponse ResponseClass="Success" 
                                                              xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                                              xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                                                              xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
            <ResponseCode>NoError</ResponseCode>
            <ErrorCount>0</ErrorCount>
            <ErrorDetails />
        </AddEntityFeedbackResponse>
    </s:Body>
</s:Envelope> 

```

### <a name="the-response-soap-body-contains-the-following-elements"></a>応答 SOAP 本文には、次の要素が含まれています。

#### <a name="errors"></a>エラー 
  
API はフィードバックエントリのバッチをログに記録することができ、できることをすべてログに記録します。 このフィールドは、ログに記録されなかったエラーエントリの数を表します。
    
#### <a name="errordetails"></a>ErrorDetails
  
上記のエラーに関連する詳細情報 `;` 。
    
### <a name="currently-supported-values"></a>現在サポートされている値

|**ClientIdType 列挙型**|
|:-----|
|Desktop  <br/> |
|Exchange  <br/> |
|IMAP4  <br/> |
|Lync  <br/> |
|MacMail  <br/> |
|MacOutlook  <br/> |
|Mobile  <br/> |
|Other  <br/> |
|Outlook  <br/> |
|Outlookservice.swift  <br/> |
|POP3  <br/> |
|Tablet  <br/> |
|Web  <br/> |
   
|**EntityAddSource 列挙**|
|:-----|
|ActiveDirectory  <br/> |
|EntityRelevanceApi  <br/> |
|EntityRelevanceApiCache  <br/> |
|ExplicitTyping  <br/> |
|LocalCache  <br/> |
|LocalCacheAndEntityRelevanceAPI  <br/> |
|なし  <br/> |
|その他  <br/> |
|貼り付け  <br/> |
   
### <a name="addentityfeedback-operation-error-response"></a>AddEntityFeedback 操作エラー応答

EWS に汎用のエラーコードについては[、「応答](responsecode.md)」を参照してください。
  
### <a name="example-of-addentityfeedback-in-conjunction-with-findpeople"></a>FindPeople と共に追加される AddEntityFeedback の例

#### <a name="findpeople-request"></a>FindPeople 要求
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
<soap:Body >
    <m:FindPeople>
      <m:IndexedPageItemView BasePoint="Beginning" MaxEntriesReturned="100" Offset="0"/>
      <m:QueryString>user1</m:QueryString>
      <m:SearchPeopleSuggestionIndex>true</m:SearchPeopleSuggestionIndex>
    </m:FindPeople>
  </soap:Body>
</soap:Envelope>    
    
```

#### <a name="findpeople-response"></a>FindPeople 応答

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
    <s:Header>
        <h:ServerVersionInfo MajorVersion="15" MinorVersion="1" MajorBuildNumber="302" MinorBuildNumber="0" Version="V2_68" xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
    </s:Header>
    <s:Body>
        <FindPeopleResponse ResponseClass="Success" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
            <ResponseCode>NoError</ResponseCode>
            <People>
                <Persona xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
                    <PersonaId Id="AAUQAFjZ4UxX8SZCqSPFsmh0cSo=" />
                    <PersonaType>Person</PersonaType>
                    <CreationTime>2015-10-02T23:25:42</CreationTime>
                    <DisplayName>user2</DisplayName>
…
                  </Persona>
            </People>
            <TotalNumberOfPeopleInView>0</TotalNumberOfPeopleInView>
            <FirstMatchingRowIndex>0</FirstMatchingRowIndex>
            <FirstLoadedRowIndex>0</FirstLoadedRowIndex>
            <TransactionId>b56ad16e-5d5a-4574-90f8-b8dd57382be6</TransactionId>
        </FindPeopleResponse>
    </s:Body>
</s:Envelope>

```

#### <a name="addentityfeedback-request"></a>AddEntityFeedback 要求

```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:AddEntityFeedback>
<m:EntityFeedbackEntries>
<t:EntityFeedbackEntry>
         <t:ClientEventTimeUtc>2015-07-05T22:16:18+00:00</t:ClientEventTimeUtc>
         <t:ClientEventTimeLocal>2015-07-05T22:16:18+00:00</t:ClientEventTimeLocal>
         <t:ClientSessionId>00000000-0000-0000-0000-000000000012</t:ClientSessionId>
         <t:ClientVersion>15.01.0101.01</t:ClientVersion>
         <t:ClientId>Web</t:ClientId>
         <t:TransactionId>b56ad16e-5d5a-4574-90f8-b8dd57382be6</t:TransactionId>
         <t:EventType>EntityAdded</t:EventType>
         <t:TargetEntityList>["user1@ms7.com"]</t:TargetEntityList>
         <t:SourceOfEntityAdded>EntityRelevanceApi</t:SourceOfEntityAdded>
         <t:JSONPropertyBag></t:JSONPropertyBag>
</t:EntityFeedbackEntry>
</m:EntityFeedbackEntries>
      </m:AddEntityFeedback>
   </soap:Body>
</soap:Envelope>

```

> [!NOTE]
> FindPeople response トランザクション ID を AddEntityFeedback 要求トランザクション ID として使用します。 
  
#### <a name="addentityfeedback-response"></a>AddEntityFeedback の応答

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
    <s:Header>
        <h:ServerVersionInfo MajorVersion="15" MinorVersion="1" MajorBuildNumber="302" MinorBuildNumber="0" Version="V2_68" xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
    </s:Header>
    <s:Body>
        <AddEntityFeedbackResponse ResponseClass="Success" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
            <ResponseCode>NoError</ResponseCode>
            <ErrorCount>0</ErrorCount>
            <ErrorDetails />
        </AddEntityFeedbackResponse>
    </s:Body>
</s:Envelope>

```


