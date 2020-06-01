---
title: PerformReminderAction 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c597bb0e-13b0-422e-9c23-970463e2a5c3
description: PerformReminderAction EWS 操作についての情報を検索します。
ms.openlocfilehash: 4c069d541e9a42167c447a50c405399958d3608d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462291"
---
# <a name="performreminderaction-operation"></a><span data-ttu-id="19b4f-103">PerformReminderAction 操作</span><span class="sxs-lookup"><span data-stu-id="19b4f-103">PerformReminderAction operation</span></span>

<span data-ttu-id="19b4f-104">**PerformReminderAction** EWS 操作についての情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="19b4f-104">Find information about the **PerformReminderAction** EWS operation.</span></span> 
  
<span data-ttu-id="19b4f-105">**PerformReminderAction** Exchange Web サービス (EWS) の操作によって、アラームの [消去] または [再通知] アクションが開始されます。</span><span class="sxs-lookup"><span data-stu-id="19b4f-105">The **PerformReminderAction** Exchange Web Services (EWS) operation initiates a dismiss or snooze action on a reminder.</span></span> 
  
<span data-ttu-id="19b4f-106">この操作は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="19b4f-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-performreminderaction-operation"></a><span data-ttu-id="19b4f-107">PerformReminderAction 操作の使用</span><span class="sxs-lookup"><span data-stu-id="19b4f-107">Using the PerformReminderAction operation</span></span>

<span data-ttu-id="19b4f-108">**PerformReminderAction**操作を使用して、 [getreminders](getreminders-operation.md)操作によって返されるアラームを消去または再通知 (遅延) することができます。</span><span class="sxs-lookup"><span data-stu-id="19b4f-108">You can use the **PerformReminderAction** operation to dismiss or snooze (delay) reminders returned by the [GetReminders](getreminders-operation.md) operation.</span></span> <span data-ttu-id="19b4f-109">アラームを再通知するには、「再**通知**」に「 [NewReminderTime](newremindertime.md) [」の値](actiontype-reminderactiontype.md)を設定し、現在の[ReminderTime](remindertime.md)より後の時刻に設定します。それ以外の場合は、 **NewReminderTime**はサーバーによって無視されます。</span><span class="sxs-lookup"><span data-stu-id="19b4f-109">To snooze a reminder, set the [ActionType](actiontype-reminderactiontype.md) to **Snooze**, and set the [NewReminderTime](newremindertime.md) value to a time later than the current [ReminderTime](remindertime.md), otherwise the **NewReminderTime** is ignored by the server.</span></span> <span data-ttu-id="19b4f-110">アラームが定期的な会議の発生を対象としていて、アラームに対して次の発生のアラームを過ぎている**NewReminderTime**を使用して再**通知**が行われる場合、アラームは実際には消去されます。</span><span class="sxs-lookup"><span data-stu-id="19b4f-110">If the reminder is for an occurrence of a recurring meeting, and the **Snooze** action is taken on the reminder with a **NewReminderTime** that is past the reminder of the next occurrence, the reminder is effectively dismissed.</span></span> 
  
<span data-ttu-id="19b4f-111">アラームを消すには、 **ActionType**を [**消去**] に設定します。</span><span class="sxs-lookup"><span data-stu-id="19b4f-111">To dismiss a reminder, set the **ActionType** to **Dismiss**.</span></span> <span data-ttu-id="19b4f-112">サーバーは、要求を処理するときに、アイテムの[IsReminderSet](isreminderset.md)値を**True**から**False**に変更します。</span><span class="sxs-lookup"><span data-stu-id="19b4f-112">When the server processes the request, the server changes the [IsReminderSet](isreminderset.md) value for the item from **True** to **False**.</span></span>
  
### <a name="performreminderaction-operation-soap-headers"></a><span data-ttu-id="19b4f-113">PerformReminderAction 操作の SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="19b4f-113">PerformReminderAction operation SOAP headers</span></span>

<span data-ttu-id="19b4f-114">**PerformReminderAction**操作では、次の表に示す SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="19b4f-114">The **PerformReminderAction** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="19b4f-115">**ヘッダー名**</span><span class="sxs-lookup"><span data-stu-id="19b4f-115">**Header name**</span></span>|<span data-ttu-id="19b4f-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="19b4f-116">**Element**</span></span>|<span data-ttu-id="19b4f-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="19b4f-117">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="19b4f-118">**偽装**</span><span class="sxs-lookup"><span data-stu-id="19b4f-118">**Impersonation**</span></span> <br/> |[<span data-ttu-id="19b4f-119">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="19b4f-119">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="19b4f-120">クライアントアプリケーションが偽装しているユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="19b4f-120">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="19b4f-121">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="19b4f-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="19b4f-122">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="19b4f-122">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="19b4f-123">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="19b4f-123">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="19b4f-124">RFC 3066 で定義されているように、メールボックスへのアクセスに使用されるカルチャ (言語の識別用のタグ) を識別します。</span><span class="sxs-lookup"><span data-stu-id="19b4f-124">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="19b4f-125">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="19b4f-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="19b4f-126">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="19b4f-126">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="19b4f-127">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="19b4f-127">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="19b4f-128">操作要求のスキーマバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="19b4f-128">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="19b4f-129">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="19b4f-129">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="19b4f-130">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="19b4f-130">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="19b4f-131">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="19b4f-131">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="19b4f-132">要求に応答したサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="19b4f-132">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="19b4f-133">このヘッダーは応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="19b4f-133">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="performreminderaction-operation-request-example"></a><span data-ttu-id="19b4f-134">PerformReminderAction 操作要求の例</span><span class="sxs-lookup"><span data-stu-id="19b4f-134">PerformReminderAction operation request example</span></span>

<span data-ttu-id="19b4f-135">次の**PerformReminderAction**操作要求の例は、現在のアラームを再通知し、新しいアラーム時刻を設定する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="19b4f-135">The following example of a **PerformReminderAction** operation request shows how to snooze a current reminder and set a new reminder time.</span></span> <span data-ttu-id="19b4f-136">[ItemId](itemid.md)の**changekey**を含める必要があります。また、 **NewReminderTime**は、 [Getreminders](getreminders-operation.md)操作によって返される**ReminderTime**より後の時刻に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="19b4f-136">Note that you need to include the **ChangeKey** for the [ItemId](itemid.md) and the **NewReminderTime** must be set to a time later than the **ReminderTime** returned by the [GetReminders](getreminders-operation.md) operation.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
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
> <span data-ttu-id="19b4f-137">**ItemId**の値は読みやすいように短縮されています。</span><span class="sxs-lookup"><span data-stu-id="19b4f-137">The **ItemId** value has been shortened to preserve readability.</span></span> 
  
<span data-ttu-id="19b4f-138">要求 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="19b4f-138">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="19b4f-139">PerformReminderAction</span><span class="sxs-lookup"><span data-stu-id="19b4f-139">PerformReminderAction</span></span>](performreminderaction.md)
    
- [<span data-ttu-id="19b4f-140">ReminderItemActions</span><span class="sxs-lookup"><span data-stu-id="19b4f-140">ReminderItemActions</span></span>](reminderitemactions.md)
    
- [<span data-ttu-id="19b4f-141">ReminderItemAction</span><span class="sxs-lookup"><span data-stu-id="19b4f-141">ReminderItemAction</span></span>](reminderitemaction.md)
    
- [<span data-ttu-id="19b4f-142">ActionType</span><span class="sxs-lookup"><span data-stu-id="19b4f-142">ActionType</span></span>](actiontype-reminderactiontype.md)
    
- [<span data-ttu-id="19b4f-143">ItemId</span><span class="sxs-lookup"><span data-stu-id="19b4f-143">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="19b4f-144">NewReminderTime</span><span class="sxs-lookup"><span data-stu-id="19b4f-144">NewReminderTime</span></span>](newremindertime.md)
    
## <a name="successful-performreminderaction-operation-response"></a><span data-ttu-id="19b4f-145">成功した PerformReminderAction 操作の応答</span><span class="sxs-lookup"><span data-stu-id="19b4f-145">Successful PerformReminderAction operation response</span></span>

<span data-ttu-id="19b4f-146">次の例は、 **PerformReminderAction**操作要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="19b4f-146">The following example shows a successful response to a **PerformReminderAction** operation request.</span></span> <span data-ttu-id="19b4f-147">**Updateditemids**要素には、更新された予定表アイテムの**itemids**が含まれています。</span><span class="sxs-lookup"><span data-stu-id="19b4f-147">The **UpdatedItemIds** element contains the **ItemIds** of the updated calendar item.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <ServerVersionInfo MajorVersion="15"
                       MinorVersion="0"
                       MajorBuildNumber="921"
                       MinorBuildNumber="20"
                       Version="V2_10"
                       xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <PerformReminderActionResponse ResponseClass="Success"
                                   xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <UpdatedItemIds>
        <ItemId Id="vwAAAA=="
                ChangeKey="DwAAABYAAAB4to43JyybTYwHLBM1k8MxAAAJKP+S"/>
      </UpdatedItemIds>
    </PerformReminderActionResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="19b4f-148">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="19b4f-148">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="19b4f-149">PerformReminderActionResponse</span><span class="sxs-lookup"><span data-stu-id="19b4f-149">PerformReminderActionResponse</span></span>](performreminderactionresponse.md)
    
- [<span data-ttu-id="19b4f-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="19b4f-150">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="19b4f-151">UpdatedItemIds</span><span class="sxs-lookup"><span data-stu-id="19b4f-151">UpdatedItemIds</span></span>](updateditemids.md)
    
- [<span data-ttu-id="19b4f-152">ItemId</span><span class="sxs-lookup"><span data-stu-id="19b4f-152">ItemId</span></span>](itemid.md)
    
## <a name="performreminderaction-operation-error-response-example"></a><span data-ttu-id="19b4f-153">PerformReminderAction 操作エラー応答の例</span><span class="sxs-lookup"><span data-stu-id="19b4f-153">PerformReminderAction operation error response example</span></span>

<span data-ttu-id="19b4f-154">次の例は、サーバーで変更が行われていない場合の**PerformReminderAction**操作要求への応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="19b4f-154">The following example shows a response to a **PerformReminderAction** operation request when no change was made on the server.</span></span> <span data-ttu-id="19b4f-155">これは、要求が送信されたものの、 **Updateditemids**が返されなかったこと、つまりアラームが変更されなかったことを示す応答です。</span><span class="sxs-lookup"><span data-stu-id="19b4f-155">This is a response in which a request was sent, but no **UpdatedItemIds** were returned, meaning no reminders were changed.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <ServerVersionInfo MajorVersion="15"
                       MinorVersion="0"
                       MajorBuildNumber="918"
                       MinorBuildNumber="7"
                       Version="V2_10"
                       xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <PerformReminderActionResponse ResponseClass="Success"
                                   xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <UpdatedItemIds />
    </PerformReminderActionResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="19b4f-156">エラー応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="19b4f-156">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="19b4f-157">PerformReminderActionResponse</span><span class="sxs-lookup"><span data-stu-id="19b4f-157">PerformReminderActionResponse</span></span>](performreminderactionresponse.md)
    
- [<span data-ttu-id="19b4f-158">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="19b4f-158">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="19b4f-159">UpdatedItemIds</span><span class="sxs-lookup"><span data-stu-id="19b4f-159">UpdatedItemIds</span></span>](updateditemids.md)
    
<span data-ttu-id="19b4f-160">EWS に汎用的なその他のエラーコードについては、「/」を[参照して](responsecode.md)ください。</span><span class="sxs-lookup"><span data-stu-id="19b4f-160">For additional error codes that are generic to EWS, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="19b4f-161">関連項目</span><span class="sxs-lookup"><span data-stu-id="19b4f-161">See also</span></span>


- [<span data-ttu-id="19b4f-162">GetReminders 操作</span><span class="sxs-lookup"><span data-stu-id="19b4f-162">GetReminders operation</span></span>](getreminders-operation.md)
    

