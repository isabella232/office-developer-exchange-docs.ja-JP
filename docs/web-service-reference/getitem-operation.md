---
title: GetItem 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
api_name:
- GetItem
api_type:
- schema
ms.assetid: e3590b8b-c2a7-4dad-a014-6360197b68e4
description: GetItem EWS 操作に関する情報を検索します。
localization_priority: Priority
ms.openlocfilehash: 8871dde183974454fc27dbddda489e6b0a70f3aa
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463329"
---
# <a name="getitem-operation"></a><span data-ttu-id="68c64-103">GetItem 操作</span><span class="sxs-lookup"><span data-stu-id="68c64-103">GetItem operation</span></span>

<span data-ttu-id="68c64-104">**GetItem** EWS 操作に関する情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="68c64-104">Find information about the **GetItem** EWS operation.</span></span> 
  
<span data-ttu-id="68c64-105">**GetItem**操作は、Exchange ストアからアイテムを取得します。</span><span class="sxs-lookup"><span data-stu-id="68c64-105">The **GetItem** operation gets items from the Exchange store.</span></span> 
  
## <a name="using-the-getitem-operation"></a><span data-ttu-id="68c64-106">GetItem 操作の使用</span><span class="sxs-lookup"><span data-stu-id="68c64-106">Using the GetItem operation</span></span>

<span data-ttu-id="68c64-107">**GetItem**操作は、多くのアイテムプロパティを返します。</span><span class="sxs-lookup"><span data-stu-id="68c64-107">The **GetItem** operation returns many item properties.</span></span> <span data-ttu-id="68c64-108">**GetItem**応答で返されるプロパティは、要求された図形、要求された追加プロパティ、および返されるアイテムの種類によって異なります。</span><span class="sxs-lookup"><span data-stu-id="68c64-108">The properties that are returned in a **GetItem** response vary based on the requested shape, requested additional properties, and the type of item returned.</span></span> 
  
<span data-ttu-id="68c64-109">[Message](message-ex15websvcsotherref.md)要素は、電子メールメッセージと、Exchange Web サービス (EWS) スキーマで厳密に型指定されていないその他すべてのアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="68c64-109">[Message](message-ex15websvcsotherref.md) elements represent email messages and all other items that are not strongly typed by the Exchange Web Services (EWS) schema.</span></span> <span data-ttu-id="68c64-110">IPM などのアイテム。共有と IPM. InfoPath は、[メッセージ](message-ex15websvcsotherref.md)要素として返されます。</span><span class="sxs-lookup"><span data-stu-id="68c64-110">Items such as IPM.Sharing and IPM.InfoPath are returned as [Message](message-ex15websvcsotherref.md) elements.</span></span> <span data-ttu-id="68c64-111">Exchange は、応答で基本[Item](item.md)要素を返しません。</span><span class="sxs-lookup"><span data-stu-id="68c64-111">Exchange does not return the base [Item](item.md) element in responses.</span></span> 
  
<span data-ttu-id="68c64-112">**GetItem**操作では、添付ファイルは返されません。</span><span class="sxs-lookup"><span data-stu-id="68c64-112">The **GetItem** operation does not return attachments.</span></span> <span data-ttu-id="68c64-113">添付されているアイテムまたはファイルに関するメタデータを返します。</span><span class="sxs-lookup"><span data-stu-id="68c64-113">It does return metadata about an attached item or file.</span></span> <span data-ttu-id="68c64-114">添付ファイルを取得するには、 [getattachment 操作](getattachment-operation.md)を使用します。</span><span class="sxs-lookup"><span data-stu-id="68c64-114">To return an attachment, use the [GetAttachment operation](getattachment-operation.md).</span></span>
  
## <a name="getitem-operation-soap-headers"></a><span data-ttu-id="68c64-115">GetItem 操作 SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="68c64-115">GetItem operation SOAP headers</span></span>

<span data-ttu-id="68c64-116">**GetItem**操作では、次の表に示す SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="68c64-116">The **GetItem** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="68c64-117">ヘッダー \* \* \* \*</span><span class="sxs-lookup"><span data-stu-id="68c64-117">\*\*\*\*Header\*\*\*\*</span></span>|<span data-ttu-id="68c64-118">\*\*\*\*Element\*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="68c64-118">\*\*\*\*Element\*\*\*\*</span></span>|<span data-ttu-id="68c64-119">\*\*\*\*説明\*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="68c64-119">\*\*\*\*Description\*\*\*\*</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="68c64-120">**DateTimePrecision**</span><span class="sxs-lookup"><span data-stu-id="68c64-120">**DateTimePrecision**</span></span> <br/> |[<span data-ttu-id="68c64-121">DateTimePrecision</span><span class="sxs-lookup"><span data-stu-id="68c64-121">DateTimePrecision</span></span>](datetimeprecision.md) <br/> |<span data-ttu-id="68c64-122">サーバーからの応答におけるデータ/時刻値の解決方法を秒単位で指定します。またはミリ秒単位で指定します。</span><span class="sxs-lookup"><span data-stu-id="68c64-122">Specifies the resolution of data/time values in responses from the server, either in seconds or in milliseconds.</span></span>  <br/> |
|<span data-ttu-id="68c64-123">**偽装**</span><span class="sxs-lookup"><span data-stu-id="68c64-123">**Impersonation**</span></span> <br/> |[<span data-ttu-id="68c64-124">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="68c64-124">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="68c64-125">クライアントアプリケーションが偽装しているユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="68c64-125">Identifies the user whom the client application is impersonating.</span></span>  <br/> |
|<span data-ttu-id="68c64-126">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="68c64-126">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="68c64-127">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="68c64-127">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="68c64-128">RFC 3066 で定義されているように、メールボックスへのアクセスに使用されるカルチャ (言語の識別用のタグ) を識別します。</span><span class="sxs-lookup"><span data-stu-id="68c64-128">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span>  <br/> |
|<span data-ttu-id="68c64-129">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="68c64-129">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="68c64-130">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="68c64-130">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="68c64-131">操作要求のスキーマバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="68c64-131">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="68c64-132">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="68c64-132">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="68c64-133">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="68c64-133">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="68c64-134">要求に応答したサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="68c64-134">Identifies the version of the server that responded to the request.</span></span>  <br/> |
|<span data-ttu-id="68c64-135">**TimeZoneContext**</span><span class="sxs-lookup"><span data-stu-id="68c64-135">**TimeZoneContext**</span></span> <br/> |[<span data-ttu-id="68c64-136">TimeZoneContext</span><span class="sxs-lookup"><span data-stu-id="68c64-136">TimeZoneContext</span></span>](timezonecontext.md) <br/> |<span data-ttu-id="68c64-137">サーバーからのすべての応答に使用するタイムゾーンを指定します。</span><span class="sxs-lookup"><span data-stu-id="68c64-137">Identifies the time zone to be used for all responses from the server.</span></span>  <br/> |
   
## <a name="in-this-section"></a><span data-ttu-id="68c64-138">このセクションの内容</span><span class="sxs-lookup"><span data-stu-id="68c64-138">In This Section</span></span>

[<span data-ttu-id="68c64-139">GetItem 操作 (電子メールメッセージ)</span><span class="sxs-lookup"><span data-stu-id="68c64-139">GetItem operation (email message)</span></span>](getitem-operation-email-message.md)
  
[<span data-ttu-id="68c64-140">GetItem 操作 (予定表アイテム)</span><span class="sxs-lookup"><span data-stu-id="68c64-140">GetItem operation (calendar item)</span></span>](getitem-operation-calendar-item.md)
  
[<span data-ttu-id="68c64-141">GetItem 操作 (タスク)</span><span class="sxs-lookup"><span data-stu-id="68c64-141">GetItem operation (task)</span></span>](getitem-operation-task.md)
  
[<span data-ttu-id="68c64-142">GetItem 操作 (連絡先)</span><span class="sxs-lookup"><span data-stu-id="68c64-142">GetItem operation (contact)</span></span>](getitem-operation-contact.md)
  
## <a name="see-also"></a><span data-ttu-id="68c64-143">関連項目</span><span class="sxs-lookup"><span data-stu-id="68c64-143">See also</span></span>



[<span data-ttu-id="68c64-144">Exchange 用 EWS リファレンス</span><span class="sxs-lookup"><span data-stu-id="68c64-144">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)

