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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44452553"
---
# <a name="convertid-operation"></a><span data-ttu-id="6a044-103">ConvertId 操作</span><span class="sxs-lookup"><span data-stu-id="6a044-103">ConvertId operation</span></span>

<span data-ttu-id="6a044-104">**コンバーター**の EWS 操作に関する情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="6a044-104">Find information about the **ConvertId** EWS operation.</span></span> 
  
<span data-ttu-id="6a044-105">変換**tid** Exchange Web サービス (EWS) 操作は、アイテムとフォルダーの識別子を、exchange Online、Office 365 の一部としての exchange Online、exchange Server 2013 以降のオンプレミスバージョンの exchange で受け入れられる形式の間で変換します。</span><span class="sxs-lookup"><span data-stu-id="6a044-105">The **ConvertId** Exchange Web Services (EWS) operation converts item and folder identifiers between formats that are accepted by Exchange Online, Exchange Online as part of Office 365, and on-premises versions of Exchange starting with Exchange Server 2013.</span></span> 
  
## <a name="using-the-convertid-operation"></a><span data-ttu-id="6a044-106">[収束 Tid 操作の使用方法」</span><span class="sxs-lookup"><span data-stu-id="6a044-106">Using the ConvertId operation</span></span>
<span data-ttu-id="6a044-107"><a name="bk_usingConvertId"> </a></span><span class="sxs-lookup"><span data-stu-id="6a044-107"><a name="bk_usingConvertId"> </a></span></span>

<span data-ttu-id="6a044-108">次の識別子は、[変換**tid**操作を使用して変換できます。</span><span class="sxs-lookup"><span data-stu-id="6a044-108">You can convert the following identifiers by using the **ConvertId** operation:</span></span> 
  
- <span data-ttu-id="6a044-109">Exchange 2007 の最初のリリースバージョンでの EWS の識別子形式。</span><span class="sxs-lookup"><span data-stu-id="6a044-109">The identifier format for EWS in the initial release version of Exchange 2007.</span></span> <span data-ttu-id="6a044-110">これは `EwsLegacyId` [idformat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx)列挙の列挙値で表されます。</span><span class="sxs-lookup"><span data-stu-id="6a044-110">This is represented by the  `EwsLegacyId` enumeration value in the [IdFormat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx) enumeration.</span></span> 
    
- <span data-ttu-id="6a044-111">Exchange 2007 SP1 または Exchange 2010 の EWS の識別子形式。</span><span class="sxs-lookup"><span data-stu-id="6a044-111">The identifier format for EWS in Exchange 2007 SP1 or Exchange 2010.</span></span> <span data-ttu-id="6a044-112">これは `EwsId` [idformat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx)の列挙値で表されます。</span><span class="sxs-lookup"><span data-stu-id="6a044-112">This is represented by the  `EwsId` enumeration value in [IdFormat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx).</span></span>
    
- <span data-ttu-id="6a044-113">**PR_ENTRYID**プロパティのように、MAPI 識別子を示します。</span><span class="sxs-lookup"><span data-stu-id="6a044-113">The MAPI identifier, as in the **PR_ENTRYID** property.</span></span> <span data-ttu-id="6a044-114">これは `EntryId` [idformat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx)列挙の列挙値で表されます。</span><span class="sxs-lookup"><span data-stu-id="6a044-114">This is represented by the  `EntryId` enumeration value in the [IdFormat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx) enumeration.</span></span> 
    
- <span data-ttu-id="6a044-115">可用性カレンダーイベント識別子。</span><span class="sxs-lookup"><span data-stu-id="6a044-115">The availability calendar event identifier.</span></span> <span data-ttu-id="6a044-116">これは、 **PR_ENTRYID**プロパティを16進数でエンコードした表記です。</span><span class="sxs-lookup"><span data-stu-id="6a044-116">This is a hexadecimal-encoded representation of the **PR_ENTRYID** property.</span></span> <span data-ttu-id="6a044-117">これは `HexEntryId` [idformat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx)の列挙値で表されます。</span><span class="sxs-lookup"><span data-stu-id="6a044-117">This is represented by the  `HexEntryId` enumeration value in [IdFormat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx).</span></span>
    
- <span data-ttu-id="6a044-118">Exchange ストア識別子。</span><span class="sxs-lookup"><span data-stu-id="6a044-118">The Exchange store identifier.</span></span> <span data-ttu-id="6a044-119">これは `StoreId` [idformat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx)の列挙値で表されます。</span><span class="sxs-lookup"><span data-stu-id="6a044-119">This is represented by the  `StoreId` enumeration value in [IdFormat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx).</span></span> <span data-ttu-id="6a044-120">変換**tid**操作では、パブリックフォルダーの識別子が EWS 識別子からストア識別子に変換されることはありません。</span><span class="sxs-lookup"><span data-stu-id="6a044-120">The **ConvertId** operation does not convert public folder identifiers from the EWS identifier to the store identifier.</span></span> 
    
- <span data-ttu-id="6a044-121">Outlook Web App 識別子。</span><span class="sxs-lookup"><span data-stu-id="6a044-121">The Outlook Web App identifier.</span></span> <span data-ttu-id="6a044-122">これは `OwaId` [idformat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx)の列挙値で表されます。</span><span class="sxs-lookup"><span data-stu-id="6a044-122">This is represented by the  `OwaId` enumeration value in [IdFormat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx)</span></span>
    
    <span data-ttu-id="6a044-123">この識別子から Outlook Web App に対して作成された Url の引き渡しはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6a044-123">The passing of URLs that are created from this identifier to Outlook Web App is not supported.</span></span> <span data-ttu-id="6a044-124">Outlook Web App 識別子は、Exchange 2007 および Exchange 2010 に適用されます。</span><span class="sxs-lookup"><span data-stu-id="6a044-124">The Outlook Web App identifier is applicable to Exchange 2007 and Exchange 2010.</span></span> <span data-ttu-id="6a044-125">Exchange Online の Outlook Web App と exchange Server 2013 以降のバージョンの Exchange は、EWS 識別子を使用します。</span><span class="sxs-lookup"><span data-stu-id="6a044-125">Outlook Web App for Exchange Online and versions of Exchange starting with Exchange Server 2013 uses EWS identifiers.</span></span>
    
<span data-ttu-id="6a044-126">パブリックフォルダーの識別子を EWS 識別子から Exchange Online および Exchange 2013 のストア識別子に変換するときに、変換**tid**操作が期待どおりに機能しません。</span><span class="sxs-lookup"><span data-stu-id="6a044-126">The **ConvertId** operation does not work as expected when converting public folder identifiers from the EWS identifier to the store identifier in Exchange Online and Exchange 2013.</span></span> <span data-ttu-id="6a044-127">回避策として、返された識別子を手動で更新してください。</span><span class="sxs-lookup"><span data-stu-id="6a044-127">You can manually update the identifier that is returned as a workaround.</span></span> <span data-ttu-id="6a044-128">識別子を手動で更新するには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="6a044-128">To manually update the identifier:</span></span> 
  
1. <span data-ttu-id="6a044-129">アプリケーションコードで、ターゲットアイテム/フォルダーがパブリックフォルダーにあるかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="6a044-129">In your application code, determine whether the target item/folder is in a public folder.</span></span> 
    
2. <span data-ttu-id="6a044-130">Base64 でエンコードされた識別子文字列をデコードします。</span><span class="sxs-lookup"><span data-stu-id="6a044-130">Decode the Base64-encoded identifier string.</span></span>
    
3. <span data-ttu-id="6a044-131">Type byte (21 バイト) の値が7であることを確認します。</span><span class="sxs-lookup"><span data-stu-id="6a044-131">Verify that the type byte (21st byte) has a value of 7.</span></span> <span data-ttu-id="6a044-132">値が7の場合、識別子の形式が正しくないことを示します。</span><span class="sxs-lookup"><span data-stu-id="6a044-132">A value of 7 indicates that the identifier is in the incorrect format.</span></span>
    
4. <span data-ttu-id="6a044-133">最初の4バイトをスキップします。</span><span class="sxs-lookup"><span data-stu-id="6a044-133">Skip the first four bytes.</span></span> <span data-ttu-id="6a044-134">0に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6a044-134">They must be set to zero.</span></span>
    
5. <span data-ttu-id="6a044-135">次の16バイトを次の GUID で更新します。1A447390AA6611CD9BC800AA002FC45A</span><span class="sxs-lookup"><span data-stu-id="6a044-135">Update the next 16 bytes with the following GUID: 1A447390AA6611CD9BC800AA002FC45A</span></span>
    
6. <span data-ttu-id="6a044-136">次のバイト (type byte) を値9で更新します。</span><span class="sxs-lookup"><span data-stu-id="6a044-136">Update the next byte (type byte) with a value of 9.</span></span>
    
7. <span data-ttu-id="6a044-137">識別子を Base64 でエンコードされた文字列に変更します。</span><span class="sxs-lookup"><span data-stu-id="6a044-137">Change the identifier to a Base64-encoded string.</span></span>
    
> [!NOTE]
> <span data-ttu-id="6a044-138">、**指定された**SMTP アドレスが有効な形式であることを検証します。</span><span class="sxs-lookup"><span data-stu-id="6a044-138">The **ConvertId** operation validates that a given SMTP address has a valid format.</span></span> <span data-ttu-id="6a044-139">この操作では、SMTP アドレスが有効なメールボックスを表しているかどうかは判断されません。</span><span class="sxs-lookup"><span data-stu-id="6a044-139">The operation does not determine whether an SMTP address represents a valid mailbox.</span></span> 
  
<span data-ttu-id="6a044-140">次**の表**に記載されている SOAP ヘッダーを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="6a044-140">The **ConvertId** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
<span data-ttu-id="6a044-141">**表1バケット操作の SOAP ヘッダーの収束**</span><span class="sxs-lookup"><span data-stu-id="6a044-141">**Table 1. ConvertId operation SOAP headers**</span></span>

|<span data-ttu-id="6a044-142">**Header**</span><span class="sxs-lookup"><span data-stu-id="6a044-142">**Header**</span></span>|<span data-ttu-id="6a044-143">**要素**</span><span class="sxs-lookup"><span data-stu-id="6a044-143">**Element**</span></span>|<span data-ttu-id="6a044-144">**説明**</span><span class="sxs-lookup"><span data-stu-id="6a044-144">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="6a044-145">偽装</span><span class="sxs-lookup"><span data-stu-id="6a044-145">Impersonation</span></span>  <br/> |[<span data-ttu-id="6a044-146">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="6a044-146">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="6a044-147">クライアントアプリケーションが偽装しているユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="6a044-147">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="6a044-148">これは要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="6a044-148">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="6a044-149">RequestVersion</span><span class="sxs-lookup"><span data-stu-id="6a044-149">RequestVersion</span></span>  <br/> |[<span data-ttu-id="6a044-150">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="6a044-150">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="6a044-151">要求に適用される操作要求のスキーマバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="6a044-151">Identifies the schema version for the operation request This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="6a044-152">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="6a044-152">ServerVersion</span></span>  <br/> |[<span data-ttu-id="6a044-153">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="6a044-153">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="6a044-154">要求に応答したサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="6a044-154">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="6a044-155">これは応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="6a044-155">This is applicable to a response.</span></span>  <br/> |
   
## <a name="convertid-operation-request-example"></a><span data-ttu-id="6a044-156">収束 Tid 操作要求の例</span><span class="sxs-lookup"><span data-stu-id="6a044-156">ConvertId operation request example</span></span>
<span data-ttu-id="6a044-157"><a name="bk_usingConvertId"> </a></span><span class="sxs-lookup"><span data-stu-id="6a044-157"><a name="bk_usingConvertId"> </a></span></span>

<span data-ttu-id="6a044-158">次の例**は、EWS**識別子から Outlook Web App 識別子に変換する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="6a044-158">The following example of a **ConvertId** request shows how to convert from an EWS identifier to an Outlook Web App identifier.</span></span> 
  
<span data-ttu-id="6a044-159">この操作を動作させるには、SOAP ヘッダーの[RequestServerVersion](requestserverversion.md)要素を Exchange2007_SP1 以降に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6a044-159">The [RequestServerVersion](requestserverversion.md) element in the SOAP header must be set to Exchange2007_SP1 or later for this operation to work.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="6a044-160">アイテム識別子は読みやすくするために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="6a044-160">The item identifier has been shortened to preserve readability.</span></span> 
  
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

## <a name="convertid-operation-response-example"></a><span data-ttu-id="6a044-161">収束 Tid 操作の応答の例</span><span class="sxs-lookup"><span data-stu-id="6a044-161">ConvertId operation response example</span></span>
<span data-ttu-id="6a044-162"><a name="bk_usingConvertId"> </a></span><span class="sxs-lookup"><span data-stu-id="6a044-162"><a name="bk_usingConvertId"> </a></span></span>

<span data-ttu-id="6a044-163">次の例では、[**コンバーター tid**要求に成功した応答を示します。</span><span class="sxs-lookup"><span data-stu-id="6a044-163">The following example shows a successful response to a **ConvertId** request.</span></span> <span data-ttu-id="6a044-164">この応答の例には、Outlook Web App の識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6a044-164">This response example contains an Outlook Web App identifier.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="6a044-165">読みやすくするために、Outlook Web App 識別子が短縮されています。</span><span class="sxs-lookup"><span data-stu-id="6a044-165">The Outlook Web App identifier has been shortened to preserve readability.</span></span> 
  
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

## <a name="convertid-operation-error-response-example"></a><span data-ttu-id="6a044-166">コンバーターのエラー応答の例</span><span class="sxs-lookup"><span data-stu-id="6a044-166">ConvertId operation error response example</span></span>
<span data-ttu-id="6a044-167"><a name="bk_usingConvertId"> </a></span><span class="sxs-lookup"><span data-stu-id="6a044-167"><a name="bk_usingConvertId"> </a></span></span>

<span data-ttu-id="6a044-168">次の例は、誤った種類の識別子形式を含む要求への応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="6a044-168">The following example shows the response to a request that contains the wrong type of identifier format.</span></span>
  
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

## <a name="version-differences"></a><span data-ttu-id="6a044-169">バージョンの相違点</span><span class="sxs-lookup"><span data-stu-id="6a044-169">Version differences</span></span>
<span data-ttu-id="6a044-170"><a name="bk_ConvertIdVersionDiff"> </a></span><span class="sxs-lookup"><span data-stu-id="6a044-170"><a name="bk_ConvertIdVersionDiff"> </a></span></span>

<span data-ttu-id="6a044-171">Exchange 2007 と Exchange 2007 Service Pack 1 (SP1) の最初のリリースバージョン間で EWS 識別子形式が変更されました。</span><span class="sxs-lookup"><span data-stu-id="6a044-171">The EWS identifier format changed between the initial release version of Exchange 2007 and Exchange 2007 Service Pack 1 (SP1).</span></span> <span data-ttu-id="6a044-172">Exchange 2010 以降の Office 365 の一部としての exchange Online、exchange Online、およびオンプレミスバージョンの exchange では、Exchange 2007 SP1 が使用するものと同じ識別子の形式を使用します。</span><span class="sxs-lookup"><span data-stu-id="6a044-172">Exchange Online as part of Office 365, Exchange Online, and on-premises versions of Exchange starting with Exchange 2010 use the same identifier format that Exchange 2007 SP1 uses.</span></span>
  
<span data-ttu-id="6a044-173">変換**tid**操作は、パブリックフォルダーの識別子を EWS 識別子から exchange 2007 と exchange 2010 のストア識別子に変換します。</span><span class="sxs-lookup"><span data-stu-id="6a044-173">The **ConvertId** operation converts public folder identifiers from the EWS identifier to the store identifier in Exchange 2007 and Exchange 2010.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="6a044-174">関連項目</span><span class="sxs-lookup"><span data-stu-id="6a044-174">See also</span></span>
<span data-ttu-id="6a044-175"><a name="bk_ConvertIdVersionDiff"> </a></span><span class="sxs-lookup"><span data-stu-id="6a044-175"><a name="bk_ConvertIdVersionDiff"> </a></span></span>

- [<span data-ttu-id="6a044-176">識別子の変換</span><span class="sxs-lookup"><span data-stu-id="6a044-176">Converting Identifiers</span></span>](https://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)
    
- [<span data-ttu-id="6a044-177">ConvertIdType</span><span class="sxs-lookup"><span data-stu-id="6a044-177">ConvertIdType</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.ConvertIdType.aspx)
    
- [<span data-ttu-id="6a044-178">ConvertId</span><span class="sxs-lookup"><span data-stu-id="6a044-178">ConvertId</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.ExchangeServiceBinding.ConvertId.aspx)
    

