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
description: コンバーターの EWS 操作に関する情報を検索します。
ms.openlocfilehash: 36bd47d3fc7c7ca7cea7b38222abb25fba6074ac
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44452553"
---
# <a name="convertid-operation"></a>ConvertId 操作

**コンバーター**の EWS 操作に関する情報を検索します。 
  
変換**tid** Exchange Web サービス (EWS) 操作は、アイテムとフォルダーの識別子を、exchange Online、Office 365 の一部としての exchange Online、exchange Server 2013 以降のオンプレミスバージョンの exchange で受け入れられる形式の間で変換します。 
  
## <a name="using-the-convertid-operation"></a>[収束 Tid 操作の使用方法」
<a name="bk_usingConvertId"> </a>

次の識別子は、[変換**tid**操作を使用して変換できます。 
  
- Exchange 2007 の最初のリリースバージョンでの EWS の識別子形式。 これは `EwsLegacyId` [idformat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx)列挙の列挙値で表されます。 
    
- Exchange 2007 SP1 または Exchange 2010 の EWS の識別子形式。 これは `EwsId` [idformat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx)の列挙値で表されます。
    
- **PR_ENTRYID**プロパティのように、MAPI 識別子を示します。 これは `EntryId` [idformat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx)列挙の列挙値で表されます。 
    
- 可用性カレンダーイベント識別子。 これは、 **PR_ENTRYID**プロパティを16進数でエンコードした表記です。 これは `HexEntryId` [idformat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx)の列挙値で表されます。
    
- Exchange ストア識別子。 これは `StoreId` [idformat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx)の列挙値で表されます。 変換**tid**操作では、パブリックフォルダーの識別子が EWS 識別子からストア識別子に変換されることはありません。 
    
- Outlook Web App 識別子。 これは `OwaId` [idformat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx)の列挙値で表されます。
    
    この識別子から Outlook Web App に対して作成された Url の引き渡しはサポートされていません。 Outlook Web App 識別子は、Exchange 2007 および Exchange 2010 に適用されます。 Exchange Online の Outlook Web App と exchange Server 2013 以降のバージョンの Exchange は、EWS 識別子を使用します。
    
パブリックフォルダーの識別子を EWS 識別子から Exchange Online および Exchange 2013 のストア識別子に変換するときに、変換**tid**操作が期待どおりに機能しません。 回避策として、返された識別子を手動で更新してください。 識別子を手動で更新するには、次のようにします。 
  
1. アプリケーションコードで、ターゲットアイテム/フォルダーがパブリックフォルダーにあるかどうかを確認します。 
    
2. Base64 でエンコードされた識別子文字列をデコードします。
    
3. Type byte (21 バイト) の値が7であることを確認します。 値が7の場合、識別子の形式が正しくないことを示します。
    
4. 最初の4バイトをスキップします。 0に設定する必要があります。
    
5. 次の16バイトを次の GUID で更新します。1A447390AA6611CD9BC800AA002FC45A
    
6. 次のバイト (type byte) を値9で更新します。
    
7. 識別子を Base64 でエンコードされた文字列に変更します。
    
> [!NOTE]
> 、**指定された**SMTP アドレスが有効な形式であることを検証します。 この操作では、SMTP アドレスが有効なメールボックスを表しているかどうかは判断されません。 
  
次**の表**に記載されている SOAP ヘッダーを使用することができます。 
  
**表1バケット操作の SOAP ヘッダーの収束**

|**Header**|**要素**|**説明**|
|:-----|:-----|:-----|
|偽装  <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |クライアントアプリケーションが偽装しているユーザーを識別します。 これは要求に適用されます。  <br/> |
|RequestVersion  <br/> |[RequestServerVersion](requestserverversion.md) <br/> |要求に適用される操作要求のスキーマバージョンを識別します。  <br/> |
|ServerVersion  <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |要求に応答したサーバーのバージョンを識別します。 これは応答に適用されます。  <br/> |
   
## <a name="convertid-operation-request-example"></a>収束 Tid 操作要求の例
<a name="bk_usingConvertId"> </a>

次の例**は、EWS**識別子から Outlook Web App 識別子に変換する方法を示しています。 
  
この操作を動作させるには、SOAP ヘッダーの[RequestServerVersion](requestserverversion.md)要素を Exchange2007_SP1 以降に設定する必要があります。 
  
> [!NOTE]
> アイテム識別子は読みやすくするために短縮されています。 
  
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

## <a name="convertid-operation-response-example"></a>収束 Tid 操作の応答の例
<a name="bk_usingConvertId"> </a>

次の例では、[**コンバーター tid**要求に成功した応答を示します。 この応答の例には、Outlook Web App の識別子が含まれています。 
  
> [!NOTE]
> 読みやすくするために、Outlook Web App 識別子が短縮されています。 
  
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

## <a name="convertid-operation-error-response-example"></a>コンバーターのエラー応答の例
<a name="bk_usingConvertId"> </a>

次の例は、誤った種類の識別子形式を含む要求への応答を示しています。
  
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

Exchange 2007 と Exchange 2007 Service Pack 1 (SP1) の最初のリリースバージョン間で EWS 識別子形式が変更されました。 Exchange 2010 以降の Office 365 の一部としての exchange Online、exchange Online、およびオンプレミスバージョンの exchange では、Exchange 2007 SP1 が使用するものと同じ識別子の形式を使用します。
  
変換**tid**操作は、パブリックフォルダーの識別子を EWS 識別子から exchange 2007 と exchange 2010 のストア識別子に変換します。 
  
## <a name="see-also"></a>関連項目
<a name="bk_ConvertIdVersionDiff"> </a>

- [識別子の変換](https://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)
    
- [ConvertIdType](https://msdn.microsoft.com/library/ExchangeWebServices.ConvertIdType.aspx)
    
- [ConvertId](https://msdn.microsoft.com/library/ExchangeWebServices.ExchangeServiceBinding.ConvertId.aspx)
    

