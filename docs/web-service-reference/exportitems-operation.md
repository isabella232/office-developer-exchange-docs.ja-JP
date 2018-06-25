---
title: ExportItems 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExportItems
api_type:
- schema
ms.assetid: e2846abb-0b16-4732-bbd8-038a674672f6
description: ExportItems 操作は、メールボックスからアイテムをエクスポートします。
ms.openlocfilehash: 6f0760705c05de2a615544fe52ac50b398be6040
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760383"
---
# <a name="exportitems-operation"></a><span data-ttu-id="d3bb0-103">ExportItems 操作</span><span class="sxs-lookup"><span data-stu-id="d3bb0-103">ExportItems operation</span></span>

<span data-ttu-id="d3bb0-104">**ExportItems**操作は、メールボックスからアイテムをエクスポートします。</span><span class="sxs-lookup"><span data-stu-id="d3bb0-104">The **ExportItems** operation exports items out of a mailbox.</span></span> 
  
## <a name="exportitems-request-example"></a><span data-ttu-id="d3bb0-105">ExportItems 要求の例</span><span class="sxs-lookup"><span data-stu-id="d3bb0-105">ExportItems request example</span></span>

### <a name="description"></a><span data-ttu-id="d3bb0-106">説明</span><span class="sxs-lookup"><span data-stu-id="d3bb0-106">Description</span></span>

<span data-ttu-id="d3bb0-107">**ExportItems**要求の次の例では、メールボックスからエクスポートされた 3 つの項目を取得する要求を作成する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="d3bb0-107">The following example of an **ExportItems** request shows how to form a request to get three items exported from a mailbox.</span></span> 
  
### <a name="code"></a><span data-ttu-id="d3bb0-108">コード</span><span class="sxs-lookup"><span data-stu-id="d3bb0-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
      xmlns:xsd="http://www.w3.org/2001/XMLSchema"
      xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
      xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010_SP1" />
  </soap:Header>
  <soap:Body>
    <m:ExportItems>
      <m:ItemIds>
        <t:ItemId Id="AAMkAGYzZjZmRiUsidkC+NAAAAY89GAAA="/>
        <t:ItemId Id="AAMkAGYzZjZmRiUsidkC+NAAAAY89FAAA="/>
        <t:ItemId Id="AAMkAGYzZjZmRiUsidkC+NAAAAY87NAAA="/>
      </m:ItemIds>
    </m:ExportItems>
  </soap:Body>
</soap:Envelope>
```

### <a name="comment"></a><span data-ttu-id="d3bb0-109">Comment</span><span class="sxs-lookup"><span data-stu-id="d3bb0-109">Comment</span></span>

<span data-ttu-id="d3bb0-110">アイテム識別子の例では、読みやすさを保持するために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="d3bb0-110">The item identifiers in the example have been shortened to preserve readability.</span></span>
  
### <a name="request-elements"></a><span data-ttu-id="d3bb0-111">要素を要求します。</span><span class="sxs-lookup"><span data-stu-id="d3bb0-111">Request elements</span></span>

<span data-ttu-id="d3bb0-112">次の要素は、要求で使用されます。</span><span class="sxs-lookup"><span data-stu-id="d3bb0-112">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="d3bb0-113">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="d3bb0-113">RequestServerVersion</span></span>](requestserverversion.md)
    
- [<span data-ttu-id="d3bb0-114">ExportItems</span><span class="sxs-lookup"><span data-stu-id="d3bb0-114">ExportItems</span></span>](exportitems.md)
    
- [<span data-ttu-id="d3bb0-115">Itemid (NonEmptyArrayOfItemIdsType)</span><span class="sxs-lookup"><span data-stu-id="d3bb0-115">ItemIds (NonEmptyArrayOfItemIdsType)</span></span>](itemids-nonemptyarrayofitemidstype.md)
    
- [<span data-ttu-id="d3bb0-116">ItemId</span><span class="sxs-lookup"><span data-stu-id="d3bb0-116">ItemId</span></span>](itemid.md)
    
## <a name="successful-exportitems-response-example"></a><span data-ttu-id="d3bb0-117">成功した ExportItems の応答の例</span><span class="sxs-lookup"><span data-stu-id="d3bb0-117">Successful ExportItems response example</span></span>

### <a name="description"></a><span data-ttu-id="d3bb0-118">説明</span><span class="sxs-lookup"><span data-stu-id="d3bb0-118">Description</span></span>

<span data-ttu-id="d3bb0-119">**ExportItems**要求に正常な応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d3bb0-119">The following example shows a successful response to an **ExportItems** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="d3bb0-120">コード</span><span class="sxs-lookup"><span data-stu-id="d3bb0-120">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <t:ServerVersionInfo MajorVersion="14"
    MinorVersion="1"
    MajorBuildNumber="139"
    MinorBuildNumber="0"
    Version="Exchange2010_SP1"
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
    xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
    xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
    xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
  xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:ExportItemsResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:ExportItemsResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:ItemId Id="AAMkAGYzZjZmRiUsidkC+NAAAAY89GAAA=" ChangeKey="FwAAAA=="/>
          <m:Data>
            AQAAAAgAAAAAAAAALgBlAHgAdABlAHMAdAAuAG0AaQBjAHIAbwBzAG8AZgB0AC4A
            YwBvAG0AAABTAE0AVABQAAAAVQBzAGUAcgAyAEAAYQB1AGoAaQBuAGcALQBkAG8AbQAuAGUA
            eAB0AGUAcwB0AC4AbQBpAGMAcgBvAHMAbwBmAHQALgBjAG8AbQAAALCE/jlMAAAAVQBzAGUA
            cgAyAEAAYQB1AGoAaQBuAGcALQBkAG8AbQAuAGUAeAB0AGUAcwB0AC4AbQBpAGMAcgBvAHMA
            bwBmAHQALgBjAG8AbQAAAAMAADkAAAAAAwD+DwYAAAADAARAAwACQAMADkA=
          </m:Data>
        </m:ExportItemsResponseMessage>
        <m:ExportItemsResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:ItemId Id="AAMkAGYzZjZmRiUsidkC+NAAAAY89FAAA=" ChangeKey="FwAAAA=="/>
          <m:Data>
            AQAAAAgAAAAAAAAAAQAAAAMAAAAYAAAAAQAAAAcDAgAAAAAAwAAAAAAAAEYAJACA
            QAAyAAAh9SpR08oBAwAEQAMAFkANABMOAwAAQAMAIQ4AAAAAsIQSN0oAAAAyAGEAYgAxADYA
            MQA2ADYALQBhAGUANQBkAC0ANAAyAGUAZgAtAGEANQA1ADkALQBjADgAOQAwADgANwBkADIA
            MwBkADgANAAAAAMACzf/////AwAgDmQEAAADAPcPAAAAAEAABzBPMXstUdPKAUAACDBPMXst
            UdPKAQMABTcFAAAAsIQONx4AAABtAGUAcwBzAGEAZwBlAC8AcgBmAGMAOAAyADIAAACwhAEw
            IgAAAE0AbwBzAHQAIABmAGEAcwBjAGkAbgBhAHQAaQBuAGcAAAACAfkPBAAAAAAAAAADAAFA
            FABKZ3QrAAAAZF2mAwAXAAEAAACwhBoAEgAAAEkAUABNAC4ATgBvAHQAZQAAAAMANgAAAAAA
            sIQ3ACIAAABNAG8AcwB0ACAAZgBhAHMAYwBpAG4AYQB0AGkAbgBnAAAAQAA5AACq+za80coB
            AgE7AGUAAABFWDovTz1GSVJTVCBPUkdBTklaQVRJT04vT1U9RVhDSEFOR0UgQURNSU5JU1RS
            QVRJVkUgR1JPVVAgKEZZRElCT0hGMjNTUERMVCkvQ049UkVDSVBJRU5UUy9DTj1VU0VST05F
            ALCEPQACAAAAAAACAUEAfgAAAAAAAADcp0DIwEIQGrS5CAArL+GCAQAAAAAAAAAvTz1GSVJT
            VCBPUkdBTklaQVRJT04vT1U9RVhDSEFOR0UgQURNSU5JU1RSQVRJVkUgR1JPVVAgKEZZRElC
            T0hGMjNTUERMVCkvQ049UkVDSVBJRU5UUy9DTj1VU0VST05FALCEQgAQAAAAVQB
          </m:Data>
        </m:ExportItemsResponseMessage>
        <m:ExportItemsResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:ItemId Id="AAMkAGYzZjZmRiUsidkC+NAAAAY87NAAA=" ChangeKey="CQAAAA=="/>
          <m:Data>
            AQAAAAgAAAAAAAAAAQAAAAMAAAAYAAAAAQAAAAcDAgAAAAAAwAAAAAAAAEYAJACA
            BAAAAAYAAAABDouAAAACAAAAEiAAAOSECEBbAAAAL089RklSU1QgT1JHQU5JWkFUSU9OL09V
            PUVYQ0hBTkdFIEFETUlOSVNUUkFUSVZFIEdST1VQIChGWURJQk9IRjIzU1BETFQpL0NOPVJF
            Q0lQSUVOVFMvQ049AAMAFwABAAAAsIQaABIAAABJAFAATQAuAE4AbwB0AGUAAAALACMAAAAL
            ACkAAAADADYAAAAAALCENwAyAAAASQBuAHQAZQByAGUAcwB0AGkAbgBnACAALQAgAGYAcgBv
            AG0AIABFAFcAUwBNAEEAAABAADkAAHZeFxfRygECATsAZQAAAEVYOi9PPUZJUlNUIE9SR0FO
            SVpBVElPTi9PVT1FWENIQU5HRSBBRE1JTklTVFJBVElWRSBHUk9VUCAoRllESUJPSEYyM1NQ
            RExUKS9DTj1SRUNJUElFTlRTL0NOPVVTRVJPTkUAsIQ9AAIAAAAAAAIBPwB+AAAAAAAAANyn
            QMjAQhAatLkIACsv4YIBAAAAAAAAAC9PPUZJUlNUIE9SR0FOSVpBVElPTi9PVT1FWENIQU5H
          </m:Data>
        </m:ExportItemsResponseMessage>
      </m:ResponseMessages>
    </m:ExportItemsResponse>
  </s:Body>
</s:Envelope>
```

### <a name="comment"></a><span data-ttu-id="d3bb0-121">Comment</span><span class="sxs-lookup"><span data-stu-id="d3bb0-121">Comment</span></span>

<span data-ttu-id="d3bb0-122">項目の識別子と変更キーを例には、読みやすさを保持するために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="d3bb0-122">The item identifiers and change keys in the example have been shortened to preserve readability.</span></span>
  
### <a name="response-elements"></a><span data-ttu-id="d3bb0-123">応答の要素</span><span class="sxs-lookup"><span data-stu-id="d3bb0-123">Response elements</span></span>

<span data-ttu-id="d3bb0-124">次の要素は、応答で使用されます。</span><span class="sxs-lookup"><span data-stu-id="d3bb0-124">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="d3bb0-125">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="d3bb0-125">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="d3bb0-126">ExportItemsResponse</span><span class="sxs-lookup"><span data-stu-id="d3bb0-126">ExportItemsResponse</span></span>](exportitemsresponse.md)
    
- [<span data-ttu-id="d3bb0-127">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="d3bb0-127">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="d3bb0-128">ExportItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d3bb0-128">ExportItemsResponseMessage</span></span>](exportitemsresponsemessage.md)
    
- [<span data-ttu-id="d3bb0-129">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="d3bb0-129">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="d3bb0-130">ItemId</span><span class="sxs-lookup"><span data-stu-id="d3bb0-130">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="d3bb0-131">データ (base64Binary)</span><span class="sxs-lookup"><span data-stu-id="d3bb0-131">Data (base64Binary)</span></span>](data-base64binary.md)
    
## <a name="exportitems-error-response-example"></a><span data-ttu-id="d3bb0-132">ExportItems エラー応答の例</span><span class="sxs-lookup"><span data-stu-id="d3bb0-132">ExportItems Error response example</span></span>

### <a name="description"></a><span data-ttu-id="d3bb0-133">説明</span><span class="sxs-lookup"><span data-stu-id="d3bb0-133">Description</span></span>

<span data-ttu-id="d3bb0-134">正常にエクスポートされたアイテムの 1 つと 2 つのエラーを保持する**ExportItems**要求への応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d3bb0-134">The following example shows a response to the **ExportItems** request that contains two errors and one successfully exported item.</span></span> <span data-ttu-id="d3bb0-135">例の最初の項目が正常にエクスポートされます。</span><span class="sxs-lookup"><span data-stu-id="d3bb0-135">The first item in the example is successfully exported.</span></span> <span data-ttu-id="d3bb0-136">2 番目の項目には、キー不正な変更にはが含まれています。</span><span class="sxs-lookup"><span data-stu-id="d3bb0-136">The second item contains an incorrect change key.</span></span> <span data-ttu-id="d3bb0-137">3 番目の項目は、問題のメールボックスからアイテムをエクスポートするのには試行を表します。</span><span class="sxs-lookup"><span data-stu-id="d3bb0-137">The third item represents an attempt to export an item from the wrong mailbox.</span></span> 
  
### <a name="code"></a><span data-ttu-id="d3bb0-138">コード</span><span class="sxs-lookup"><span data-stu-id="d3bb0-138">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="1" 
                         MajorBuildNumber="164" 
                         MinorBuildNumber="0" 
                         Version="Exchange2010_SP1" 
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:ExportItemsResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                           xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:ExportItemsResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:ItemId Id="AAMkADhhOGU0oMf0GPIQeAAAAUC8iAABseAAAAUFZ7AAA=" ChangeKey="CQAAAA=="/>
          <m:Data>
            AQAAAAgAAAAAAAAALgBlAHgAdABlAHMAdAAuAG0AaQBjAHIAbwBzAG8AZgB0AC4A
            YwBvAG0AAABTAE0AVABQAAAAVQBzAGUAcgAyAEAAYQB1AGoAaQBuAGcALQBkAG8AbQAuAGUA
            eAB0AGUAcwB0AC4AbQBpAGMAcgBvAHMAbwBmAHQALgBjAG8AbQAAALCE/jlMAAAAVQBzAGUA
            cgAyAEAAYQB1AGoAaQBuAGcALQBkAG8AbQAuAGUAeAB0AGUAcwB0AC4AbQBpAGMAcgBvAHMA
            bwBmAHQALgBjAG8AbQAAAAMAADkAAAAAAwD+DwYAAAADAARAAwACQAMADkA=
          </m:Data>
        </m:ExportItemsResponseMessage>
        <m:ExportItemsResponseMessage ResponseClass="Error">
          <m:MessageText>The change key is invalid.</m:MessageText>
          <m:ResponseCode>ErrorInvalidChangeKey</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:ExportItemsResponseMessage>
        <m:ExportItemsResponseMessage ResponseClass="Error">
          <m:MessageText>No mailbox with such guid.</m:MessageText>
          <m:ResponseCode>ErrorNonExistentMailbox</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:MessageXml>
            <t:Value Name="MailboxGuid">f3f6f699-2254-40ce-9994-388d9d98419e</t:Value>
          </m:MessageXml>
        </m:ExportItemsResponseMessage>
      </m:ResponseMessages>
    </m:ExportItemsResponse>
  </s:Body>
</s:Envelope>

```

### <a name="comments"></a><span data-ttu-id="d3bb0-139">コメント</span><span class="sxs-lookup"><span data-stu-id="d3bb0-139">Comments</span></span>

<span data-ttu-id="d3bb0-140">項目の識別子、キーを変更して、データの例では、読みやすさを保持するために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="d3bb0-140">The item identifiers, change keys, and data in the example have been shortened to preserve readability.</span></span>
  
### <a name="error-response-elements"></a><span data-ttu-id="d3bb0-141">エラー応答の要素</span><span class="sxs-lookup"><span data-stu-id="d3bb0-141">Error response elements</span></span>

<span data-ttu-id="d3bb0-142">エラー応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="d3bb0-142">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="d3bb0-143">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="d3bb0-143">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="d3bb0-144">ExportItemsResponse</span><span class="sxs-lookup"><span data-stu-id="d3bb0-144">ExportItemsResponse</span></span>](exportitemsresponse.md)
    
- [<span data-ttu-id="d3bb0-145">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="d3bb0-145">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="d3bb0-146">ExportItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d3bb0-146">ExportItemsResponseMessage</span></span>](exportitemsresponsemessage.md)
    
- [<span data-ttu-id="d3bb0-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="d3bb0-147">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="d3bb0-148">ItemId</span><span class="sxs-lookup"><span data-stu-id="d3bb0-148">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="d3bb0-149">データ (base64Binary)</span><span class="sxs-lookup"><span data-stu-id="d3bb0-149">Data (base64Binary)</span></span>](data-base64binary.md)
    
- [<span data-ttu-id="d3bb0-150">MessageText</span><span class="sxs-lookup"><span data-stu-id="d3bb0-150">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="d3bb0-151">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="d3bb0-151">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="d3bb0-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="d3bb0-152">MessageXml</span></span>](messagexml.md)
    
- <span data-ttu-id="d3bb0-153">**値**</span><span class="sxs-lookup"><span data-stu-id="d3bb0-153">**Value**</span></span>
    
> [!NOTE]
> <span data-ttu-id="d3bb0-154">**値**要素がスキーマ内に存在しません。</span><span class="sxs-lookup"><span data-stu-id="d3bb0-154">The **Value** element does not exist in the schema.</span></span> <span data-ttu-id="d3bb0-155">この要素は、任意の整形式の XML を含めることができます[MessageXml](messagexml.md)要素は、**値**のインスタンスの要素が発生するために有効です。</span><span class="sxs-lookup"><span data-stu-id="d3bb0-155">This element is valid because the [MessageXml](messagexml.md) element, in which the **Value** instance element occurs, can contain any well-formed XML.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="d3bb0-156">関連項目</span><span class="sxs-lookup"><span data-stu-id="d3bb0-156">See also</span></span>



[<span data-ttu-id="d3bb0-157">UploadItems 操作</span><span class="sxs-lookup"><span data-stu-id="d3bb0-157">UploadItems operation</span></span>](uploaditems-operation.md)


[<span data-ttu-id="d3bb0-158">Exchange での EWS の操作</span><span class="sxs-lookup"><span data-stu-id="d3bb0-158">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
  
- [<span data-ttu-id="d3bb0-159">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="d3bb0-159">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

