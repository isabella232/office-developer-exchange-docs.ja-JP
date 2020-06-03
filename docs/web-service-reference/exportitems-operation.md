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
ms.openlocfilehash: 547a490a27d2414d2eda1d89cdac036a34eddccd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526047"
---
# <a name="exportitems-operation"></a><span data-ttu-id="0314e-103">ExportItems 操作</span><span class="sxs-lookup"><span data-stu-id="0314e-103">ExportItems operation</span></span>

<span data-ttu-id="0314e-104">**ExportItems**操作は、メールボックスからアイテムをエクスポートします。</span><span class="sxs-lookup"><span data-stu-id="0314e-104">The **ExportItems** operation exports items out of a mailbox.</span></span> 
  
## <a name="exportitems-request-example"></a><span data-ttu-id="0314e-105">ExportItems 要求の例</span><span class="sxs-lookup"><span data-stu-id="0314e-105">ExportItems request example</span></span>

### <a name="description"></a><span data-ttu-id="0314e-106">Description</span><span class="sxs-lookup"><span data-stu-id="0314e-106">Description</span></span>

<span data-ttu-id="0314e-107">次の**ExportItems**要求の例は、メールボックスからエクスポートされた3つのアイテムを取得するための要求を形成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="0314e-107">The following example of an **ExportItems** request shows how to form a request to get three items exported from a mailbox.</span></span> 
  
### <a name="code"></a><span data-ttu-id="0314e-108">コード</span><span class="sxs-lookup"><span data-stu-id="0314e-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
      xmlns:xsd="http://www.w3.org/2001/XMLSchema"
      xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
      xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comment"></a><span data-ttu-id="0314e-109">コメント</span><span class="sxs-lookup"><span data-stu-id="0314e-109">Comment</span></span>

<span data-ttu-id="0314e-110">この例のアイテム識別子は読みやすいように短縮されています。</span><span class="sxs-lookup"><span data-stu-id="0314e-110">The item identifiers in the example have been shortened to preserve readability.</span></span>
  
### <a name="request-elements"></a><span data-ttu-id="0314e-111">Request 要素</span><span class="sxs-lookup"><span data-stu-id="0314e-111">Request elements</span></span>

<span data-ttu-id="0314e-112">要求では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="0314e-112">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="0314e-113">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="0314e-113">RequestServerVersion</span></span>](requestserverversion.md)
    
- [<span data-ttu-id="0314e-114">ExportItems</span><span class="sxs-lookup"><span data-stu-id="0314e-114">ExportItems</span></span>](exportitems.md)
    
- [<span data-ttu-id="0314e-115">ItemIds (非 Emptyarrayofitemidstype)</span><span class="sxs-lookup"><span data-stu-id="0314e-115">ItemIds (NonEmptyArrayOfItemIdsType)</span></span>](itemids-nonemptyarrayofitemidstype.md)
    
- [<span data-ttu-id="0314e-116">ItemId</span><span class="sxs-lookup"><span data-stu-id="0314e-116">ItemId</span></span>](itemid.md)
    
## <a name="successful-exportitems-response-example"></a><span data-ttu-id="0314e-117">Successful ExportItems response の例</span><span class="sxs-lookup"><span data-stu-id="0314e-117">Successful ExportItems response example</span></span>

### <a name="description"></a><span data-ttu-id="0314e-118">Description</span><span class="sxs-lookup"><span data-stu-id="0314e-118">Description</span></span>

<span data-ttu-id="0314e-119">次の例は、 **ExportItems**要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="0314e-119">The following example shows a successful response to an **ExportItems** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="0314e-120">コード</span><span class="sxs-lookup"><span data-stu-id="0314e-120">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <t:ServerVersionInfo MajorVersion="14"
    MinorVersion="1"
    MajorBuildNumber="139"
    MinorBuildNumber="0"
    Version="Exchange2010_SP1"
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
    xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
    xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
    xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
  xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:ExportItemsResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

### <a name="comment"></a><span data-ttu-id="0314e-121">コメント</span><span class="sxs-lookup"><span data-stu-id="0314e-121">Comment</span></span>

<span data-ttu-id="0314e-122">この例のアイテム識別子と変更キーは、読みやすくするために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="0314e-122">The item identifiers and change keys in the example have been shortened to preserve readability.</span></span>
  
### <a name="response-elements"></a><span data-ttu-id="0314e-123">Response 要素</span><span class="sxs-lookup"><span data-stu-id="0314e-123">Response elements</span></span>

<span data-ttu-id="0314e-124">応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="0314e-124">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="0314e-125">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="0314e-125">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="0314e-126">ExportItemsResponse</span><span class="sxs-lookup"><span data-stu-id="0314e-126">ExportItemsResponse</span></span>](exportitemsresponse.md)
    
- [<span data-ttu-id="0314e-127">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="0314e-127">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="0314e-128">ExportItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="0314e-128">ExportItemsResponseMessage</span></span>](exportitemsresponsemessage.md)
    
- [<span data-ttu-id="0314e-129">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="0314e-129">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="0314e-130">ItemId</span><span class="sxs-lookup"><span data-stu-id="0314e-130">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="0314e-131">Data (base64Binary)</span><span class="sxs-lookup"><span data-stu-id="0314e-131">Data (base64Binary)</span></span>](data-base64binary.md)
    
## <a name="exportitems-error-response-example"></a><span data-ttu-id="0314e-132">ExportItems エラー応答の例</span><span class="sxs-lookup"><span data-stu-id="0314e-132">ExportItems Error response example</span></span>

### <a name="description"></a><span data-ttu-id="0314e-133">Description</span><span class="sxs-lookup"><span data-stu-id="0314e-133">Description</span></span>

<span data-ttu-id="0314e-134">次の例は、2つのエラーと1つのアイテムが正常にエクスポートされた**ExportItems**要求への応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="0314e-134">The following example shows a response to the **ExportItems** request that contains two errors and one successfully exported item.</span></span> <span data-ttu-id="0314e-135">この例の最初の項目は正常にエクスポートされています。</span><span class="sxs-lookup"><span data-stu-id="0314e-135">The first item in the example is successfully exported.</span></span> <span data-ttu-id="0314e-136">2番目の項目に不適切な変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="0314e-136">The second item contains an incorrect change key.</span></span> <span data-ttu-id="0314e-137">3番目の項目は、誤ったメールボックスからアイテムをエクスポートしようとしたことを表します。</span><span class="sxs-lookup"><span data-stu-id="0314e-137">The third item represents an attempt to export an item from the wrong mailbox.</span></span> 
  
### <a name="code"></a><span data-ttu-id="0314e-138">コード</span><span class="sxs-lookup"><span data-stu-id="0314e-138">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="1" 
                         MajorBuildNumber="164" 
                         MinorBuildNumber="0" 
                         Version="Exchange2010_SP1" 
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:ExportItemsResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                           xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

### <a name="comments"></a><span data-ttu-id="0314e-139">コメント</span><span class="sxs-lookup"><span data-stu-id="0314e-139">Comments</span></span>

<span data-ttu-id="0314e-140">この例のアイテム識別子、変更キー、データは、読みやすくするために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="0314e-140">The item identifiers, change keys, and data in the example have been shortened to preserve readability.</span></span>
  
### <a name="error-response-elements"></a><span data-ttu-id="0314e-141">エラー応答要素</span><span class="sxs-lookup"><span data-stu-id="0314e-141">Error response elements</span></span>

<span data-ttu-id="0314e-142">エラー応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="0314e-142">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="0314e-143">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="0314e-143">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="0314e-144">ExportItemsResponse</span><span class="sxs-lookup"><span data-stu-id="0314e-144">ExportItemsResponse</span></span>](exportitemsresponse.md)
    
- [<span data-ttu-id="0314e-145">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="0314e-145">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="0314e-146">ExportItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="0314e-146">ExportItemsResponseMessage</span></span>](exportitemsresponsemessage.md)
    
- [<span data-ttu-id="0314e-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="0314e-147">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="0314e-148">ItemId</span><span class="sxs-lookup"><span data-stu-id="0314e-148">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="0314e-149">Data (base64Binary)</span><span class="sxs-lookup"><span data-stu-id="0314e-149">Data (base64Binary)</span></span>](data-base64binary.md)
    
- [<span data-ttu-id="0314e-150">MessageText</span><span class="sxs-lookup"><span data-stu-id="0314e-150">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="0314e-151">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="0314e-151">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="0314e-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="0314e-152">MessageXml</span></span>](messagexml.md)
    
- <span data-ttu-id="0314e-153">**値**</span><span class="sxs-lookup"><span data-stu-id="0314e-153">**Value**</span></span>
    
> [!NOTE]
> <span data-ttu-id="0314e-154">**Value**要素がスキーマに存在しません。</span><span class="sxs-lookup"><span data-stu-id="0314e-154">The **Value** element does not exist in the schema.</span></span> <span data-ttu-id="0314e-155">この要素は、**値**instance 要素が発生する[MessageXml](messagexml.md)要素が整形式の XML を含むことができるため、有効です。</span><span class="sxs-lookup"><span data-stu-id="0314e-155">This element is valid because the [MessageXml](messagexml.md) element, in which the **Value** instance element occurs, can contain any well-formed XML.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="0314e-156">関連項目</span><span class="sxs-lookup"><span data-stu-id="0314e-156">See also</span></span>



[<span data-ttu-id="0314e-157">UploadItems 操作</span><span class="sxs-lookup"><span data-stu-id="0314e-157">UploadItems operation</span></span>](uploaditems-operation.md)


[<span data-ttu-id="0314e-158">Exchange での EWS 操作</span><span class="sxs-lookup"><span data-stu-id="0314e-158">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
  
- [<span data-ttu-id="0314e-159">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="0314e-159">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

