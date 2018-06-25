---
title: PerformReminderAction 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c597bb0e-13b0-422e-9c23-970463e2a5c3
description: 操作 PerformReminderAction EWS についての情報を検索します。
ms.openlocfilehash: 778fbb508413721f58cfcf9143a5296874e6cd1c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832722"
---
# <a name="performreminderaction-operation"></a><span data-ttu-id="0c736-103">PerformReminderAction 操作</span><span class="sxs-lookup"><span data-stu-id="0c736-103">PerformReminderAction operation</span></span>

<span data-ttu-id="0c736-104">**PerformReminderAction** EWS の操作に関する情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="0c736-104">Find information about the **PerformReminderAction** EWS operation.</span></span> 
  
<span data-ttu-id="0c736-105">**PerformReminderAction** Exchange Web サービス (EWS) 操作では、アラームのアラームを消すか、アラームの操作を開始します。</span><span class="sxs-lookup"><span data-stu-id="0c736-105">The **PerformReminderAction** Exchange Web Services (EWS) operation initiates a dismiss or snooze action on a reminder.</span></span> 
  
<span data-ttu-id="0c736-106">この操作は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="0c736-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-performreminderaction-operation"></a><span data-ttu-id="0c736-107">PerformReminderAction 操作を使用します。</span><span class="sxs-lookup"><span data-stu-id="0c736-107">Using the PerformReminderAction operation</span></span>

<span data-ttu-id="0c736-108">**PerformReminderAction**操作を使用するには消去または[GetReminders](getreminders-operation.md)操作によって返される (遅延) アラームの再通知します。</span><span class="sxs-lookup"><span data-stu-id="0c736-108">You can use the **PerformReminderAction** operation to dismiss or snooze (delay) reminders returned by the [GetReminders](getreminders-operation.md) operation.</span></span> <span data-ttu-id="0c736-109">アラームの再通知、**再通知**を、[ファイアウォール](actiontype-reminderactiontype.md)に設定し、 [NewReminderTime](newremindertime.md)の値を設定、現在の[ReminderTime](remindertime.md)よりも後ろにそれ以外の場合**NewReminderTime**は、サーバーによって無視されます。</span><span class="sxs-lookup"><span data-stu-id="0c736-109">To snooze a reminder, set the [ActionType](actiontype-reminderactiontype.md) to **Snooze**, and set the [NewReminderTime](newremindertime.md) value to a time later than the current [ReminderTime](remindertime.md), otherwise the **NewReminderTime** is ignored by the server.</span></span> <span data-ttu-id="0c736-110">アラームでは、定期的な会議と一致すると、**再通知**に対して操作を行う次の回のアラームが**NewReminderTime**で、アラーム、アラームが消される効果的に。</span><span class="sxs-lookup"><span data-stu-id="0c736-110">If the reminder is for an occurrence of a recurring meeting, and the **Snooze** action is taken on the reminder with a **NewReminderTime** that is past the reminder of the next occurrence, the reminder is effectively dismissed.</span></span> 
  
<span data-ttu-id="0c736-111">アラームを消すには、**アラームを消す**に**ファイアウォール**を設定します。</span><span class="sxs-lookup"><span data-stu-id="0c736-111">To dismiss a reminder, set the **ActionType** to **Dismiss**.</span></span> <span data-ttu-id="0c736-112">サーバーは、要求を処理するときサーバーは、 **false を指定**する**True**から項目の[IsReminderSet](isreminderset.md)の値を変更します。</span><span class="sxs-lookup"><span data-stu-id="0c736-112">When the server processes the request, the server changes the [IsReminderSet](isreminderset.md) value for the item from **True** to **False**.</span></span>
  
### <a name="performreminderaction-operation-soap-headers"></a><span data-ttu-id="0c736-113">PerformReminderAction 操作の SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0c736-113">PerformReminderAction operation SOAP headers</span></span>

<span data-ttu-id="0c736-114">**PerformReminderAction**操作は、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="0c736-114">The **PerformReminderAction** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="0c736-115">**ヘッダー名**</span><span class="sxs-lookup"><span data-stu-id="0c736-115">**Header name**</span></span>|<span data-ttu-id="0c736-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="0c736-116">**Element**</span></span>|<span data-ttu-id="0c736-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="0c736-117">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="0c736-118">**偽装**</span><span class="sxs-lookup"><span data-stu-id="0c736-118">**Impersonation**</span></span> <br/> |[<span data-ttu-id="0c736-119">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="0c736-119">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="0c736-120">クライアント アプリケーションが偽装するユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="0c736-120">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="0c736-121">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="0c736-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="0c736-122">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="0c736-122">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="0c736-123">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="0c736-123">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="0c736-124">RFC 3066、」タグの「識別の言語」を使用してメールボックスへのアクセスに定義されているカルチャを識別します。</span><span class="sxs-lookup"><span data-stu-id="0c736-124">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="0c736-125">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="0c736-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="0c736-126">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="0c736-126">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="0c736-127">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="0c736-127">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="0c736-128">操作要求のスキーマのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="0c736-128">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="0c736-129">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="0c736-129">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="0c736-130">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="0c736-130">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="0c736-131">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="0c736-131">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="0c736-132">要求に応答するサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="0c736-132">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="0c736-133">このヘッダーは、応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="0c736-133">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="performreminderaction-operation-request-example"></a><span data-ttu-id="0c736-134">PerformReminderAction 操作の要求の例</span><span class="sxs-lookup"><span data-stu-id="0c736-134">PerformReminderAction operation request example</span></span>

<span data-ttu-id="0c736-135">**PerformReminderAction**操作要求の次の例では、現在のアラームの再通知し、新しいアラーム時刻を設定する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="0c736-135">The following example of a **PerformReminderAction** operation request shows how to snooze a current reminder and set a new reminder time.</span></span> <span data-ttu-id="0c736-136">[アイテム Id](itemid.md)の**変更キー**を含めるようにする必要があり、 **NewReminderTime**は、 [GetReminders](getreminders-operation.md)操作によって返される**ReminderTime**より後の時刻に設定する必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="0c736-136">Note that you need to include the **ChangeKey** for the [ItemId](itemid.md) and the **NewReminderTime** must be set to a time later than the **ReminderTime** returned by the [GetReminders](getreminders-operation.md) operation.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:PerformReminderAction>
      <m:ReminderItemActions>
        <t:ReminderItemAction>
          <t:ActionType>Snooze</t:ActionType>
          <t:ItemId Id="vwAAAA=="
           ChangeKey="DwAAABQAAACOs0HEMq1WTKpI7sNu5qXNAAAUDA=="/>
          <t:NewReminderTime>2014-04-16T17:00:00Z</t:NewReminderTime>
        </t:ReminderItemAction>
      </m:ReminderItemActions>
    </m:PerformReminderAction>
  </soap:Body>
</soap:Envelope>
```

> [!NOTE]
> <span data-ttu-id="0c736-137">**ItemId**の値が小さすぎると読みやすさを保持します。</span><span class="sxs-lookup"><span data-stu-id="0c736-137">The **ItemId** value has been shortened to preserve readability.</span></span> 
  
<span data-ttu-id="0c736-138">要求 SOAP 本体にはには、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0c736-138">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="0c736-139">PerformReminderAction</span><span class="sxs-lookup"><span data-stu-id="0c736-139">PerformReminderAction</span></span>](performreminderaction.md)
    
- [<span data-ttu-id="0c736-140">ReminderItemActions</span><span class="sxs-lookup"><span data-stu-id="0c736-140">ReminderItemActions</span></span>](reminderitemactions.md)
    
- [<span data-ttu-id="0c736-141">ReminderItemAction</span><span class="sxs-lookup"><span data-stu-id="0c736-141">ReminderItemAction</span></span>](reminderitemaction.md)
    
- [<span data-ttu-id="0c736-142">ファイアウォール</span><span class="sxs-lookup"><span data-stu-id="0c736-142">ActionType</span></span>](actiontype-reminderactiontype.md)
    
- [<span data-ttu-id="0c736-143">ItemId</span><span class="sxs-lookup"><span data-stu-id="0c736-143">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="0c736-144">NewReminderTime</span><span class="sxs-lookup"><span data-stu-id="0c736-144">NewReminderTime</span></span>](newremindertime.md)
    
## <a name="successful-performreminderaction-operation-response"></a><span data-ttu-id="0c736-145">PerformReminderAction 操作の成功の応答</span><span class="sxs-lookup"><span data-stu-id="0c736-145">Successful PerformReminderAction operation response</span></span>

<span data-ttu-id="0c736-146">成功した要求への応答、 **PerformReminderAction**操作の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0c736-146">The following example shows a successful response to a **PerformReminderAction** operation request.</span></span> <span data-ttu-id="0c736-147">**UpdatedItemIds**要素には、更新された予定表アイテムの**Itemid**が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0c736-147">The **UpdatedItemIds** element contains the **ItemIds** of the updated calendar item.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <ServerVersionInfo MajorVersion="15"
                       MinorVersion="0"
                       MajorBuildNumber="921"
                       MinorBuildNumber="20"
                       Version="V2_10"
                       xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <PerformReminderActionResponse ResponseClass="Success"
                                   xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <UpdatedItemIds>
        <ItemId Id="vwAAAA=="
                ChangeKey="DwAAABYAAAB4to43JyybTYwHLBM1k8MxAAAJKP+S"/>
      </UpdatedItemIds>
    </PerformReminderActionResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="0c736-148">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0c736-148">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="0c736-149">PerformReminderActionResponse</span><span class="sxs-lookup"><span data-stu-id="0c736-149">PerformReminderActionResponse</span></span>](performreminderactionresponse.md)
    
- [<span data-ttu-id="0c736-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="0c736-150">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="0c736-151">UpdatedItemIds</span><span class="sxs-lookup"><span data-stu-id="0c736-151">UpdatedItemIds</span></span>](updateditemids.md)
    
- [<span data-ttu-id="0c736-152">ItemId</span><span class="sxs-lookup"><span data-stu-id="0c736-152">ItemId</span></span>](itemid.md)
    
## <a name="performreminderaction-operation-error-response-example"></a><span data-ttu-id="0c736-153">PerformReminderAction 操作のエラー応答の例</span><span class="sxs-lookup"><span data-stu-id="0c736-153">PerformReminderAction operation error response example</span></span>

<span data-ttu-id="0c736-154">次の例は、サーバー上で変更が行われたいないときに、 **PerformReminderAction**操作の要求への応答を示します。</span><span class="sxs-lookup"><span data-stu-id="0c736-154">The following example shows a response to a **PerformReminderAction** operation request when no change was made on the server.</span></span> <span data-ttu-id="0c736-155">これは、応答の要求は送信されましたが、 **UpdatedItemIds**はありませんでした、アラームが変更されていないことを意味します。</span><span class="sxs-lookup"><span data-stu-id="0c736-155">This is a response in which a request was sent, but no **UpdatedItemIds** were returned, meaning no reminders were changed.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <ServerVersionInfo MajorVersion="15"
                       MinorVersion="0"
                       MajorBuildNumber="918"
                       MinorBuildNumber="7"
                       Version="V2_10"
                       xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <PerformReminderActionResponse ResponseClass="Success"
                                   xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <UpdatedItemIds />
    </PerformReminderActionResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="0c736-156">エラー応答 SOAP 本体にはには、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0c736-156">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="0c736-157">PerformReminderActionResponse</span><span class="sxs-lookup"><span data-stu-id="0c736-157">PerformReminderActionResponse</span></span>](performreminderactionresponse.md)
    
- [<span data-ttu-id="0c736-158">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="0c736-158">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="0c736-159">UpdatedItemIds</span><span class="sxs-lookup"><span data-stu-id="0c736-159">UpdatedItemIds</span></span>](updateditemids.md)
    
<span data-ttu-id="0c736-160">EWS を汎用のエラー コードは、 [ResponseCode](responsecode.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0c736-160">For additional error codes that are generic to EWS, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="0c736-161">関連項目</span><span class="sxs-lookup"><span data-stu-id="0c736-161">See also</span></span>


- [<span data-ttu-id="0c736-162">GetReminders 操作</span><span class="sxs-lookup"><span data-stu-id="0c736-162">GetReminders operation</span></span>](getreminders-operation.md)
    

