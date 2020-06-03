---
title: FindItem 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
api_name:
- FindItem
api_type:
- schema
ms.assetid: ebad6aae-16e7-44de-ae63-a95b24539729
description: FindItem EWS 操作についての情報を検索します。
localization_priority: Priority
ms.openlocfilehash: 499d1ee80ef323c883fa86eb125d8c037fb37d4e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462557"
---
# <a name="finditem-operation"></a><span data-ttu-id="d052d-103">FindItem 操作</span><span class="sxs-lookup"><span data-stu-id="d052d-103">FindItem operation</span></span>

<span data-ttu-id="d052d-104">**FindItem** EWS 操作についての情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="d052d-104">Find information about the **FindItem** EWS operation.</span></span> 
  
<span data-ttu-id="d052d-105">**FindItem**操作は、ユーザーのメールボックスにあるアイテムを検索します。</span><span class="sxs-lookup"><span data-stu-id="d052d-105">The **FindItem** operation searches for items that are located in a user's mailbox.</span></span> <span data-ttu-id="d052d-106">この操作では、検索結果が発信者に返される方法をフィルター処理し、書式設定するためのさまざまな方法を提供します。</span><span class="sxs-lookup"><span data-stu-id="d052d-106">This operation provides many ways to filter and format how search results are returned to the caller.</span></span> 
  
## <a name="using-the-finditem-operation"></a><span data-ttu-id="d052d-107">FindItem 操作の使用</span><span class="sxs-lookup"><span data-stu-id="d052d-107">Using the FindItem operation</span></span>

<span data-ttu-id="d052d-108">**FindItem**操作要求では、メールボックスを検索して、そのデータが応答で返される方法を書式設定するさまざまな方法を使用できます。</span><span class="sxs-lookup"><span data-stu-id="d052d-108">The **FindItem** operation request provides many ways for you to search a mailbox and format how the data is returned in a response.</span></span> <span data-ttu-id="d052d-109">**FindItem**要求では、次のものを指定できます。</span><span class="sxs-lookup"><span data-stu-id="d052d-109">You can specify the following in a **FindItem** request:</span></span> 
  
- <span data-ttu-id="d052d-110">検索が浅い、または削除済みの走査であるかどうか。</span><span class="sxs-lookup"><span data-stu-id="d052d-110">Whether the search is a shallow or soft-deleted traversal.</span></span> <span data-ttu-id="d052d-111">これを指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d052d-111">Specifying this is required.</span></span> <span data-ttu-id="d052d-112">検索条件に一致するアイテムが存在する場合でも、削除済み検査と検索制限を組み合わせると、返されるアイテムが0になることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="d052d-112">Note that a soft-deleted traversal combined with a search restriction will result in zero items returned, even if there are items that match the search criteria.</span></span>
    
- <span data-ttu-id="d052d-113">アイテムの応答の形状。</span><span class="sxs-lookup"><span data-stu-id="d052d-113">The response shape of items.</span></span> <span data-ttu-id="d052d-114">これは、応答で返されるプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="d052d-114">This identifies the properties that are returned in the response.</span></span> <span data-ttu-id="d052d-115">これを指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d052d-115">Specifying this is required.</span></span>
    
- <span data-ttu-id="d052d-116">検索を実行するフォルダー。</span><span class="sxs-lookup"><span data-stu-id="d052d-116">The folders from which to perform the search.</span></span> <span data-ttu-id="d052d-117">これを指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d052d-117">Specifying this is required.</span></span>
    
- <span data-ttu-id="d052d-118">ページ内のビューデータを返すページングメカニズムとビューの種類。</span><span class="sxs-lookup"><span data-stu-id="d052d-118">The paging mechanism and view types for returning view data in pages.</span></span> <span data-ttu-id="d052d-119">この指定は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="d052d-119">Specifying this is optional.</span></span>
    
- <span data-ttu-id="d052d-120">返されるアイテムをグループ化および並べ替えするためのオプション。</span><span class="sxs-lookup"><span data-stu-id="d052d-120">Options for grouping and sorting the items that are returned.</span></span> <span data-ttu-id="d052d-121">この指定は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="d052d-121">Specifying this is optional.</span></span>
    
- <span data-ttu-id="d052d-122">返されるアイテムをフィルター処理するための検索制限または高度なクエリ構文 (AQS) 文字列。</span><span class="sxs-lookup"><span data-stu-id="d052d-122">Search restrictions or Advanced Query Syntax (AQS) strings for filtering the items that are returned.</span></span> <span data-ttu-id="d052d-123">コンテンツインデックス検索での AQS の使用の詳細については、「 [QueryString (String)](querystring-string.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d052d-123">For more information about using AQS for content index searches, see [QueryString (String)](querystring-string.md).</span></span> <span data-ttu-id="d052d-124">この指定は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="d052d-124">Specifying this is optional.</span></span>
    
- <span data-ttu-id="d052d-125">応答で返されるアイテムの並べ替え順序を示します。</span><span class="sxs-lookup"><span data-stu-id="d052d-125">The sort order for items returned in the response.</span></span> <span data-ttu-id="d052d-126">この指定は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="d052d-126">Specifying this is optional.</span></span>
    
<span data-ttu-id="d052d-127">**FindItem**操作は、任意の streamable プロパティの最初の512バイトのみを返します。</span><span class="sxs-lookup"><span data-stu-id="d052d-127">The **FindItem** operation returns only the first 512 bytes of any streamable property.</span></span> <span data-ttu-id="d052d-128">Unicode の場合は、Null 終了の Unicode 文字列を使用して最初の 255 文字を返します。</span><span class="sxs-lookup"><span data-stu-id="d052d-128">For Unicode, it returns the first 255 characters by using a null-terminated Unicode string.</span></span> <span data-ttu-id="d052d-129">メッセージ本文の形式や受信者リストは返されません。</span><span class="sxs-lookup"><span data-stu-id="d052d-129">It does not return any of the message body formats or the recipient lists.</span></span> <span data-ttu-id="d052d-130">**FindItem**は受信者の概要を返します。</span><span class="sxs-lookup"><span data-stu-id="d052d-130">**FindItem** will return a recipient summary.</span></span> <span data-ttu-id="d052d-131">[GetItem 操作](getitem-operation.md)を使用して、アイテムの詳細を取得できます。</span><span class="sxs-lookup"><span data-stu-id="d052d-131">You can use the [GetItem operation](getitem-operation.md) to get the details of an item.</span></span> 
  
 <span data-ttu-id="d052d-132">**FindItem**は、 [Name (emailaddresstype)](name-emailaddresstype.md)要素のみを返します。次のフィールドの[Mailbox](mailbox.md)要素には、 [EmailAddress (nonemptystringtype)](emailaddress-nonemptystringtype.md)要素は返されません。</span><span class="sxs-lookup"><span data-stu-id="d052d-132">**FindItem** returns only the [Name (EmailAddressType)](name-emailaddresstype.md) element and does not return the [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) element in the [Mailbox](mailbox.md) element for the following fields:</span></span> 
  
- <span data-ttu-id="d052d-133">メッセージの [[差出人](from.md)] フィールド</span><span class="sxs-lookup"><span data-stu-id="d052d-133">The [From](from.md) field for messages</span></span> 
    
- <span data-ttu-id="d052d-134">メッセージの[Sender](sender.md)フィールド</span><span class="sxs-lookup"><span data-stu-id="d052d-134">The [Sender](sender.md) field for messages</span></span> 
    
- <span data-ttu-id="d052d-135">予定表アイテムの[開催者](organizer.md)フィールド</span><span class="sxs-lookup"><span data-stu-id="d052d-135">The [Organizer](organizer.md) field for calendar items</span></span> 
    
> [!NOTE]
> <span data-ttu-id="d052d-136">**FindItem**操作は、 [CalendarView](calendarview.md)要素で結果を返すことができます。</span><span class="sxs-lookup"><span data-stu-id="d052d-136">The **FindItem** operation can return results in a [CalendarView](calendarview.md) element.</span></span> <span data-ttu-id="d052d-137">**CalendarView**要素は、1つの予定表アイテムと定期的な会議のすべてのオカレンスを返します。</span><span class="sxs-lookup"><span data-stu-id="d052d-137">The **CalendarView** element returns single calendar items and all occurrences of recurring meetings.</span></span> <span data-ttu-id="d052d-138">**CalendarView**要素を使用しない場合は、1つの予定表アイテムと定期的な予定表アイテムが返されます。</span><span class="sxs-lookup"><span data-stu-id="d052d-138">If a **CalendarView** element is not used, single calendar items and recurring master calendar items are returned.</span></span> <span data-ttu-id="d052d-139">**CalendarView**要素が使用されていない場合は、定期的なマスターからオカレンスを展開する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d052d-139">The occurrences must be expanded from the recurring master if a **CalendarView** element is not used.</span></span> 
  
<span data-ttu-id="d052d-140">**FindItem**操作では、次の表に示す SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="d052d-140">The **FindItem** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
<span data-ttu-id="d052d-141">**表1FindItem 操作の SOAP ヘッダー**</span><span class="sxs-lookup"><span data-stu-id="d052d-141">**Table 1. FindItem operation SOAP headers**</span></span>

|<span data-ttu-id="d052d-142">**Header**</span><span class="sxs-lookup"><span data-stu-id="d052d-142">**Header**</span></span>|<span data-ttu-id="d052d-143">**要素**</span><span class="sxs-lookup"><span data-stu-id="d052d-143">**Element**</span></span>|<span data-ttu-id="d052d-144">**説明**</span><span class="sxs-lookup"><span data-stu-id="d052d-144">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="d052d-145">**DateTimePrecision**</span><span class="sxs-lookup"><span data-stu-id="d052d-145">**DateTimePrecision**</span></span> <br/> |[<span data-ttu-id="d052d-146">DateTimePrecision</span><span class="sxs-lookup"><span data-stu-id="d052d-146">DateTimePrecision</span></span>](datetimeprecision.md) <br/> |<span data-ttu-id="d052d-147">サーバーからの応答におけるデータ/時刻値の解決方法を秒単位で指定します。またはミリ秒単位で指定します。</span><span class="sxs-lookup"><span data-stu-id="d052d-147">Specifies the resolution of data/time values in responses from the server, either in seconds or in milliseconds.</span></span> <span data-ttu-id="d052d-148">これは要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="d052d-148">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="d052d-149">**偽装**</span><span class="sxs-lookup"><span data-stu-id="d052d-149">**Impersonation**</span></span> <br/> |[<span data-ttu-id="d052d-150">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="d052d-150">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="d052d-151">クライアントアプリケーションが偽装しているユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="d052d-151">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="d052d-152">これは要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="d052d-152">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="d052d-153">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="d052d-153">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="d052d-154">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="d052d-154">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="d052d-155">メールボックスへのアクセスに使用する RFC3066 カルチャを指定します。</span><span class="sxs-lookup"><span data-stu-id="d052d-155">Identifies the RFC3066 culture to be used to access the mailbox.</span></span> <span data-ttu-id="d052d-156">これは要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="d052d-156">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="d052d-157">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="d052d-157">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="d052d-158">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="d052d-158">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="d052d-159">操作要求のスキーマバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="d052d-159">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="d052d-160">これは要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="d052d-160">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="d052d-161">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="d052d-161">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="d052d-162">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="d052d-162">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="d052d-163">要求に応答したサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="d052d-163">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="d052d-164">これは応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="d052d-164">This is applicable to a response.</span></span>  <br/> |
|<span data-ttu-id="d052d-165">**TimeZoneContext**</span><span class="sxs-lookup"><span data-stu-id="d052d-165">**TimeZoneContext**</span></span> <br/> |[<span data-ttu-id="d052d-166">TimeZoneContext</span><span class="sxs-lookup"><span data-stu-id="d052d-166">TimeZoneContext</span></span>](timezonecontext.md) <br/> |<span data-ttu-id="d052d-167">サーバーからのすべての応答に使用するタイムゾーンを指定します。</span><span class="sxs-lookup"><span data-stu-id="d052d-167">Identifies the time zone to be used for all responses from the server.</span></span> <span data-ttu-id="d052d-168">これは要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="d052d-168">This is applicable to a request.</span></span>  <br/> |
   
## <a name="finditem-operation-request-example"></a><span data-ttu-id="d052d-169">FindItem 操作要求の例</span><span class="sxs-lookup"><span data-stu-id="d052d-169">FindItem operation request example</span></span>

<span data-ttu-id="d052d-170">次の**FindItem**要求の例は、[削除済みアイテム] フォルダーにあるアイテムの[Baseshape](baseshape.md)要素の**idonly**列挙で定義されているアイテム識別子を取得する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="d052d-170">The following example of a **FindItem** request shows how to obtain the item identifier that is defined by the **IdOnly** enumeration of the [BaseShape](baseshape.md) element for items that are found in the Deleted Items folder.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
              Traversal="Shallow">
      <ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
      </ItemShape>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="deleteditems"/>
      </ParentFolderIds>
    </FindItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="d052d-171">要求では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="d052d-171">The following elements are used in the request:</span></span> 
  
- [<span data-ttu-id="d052d-172">FindItem</span><span class="sxs-lookup"><span data-stu-id="d052d-172">FindItem</span></span>](finditem.md)
    
- [<span data-ttu-id="d052d-173">ItemShape</span><span class="sxs-lookup"><span data-stu-id="d052d-173">ItemShape</span></span>](itemshape.md)
    
- [<span data-ttu-id="d052d-174">BaseShape</span><span class="sxs-lookup"><span data-stu-id="d052d-174">BaseShape</span></span>](baseshape.md)
    
- [<span data-ttu-id="d052d-175">ParentFolderIds</span><span class="sxs-lookup"><span data-stu-id="d052d-175">ParentFolderIds</span></span>](parentfolderids.md)
    
- [<span data-ttu-id="d052d-176">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="d052d-176">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
<span data-ttu-id="d052d-177">**FindItem**要求メッセージのその他のオプションについては、スキーマ階層を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d052d-177">For more options for a **FindItem** request message, explore the schema hierarchy.</span></span> <span data-ttu-id="d052d-178">[FindItem](finditem.md)要素から開始します。</span><span class="sxs-lookup"><span data-stu-id="d052d-178">Start at the [FindItem](finditem.md) element.</span></span> 
  
## <a name="successful-finditem-operation-response"></a><span data-ttu-id="d052d-179">成功した FindItem 操作応答</span><span class="sxs-lookup"><span data-stu-id="d052d-179">Successful FindItem operation response</span></span>

<span data-ttu-id="d052d-180">次の例は、 **FindItem**要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="d052d-180">The following example shows a successful response to the **FindItem** request.</span></span> 
  
<span data-ttu-id="d052d-181">[Message](message-ex15websvcsotherref.md)要素は、電子メールメッセージと、EWS スキーマで厳密に型指定されていないその他すべてのアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="d052d-181">[Message](message-ex15websvcsotherref.md) elements represent email messages and all other items that are not strongly typed by the EWS schema.</span></span> <span data-ttu-id="d052d-182">IPM などのアイテム。共有と IPM. InfoPath は、[メッセージ](message-ex15websvcsotherref.md)要素として返されます。</span><span class="sxs-lookup"><span data-stu-id="d052d-182">Items such as IPM.Sharing and IPM.InfoPath are returned as [Message](message-ex15websvcsotherref.md) elements.</span></span> <span data-ttu-id="d052d-183">Exchange は、応答で基本[Item](item.md)要素を返しません。</span><span class="sxs-lookup"><span data-stu-id="d052d-183">Exchange does not return the base [Item](item.md) element in responses.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder TotalItemsInView="10" IncludesLastItemInRange="true">
            <t:Items>
              <t:Message>
                <t:ItemId Id="AS4AUn=" ChangeKey="fsVU4==" />
              </t:Message>
              <t:Message>
                <t:ItemId Id="AS4AUM=" ChangeKey="fsVUA==" />
              </t:Message>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </FindItemResponse>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="d052d-184">応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="d052d-184">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="d052d-185">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="d052d-185">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="d052d-186">FindItemResponse</span><span class="sxs-lookup"><span data-stu-id="d052d-186">FindItemResponse</span></span>](finditemresponse.md)
    
- [<span data-ttu-id="d052d-187">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="d052d-187">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="d052d-188">FindItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d052d-188">FindItemResponseMessage</span></span>](finditemresponsemessage.md)
    
- [<span data-ttu-id="d052d-189">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="d052d-189">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="d052d-190">RootFolder (FindItemResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="d052d-190">RootFolder (FindItemResponseMessage)</span></span>](rootfolder-finditemresponsemessage.md)
    
- [<span data-ttu-id="d052d-191">Items</span><span class="sxs-lookup"><span data-stu-id="d052d-191">Items</span></span>](items.md)
    
- [<span data-ttu-id="d052d-192">Message</span><span class="sxs-lookup"><span data-stu-id="d052d-192">Message</span></span>](message-ex15websvcsotherref.md)
    
- [<span data-ttu-id="d052d-193">ItemId</span><span class="sxs-lookup"><span data-stu-id="d052d-193">ItemId</span></span>](itemid.md)
    
<span data-ttu-id="d052d-194">**FindItem**応答メッセージのその他のオプションについては、スキーマ階層を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d052d-194">For more options for a **FindItem** response message, explore the schema hierarchy.</span></span> <span data-ttu-id="d052d-195">[Finditemresponse](finditemresponse.md)要素から開始します。</span><span class="sxs-lookup"><span data-stu-id="d052d-195">Start at the [FindItemResponse](finditemresponse.md) element.</span></span> 
  
## <a name="finditem-operation-error-response"></a><span data-ttu-id="d052d-196">FindItem 操作エラー応答</span><span class="sxs-lookup"><span data-stu-id="d052d-196">FindItem operation error response</span></span>

<span data-ttu-id="d052d-197">次の例は、 **FindItem**要求に対するエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="d052d-197">The following example shows an error response to a **FindItem** request.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Error">
          <m:MessageText>Id is malformed.</m:MessageText>
          <m:ResponseCode>ErrorInvalidIdMalformed</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </FindItemResponse>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="d052d-198">エラー応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="d052d-198">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="d052d-199">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="d052d-199">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="d052d-200">FindItemResponse</span><span class="sxs-lookup"><span data-stu-id="d052d-200">FindItemResponse</span></span>](finditemresponse.md)
    
- [<span data-ttu-id="d052d-201">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="d052d-201">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="d052d-202">FindItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d052d-202">FindItemResponseMessage</span></span>](finditemresponsemessage.md)
    
- [<span data-ttu-id="d052d-203">MessageText</span><span class="sxs-lookup"><span data-stu-id="d052d-203">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="d052d-204">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="d052d-204">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="d052d-205">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="d052d-205">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="d052d-206">**FindItem**エラー応答メッセージのその他のオプションについては、スキーマ階層を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d052d-206">For more options for a **FindItem** error response message, explore the schema hierarchy.</span></span> <span data-ttu-id="d052d-207">[Finditemresponse](finditemresponse.md)要素から開始します。</span><span class="sxs-lookup"><span data-stu-id="d052d-207">Start at the [FindItemResponse](finditemresponse.md) element.</span></span> 
  
## <a name="version-differences"></a><span data-ttu-id="d052d-208">バージョンの相違点</span><span class="sxs-lookup"><span data-stu-id="d052d-208">Version differences</span></span>

<span data-ttu-id="d052d-209">メジャーバージョン15以降のバージョンの Exchange は、アーカイブメールボックス内の複数のフォルダーを検索するために**FindItem**操作を使用し[て、15.0.898.11](responsecode.md)の ErrorInvalidOperation 値を返します。</span><span class="sxs-lookup"><span data-stu-id="d052d-209">Versions of Exchange starting with major version 15 and ending with build 15.0.898.11 return an ErrorInvalidOperation value in the [ResponseCode](responsecode.md) element when the **FindItem** operation is used to search multiple folders in an archive mailbox.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="d052d-210">関連項目</span><span class="sxs-lookup"><span data-stu-id="d052d-210">See also</span></span>

- [<span data-ttu-id="d052d-211">アイテムの検索</span><span class="sxs-lookup"><span data-stu-id="d052d-211">Finding Items</span></span>](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)
    
- [<span data-ttu-id="d052d-212">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="d052d-212">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
    
- <span data-ttu-id="d052d-213">**FindItemType**</span><span class="sxs-lookup"><span data-stu-id="d052d-213">**FindItemType**</span></span>
    

