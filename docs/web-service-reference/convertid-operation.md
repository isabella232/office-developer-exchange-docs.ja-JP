---
title: ConvertId 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ConvertId
api_type:
- schema
ms.assetid: 47d96cf6-9e2f-4fc0-9682-7258d3fbf918
description: ConvertId EWS 操作に関する情報を検索します。
ms.openlocfilehash: 04f20d8446ab3117adb3f00ea17f93c068eeffb9
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59536632"
---
# <a name="convertid-operation"></a>ConvertId 操作

ConvertId EWS **操作に** 関する情報を検索します。 
  
**ConvertId** Exchange Web Services (EWS) 操作は、Office 365 の一部として Exchange Online、Exchange Online、および Exchange Server 2013 から始まるオンプレミスバージョンの Exchange で受け入れられる形式の間でアイテム識別子とフォルダー識別子を変換します。 
  
## <a name="using-the-convertid-operation"></a>ConvertId 操作の使用
<a name="bk_usingConvertId"> </a>

ConvertId 操作を使用して、次の識別子 **を変換** できます。 
  
- 2007 年の最初のリリース バージョンの EWS Exchange形式。 これは  `EwsLegacyId` [、IdFormat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx) 列挙の列挙値で表されます。 
    
- 2007 SP1 または 2010 Exchange EWS の識別子Exchange形式。 これは IdFormat の列挙  `EwsId` 値で [表されます](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx)。
    
- MAPI 識別子 (プロパティの **プロパティPR_ENTRYIDします** 。 これは  `EntryId` [、IdFormat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx) 列挙の列挙値で表されます。 
    
- 利用可能な予定表のイベント識別子。 これは、16 進数でエンコードされたプロパティ **のPR_ENTRYID** です。 これは IdFormat の列挙  `HexEntryId` 値で [表されます](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx)。
    
- ストアExchange識別子。 これは IdFormat の列挙  `StoreId` 値で [表されます](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx)。 **ConvertId 操作** では、パブリック フォルダー識別子が EWS 識別子からストア識別子に変換されるのではありません。 
    
- このOutlook Web App識別子です。 これは IdFormat の列挙  `OwaId` 値で [表されます。](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx)
    
    この識別子からユーザーに作成された URL のOutlook Web Appはサポートされていません。 このOutlook Web App識別子は、2007 年および 2010 年Exchange 2010 年Exchange適用されます。 Outlook Web App 2013 Exchange Onlineから始まるExchangeバージョンの場合、EWS Exchange Serverが使用されます。
    
EWS 識別子から 2013 年および 2013 年 2013 年のストア識別子にパブリック フォルダー識別子を変換する場合 **、ConvertId** 操作Exchange Online Exchange動作しません。 回避策として、返された識別子を手動で更新してください。 識別子を手動で更新するには、次の操作を行います。 
  
1. アプリケーション コードで、ターゲット アイテム/フォルダーがパブリック フォルダー内にあるかどうかを判断します。 
    
2. Base64 でエンコードされた識別子文字列をデコードします。
    
3. 型バイト (21st バイト) の値が 7 を持つ必要があることを確認します。 値 7 は、識別子が正しくない形式を示します。
    
4. 最初の 4 バイトをスキップします。 これらは 0 に設定する必要があります。
    
5. 次の 16 バイトを次の GUID で更新します。1A447390AA6611CD9BC800AA002FC45A
    
6. 値 9 で次のバイト (バイト型) を更新します。
    
7. 識別子を Base64 エンコード文字列に変更します。
    
> [!NOTE]
> **ConvertId 操作は**、特定の SMTP アドレスに有効な形式が設定されているのを検証します。 この操作では、SMTP アドレスが有効なメールボックスを表すかどうかは判断されません。 
  
**ConvertId 操作では**、次の表に示す SOAP ヘッダーを使用できます。 
  
**表 1.ConvertId 操作 SOAP ヘッダー**

|**Header**|**Element**|**説明**|
|:-----|:-----|:-----|
|偽装  <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |クライアント アプリケーションが偽装しているユーザーを識別します。 これは要求に適用されます。  <br/> |
|RequestVersion  <br/> |[RequestServerVersion](requestserverversion.md) <br/> |操作要求のスキーマ バージョンを識別します。これは要求に適用されます。  <br/> |
|ServerVersion  <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |要求に応答したサーバーのバージョンを識別します。 これは、応答に適用されます。  <br/> |
   
## <a name="convertid-operation-request-example"></a>ConvertId 操作要求の例
<a name="bk_usingConvertId"> </a>

ConvertId 要求の次の **例は**、EWS 識別子から識別子に変換するOutlook Web Appします。 
  
この [操作を機能](requestserverversion.md) するには、SOAP ヘッダーの RequestServerVersion 要素を Exchange2007_SP1以降に設定する必要があります。 
  
> [!NOTE]
> アイテム識別子は、読みやすさを維持するために短縮されました。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010"/>
  </soap:Header>
  <soap:Body>
    <ConvertId xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               DestinationFormat="OwaId">
      <SourceIds>
        <t:AlternateId Format="EwsId" Id="AAMkAGZhN2IxYTA0LWNiNzItN="
                       Mailbox="user1@example.com"/>
      </SourceIds>
    </ConvertId>
  </soap:Body>
</soap:Envelope>
```

## <a name="convertid-operation-response-example"></a>ConvertId 操作応答の例
<a name="bk_usingConvertId"> </a>

次の例は **、ConvertId** 要求に対する正常な応答を示しています。 この応答の例には、識別子Outlook Web App含まれている。 
  
> [!NOTE]
> 読Outlook Web Appを維持するために、識別子の値が短縮されました。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="1" 
                         MajorBuildNumber="191" MinorBuildNumber="0" 
                         Version="Exchange2010" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ConvertIdResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

## <a name="convertid-operation-error-response-example"></a>ConvertId 操作エラー応答の例
<a name="bk_usingConvertId"> </a>

次の例は、誤った種類の識別子形式を含む要求に対する応答を示しています。
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <ServerVersionInfo MajorVersion="8" MinorVersion="1" 
                       MajorBuildNumber="206" MinorBuildNumber="0"
                       Version="Exchange2010" 
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ConvertIdResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

EWS 識別子の形式は、Exchange 2007 と Exchange 2007 Service Pack 1 (SP1) の初期リリース バージョンの間で変更されました。 Exchange Online Office 365、Exchange Online、および Exchange のオンプレミス バージョンの一部として、Exchange 2010 で始まるExchange SP1 が使用する識別子形式を使用します。
  
**ConvertId 操作は**、パブリック フォルダー識別子を EWS 識別子から Exchange 2007 および Exchange 2010 に変換します。 
  
## <a name="see-also"></a>関連項目
<a name="bk_ConvertIdVersionDiff"> </a>

- [識別子の変換](https://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)
    
- [ConvertIdType](https://msdn.microsoft.com/library/ExchangeWebServices.ConvertIdType.aspx)
    
- [ConvertId](https://msdn.microsoft.com/library/ExchangeWebServices.ExchangeServiceBinding.ConvertId.aspx)
    

