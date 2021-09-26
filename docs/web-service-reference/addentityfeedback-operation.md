---
title: AddEntityFeedback 操作
manager: luken
ms.date: 4/18/2016
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 00e40197-5794-4268-b937-bd65aa044890
description: AddEntityFeedback 操作は、サーバー側の問題に対応するエラー情報を返します。
ms.openlocfilehash: d4322bcc075c8c68b1f3d5f2ae22badea02be452
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546827"
---
# <a name="addentityfeedback-operation"></a>AddEntityFeedback 操作

**AddEntityFeedback 操作は**、サーバー側の問題に対応するエラー情報を返します。 
  
この操作は、ログに記録されるイベントの種類に依存します。 最も重要なイベントの 1 つは、選択されているエンティティに対応する **EntityAdded** です。 この操作はバッチなので、1 つの要求でエントリのバッチをログに記録するために使用できます。 
  
## <a name="findpeople-request-examples"></a>FindPeople 要求の例

**AddEntityFeedback 操作** は、クライアントがサービスによって返されるエンティティとの対話の詳細をログに記録する方法を提供します。 これは、各クライアントの背後での関連性を向上させるシグナルとして使用できます。 例えば、クライアントは、この操作を使用して **、FindPeople** から返されるユーザー エンティティに対するフィードバックを提供できます。
  
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

### <a name="the-request-soap-body-contents"></a>要求 SOAP 本文の内容

soap 要求には、1 つの **要素 EntityFeedbackEntries が含まれる**。 次に **、EntityFeedbackEntry オブジェクトの配列が含** まれます。 配列内の各エントリには、次の要素を含めできます。 
  
|**要求のパラメータ**|**必須**|**説明**|**型**|
|:-----|:-----|:-----|:-----|
|**ClientEventTimeUtc** <br/> |必要  <br/> |クライアント側でイベントが発生した UTC 時刻。  <br/> |DateTime  <br/> |
|**ClientEventTimeLocal** <br/> |必要  <br/> |クライアント側でイベントが発生したローカル時刻。  <br/> |DateTime  <br/> |
|**ClientId** <br/> |必要  <br/> |クライアントの種類 (例: Outlook、OWA など)。  <br/> |ClientIDType 列挙  <br/> |
|**ClientSessionId** <br/> |必要  <br/> |GUID セッション ID を識別します。 クライアントで生成されます。  <br/> |GUID  <br/> |
|**ClientVersion** <br/> |必要  <br/> |クライアントのバージョン (例: 15.01.0101.000)。  <br/> |String  <br/> |
|**EntityAddSource** <br/> |いいえ  <br/> |EntityAded のソース (EntityRelevanceAPI、型、貼り付けなど)。  <br/> |EntityAddSource 列挙  <br/> |
|**EntrySequenceNumber** <br/> |必要  <br/> |クライアント セッションごとの増分整数。 データ損失の検出に使用されます。  <br/> |Int  <br/> |
|**EventType** <br/> |必要  <br/> |イベントの種類 (エンティティの追加、エンティティの削除など)。  <br/> |String  <br/> |
|**JSONPropertyBag** <br/> |いいえ  <br/> |イベントに関連付けられた追加のプロパティ (キーと値のペアの JSON BLOB)。  <br/> |JSON Blob  <br/> |
|**TargetEntityList** <br/> |いいえ  <br/> |イベントに関連付けられているエンティティの一覧。  <br/> |JSON 文字列  <br/> |
|**TransactionId** <br/> |いいえ  <br/> |クエリ ログ内の ID を関連付ける ID (GUID)。  <br/> |String  <br/> |
   
### <a name="successful-addentityfeedback-operation-response"></a>AddEntityFeedback 操作の応答の成功

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

### <a name="the-response-soap-body-contains-the-following-elements"></a>応答 SOAP 本文には、次の要素が含まれています

#### <a name="errors"></a>エラー 
  
API はフィードバック エントリのバッチをログに記録できます。できるすべてのログを記録します。 このフィールドは、ログに記録されていないエラー エントリの数を表します。
    
#### <a name="errordetails"></a>ErrorDetails
  
上記のエラーに関する詳細は、 `;` によって分離されます。
    
### <a name="currently-supported-values"></a>現在サポートされている値

|**ClientIdType 列挙**|
|:-----|
|デスクトップ  <br/> |
|Exchange  <br/> |
|IMAP4  <br/> |
|Lync  <br/> |
|MacMail  <br/> |
|MacOutlook  <br/> |
|Mobile  <br/> |
|Other  <br/> |
|Outlook  <br/> |
|OutlookService  <br/> |
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

EWS に汎用的なエラー コードについては [、「ResponseCode」を参照してください](responsecode.md)。
  
### <a name="example-of-addentityfeedback-in-conjunction-with-findpeople"></a>FindPeople と組み合わせて AddEntityFeedback の例

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
> AddEntityFeedback 要求トランザクション ID として FindPeople 応答トランザクション ID を使用する。 
  
#### <a name="addentityfeedback-response"></a>AddEntityFeedback 応答

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


