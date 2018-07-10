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
description: InternetMessageHeader 要素は、ヘッダー コレクション内の指定したヘッダーのインターネット メッセージ ヘッダーを表します。 インターネット メッセージ ヘッダーのコレクション全体を取得するには、PR_TRANSPORT_MESSAGE_HEADERS プロパティを使用します。 EWS およびインターネット メッセージ ヘッダーの詳細については、EWS、MIME、および不足しているインターネットの seeGetting のインターネット メッセージ ヘッダー メッセージ ヘッダーを使用します。
ms.openlocfilehash: 9457cdabe99c0adcb8183cbc039cc86db881fec7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831952"
---
# <a name="internetmessageheader"></a><span data-ttu-id="7994c-105">InternetMessageHeader</span><span class="sxs-lookup"><span data-stu-id="7994c-105">InternetMessageHeader</span></span>

<span data-ttu-id="7994c-106">**InternetMessageHeader**要素は、ヘッダー コレクション内の指定したヘッダーのインターネット メッセージ ヘッダーを表します。</span><span class="sxs-lookup"><span data-stu-id="7994c-106">The **InternetMessageHeader** element represents the Internet message header for a given header within the headers collection.</span></span> <span data-ttu-id="7994c-107">インターネット メッセージ ヘッダーのコレクション全体を取得するには、 **PR_TRANSPORT_MESSAGE_HEADERS**プロパティを使用します。</span><span class="sxs-lookup"><span data-stu-id="7994c-107">To get the entire collection of Internet message headers, use the **PR_TRANSPORT_MESSAGE_HEADERS** property.</span></span> <span data-ttu-id="7994c-108">EWS およびインターネット メッセージ ヘッダーの詳細についてを参照してください["EWS、MIME、および不足しているインターネット メッセージ ヘッダー](http://msdn.microsoft.com/ja-jp/library/exchange/hh545614%28v=exchg.140%29.aspx)の取得インターネット メッセージのヘッダーです。</span><span class="sxs-lookup"><span data-stu-id="7994c-108">For more information about EWS and Internet message headers, see "Getting Internet message headers in [EWS, MIME, and the missing Internet message headers](http://msdn.microsoft.com/ja-jp/library/exchange/hh545614%28v=exchg.140%29.aspx).</span></span>
  
```XML
<InternetMessageHeader HeaderName=""/>
```

 <span data-ttu-id="7994c-109">**InternetHeaderType**</span><span class="sxs-lookup"><span data-stu-id="7994c-109">**InternetHeaderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7994c-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="7994c-110">Attributes and elements</span></span>

<span data-ttu-id="7994c-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7994c-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7994c-112">属性</span><span class="sxs-lookup"><span data-stu-id="7994c-112">Attributes</span></span>

|<span data-ttu-id="7994c-113">**属性**</span><span class="sxs-lookup"><span data-stu-id="7994c-113">**Attribute**</span></span>|<span data-ttu-id="7994c-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="7994c-114">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7994c-115">**HeaderName**</span><span class="sxs-lookup"><span data-stu-id="7994c-115">**HeaderName**</span></span> <br/> |<span data-ttu-id="7994c-116">ヘッダー名を識別します。</span><span class="sxs-lookup"><span data-stu-id="7994c-116">Identifies the header name.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="7994c-117">子要素</span><span class="sxs-lookup"><span data-stu-id="7994c-117">Child elements</span></span>

<span data-ttu-id="7994c-118">なし。</span><span class="sxs-lookup"><span data-stu-id="7994c-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7994c-119">親要素</span><span class="sxs-lookup"><span data-stu-id="7994c-119">Parent elements</span></span>

|<span data-ttu-id="7994c-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="7994c-120">**Element**</span></span>|<span data-ttu-id="7994c-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="7994c-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7994c-122">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="7994c-122">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="7994c-123">メールボックス内のアイテムに含まれるすべてのインターネット メッセージ ヘッダーのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="7994c-123">Represents the collection of all Internet message headers that are contained in an item in a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7994c-124">テキスト値</span><span class="sxs-lookup"><span data-stu-id="7994c-124">Text value</span></span>

<span data-ttu-id="7994c-125">テキスト値は、ヘッダーの値を表します。</span><span class="sxs-lookup"><span data-stu-id="7994c-125">The text value represents the value for the header.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7994c-126">備考</span><span class="sxs-lookup"><span data-stu-id="7994c-126">Remarks</span></span>

<span data-ttu-id="7994c-127">**PR_TRANSPORT_MESSAGE_HEADERS**プロパティのプロパティの定義を拡張する EWS マネージ API は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="7994c-127">The following is the EWS Managed API extended property definition for the **PR_TRANSPORT_MESSAGE_HEADERS** property.</span></span> 
  
```cs
ExtendedPropertyDefinition transportMsgHdr = new ExtendedPropertyDefinition(0x007D, MapiPropertyType.String);
```

<span data-ttu-id="7994c-128">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="7994c-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7994c-129">要素情報</span><span class="sxs-lookup"><span data-stu-id="7994c-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7994c-130">名前空間</span><span class="sxs-lookup"><span data-stu-id="7994c-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7994c-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7994c-131">Schema Name</span></span>  <br/> |<span data-ttu-id="7994c-132">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="7994c-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="7994c-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7994c-133">Validation File</span></span>  <br/> |<span data-ttu-id="7994c-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7994c-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7994c-135">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="7994c-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="7994c-136">False</span><span class="sxs-lookup"><span data-stu-id="7994c-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7994c-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="7994c-137">See also</span></span>



- [<span data-ttu-id="7994c-138">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="7994c-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="7994c-139">EWS、MIME、および不足しているインターネット メッセージのヘッダー</span><span class="sxs-lookup"><span data-stu-id="7994c-139">EWS, MIME, and the missing Internet message headers</span></span>](http://msdn.microsoft.com/ja-jp/library/exchange/hh545614%28v=exchg.140%29.aspx)

