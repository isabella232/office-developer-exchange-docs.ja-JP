---
title: InternetMessageHeader
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- InternetMessageHeader
api_type:
- schema
ms.assetid: c70675f8-6feb-4c89-ba48-bce0479b308b
description: InternetMessageHeader 要素は、ヘッダーコレクション内の指定されたヘッダーのインターネットメッセージヘッダーを表します。 インターネットメッセージヘッダーのコレクション全体を取得するには、PR_TRANSPORT_MESSAGE_HEADERS プロパティを使用します。 EWS およびインターネットメッセージヘッダーの詳細については、「EWS、MIME、および不足しているインターネットメッセージヘッダーのインターネットメッセージヘッダーを取得する」を参照してください。
ms.openlocfilehash: 7b662617e0b1a1fcdcce3449b729485ba6e0956b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459308"
---
# <a name="internetmessageheader"></a><span data-ttu-id="84c1b-105">InternetMessageHeader</span><span class="sxs-lookup"><span data-stu-id="84c1b-105">InternetMessageHeader</span></span>

<span data-ttu-id="84c1b-106">**Internetmessageheader**要素は、ヘッダーコレクション内の指定されたヘッダーのインターネットメッセージヘッダーを表します。</span><span class="sxs-lookup"><span data-stu-id="84c1b-106">The **InternetMessageHeader** element represents the Internet message header for a given header within the headers collection.</span></span> <span data-ttu-id="84c1b-107">インターネットメッセージヘッダーのコレクション全体を取得するには、 **PR_TRANSPORT_MESSAGE_HEADERS**プロパティを使用します。</span><span class="sxs-lookup"><span data-stu-id="84c1b-107">To get the entire collection of Internet message headers, use the **PR_TRANSPORT_MESSAGE_HEADERS** property.</span></span> <span data-ttu-id="84c1b-108">EWS およびインターネットメッセージヘッダーの詳細については、「 [ews、MIME、および不足しているインターネットメッセージ](https://msdn.microsoft.com/library/exchange/hh545614%28v=exchg.140%29.aspx)ヘッダーのインターネットメッセージヘッダーを取得する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="84c1b-108">For more information about EWS and Internet message headers, see "Getting Internet message headers in [EWS, MIME, and the missing Internet message headers](https://msdn.microsoft.com/library/exchange/hh545614%28v=exchg.140%29.aspx).</span></span>
  
```XML
<InternetMessageHeader HeaderName=""/>
```

 <span data-ttu-id="84c1b-109">**InternetHeaderType**</span><span class="sxs-lookup"><span data-stu-id="84c1b-109">**InternetHeaderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="84c1b-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="84c1b-110">Attributes and elements</span></span>

<span data-ttu-id="84c1b-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="84c1b-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="84c1b-112">属性</span><span class="sxs-lookup"><span data-stu-id="84c1b-112">Attributes</span></span>

|<span data-ttu-id="84c1b-113">**属性**</span><span class="sxs-lookup"><span data-stu-id="84c1b-113">**Attribute**</span></span>|<span data-ttu-id="84c1b-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="84c1b-114">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="84c1b-115">**ヘッド Ername**</span><span class="sxs-lookup"><span data-stu-id="84c1b-115">**HeaderName**</span></span> <br/> |<span data-ttu-id="84c1b-116">ヘッダー名を識別します。</span><span class="sxs-lookup"><span data-stu-id="84c1b-116">Identifies the header name.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="84c1b-117">子要素</span><span class="sxs-lookup"><span data-stu-id="84c1b-117">Child elements</span></span>

<span data-ttu-id="84c1b-118">なし。</span><span class="sxs-lookup"><span data-stu-id="84c1b-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="84c1b-119">親要素</span><span class="sxs-lookup"><span data-stu-id="84c1b-119">Parent elements</span></span>

|<span data-ttu-id="84c1b-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="84c1b-120">**Element**</span></span>|<span data-ttu-id="84c1b-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="84c1b-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="84c1b-122">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="84c1b-122">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="84c1b-123">メールボックス内のアイテムに含まれるすべてのインターネットメッセージヘッダーのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="84c1b-123">Represents the collection of all Internet message headers that are contained in an item in a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="84c1b-124">テキスト値</span><span class="sxs-lookup"><span data-stu-id="84c1b-124">Text value</span></span>

<span data-ttu-id="84c1b-125">Text 値は、ヘッダーの値を表します。</span><span class="sxs-lookup"><span data-stu-id="84c1b-125">The text value represents the value for the header.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="84c1b-126">注釈</span><span class="sxs-lookup"><span data-stu-id="84c1b-126">Remarks</span></span>

<span data-ttu-id="84c1b-127">**PR_TRANSPORT_MESSAGE_HEADERS**プロパティの EWS マネージ API 拡張プロパティの定義を次に示します。</span><span class="sxs-lookup"><span data-stu-id="84c1b-127">The following is the EWS Managed API extended property definition for the **PR_TRANSPORT_MESSAGE_HEADERS** property.</span></span> 
  
```cs
ExtendedPropertyDefinition transportMsgHdr = new ExtendedPropertyDefinition(0x007D, MapiPropertyType.String);
```

<span data-ttu-id="84c1b-128">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="84c1b-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="84c1b-129">要素の情報</span><span class="sxs-lookup"><span data-stu-id="84c1b-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="84c1b-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="84c1b-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="84c1b-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="84c1b-131">Schema Name</span></span>  <br/> |<span data-ttu-id="84c1b-132">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="84c1b-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="84c1b-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="84c1b-133">Validation File</span></span>  <br/> |<span data-ttu-id="84c1b-134">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="84c1b-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="84c1b-135">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="84c1b-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="84c1b-136">正しくない</span><span class="sxs-lookup"><span data-stu-id="84c1b-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="84c1b-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="84c1b-137">See also</span></span>



- [<span data-ttu-id="84c1b-138">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="84c1b-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="84c1b-139">EWS、MIME、および欠落しているインターネット メッセージ ヘッダー</span><span class="sxs-lookup"><span data-stu-id="84c1b-139">EWS, MIME, and the missing Internet message headers</span></span>](https://msdn.microsoft.com/library/exchange/hh545614%28v=exchg.140%29.aspx)

