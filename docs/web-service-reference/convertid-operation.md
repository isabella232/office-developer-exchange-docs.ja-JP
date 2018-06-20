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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759768"
---
# <a name="convertid-operation"></a><span data-ttu-id="14472-103">ConvertId 操作</span><span class="sxs-lookup"><span data-stu-id="14472-103">ConvertId operation</span></span>

<span data-ttu-id="14472-104">**ConvertId** EWS の操作に関する情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="14472-104">Find information about the **ConvertId** EWS operation.</span></span> 
  
<span data-ttu-id="14472-105">**ConvertId** Exchange Web サービス (EWS) の操作 Exchange オンラインになって、Office 365 の一部として Exchange Online で受け入れられる形式の間でのアイテムおよびフォルダーの識別子を変換し、設置型バージョンの Exchange が Exchange Server で始まる2013。</span><span class="sxs-lookup"><span data-stu-id="14472-105">The **ConvertId** Exchange Web Services (EWS) operation converts item and folder identifiers between formats that are accepted by Exchange Online, Exchange Online as part of Office 365, and on-premises versions of Exchange starting with Exchange Server 2013.</span></span> 
  
## <a name="using-the-convertid-operation"></a><span data-ttu-id="14472-106">ConvertId 操作を使用します。</span><span class="sxs-lookup"><span data-stu-id="14472-106">Using the ConvertId operation</span></span>
<span data-ttu-id="14472-107"><a name="bk_usingConvertId"> </a></span><span class="sxs-lookup"><span data-stu-id="14472-107"></span></span>

<span data-ttu-id="14472-108">**ConvertId**操作を使用して、次の識別子を変換できます。</span><span class="sxs-lookup"><span data-stu-id="14472-108">You can convert the following identifiers by using the **ConvertId** operation:</span></span> 
  
- <span data-ttu-id="14472-109">EWS の初期リリース版の Exchange 2007 での識別子形式です。</span><span class="sxs-lookup"><span data-stu-id="14472-109">The identifier format for EWS in the initial release version of Exchange 2007.</span></span> <span data-ttu-id="14472-110">これは、 `EwsLegacyId` [フェース id フォーマット](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx)の列挙体の列挙値。</span><span class="sxs-lookup"><span data-stu-id="14472-110">This is represented by the  `EwsLegacyId` enumeration value in the [IdFormat](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx) enumeration.</span></span> 
    
- <span data-ttu-id="14472-111">EWS では、Exchange 2007 SP1 または Exchange 2010 の識別子の形式です。</span><span class="sxs-lookup"><span data-stu-id="14472-111">The identifier format for EWS in Exchange 2007 SP1 or Exchange 2010.</span></span> <span data-ttu-id="14472-112">これは、 `EwsId` [フェース id フォーマット](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx)の列挙値。</span><span class="sxs-lookup"><span data-stu-id="14472-112">This is represented by the  `EwsId` enumeration value in [IdFormat](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx).</span></span>
    
- <span data-ttu-id="14472-113">**PR_ENTRYID**プロパティと同様に、MAPI 識別子です。</span><span class="sxs-lookup"><span data-stu-id="14472-113">The MAPI identifier, as in the **PR_ENTRYID** property.</span></span> <span data-ttu-id="14472-114">これは、 `EntryId` [フェース id フォーマット](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx)の列挙体の列挙値。</span><span class="sxs-lookup"><span data-stu-id="14472-114">This is represented by the  `EntryId` enumeration value in the [IdFormat](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx) enumeration.</span></span> 
    
- <span data-ttu-id="14472-115">可用性の予定表イベントの識別子です。</span><span class="sxs-lookup"><span data-stu-id="14472-115">The availability calendar event identifier.</span></span> <span data-ttu-id="14472-116">これは、 **PR_ENTRYID**プロパティの 16 進数でエンコードされた表現です。</span><span class="sxs-lookup"><span data-stu-id="14472-116">This is a hexadecimal-encoded representation of the **PR_ENTRYID** property.</span></span> <span data-ttu-id="14472-117">これは、 `HexEntryId` [フェース id フォーマット](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx)の列挙値。</span><span class="sxs-lookup"><span data-stu-id="14472-117">This is represented by the  `HexEntryId` enumeration value in [IdFormat](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx).</span></span>
    
- <span data-ttu-id="14472-118">Exchange ストアの識別子です。</span><span class="sxs-lookup"><span data-stu-id="14472-118">The Exchange store identifier.</span></span> <span data-ttu-id="14472-119">これは、 `StoreId` [フェース id フォーマット](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx)の列挙値。</span><span class="sxs-lookup"><span data-stu-id="14472-119">This is represented by the  `StoreId` enumeration value in [IdFormat](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx).</span></span> <span data-ttu-id="14472-120">**ConvertId**操作は変換されませんパブリック フォルダーの識別子 EWS id からストア識別子に。</span><span class="sxs-lookup"><span data-stu-id="14472-120">The **ConvertId** operation does not convert public folder identifiers from the EWS identifier to the store identifier.</span></span> 
    
- <span data-ttu-id="14472-121">Outlook Web App の識別子です。</span><span class="sxs-lookup"><span data-stu-id="14472-121">The Outlook Web App identifier.</span></span> <span data-ttu-id="14472-122">これは、 `OwaId` [フェース id フォーマット](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx)の列挙値</span><span class="sxs-lookup"><span data-stu-id="14472-122">This is represented by the  `OwaId` enumeration value in [IdFormat](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx)</span></span>
    
    <span data-ttu-id="14472-123">Outlook Web App にこの識別子から作成される Url を渡すことはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="14472-123">The passing of URLs that are created from this identifier to Outlook Web App is not supported.</span></span> <span data-ttu-id="14472-124">Outlook Web App id は、Exchange 2007 および Exchange 2010 に適用されます。</span><span class="sxs-lookup"><span data-stu-id="14472-124">The Outlook Web App identifier is applicable to Exchange 2007 and Exchange 2010.</span></span> <span data-ttu-id="14472-125">Exchange Online とのバージョンの Exchange が Exchange Server 2013 で始まるため、Outlook Web App では、EWS 識別子を使用します。</span><span class="sxs-lookup"><span data-stu-id="14472-125">Outlook Web App for Exchange Online and versions of Exchange starting with Exchange Server 2013 uses EWS identifiers.</span></span>
    
<span data-ttu-id="14472-126">**ConvertId**操作は、ストアの識別子には、オンラインの Exchange および Exchange 2013 の EWS 識別子からパブリック フォルダーの識別子を変換するときに期待どおりには動作しません。</span><span class="sxs-lookup"><span data-stu-id="14472-126">The **ConvertId** operation does not work as expected when converting public folder identifiers from the EWS identifier to the store identifier in Exchange Online and Exchange 2013.</span></span> <span data-ttu-id="14472-127">回避策として返される id を手動で更新することができます。</span><span class="sxs-lookup"><span data-stu-id="14472-127">You can manually update the identifier that is returned as a workaround.</span></span> <span data-ttu-id="14472-128">Id を手動で更新するには。</span><span class="sxs-lookup"><span data-stu-id="14472-128">To manually update the identifier:</span></span> 
  
1. <span data-ttu-id="14472-129">アプリケーション コードでは、対象のアイテムまたはフォルダーが、パブリック フォルダーかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="14472-129">In your application code, determine whether the target item/folder is in a public folder.</span></span> 
    
2. <span data-ttu-id="14472-130">識別子の Base64 でエンコードされた文字列をデコードします。</span><span class="sxs-lookup"><span data-stu-id="14472-130">Decode the Base64-encoded identifier string.</span></span>
    
3. <span data-ttu-id="14472-131">確認する型のバイト (21 バイト) は、7 の値を持ちます。</span><span class="sxs-lookup"><span data-stu-id="14472-131">Verify that the type byte (21st byte) has a value of 7.</span></span> <span data-ttu-id="14472-132">7 の値は、誤った形式の識別子であることを示します。</span><span class="sxs-lookup"><span data-stu-id="14472-132">A value of 7 indicates that the identifier is in the incorrect format.</span></span>
    
4. <span data-ttu-id="14472-133">最初の 4 バイトをスキップします。</span><span class="sxs-lookup"><span data-stu-id="14472-133">Skip the first four bytes.</span></span> <span data-ttu-id="14472-134">それらはゼロに設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="14472-134">They must be set to zero.</span></span>
    
5. <span data-ttu-id="14472-135">次の GUID を使用して、次の 16 バイトを更新: 1A447390AA6611CD9BC800AA002FC45A</span><span class="sxs-lookup"><span data-stu-id="14472-135">Update the next 16 bytes with the following GUID: 1A447390AA6611CD9BC800AA002FC45A</span></span>
    
6. <span data-ttu-id="14472-136">9 の値を持つには、次のバイト (byte 型) を更新します。</span><span class="sxs-lookup"><span data-stu-id="14472-136">Update the next byte (type byte) with a value of 9.</span></span>
    
7. <span data-ttu-id="14472-137">Base64 でエンコードされた文字列に識別子を変更します。</span><span class="sxs-lookup"><span data-stu-id="14472-137">Change the identifier to a Base64-encoded string.</span></span>
    
> [!NOTE]
> <span data-ttu-id="14472-138">**ConvertId**操作は、指定した SMTP アドレスが有効な形式を持っているを検証します。</span><span class="sxs-lookup"><span data-stu-id="14472-138">The **ConvertId** operation validates that a given SMTP address has a valid format.</span></span> <span data-ttu-id="14472-139">操作は、SMTP アドレスが有効なメールボックスを表すかどうかを判断できません。</span><span class="sxs-lookup"><span data-stu-id="14472-139">The operation does not determine whether an SMTP address represents a valid mailbox.</span></span> 
  
<span data-ttu-id="14472-140">**ConvertId**操作は、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="14472-140">The **ConvertId** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
<span data-ttu-id="14472-141">**表 1 です。ConvertId 操作の SOAP ヘッダー**</span><span class="sxs-lookup"><span data-stu-id="14472-141">**Table 1. ConvertId operation SOAP headers**</span></span>

|<span data-ttu-id="14472-142">**Header**</span><span class="sxs-lookup"><span data-stu-id="14472-142">**Header**</span></span>|<span data-ttu-id="14472-143">**要素**</span><span class="sxs-lookup"><span data-stu-id="14472-143">**Element**</span></span>|<span data-ttu-id="14472-144">**説明**</span><span class="sxs-lookup"><span data-stu-id="14472-144">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="14472-145">偽装</span><span class="sxs-lookup"><span data-stu-id="14472-145">Impersonation</span></span>  <br/> |[<span data-ttu-id="14472-146">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="14472-146">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="14472-147">クライアント アプリケーションが偽装するユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="14472-147">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="14472-148">これは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="14472-148">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="14472-149">RequestVersion</span><span class="sxs-lookup"><span data-stu-id="14472-149">RequestVersion</span></span>  <br/> |[<span data-ttu-id="14472-150">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="14472-150">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="14472-151">これは、要求に適用する操作要求のスキーマのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="14472-151">Identifies the schema version for the operation request This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="14472-152">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="14472-152">ServerVersion</span></span>  <br/> |[<span data-ttu-id="14472-153">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="14472-153">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="14472-154">要求に応答するサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="14472-154">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="14472-155">これは、応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="14472-155">This is applicable to a response.</span></span>  <br/> |
   
## <a name="convertid-operation-request-example"></a><span data-ttu-id="14472-156">ConvertId 操作の要求の例</span><span class="sxs-lookup"><span data-stu-id="14472-156">ConvertId operation request example</span></span>
<span data-ttu-id="14472-157"><a name="bk_usingConvertId"> </a></span><span class="sxs-lookup"><span data-stu-id="14472-157"></span></span>

<span data-ttu-id="14472-158">**ConvertId**要求の次の例では、EWS 識別子から Outlook Web App の識別子に変換する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="14472-158">The following example of a **ConvertId** request shows how to convert from an EWS identifier to an Outlook Web App identifier.</span></span> 
  
<span data-ttu-id="14472-159">Exchange2007_SP1 に、後でこの操作を行うには、SOAP ヘッダー内の[RequestServerVersion](requestserverversion.md)要素を設定してください。</span><span class="sxs-lookup"><span data-stu-id="14472-159">The [RequestServerVersion](requestserverversion.md) element in the SOAP header must be set to Exchange2007_SP1 or later for this operation to work.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="14472-160">項目の識別子が読みやすさを保持するために小さすぎます。</span><span class="sxs-lookup"><span data-stu-id="14472-160">The item identifier has been shortened to preserve readability.</span></span> 
  
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

## <a name="convertid-operation-response-example"></a><span data-ttu-id="14472-161">ConvertId 操作の応答の例</span><span class="sxs-lookup"><span data-stu-id="14472-161">ConvertId operation response example</span></span>
<span data-ttu-id="14472-162"><a name="bk_usingConvertId"> </a></span><span class="sxs-lookup"><span data-stu-id="14472-162"></span></span>

<span data-ttu-id="14472-163">**ConvertId**要求に正常な応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="14472-163">The following example shows a successful response to a **ConvertId** request.</span></span> <span data-ttu-id="14472-164">この応答の例には、Outlook Web App の識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="14472-164">This response example contains an Outlook Web App identifier.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="14472-165">読みやすさを保持するために Outlook Web App id が小さすぎます。</span><span class="sxs-lookup"><span data-stu-id="14472-165">The Outlook Web App identifier has been shortened to preserve readability.</span></span> 
  
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

## <a name="convertid-operation-error-response-example"></a><span data-ttu-id="14472-166">ConvertId 操作のエラー応答の例</span><span class="sxs-lookup"><span data-stu-id="14472-166">ConvertId operation error response example</span></span>
<span data-ttu-id="14472-167"><a name="bk_usingConvertId"> </a></span><span class="sxs-lookup"><span data-stu-id="14472-167"></span></span>

<span data-ttu-id="14472-168">識別子の形式の間違った型を含む要求に対する応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="14472-168">The following example shows the response to a request that contains the wrong type of identifier format.</span></span>
  
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

## <a name="version-differences"></a><span data-ttu-id="14472-169">バージョンの相違点</span><span class="sxs-lookup"><span data-stu-id="14472-169">Version differences</span></span>
<span data-ttu-id="14472-170"><a name="bk_ConvertIdVersionDiff"> </a></span><span class="sxs-lookup"><span data-stu-id="14472-170"></span></span>

<span data-ttu-id="14472-171">初期リリース版の Exchange 2007 および Exchange 2007 Service Pack 1 (SP1) の間で変更する EWS 識別子の形式です。</span><span class="sxs-lookup"><span data-stu-id="14472-171">The EWS identifier format changed between the initial release version of Exchange 2007 and Exchange 2007 Service Pack 1 (SP1).</span></span> <span data-ttu-id="14472-172">Exchange オンライン Office 365 の一部として、Exchange Online では、および設置型のバージョンの Exchange が Exchange 2010 で始まるは、Exchange 2007 SP1 を使用している同じ識別子の形式を使用します。</span><span class="sxs-lookup"><span data-stu-id="14472-172">Exchange Online as part of Office 365, Exchange Online, and on-premises versions of Exchange starting with Exchange 2010 use the same identifier format that Exchange 2007 SP1 uses.</span></span>
  
<span data-ttu-id="14472-173">**ConvertId**操作は、パブリック フォルダーの識別子を EWS 識別子から Exchange 2007 および Exchange 2010 ストア識別子に変換します。</span><span class="sxs-lookup"><span data-stu-id="14472-173">The **ConvertId** operation converts public folder identifiers from the EWS identifier to the store identifier in Exchange 2007 and Exchange 2010.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="14472-174">関連項目</span><span class="sxs-lookup"><span data-stu-id="14472-174">See also</span></span>
<span data-ttu-id="14472-175"><a name="bk_ConvertIdVersionDiff"> </a></span><span class="sxs-lookup"><span data-stu-id="14472-175"></span></span>

- [<span data-ttu-id="14472-176">識別子に変換します。</span><span class="sxs-lookup"><span data-stu-id="14472-176">Converting Identifiers</span></span>](http://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)
    
- [<span data-ttu-id="14472-177">ConvertIdType</span><span class="sxs-lookup"><span data-stu-id="14472-177">ConvertIdType</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.ConvertIdType.aspx)
    
- [<span data-ttu-id="14472-178">ConvertId</span><span class="sxs-lookup"><span data-stu-id="14472-178">ConvertId</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.ExchangeServiceBinding.ConvertId.aspx)
    

