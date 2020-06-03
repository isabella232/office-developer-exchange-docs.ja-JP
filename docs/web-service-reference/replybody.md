---
title: ReplyBody
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ReplyBody
api_type:
- schema
ms.assetid: bb184144-3e4b-4419-a883-cc9fab1085e6
description: ReplyBody 要素には、不在 (OOF) メッセージと、メッセージに使用する言語が含まれています。
ms.openlocfilehash: 496d336d1f87d9ea493ba7da362eef5a416fd899
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465304"
---
# <a name="replybody"></a><span data-ttu-id="c7972-103">ReplyBody</span><span class="sxs-lookup"><span data-stu-id="c7972-103">ReplyBody</span></span>

<span data-ttu-id="c7972-104">**ReplyBody**要素には、不在 (OOF) メッセージと、メッセージに使用する言語が含まれています。</span><span class="sxs-lookup"><span data-stu-id="c7972-104">The **ReplyBody** element contains an Out of Office (OOF) message and the language used for the message.</span></span> 
  
```XML
<ReplyBody xml:lang="">
   <Message/>
</ReplyBody>
```

 <span data-ttu-id="c7972-105">**ReplyBody**</span><span class="sxs-lookup"><span data-stu-id="c7972-105">**ReplyBody**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c7972-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="c7972-106">Attributes and elements</span></span>

<span data-ttu-id="c7972-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c7972-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c7972-108">属性</span><span class="sxs-lookup"><span data-stu-id="c7972-108">Attributes</span></span>

|<span data-ttu-id="c7972-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="c7972-109">**Attribute**</span></span>|<span data-ttu-id="c7972-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="c7972-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c7972-111">xml: lang</span><span class="sxs-lookup"><span data-stu-id="c7972-111">xml:lang</span></span>  <br/> |<span data-ttu-id="c7972-112">**ReplyBody**の内容で使用する言語を指定します。</span><span class="sxs-lookup"><span data-stu-id="c7972-112">Specifies the language used in the **ReplyBody** contents.</span></span> <span data-ttu-id="c7972-113">この属性は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="c7972-113">This attribute is optional.</span></span> <span data-ttu-id="c7972-114">この属性に指定できる値は、IETF RFC 3066 で定義されています。</span><span class="sxs-lookup"><span data-stu-id="c7972-114">The possible values of this attribute are defined by IETF RFC 3066.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="c7972-115">子要素</span><span class="sxs-lookup"><span data-stu-id="c7972-115">Child elements</span></span>

|<span data-ttu-id="c7972-116">**Element**</span><span class="sxs-lookup"><span data-stu-id="c7972-116">**Element**</span></span>|<span data-ttu-id="c7972-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="c7972-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c7972-118">メッセージ (可用性)</span><span class="sxs-lookup"><span data-stu-id="c7972-118">Message (Availability)</span></span>](message-availability.md) <br/> |<span data-ttu-id="c7972-119">不在 (OOF) 応答を含みます。</span><span class="sxs-lookup"><span data-stu-id="c7972-119">Contains the out of office (OOF) response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c7972-120">親要素</span><span class="sxs-lookup"><span data-stu-id="c7972-120">Parent elements</span></span>

|<span data-ttu-id="c7972-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="c7972-121">**Element**</span></span>|<span data-ttu-id="c7972-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="c7972-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c7972-123">不在</span><span class="sxs-lookup"><span data-stu-id="c7972-123">OutOfOffice</span></span>](outofoffice.md) <br/> |<span data-ttu-id="c7972-124">OOF 応答メッセージと、メールボックスの応答メッセージを送信するための時間を定義します。</span><span class="sxs-lookup"><span data-stu-id="c7972-124">Defines the OOF response message and a duration time for sending the response message for a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c7972-125">テキスト値</span><span class="sxs-lookup"><span data-stu-id="c7972-125">Text value</span></span>

<span data-ttu-id="c7972-126">なし。</span><span class="sxs-lookup"><span data-stu-id="c7972-126">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c7972-127">注釈</span><span class="sxs-lookup"><span data-stu-id="c7972-127">Remarks</span></span>

<span data-ttu-id="c7972-128">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="c7972-128">This element is required.</span></span>
  
<span data-ttu-id="c7972-129">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="c7972-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c7972-130">要素の情報</span><span class="sxs-lookup"><span data-stu-id="c7972-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c7972-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="c7972-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c7972-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c7972-132">Schema Name</span></span>  <br/> |<span data-ttu-id="c7972-133">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="c7972-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="c7972-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c7972-134">Validation File</span></span>  <br/> |<span data-ttu-id="c7972-135">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="c7972-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c7972-136">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="c7972-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="c7972-137">正しくない</span><span class="sxs-lookup"><span data-stu-id="c7972-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c7972-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="c7972-138">See also</span></span>



- [<span data-ttu-id="c7972-139">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="c7972-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

