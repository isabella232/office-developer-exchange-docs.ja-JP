---
title: FindItem 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindItem
api_type:
- schema
ms.assetid: ebad6aae-16e7-44de-ae63-a95b24539729
description: FindItem EWS に関する情報の検索操作です。
ms.openlocfilehash: b033ac2930981819a20f1336d40058a5f7c03b89
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760521"
---
# <a name="finditem-operation"></a><span data-ttu-id="eea2a-103">FindItem 操作</span><span class="sxs-lookup"><span data-stu-id="eea2a-103">FindItem operation</span></span>

<span data-ttu-id="eea2a-104">**FindItem** EWS の操作に関する情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="eea2a-104">Find information about the **FindItem** EWS operation.</span></span> 
  
<span data-ttu-id="eea2a-105">**FindItem**操作は、ユーザーのメールボックス内にある項目を検索します。</span><span class="sxs-lookup"><span data-stu-id="eea2a-105">The **FindItem** operation searches for items that are located in a user's mailbox.</span></span> <span data-ttu-id="eea2a-106">この操作は、多くのフィルタ リングする方法と検索結果がどのように呼び出し元に返される形式を提供します。</span><span class="sxs-lookup"><span data-stu-id="eea2a-106">This operation provides many ways to filter and format how search results are returned to the caller.</span></span> 
  
## <a name="using-the-finditem-operation"></a><span data-ttu-id="eea2a-107">FindItem 操作を使用します。</span><span class="sxs-lookup"><span data-stu-id="eea2a-107">Using the FindItem operation</span></span>

<span data-ttu-id="eea2a-108">**FindItem**操作の要求は、メールボックスとデータがどのように応答で返される形式を検索するためのさまざまな方法を提供します。</span><span class="sxs-lookup"><span data-stu-id="eea2a-108">The **FindItem** operation request provides many ways for you to search a mailbox and format how the data is returned in a response.</span></span> <span data-ttu-id="eea2a-109">**FindItem**要求では、以下を指定できます。</span><span class="sxs-lookup"><span data-stu-id="eea2a-109">You can specify the following in a **FindItem** request:</span></span> 
  
- <span data-ttu-id="eea2a-110">かどうか検索では、浅いまたはソフト削除走査の実行がされます。</span><span class="sxs-lookup"><span data-stu-id="eea2a-110">Whether the search is a shallow or soft-deleted traversal.</span></span> <span data-ttu-id="eea2a-111">これを指定することが必要です。</span><span class="sxs-lookup"><span data-stu-id="eea2a-111">Specifying this is required.</span></span> <span data-ttu-id="eea2a-112">検索の制限と組み合わせて、ソフト削除走査が返される項目の数を 0 にすると、でもある場合に一致するアイテムの検索条件を注意してください。</span><span class="sxs-lookup"><span data-stu-id="eea2a-112">Note that a soft-deleted traversal combined with a search restriction will result in zero items returned, even if there are items that match the search criteria.</span></span>
    
- <span data-ttu-id="eea2a-113">アイテムの応答の図形です。</span><span class="sxs-lookup"><span data-stu-id="eea2a-113">The response shape of items.</span></span> <span data-ttu-id="eea2a-114">応答で返されるプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="eea2a-114">This identifies the properties that are returned in the response.</span></span> <span data-ttu-id="eea2a-115">これを指定することが必要です。</span><span class="sxs-lookup"><span data-stu-id="eea2a-115">Specifying this is required.</span></span>
    
- <span data-ttu-id="eea2a-116">検索を実行するフォルダーです。</span><span class="sxs-lookup"><span data-stu-id="eea2a-116">The folders from which to perform the search.</span></span> <span data-ttu-id="eea2a-117">これを指定することが必要です。</span><span class="sxs-lookup"><span data-stu-id="eea2a-117">Specifying this is required.</span></span>
    
- <span data-ttu-id="eea2a-118">ページング機構とビューの種類を返すためでは、ページのデータを表示します。</span><span class="sxs-lookup"><span data-stu-id="eea2a-118">The paging mechanism and view types for returning view data in pages.</span></span> <span data-ttu-id="eea2a-119">この指定は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="eea2a-119">Specifying this is optional.</span></span>
    
- <span data-ttu-id="eea2a-120">グループ化して、返されるアイテムの並べ替えのオプションです。</span><span class="sxs-lookup"><span data-stu-id="eea2a-120">Options for grouping and sorting the items that are returned.</span></span> <span data-ttu-id="eea2a-121">この指定は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="eea2a-121">Specifying this is optional.</span></span>
    
- <span data-ttu-id="eea2a-122">制限または返される項目をフィルター処理するための高度なクエリ構文 (AQS) 文字列を検索します。</span><span class="sxs-lookup"><span data-stu-id="eea2a-122">Search restrictions or Advanced Query Syntax (AQS) strings for filtering the items that are returned.</span></span> <span data-ttu-id="eea2a-123">AQS を使用して、コンテンツのインデックス検索の詳細については、[クエリ文字列 (文字列)](querystring-string.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="eea2a-123">For more information about using AQS for content index searches, see [QueryString (String)](querystring-string.md).</span></span> <span data-ttu-id="eea2a-124">この指定は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="eea2a-124">Specifying this is optional.</span></span>
    
- <span data-ttu-id="eea2a-125">応答で返されたアイテムの並べ替え順序です。</span><span class="sxs-lookup"><span data-stu-id="eea2a-125">The sort order for items returned in the response.</span></span> <span data-ttu-id="eea2a-126">この指定は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="eea2a-126">Specifying this is optional.</span></span>
    
<span data-ttu-id="eea2a-127">**FindItem**操作では、ストリーム再生可能なプロパティの最初の 512 バイトのみを返します。</span><span class="sxs-lookup"><span data-stu-id="eea2a-127">The **FindItem** operation returns only the first 512 bytes of any streamable property.</span></span> <span data-ttu-id="eea2a-128">Unicode では、null で終わる Unicode 文字列を使用して、最初の 255 文字を返します。</span><span class="sxs-lookup"><span data-stu-id="eea2a-128">For Unicode, it returns the first 255 characters by using a null-terminated Unicode string.</span></span> <span data-ttu-id="eea2a-129">メッセージ本文の形式または受信者の一覧は返されません。</span><span class="sxs-lookup"><span data-stu-id="eea2a-129">It does not return any of the message body formats or the recipient lists.</span></span> <span data-ttu-id="eea2a-130">**FindItem**受信者はサマリー返されます。</span><span class="sxs-lookup"><span data-stu-id="eea2a-130">**FindItem** will return a recipient summary.</span></span> <span data-ttu-id="eea2a-131">[GetItem 操作](getitem-operation.md)を使用すると、アイテムの詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="eea2a-131">You can use the [GetItem operation](getitem-operation.md) to get the details of an item.</span></span> 
  
 <span data-ttu-id="eea2a-132">**FindItem**は[名 (EmailAddressType)](name-emailaddresstype.md)の要素のみを返し、[メールボックス](mailbox.md)の要素に次のフィールド[(NonEmptyStringType) の EmailAddress](emailaddress-nonemptystringtype.md)要素を返しません。</span><span class="sxs-lookup"><span data-stu-id="eea2a-132">**FindItem** returns only the [Name (EmailAddressType)](name-emailaddresstype.md) element and does not return the [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) element in the [Mailbox](mailbox.md) element for the following fields:</span></span> 
  
- <span data-ttu-id="eea2a-133">メッセージの [[差出人](from.md)] フィールド</span><span class="sxs-lookup"><span data-stu-id="eea2a-133">The [From](from.md) field for messages</span></span> 
    
- <span data-ttu-id="eea2a-134">メッセージの[[送信者](sender.md)] フィールド</span><span class="sxs-lookup"><span data-stu-id="eea2a-134">The [Sender](sender.md) field for messages</span></span> 
    
- <span data-ttu-id="eea2a-135">予定表アイテムの[開催者](organizer.md)フィールド</span><span class="sxs-lookup"><span data-stu-id="eea2a-135">The [Organizer](organizer.md) field for calendar items</span></span> 
    
> [!NOTE]
> <span data-ttu-id="eea2a-136">**FindItem**操作では、[予定表ビュー](calendarview.md)の要素の結果を返すことができます。</span><span class="sxs-lookup"><span data-stu-id="eea2a-136">The **FindItem** operation can return results in a [CalendarView](calendarview.md) element.</span></span> <span data-ttu-id="eea2a-137">**予定表ビュー**の要素は、1 つの予定表アイテムと定期的な会議のすべての出現回数を返します。</span><span class="sxs-lookup"><span data-stu-id="eea2a-137">The **CalendarView** element returns single calendar items and all occurrences of recurring meetings.</span></span> <span data-ttu-id="eea2a-138">**予定表ビュー**の要素を使用しない場合は、1 つの予定表アイテムと定期的なマスターの予定表アイテムが返されます。</span><span class="sxs-lookup"><span data-stu-id="eea2a-138">If a **CalendarView** element is not used, single calendar items and recurring master calendar items are returned.</span></span> <span data-ttu-id="eea2a-139">**予定表ビュー**の要素を使用しない場合は、定期的なマスターから出現するを展開する必要があります。</span><span class="sxs-lookup"><span data-stu-id="eea2a-139">The occurrences must be expanded from the recurring master if a **CalendarView** element is not used.</span></span> 
  
<span data-ttu-id="eea2a-140">**FindItem**操作では、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="eea2a-140">The **FindItem** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
<span data-ttu-id="eea2a-141">**表 1 です。FindItem 操作の SOAP ヘッダー**</span><span class="sxs-lookup"><span data-stu-id="eea2a-141">**Table 1. FindItem operation SOAP headers**</span></span>

|<span data-ttu-id="eea2a-142">**Header**</span><span class="sxs-lookup"><span data-stu-id="eea2a-142">**Header**</span></span>|<span data-ttu-id="eea2a-143">**要素**</span><span class="sxs-lookup"><span data-stu-id="eea2a-143">**Element**</span></span>|<span data-ttu-id="eea2a-144">**説明**</span><span class="sxs-lookup"><span data-stu-id="eea2a-144">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="eea2a-145">**DateTimePrecision**</span><span class="sxs-lookup"><span data-stu-id="eea2a-145">**DateTimePrecision**</span></span> <br/> |[<span data-ttu-id="eea2a-146">DateTimePrecision</span><span class="sxs-lookup"><span data-stu-id="eea2a-146">DateTimePrecision</span></span>](datetimeprecision.md) <br/> |<span data-ttu-id="eea2a-147">秒またはミリ秒単位のいずれか、サーバーからの応答では、日付/時刻値の解像度を指定します。</span><span class="sxs-lookup"><span data-stu-id="eea2a-147">Specifies the resolution of data/time values in responses from the server, either in seconds or in milliseconds.</span></span> <span data-ttu-id="eea2a-148">これは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="eea2a-148">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="eea2a-149">**偽装**</span><span class="sxs-lookup"><span data-stu-id="eea2a-149">**Impersonation**</span></span> <br/> |[<span data-ttu-id="eea2a-150">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="eea2a-150">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="eea2a-151">クライアント アプリケーションが偽装するユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="eea2a-151">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="eea2a-152">これは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="eea2a-152">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="eea2a-153">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="eea2a-153">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="eea2a-154">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="eea2a-154">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="eea2a-155">RFC3066 カルチャを使用してメールボックスへのアクセスを識別します。</span><span class="sxs-lookup"><span data-stu-id="eea2a-155">Identifies the RFC3066 culture to be used to access the mailbox.</span></span> <span data-ttu-id="eea2a-156">これは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="eea2a-156">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="eea2a-157">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="eea2a-157">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="eea2a-158">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="eea2a-158">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="eea2a-159">操作要求のスキーマのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="eea2a-159">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="eea2a-160">これは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="eea2a-160">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="eea2a-161">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="eea2a-161">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="eea2a-162">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="eea2a-162">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="eea2a-163">要求に応答するサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="eea2a-163">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="eea2a-164">これは、応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="eea2a-164">This is applicable to a response.</span></span>  <br/> |
|<span data-ttu-id="eea2a-165">**TimeZoneContext**</span><span class="sxs-lookup"><span data-stu-id="eea2a-165">**TimeZoneContext**</span></span> <br/> |[<span data-ttu-id="eea2a-166">TimeZoneContext</span><span class="sxs-lookup"><span data-stu-id="eea2a-166">TimeZoneContext</span></span>](timezonecontext.md) <br/> |<span data-ttu-id="eea2a-167">サーバーからのすべての応答に使用するタイム ゾーンを識別します。</span><span class="sxs-lookup"><span data-stu-id="eea2a-167">Identifies the time zone to be used for all responses from the server.</span></span> <span data-ttu-id="eea2a-168">これは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="eea2a-168">This is applicable to a request.</span></span>  <br/> |
   
## <a name="finditem-operation-request-example"></a><span data-ttu-id="eea2a-169">FindItem 操作要求の例</span><span class="sxs-lookup"><span data-stu-id="eea2a-169">FindItem operation request example</span></span>

<span data-ttu-id="eea2a-170">**FindItem**要求の次の例では、削除済みアイテム フォルダーにあるアイテムの[BaseShape](baseshape.md)の要素の**IdOnly**列挙で定義されている項目の識別子を取得する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="eea2a-170">The following example of a **FindItem** request shows how to obtain the item identifier that is defined by the **IdOnly** enumeration of the [BaseShape](baseshape.md) element for items that are found in the Deleted Items folder.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
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

<span data-ttu-id="eea2a-171">次の要素は、要求で使用されます。</span><span class="sxs-lookup"><span data-stu-id="eea2a-171">The following elements are used in the request:</span></span> 
  
- [<span data-ttu-id="eea2a-172">FindItem</span><span class="sxs-lookup"><span data-stu-id="eea2a-172">FindItem</span></span>](finditem.md)
    
- [<span data-ttu-id="eea2a-173">ItemShape</span><span class="sxs-lookup"><span data-stu-id="eea2a-173">ItemShape</span></span>](itemshape.md)
    
- [<span data-ttu-id="eea2a-174">BaseShape</span><span class="sxs-lookup"><span data-stu-id="eea2a-174">BaseShape</span></span>](baseshape.md)
    
- [<span data-ttu-id="eea2a-175">ParentFolderIds</span><span class="sxs-lookup"><span data-stu-id="eea2a-175">ParentFolderIds</span></span>](parentfolderids.md)
    
- [<span data-ttu-id="eea2a-176">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="eea2a-176">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
<span data-ttu-id="eea2a-177">**FindItem**要求メッセージの詳細については、スキーマの階層構造を表示します。</span><span class="sxs-lookup"><span data-stu-id="eea2a-177">For more options for a **FindItem** request message, explore the schema hierarchy.</span></span> <span data-ttu-id="eea2a-178">[FindItem](finditem.md)要素から開始します。</span><span class="sxs-lookup"><span data-stu-id="eea2a-178">Start at the [FindItem](finditem.md) element.</span></span> 
  
## <a name="successful-finditem-operation-response"></a><span data-ttu-id="eea2a-179">FindItem 操作の成功の応答</span><span class="sxs-lookup"><span data-stu-id="eea2a-179">Successful FindItem operation response</span></span>

<span data-ttu-id="eea2a-180">**FindItem**要求に正常な応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="eea2a-180">The following example shows a successful response to the **FindItem** request.</span></span> 
  
<span data-ttu-id="eea2a-181">[メッセージ](message-ex15websvcsotherref.md)要素は、電子メール メッセージおよび EWS スキーマが厳密に型指定されない他のすべての項目を表します。</span><span class="sxs-lookup"><span data-stu-id="eea2a-181">[Message](message-ex15websvcsotherref.md) elements represent email messages and all other items that are not strongly typed by the EWS schema.</span></span> <span data-ttu-id="eea2a-182">IPM などの項目です。共有し、IPM.InfoPath は、[メッセージ](message-ex15websvcsotherref.md)の要素として返されます。</span><span class="sxs-lookup"><span data-stu-id="eea2a-182">Items such as IPM.Sharing and IPM.InfoPath are returned as [Message](message-ex15websvcsotherref.md) elements.</span></span> <span data-ttu-id="eea2a-183">Exchange では、応答の基本要素の[項目](item.md)が返されません。</span><span class="sxs-lookup"><span data-stu-id="eea2a-183">Exchange does not return the base [Item](item.md) element in responses.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

<span data-ttu-id="eea2a-184">次の要素は、応答で使用されます。</span><span class="sxs-lookup"><span data-stu-id="eea2a-184">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="eea2a-185">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="eea2a-185">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="eea2a-186">FindItemResponse</span><span class="sxs-lookup"><span data-stu-id="eea2a-186">FindItemResponse</span></span>](finditemresponse.md)
    
- [<span data-ttu-id="eea2a-187">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="eea2a-187">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="eea2a-188">FindItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="eea2a-188">FindItemResponseMessage</span></span>](finditemresponsemessage.md)
    
- [<span data-ttu-id="eea2a-189">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="eea2a-189">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="eea2a-190">RootFolder (FindItemResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="eea2a-190">RootFolder (FindItemResponseMessage)</span></span>](rootfolder-finditemresponsemessage.md)
    
- [<span data-ttu-id="eea2a-191">Items</span><span class="sxs-lookup"><span data-stu-id="eea2a-191">Items</span></span>](items.md)
    
- [<span data-ttu-id="eea2a-192">Message</span><span class="sxs-lookup"><span data-stu-id="eea2a-192">Message</span></span>](message-ex15websvcsotherref.md)
    
- [<span data-ttu-id="eea2a-193">ItemId</span><span class="sxs-lookup"><span data-stu-id="eea2a-193">ItemId</span></span>](itemid.md)
    
<span data-ttu-id="eea2a-194">**FindItem**応答メッセージの詳細については、スキーマの階層構造を表示します。</span><span class="sxs-lookup"><span data-stu-id="eea2a-194">For more options for a **FindItem** response message, explore the schema hierarchy.</span></span> <span data-ttu-id="eea2a-195">[FindItemResponse](finditemresponse.md)要素から開始します。</span><span class="sxs-lookup"><span data-stu-id="eea2a-195">Start at the [FindItemResponse](finditemresponse.md) element.</span></span> 
  
## <a name="finditem-operation-error-response"></a><span data-ttu-id="eea2a-196">FindItem 操作のエラー応答</span><span class="sxs-lookup"><span data-stu-id="eea2a-196">FindItem operation error response</span></span>

<span data-ttu-id="eea2a-197">**FindItem**要求に対してエラー応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="eea2a-197">The following example shows an error response to a **FindItem** request.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

<span data-ttu-id="eea2a-198">エラー応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="eea2a-198">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="eea2a-199">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="eea2a-199">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="eea2a-200">FindItemResponse</span><span class="sxs-lookup"><span data-stu-id="eea2a-200">FindItemResponse</span></span>](finditemresponse.md)
    
- [<span data-ttu-id="eea2a-201">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="eea2a-201">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="eea2a-202">FindItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="eea2a-202">FindItemResponseMessage</span></span>](finditemresponsemessage.md)
    
- [<span data-ttu-id="eea2a-203">MessageText</span><span class="sxs-lookup"><span data-stu-id="eea2a-203">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="eea2a-204">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="eea2a-204">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="eea2a-205">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="eea2a-205">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="eea2a-206">**FindItem**エラーの応答メッセージの詳細については、スキーマの階層構造を表示します。</span><span class="sxs-lookup"><span data-stu-id="eea2a-206">For more options for a **FindItem** error response message, explore the schema hierarchy.</span></span> <span data-ttu-id="eea2a-207">[FindItemResponse](finditemresponse.md)要素から開始します。</span><span class="sxs-lookup"><span data-stu-id="eea2a-207">Start at the [FindItemResponse](finditemresponse.md) element.</span></span> 
  
## <a name="version-differences"></a><span data-ttu-id="eea2a-208">バージョンの相違点</span><span class="sxs-lookup"><span data-stu-id="eea2a-208">Version differences</span></span>

<span data-ttu-id="eea2a-209">バージョンの Exchange でメジャー バージョン 15 で開始および終了は、 **FindItem**操作を使用して、アーカイブ メールボックスに複数のフォルダーを検索する場合に、15.0.898.11 の戻り値の[ResponseCode](responsecode.md)要素内の ErrorInvalidOperation 値を構築します。</span><span class="sxs-lookup"><span data-stu-id="eea2a-209">Versions of Exchange starting with major version 15 and ending with build 15.0.898.11 return an ErrorInvalidOperation value in the [ResponseCode](responsecode.md) element when the **FindItem** operation is used to search multiple folders in an archive mailbox.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="eea2a-210">関連項目</span><span class="sxs-lookup"><span data-stu-id="eea2a-210">See also</span></span>

- [<span data-ttu-id="eea2a-211">項目を検索します。</span><span class="sxs-lookup"><span data-stu-id="eea2a-211">Finding Items</span></span>](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)
    
- [<span data-ttu-id="eea2a-212">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="eea2a-212">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
    
- <span data-ttu-id="eea2a-213">**FindItemType**</span><span class="sxs-lookup"><span data-stu-id="eea2a-213">**FindItemType**</span></span>
    

