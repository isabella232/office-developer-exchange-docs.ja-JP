---
title: GetReminders 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1b56f83f-3b87-4b55-8259-fde6692da681
description: 操作 GetReminders EWS についての情報を検索します。
ms.openlocfilehash: 803dabf51b94dbd8fb01f2709a42ff59a597bfd1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760843"
---
# <a name="getreminders-operation"></a><span data-ttu-id="92584-103">GetReminders 操作</span><span class="sxs-lookup"><span data-stu-id="92584-103">GetReminders operation</span></span>

<span data-ttu-id="92584-104">**GetReminders** EWS の操作に関する情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="92584-104">Find information about the **GetReminders** EWS operation.</span></span> 
  
<span data-ttu-id="92584-105">**GetReminders** Exchange Web サービス (EWS) の操作は、予定表および仕事アイテムのアラーム機能を取得します。</span><span class="sxs-lookup"><span data-stu-id="92584-105">The **GetReminders** Exchange Web Services (EWS) operation retrieves reminders for calendar and task items.</span></span> 
  
<span data-ttu-id="92584-106">この操作は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="92584-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getreminders-operation"></a><span data-ttu-id="92584-107">GetReminders 操作を使用します。</span><span class="sxs-lookup"><span data-stu-id="92584-107">Using the GetReminders operation</span></span>

<span data-ttu-id="92584-108">**GetReminders**操作は、要求で渡される要素の値によって、ユーザーのメールボックスで、現在および将来の予定表および仕事のアイテムのアラームを取得します。</span><span class="sxs-lookup"><span data-stu-id="92584-108">The **GetReminders** operation gets reminders for current and future calendar and task items in the user's mailbox, depending on the element values passed in the request.</span></span> <span data-ttu-id="92584-109">操作には、すべての現在および将来の予定表アイテムにアラームを設定するタスクを取得できます。</span><span class="sxs-lookup"><span data-stu-id="92584-109">The operation can retrieve all current and future calendar items as well as tasks that have a reminder set.</span></span> <span data-ttu-id="92584-110">応答には、プライベートの予定表アイテムが含まれます。</span><span class="sxs-lookup"><span data-stu-id="92584-110">Private calendar items are included in responses.</span></span> <span data-ttu-id="92584-111">タスク アラームなしの応答に含まれないもアラームを設定した e メールまたはフォロー アップ フラグ。</span><span class="sxs-lookup"><span data-stu-id="92584-111">Tasks without reminders are not included in responses, nor are emails with reminders or follow up flags.</span></span> 
  
<span data-ttu-id="92584-112">現在のすべてのアラームを取得するには、**すべて**を[ReminderType](remindertype.md)と現在の時刻に[終了時刻](endtime-remindermessagedatatype.md)の設定をお勧めします。</span><span class="sxs-lookup"><span data-stu-id="92584-112">To retrieve all current reminders, we recommend setting the [ReminderType](remindertype.md) to **All** and the [EndTime](endtime-remindermessagedatatype.md) to the current time.</span></span> 
  
<span data-ttu-id="92584-113">[BeginTime](begintime.md)と**終了時刻**の要素が要求に含まれている場合、応答には、任意の予定表のアラームが含まれています、**形式の BeginTime**と**終了時刻**の間に発生するアラーム設定している間に発生する作業項目。</span><span class="sxs-lookup"><span data-stu-id="92584-113">If the [BeginTime](begintime.md) and **EndTime** elements are included in the request, the response includes reminders for any calendar and task items that occur between have a reminder that occurs between the **BeginTime** and **EndTime**.</span></span>
  
<span data-ttu-id="92584-114">**BeginTime**と**終了時刻**の要素が含まれる場合、次の表は**ReminderType**要素の動作を説明します。</span><span class="sxs-lookup"><span data-stu-id="92584-114">The following table describes the behavior of the **ReminderType** element when the **BeginTime** and **EndTime** elements are included.</span></span> 
  
|<span data-ttu-id="92584-115">* ReminderType * 要素値 * *</span><span class="sxs-lookup"><span data-stu-id="92584-115">****ReminderType** element value**</span></span>|<span data-ttu-id="92584-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="92584-116">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="92584-117">All</span><span class="sxs-lookup"><span data-stu-id="92584-117">All</span></span>  <br/> |<span data-ttu-id="92584-118">**BeginTime**と**終了時刻**の間で発生するアラームです。</span><span class="sxs-lookup"><span data-stu-id="92584-118">Reminders that occur between the **BeginTime** and **EndTime**.</span></span>  <br/> |
|<span data-ttu-id="92584-119">現在の</span><span class="sxs-lookup"><span data-stu-id="92584-119">Current</span></span>  <br/> |<span data-ttu-id="92584-120">アラームは**すべて**、によって返されるとイベントが、継続中の場合、要求された時間ウィンドウよりも前のアラームと期間に関係なくすべての予定です。</span><span class="sxs-lookup"><span data-stu-id="92584-120">Reminders returned by **All**, plus reminders that are earlier than the requested time window if the event is still ongoing, plus all appointments regardless of age.</span></span>  <br/> |
|<span data-ttu-id="92584-121">古い</span><span class="sxs-lookup"><span data-stu-id="92584-121">Old</span></span>  <br/> |<span data-ttu-id="92584-122">アラームが-すべての予定はまだ完了していないイベント-**すべて**が返されます。</span><span class="sxs-lookup"><span data-stu-id="92584-122">Reminders returned by **All**, minus events that haven't completed yet, minus all appointments.</span></span> <span data-ttu-id="92584-123">**BeginTime**と**終了時刻**の要素は、**古い**値を使用して設定してください。</span><span class="sxs-lookup"><span data-stu-id="92584-123">The **BeginTime** and **EndTime** elements must be set to use the **Old** value.</span></span>  <br/> |
   
### <a name="getreminders-operation-soap-headers"></a><span data-ttu-id="92584-124">GetReminders 操作の SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="92584-124">GetReminders operation SOAP headers</span></span>

<span data-ttu-id="92584-125">**GetReminders**操作は、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="92584-125">The **GetReminders** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="92584-126">**ヘッダー名**</span><span class="sxs-lookup"><span data-stu-id="92584-126">**Header name**</span></span>|<span data-ttu-id="92584-127">**要素**</span><span class="sxs-lookup"><span data-stu-id="92584-127">**Element**</span></span>|<span data-ttu-id="92584-128">**説明**</span><span class="sxs-lookup"><span data-stu-id="92584-128">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="92584-129">**偽装**</span><span class="sxs-lookup"><span data-stu-id="92584-129">**Impersonation**</span></span> <br/> |[<span data-ttu-id="92584-130">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="92584-130">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="92584-131">クライアント アプリケーションが偽装するユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="92584-131">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="92584-132">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="92584-132">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="92584-133">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="92584-133">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="92584-134">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="92584-134">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="92584-135">RFC 3066、」タグの「識別の言語」を使用してメールボックスへのアクセスに定義されているカルチャを識別します。</span><span class="sxs-lookup"><span data-stu-id="92584-135">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="92584-136">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="92584-136">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="92584-137">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="92584-137">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="92584-138">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="92584-138">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="92584-139">操作要求のスキーマのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="92584-139">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="92584-140">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="92584-140">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="92584-141">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="92584-141">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="92584-142">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="92584-142">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="92584-143">要求に応答するサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="92584-143">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="92584-144">このヘッダーは、応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="92584-144">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getreminders-operation-request-example"></a><span data-ttu-id="92584-145">GetReminders 操作の要求の例</span><span class="sxs-lookup"><span data-stu-id="92584-145">GetReminders operation request example</span></span>

<span data-ttu-id="92584-146">**GetReminders**操作要求の次の使用例は、**形式の BeginTime**と**終了時刻**の間で発生する最初の 5 つの予定表アイテムを取得する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="92584-146">The following example of a **GetReminders** operation request shows how to retrieve the first five calendar items that occur between the **BeginTime** and **EndTime**.</span></span>
  
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
    <m:GetReminders>
      <m:EndTime>2014-04-16T21:00:00Z</m:EndTime>
      <m:ReminderType>All</m:ReminderType>
    </m:GetReminders>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="92584-147">例要求 SOAP 本体にはには、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="92584-147">The example request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="92584-148">GetReminders</span><span class="sxs-lookup"><span data-stu-id="92584-148">GetReminders</span></span>](getreminders.md)
    
- [<span data-ttu-id="92584-149">終了時刻</span><span class="sxs-lookup"><span data-stu-id="92584-149">EndTime</span></span>](endtime-remindermessagedatatype.md)
    
- [<span data-ttu-id="92584-150">ReminderType</span><span class="sxs-lookup"><span data-stu-id="92584-150">ReminderType</span></span>](remindertype.md)
    
<span data-ttu-id="92584-151">SOAP 本体には、次の要素を含めることも。</span><span class="sxs-lookup"><span data-stu-id="92584-151">The SOAP body can also contain the following elements:</span></span>
  
- [<span data-ttu-id="92584-152">BeginTime</span><span class="sxs-lookup"><span data-stu-id="92584-152">BeginTime</span></span>](begintime.md)
    
- [<span data-ttu-id="92584-153">MaxItems</span><span class="sxs-lookup"><span data-stu-id="92584-153">MaxItems</span></span>](maxitems.md)
    
## <a name="successful-getreminders-operation-response"></a><span data-ttu-id="92584-154">GetReminders 操作の成功の応答</span><span class="sxs-lookup"><span data-stu-id="92584-154">Successful GetReminders operation response</span></span>

<span data-ttu-id="92584-155">成功した要求への応答、 **GetReminders**操作の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="92584-155">The following example shows a successful response to a **GetReminders** operation request.</span></span> <span data-ttu-id="92584-156">応答には、「チーム ミーティング」の予定表アイテムのアラームを設定し、"会議ノートを送信するタスクの「タスクのアラームが含まれています。</span><span class="sxs-lookup"><span data-stu-id="92584-156">The response contains a reminder for the "Team meeting" calendar item and a reminder for the "Task to send meeting notes" task.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="92584-157">識別子は、読みやすさを保持するために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="92584-157">Identifiers have been shortened to preserve readability.</span></span> 
  
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
    <GetRemindersResponse ResponseClass="Success"
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <Reminders>
        <Reminder xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <Subject>Team meeting</Subject>
          <Location />
          <ReminderTime>2014-04-15T21:00:00Z</ReminderTime>
          <StartDate>2014-04-15T21:00:00Z</StartDate>
          <EndDate>2014-04-15T21:30:00Z</EndDate>
          <ItemId Id="vQAAAA=="
                  ChangeKey="DwAAABYAAAB4to43JyybTYwHLBM1k8MxAAACRoV4" />
          <RecurringMasterItemId Id="K7u5AAA=" ChangeKey="DwAAABYAAAB4to43JyybTYwHLBM1k8MxAAACRoV0" />
          <ReminderGroup>Calendar</ReminderGroup>
          <UID>6CF2FA62</UID>
        </Reminder>
        <Reminder xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <Subject>Task to send meeting notes</Subject>
          <Location />
          <ReminderTime>2014-04-16T14:00:00Z</ReminderTime>
          <StartDate>0001-01-02T00:00:00Z</StartDate>
          <EndDate>0001-01-02T00:00:00Z</EndDate>
          <ItemId Id="vAAAAA=="
                  ChangeKey="EwAAABQAAACOs0HEMq1WTKpI7sNu5qXNAAAIDg==" />
          <ReminderGroup>Task</ReminderGroup>
          <UID>vAAAAA==</UID>
        </Reminder>
      </Reminders>
    </GetRemindersResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="92584-158">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="92584-158">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="92584-159">GetRemindersResponse</span><span class="sxs-lookup"><span data-stu-id="92584-159">GetRemindersResponse</span></span>](getremindersresponse.md)
    
- [<span data-ttu-id="92584-160">Reminders</span><span class="sxs-lookup"><span data-stu-id="92584-160">Reminders</span></span>](reminders.md)
    
- [<span data-ttu-id="92584-161">Reminder</span><span class="sxs-lookup"><span data-stu-id="92584-161">Reminder</span></span>](reminder.md)
    
- [<span data-ttu-id="92584-162">Subject</span><span class="sxs-lookup"><span data-stu-id="92584-162">Subject</span></span>](subject.md)
    
- [<span data-ttu-id="92584-163">場所</span><span class="sxs-lookup"><span data-stu-id="92584-163">Location</span></span>](location-remindermessagedatatype.md)
    
- [<span data-ttu-id="92584-164">ReminderTime</span><span class="sxs-lookup"><span data-stu-id="92584-164">ReminderTime</span></span>](remindertime.md)
    
- [<span data-ttu-id="92584-165">開始日</span><span class="sxs-lookup"><span data-stu-id="92584-165">StartDate</span></span>](startdate.md)
    
- [<span data-ttu-id="92584-166">終了日</span><span class="sxs-lookup"><span data-stu-id="92584-166">EndDate</span></span>](enddate-remindertype.md)
    
- [<span data-ttu-id="92584-167">ItemId</span><span class="sxs-lookup"><span data-stu-id="92584-167">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="92584-168">RecurringMasterItemId</span><span class="sxs-lookup"><span data-stu-id="92584-168">RecurringMasterItemId</span></span>](recurringmasteritemid.md)
    
- [<span data-ttu-id="92584-169">ReminderGroup</span><span class="sxs-lookup"><span data-stu-id="92584-169">ReminderGroup</span></span>](remindergroup.md)
    
- [<span data-ttu-id="92584-170">UID</span><span class="sxs-lookup"><span data-stu-id="92584-170">UID</span></span>](uid-remindertype.md)
    
## <a name="getreminders-operation-error-response-example"></a><span data-ttu-id="92584-171">GetReminders 操作のエラー応答の例</span><span class="sxs-lookup"><span data-stu-id="92584-171">GetReminders operation error response example</span></span>

<span data-ttu-id="92584-172">**GetReminders**操作の要求に対してエラー応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="92584-172">The following example shows an error response to a **GetReminders** operation request.</span></span> <span data-ttu-id="92584-173">これは、終了日が開始日より前の要求に応答します。</span><span class="sxs-lookup"><span data-stu-id="92584-173">This is a response to a request in which the end date was earlier than the start date.</span></span> 
  
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
    <GetRemindersResponse ResponseClass="Error"
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <MessageText>EndDate is earlier than StartDate</MessageText>
      <ResponseCode>ErrorInvalidOperation</ResponseCode>
      <DescriptiveLinkKey>0</DescriptiveLinkKey>
    </GetRemindersResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="92584-174">エラー応答 SOAP 本体にはには、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="92584-174">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="92584-175">GetRemindersResponse</span><span class="sxs-lookup"><span data-stu-id="92584-175">GetRemindersResponse</span></span>](getremindersresponse.md)
    
- [<span data-ttu-id="92584-176">MessageText</span><span class="sxs-lookup"><span data-stu-id="92584-176">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="92584-177">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="92584-177">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="92584-178">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="92584-178">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="92584-179">EWS を汎用的なこの操作に固有のエラー コードは、 [ResponseCode](responsecode.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="92584-179">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="92584-180">関連項目</span><span class="sxs-lookup"><span data-stu-id="92584-180">See also</span></span>


- [<span data-ttu-id="92584-181">PerformReminderAction</span><span class="sxs-lookup"><span data-stu-id="92584-181">PerformReminderAction</span></span>](performreminderaction.md)
    

