---
title: GetItem 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetItem
api_type:
- schema
ms.assetid: e3590b8b-c2a7-4dad-a014-6360197b68e4
description: 操作 GetItem EWS についての情報を検索します。
ms.openlocfilehash: 9b63032b2eaa3bf26027a42e38bfa06bedcbac86
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760776"
---
# <a name="getitem-operation"></a><span data-ttu-id="d3eea-103">GetItem 操作</span><span class="sxs-lookup"><span data-stu-id="d3eea-103">GetItem operation</span></span>

<span data-ttu-id="d3eea-104">**GetItem** EWS の操作に関する情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="d3eea-104">Find information about the **GetItem** EWS operation.</span></span> 
  
<span data-ttu-id="d3eea-105">**GetItem**操作は、Exchange ストアから項目を取得します。</span><span class="sxs-lookup"><span data-stu-id="d3eea-105">The **GetItem** operation gets items from the Exchange store.</span></span> 
  
## <a name="using-the-getitem-operation"></a><span data-ttu-id="d3eea-106">GetItem 操作を使用します。</span><span class="sxs-lookup"><span data-stu-id="d3eea-106">Using the GetItem operation</span></span>

<span data-ttu-id="d3eea-107">**GetItem**操作は、多くのアイテムのプロパティを返します。</span><span class="sxs-lookup"><span data-stu-id="d3eea-107">The **GetItem** operation returns many item properties.</span></span> <span data-ttu-id="d3eea-108">**GetItem**応答で返されるプロパティによって要求された図形を要求された追加のプロパティと項目の型が返されます。</span><span class="sxs-lookup"><span data-stu-id="d3eea-108">The properties that are returned in a **GetItem** response vary based on the requested shape, requested additional properties, and the type of item returned.</span></span> 
  
<span data-ttu-id="d3eea-109">[メッセージ](message-ex15websvcsotherref.md)要素は、電子メール メッセージ、Exchange Web サービス (EWS) スキーマが厳密に型指定されない他のすべての項目を表します。</span><span class="sxs-lookup"><span data-stu-id="d3eea-109">[Message](message-ex15websvcsotherref.md) elements represent email messages and all other items that are not strongly typed by the Exchange Web Services (EWS) schema.</span></span> <span data-ttu-id="d3eea-110">IPM などの項目です。共有し、IPM.InfoPath は、[メッセージ](message-ex15websvcsotherref.md)の要素として返されます。</span><span class="sxs-lookup"><span data-stu-id="d3eea-110">Items such as IPM.Sharing and IPM.InfoPath are returned as [Message](message-ex15websvcsotherref.md) elements.</span></span> <span data-ttu-id="d3eea-111">Exchange では、応答の基本要素の[項目](item.md)が返されません。</span><span class="sxs-lookup"><span data-stu-id="d3eea-111">Exchange does not return the base [Item](item.md) element in responses.</span></span> 
  
<span data-ttu-id="d3eea-112">**GetItem**操作では、添付ファイルは返されません。</span><span class="sxs-lookup"><span data-stu-id="d3eea-112">The **GetItem** operation does not return attachments.</span></span> <span data-ttu-id="d3eea-113">添付されたアイテムやファイルについてのメタデータを返すには。</span><span class="sxs-lookup"><span data-stu-id="d3eea-113">It does return metadata about an attached item or file.</span></span> <span data-ttu-id="d3eea-114">添付ファイルを取得するには、 [GetAttachment 操作](getattachment-operation.md)を使用します。</span><span class="sxs-lookup"><span data-stu-id="d3eea-114">To return an attachment, use the [GetAttachment operation](getattachment-operation.md).</span></span>
  
## <a name="getitem-operation-soap-headers"></a><span data-ttu-id="d3eea-115">GetItem 操作の SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d3eea-115">GetItem operation SOAP headers</span></span>

<span data-ttu-id="d3eea-116">**GetItem**操作は、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="d3eea-116">The **GetItem** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="d3eea-117">ヘッダー。</span><span class="sxs-lookup"><span data-stu-id="d3eea-117">****Header****</span></span>|<span data-ttu-id="d3eea-118">****Element****</span><span class="sxs-lookup"><span data-stu-id="d3eea-118">****Element****</span></span>|<span data-ttu-id="d3eea-119">****説明****</span><span class="sxs-lookup"><span data-stu-id="d3eea-119">****Description****</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="d3eea-120">**DateTimePrecision**</span><span class="sxs-lookup"><span data-stu-id="d3eea-120">**DateTimePrecision**</span></span> <br/> |[<span data-ttu-id="d3eea-121">DateTimePrecision</span><span class="sxs-lookup"><span data-stu-id="d3eea-121">DateTimePrecision</span></span>](datetimeprecision.md) <br/> |<span data-ttu-id="d3eea-122">秒またはミリ秒単位のいずれか、サーバーからの応答では、日付/時刻値の解像度を指定します。</span><span class="sxs-lookup"><span data-stu-id="d3eea-122">Specifies the resolution of data/time values in responses from the server, either in seconds or in milliseconds.</span></span>  <br/> |
|<span data-ttu-id="d3eea-123">**偽装**</span><span class="sxs-lookup"><span data-stu-id="d3eea-123">**Impersonation**</span></span> <br/> |[<span data-ttu-id="d3eea-124">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="d3eea-124">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="d3eea-125">クライアント アプリケーションが偽装するユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="d3eea-125">Identifies the user whom the client application is impersonating.</span></span>  <br/> |
|<span data-ttu-id="d3eea-126">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="d3eea-126">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="d3eea-127">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="d3eea-127">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="d3eea-128">RFC 3066、」タグの「識別の言語」を使用してメールボックスへのアクセスに定義されているカルチャを識別します。</span><span class="sxs-lookup"><span data-stu-id="d3eea-128">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span>  <br/> |
|<span data-ttu-id="d3eea-129">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="d3eea-129">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="d3eea-130">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="d3eea-130">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="d3eea-131">操作要求のスキーマのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="d3eea-131">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="d3eea-132">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="d3eea-132">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="d3eea-133">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="d3eea-133">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="d3eea-134">要求に応答するサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="d3eea-134">Identifies the version of the server that responded to the request.</span></span>  <br/> |
|<span data-ttu-id="d3eea-135">**TimeZoneContext**</span><span class="sxs-lookup"><span data-stu-id="d3eea-135">**TimeZoneContext**</span></span> <br/> |[<span data-ttu-id="d3eea-136">TimeZoneContext</span><span class="sxs-lookup"><span data-stu-id="d3eea-136">TimeZoneContext</span></span>](timezonecontext.md) <br/> |<span data-ttu-id="d3eea-137">サーバーからのすべての応答に使用するタイム ゾーンを識別します。</span><span class="sxs-lookup"><span data-stu-id="d3eea-137">Identifies the time zone to be used for all responses from the server.</span></span>  <br/> |
   
## <a name="in-this-section"></a><span data-ttu-id="d3eea-138">���̃Z�N�V�����̓�e</span><span class="sxs-lookup"><span data-stu-id="d3eea-138">In This Section</span></span>

[<span data-ttu-id="d3eea-139">GetItem 操作 (電子メール)</span><span class="sxs-lookup"><span data-stu-id="d3eea-139">GetItem operation (email message)</span></span>](getitem-operation-email-message.md)
  
[<span data-ttu-id="d3eea-140">GetItem 操作 (予定表アイテム)</span><span class="sxs-lookup"><span data-stu-id="d3eea-140">GetItem operation (calendar item)</span></span>](getitem-operation-calendar-item.md)
  
[<span data-ttu-id="d3eea-141">GetItem 操作 (タスク)</span><span class="sxs-lookup"><span data-stu-id="d3eea-141">GetItem operation (task)</span></span>](getitem-operation-task.md)
  
[<span data-ttu-id="d3eea-142">GetItem 操作 (連絡先)</span><span class="sxs-lookup"><span data-stu-id="d3eea-142">GetItem operation (contact)</span></span>](getitem-operation-contact.md)
  
## <a name="see-also"></a><span data-ttu-id="d3eea-143">関連項目</span><span class="sxs-lookup"><span data-stu-id="d3eea-143">See also</span></span>



<span data-ttu-id="d3eea-144">
  [Exchange 用 EWS リファレンス](ews-reference-for-exchange.md)</span><span class="sxs-lookup"><span data-stu-id="d3eea-144">[EWS reference for Exchange](ews-reference-for-exchange.md)</span></span>

