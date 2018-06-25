---
title: ConvertId 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConvertId
api_type:
- schema
ms.assetid: 47d96cf6-9e2f-4fc0-9682-7258d3fbf918
description: 操作 ConvertId EWS についての情報を検索します。
ms.openlocfilehash: 5f1bcd8a9f0adc25b7c598ef10cc6bb139dfe02d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759768"
---
# <a name="convertid-operation"></a>ConvertId 操作

**ConvertId** EWS の操作に関する情報を検索します。 
  
**ConvertId** Exchange Web サービス (EWS) の操作 Exchange オンラインになって、Office 365 の一部として Exchange Online で受け入れられる形式の間でのアイテムおよびフォルダーの識別子を変換し、設置型バージョンの Exchange が Exchange Server で始まる2013。 
  
## <a name="using-the-convertid-operation"></a>ConvertId 操作を使用します。
<a name="bk_usingConvertId"> </a>

**ConvertId**操作を使用して、次の識別子を変換できます。 
  
- EWS の初期リリース版の Exchange 2007 での識別子形式です。 これは、 `EwsLegacyId` [フェース id フォーマット](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx)の列挙体の列挙値。 
    
- EWS では、Exchange 2007 SP1 または Exchange 2010 の識別子の形式です。 これは、 `EwsId` [フェース id フォーマット](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx)の列挙値。
    
- **PR_ENTRYID**プロパティと同様に、MAPI 識別子です。 これは、 `EntryId` [フェース id フォーマット](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx)の列挙体の列挙値。 
    
- 可用性の予定表イベントの識別子です。 これは、 **PR_ENTRYID**プロパティの 16 進数でエンコードされた表現です。 これは、 `HexEntryId` [フェース id フォーマット](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx)の列挙値。
    
- Exchange ストアの識別子です。 これは、 `StoreId` [フェース id フォーマット](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx)の列挙値。 **ConvertId**操作は変換されませんパブリック フォルダーの識別子 EWS id からストア識別子に。 
    
- Outlook Web App の識別子です。 これは、 `OwaId` [フェース id フォーマット](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx)の列挙値
    
    Outlook Web App にこの識別子から作成される Url を渡すことはサポートされていません。 Outlook Web App id は、Exchange 2007 および Exchange 2010 に適用されます。 Exchange Online とのバージョンの Exchange が Exchange Server 2013 で始まるため、Outlook Web App では、EWS 識別子を使用します。
    
**ConvertId**操作は、ストアの識別子には、オンラインの Exchange および Exchange 2013 の EWS 識別子からパブリック フォルダーの識別子を変換するときに期待どおりには動作しません。 回避策として返される id を手動で更新することができます。 Id を手動で更新するには。 
  
1. アプリケーション コードでは、対象のアイテムまたはフォルダーが、パブリック フォルダーかどうかを決定します。 
    
2. 識別子の Base64 でエンコードされた文字列をデコードします。
    
3. 確認する型のバイト (21 バイト) は、7 の値を持ちます。 7 の値は、誤った形式の識別子であることを示します。
    
4. 最初の 4 バイトをスキップします。 それらはゼロに設定する必要があります。
    
5. 次の GUID を使用して、次の 16 バイトを更新: 1A447390AA6611CD9BC800AA002FC45A
    
6. 9 の値を持つには、次のバイト (byte 型) を更新します。
    
7. Base64 でエンコードされた文字列に識別子を変更します。
    
> [!NOTE]
> **ConvertId**操作は、指定した SMTP アドレスが有効な形式を持っているを検証します。 操作は、SMTP アドレスが有効なメールボックスを表すかどうかを判断できません。 
  
**ConvertId**操作は、次の表に記載されている SOAP ヘッダーを使用できます。 
  
**表 1 です。ConvertId 操作の SOAP ヘッダー**

|**Header**|**要素**|**説明**|
|:-----|:-----|:-----|
|偽装  <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |クライアント アプリケーションが偽装するユーザーを識別します。 これは、要求に適用されます。  <br/> |
|RequestVersion  <br/> |[RequestServerVersion](requestserverversion.md) <br/> |これは、要求に適用する操作要求のスキーマのバージョンを識別します。  <br/> |
|ServerVersion  <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |要求に応答するサーバーのバージョンを識別します。 これは、応答に適用されます。  <br/> |
   
## <a name="convertid-operation-request-example"></a>ConvertId 操作の要求の例
<a name="bk_usingConvertId"> </a>

**ConvertId**要求の次の例では、EWS 識別子から Outlook Web App の識別子に変換する方法を示します。 
  
Exchange2007_SP1 に、後でこの操作を行うには、SOAP ヘッダー内の[RequestServerVersion](requestserverversion.md)要素を設定してください。 
  
> [!NOTE]
> 項目の識別子が読みやすさを保持するために小さすぎます。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010"/>
  </soap:Header>
  <soap:Body>
    <ConvertId xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               DestinationFormat="OwaId">
      <SourceIds>
        <t:AlternateId Format="EwsId" Id="AAMkAGZhN2IxYTA0LWNiNzItN="
                       Mailbox="user1@example.com"/>
      </SourceIds>
    </ConvertId>
  </soap:Body>
</soap:Envelope>
```

## <a name="convertid-operation-response-example"></a>ConvertId 操作の応答の例
<a name="bk_usingConvertId"> </a>

**ConvertId**要求に正常な応答の例を次に示します。 この応答の例には、Outlook Web App の識別子が含まれています。 
  
> [!NOTE]
> 読みやすさを保持するために Outlook Web App id が小さすぎます。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="1" 
                         MajorBuildNumber="191" MinorBuildNumber="0" 
                         Version="Exchange2010" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ConvertIdResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseMessages>
        <ConvertIdResponseMessage ResponseClass="Success">
          <ResponseCode>NoError</ResponseCode>
          <AlternateId xsi:type="t:AlternateIdType" Format="OwaId" Id="RgAAAAAS2%2" 
                         Mailbox="user@example.com" />
        </ConvertIdResponseMessage>
      </ResponseMessages>
    </ConvertIdResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="convertid-operation-error-response-example"></a>ConvertId 操作のエラー応答の例
<a name="bk_usingConvertId"> </a>

識別子の形式の間違った型を含む要求に対する応答の例を次に示します。
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <ServerVersionInfo MajorVersion="8" MinorVersion="1" 
                       MajorBuildNumber="206" MinorBuildNumber="0"
                       Version="Exchange2010" 
                       xmlns="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ConvertIdResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseMessages>
        <ConvertIdResponseMessage ResponseClass="Error">
          <MessageText>Id is malformed.</MessageText>
          <ResponseCode>ErrorInvalidIdMalformed</ResponseCode>
          <DescriptiveLinkKey>0</DescriptiveLinkKey>
        </ConvertIdResponseMessage>
      </ResponseMessages>
    </ConvertIdResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="version-differences"></a>バージョンの相違点
<a name="bk_ConvertIdVersionDiff"> </a>

初期リリース版の Exchange 2007 および Exchange 2007 Service Pack 1 (SP1) の間で変更する EWS 識別子の形式です。 Exchange オンライン Office 365 の一部として、Exchange Online では、および設置型のバージョンの Exchange が Exchange 2010 で始まるは、Exchange 2007 SP1 を使用している同じ識別子の形式を使用します。
  
**ConvertId**操作は、パブリック フォルダーの識別子を EWS 識別子から Exchange 2007 および Exchange 2010 ストア識別子に変換します。 
  
## <a name="see-also"></a>関連項目
<a name="bk_ConvertIdVersionDiff"> </a>

- [識別子に変換します。](http://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)
    
- [ConvertIdType](https://msdn.microsoft.com/library/ExchangeWebServices.ConvertIdType.aspx)
    
- [ConvertId](https://msdn.microsoft.com/library/ExchangeWebServices.ExchangeServiceBinding.ConvertId.aspx)
    

