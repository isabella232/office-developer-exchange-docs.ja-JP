---
title: AddEntityFeedback 操作
manager: luken
ms.date: 4/18/2016
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 00e40197-5794-4268-b937-bd65aa044890
description: AddEntityFeedback 操作では、サーバー側の問題に対応するエラー情報を返します。
ms.openlocfilehash: b695806f543827d78aea139ffcbd7e4af58b9fef
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759285"
---
# <a name="addentityfeedback-operation"></a>AddEntityFeedback 操作

**AddEntityFeedback**操作では、サーバー側の問題に対応するエラー情報を返します。 
  
この操作は、ログに記録されるイベントの種類に依存しています。 いずれかの最も重要なイベントは、 **EntityAdded**、選択されているエンティティに対応します。 この操作は、1 つの要求のバッチのエントリをログに記録するために使用できるように、バッチをします。 
  
## <a name="findpeople-request-examples"></a>FindPeople 要求の例

**AddEntityFeedback**操作は、クライアント サービスによって返されるエンティティとの対話の詳細をログに記録するための手段を提供します。 これは、クライアントごとにバック グラウンドで関連性を向上させるために、信号として使用できます。 など、クライアントでは、 **FindPeople**から返されたユーザー エンティティに関するフィードバックを提供するのにこの操作を使用できます。
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
                             xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                             xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="the-request-soap-body-contents"></a>要求の SOAP 本文の内容

Soap 要求には、 **EntityFeedbackEntries**の単一の要素が含まれています。 これには、 **EntityFeedbackEntry**オブジェクトの配列に含まれています。 配列内の各エントリには、次の要素を含めることができます。 
  
|**要求パラメーター**|**必須**|**説明**|**型**|
|:-----|:-----|:-----|:-----|
|**ClientEventTimeUtc** <br/> |はい  <br/> |UTC 時刻クライアント側のイベントが発生しました。  <br/> |DateTime  <br/> |
|**ClientEventTimeLocal** <br/> |はい  <br/> |現地時刻は、クライアント側のイベントが発生しました。  <br/> |DateTime  <br/> |
|**クライアント Id** <br/> |はい  <br/> |クライアント (たとえば、Outlook、OWA など) の種類です。  <br/> |ClientIDType 列挙型  <br/> |
|**ClientSessionId** <br/> |はい  <br/> |GUID は、セッション ID を識別します。 クライアント上で生成されます。  <br/> |GUID  <br/> |
|**ClientVersion** <br/> |はい  <br/> |(15.01.0101.000 など) のクライアントのバージョンです。  <br/> |String  <br/> |
|**EntityAddSource** <br/> |いいえ  <br/> |EntityAded (など、EntityRelevanceAPI、種類、貼り付け) のソースです。  <br/> |EntityAddSource 列挙型  <br/> |
|**EntrySequenceNumber** <br/> |はい  <br/> |クライアント セッションごとの増分の整数です。 データの損失を検出するために使用します。  <br/> |整数型 (Int)  <br/> |
|**EventType** <br/> |はい  <br/> |(などのエンティティが追加されると、エンティティが削除される) イベントの種類です。  <br/> |String  <br/> |
|**JSONPropertyBag** <br/> |いいえ  <br/> |イベント (キーと値のペアの JSON blob) に関連付けられた追加のプロパティ。  <br/> |JSON Blob  <br/> |
|**TargetEntityList** <br/> |いいえ  <br/> |イベントに関連付けられているエンティティの一覧です。  <br/> |JSON 文字列  <br/> |
|**TransactionId** <br/> |いいえ  <br/> |ID (GUID) クエリ ログの ID を関連付けることです。  <br/> |String  <br/> |
   
### <a name="successful-addentityfeedback-operation-response"></a>AddEntityFeedback 操作の成功の応答

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
    <s:Header>
        <h:ServerVersionInfo MajorVersion="15" 
                                MinorVersion="1" 
                                MajorBuildNumber="228" 
                                MinorBuildNumber="0" 
                                Version="V2_49" 
                                xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                                xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                                xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
    </s:Header>
    <s:Body>
        <AddEntityFeedbackResponse ResponseClass="Success" 
                                                              xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" 
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
  
フィードバック項目のバッチをログに記録できる API、ことをすべてログに記録しました。 このフィールドは、エラーのエントリが記録されていないの数を表します。
    
#### <a name="errordetails"></a>ErrorDetails
  
によって上記のエラーに関連する詳細を分離`;`。
    
### <a name="currently-supported-values"></a>現在サポートされている値

|**ClientIdType 列挙型**|
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
   
|**EntityAddSource 列挙型**|
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
   
### <a name="addentityfeedback-operation-error-response"></a>AddEntityFeedback 操作のエラー応答

EWS を汎用のエラー コードは、 [ResponseCode](responsecode.md)を参照してください。
  
### <a name="example-of-addentityfeedback-in-conjunction-with-findpeople"></a>FindPeople と共に AddEntityFeedback の例

#### <a name="findpeople-request"></a>FindPeople 要求
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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
        <h:ServerVersionInfo MajorVersion="15" MinorVersion="1" MajorBuildNumber="302" MinorBuildNumber="0" Version="V2_68" xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
    </s:Header>
    <s:Body>
        <FindPeopleResponse ResponseClass="Success" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
            <ResponseCode>NoError</ResponseCode>
            <People>
                <Persona xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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
> FindPeople を使用して AddEntityFeedback 要求のトランザクションとしてトランザクション ID を応答の id。 
  
#### <a name="addentityfeedback-response"></a>AddEntityFeedback 応答

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
    <s:Header>
        <h:ServerVersionInfo MajorVersion="15" MinorVersion="1" MajorBuildNumber="302" MinorBuildNumber="0" Version="V2_68" xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
    </s:Header>
    <s:Body>
        <AddEntityFeedbackResponse ResponseClass="Success" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
            <ResponseCode>NoError</ResponseCode>
            <ErrorCount>0</ErrorCount>
            <ErrorDetails />
        </AddEntityFeedbackResponse>
    </s:Body>
</s:Envelope>

```


