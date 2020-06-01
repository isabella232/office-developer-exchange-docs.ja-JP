---
title: 住所
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SentToAddresses
api_type:
- schema
ms.assetid: 086130d2-93b1-4de1-9553-10ec10322a0c
description: 送信 Toaddresses 要素は、条件または例外を適用するために、受信メッセージが送信される必要のある電子メールアドレスを示します。
ms.openlocfilehash: 9a901a93b666144092bf9cc8ebbf03222ac7bf6b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457418"
---
# <a name="senttoaddresses"></a><span data-ttu-id="1a959-103">住所</span><span class="sxs-lookup"><span data-stu-id="1a959-103">SentToAddresses</span></span>

<span data-ttu-id="1a959-104">送信**Toaddresses**要素は、条件または例外を適用するために、受信メッセージが送信される必要のある電子メールアドレスを示します。</span><span class="sxs-lookup"><span data-stu-id="1a959-104">The **SentToAddresses** element indicates the e-mail addresses that incoming messages have to have been sent to in order for the condition or exception to apply.</span></span> 
  
```XML
<SentToAddresses>
   <Address/>
</SentToAddresses>
```

 <span data-ttu-id="1a959-105">**ArrayOfEmailAddressesType**</span><span class="sxs-lookup"><span data-stu-id="1a959-105">**ArrayOfEmailAddressesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1a959-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="1a959-106">Attributes and elements</span></span>

<span data-ttu-id="1a959-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1a959-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1a959-108">属性</span><span class="sxs-lookup"><span data-stu-id="1a959-108">Attributes</span></span>

<span data-ttu-id="1a959-109">なし。</span><span class="sxs-lookup"><span data-stu-id="1a959-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1a959-110">子要素</span><span class="sxs-lookup"><span data-stu-id="1a959-110">Child elements</span></span>

|<span data-ttu-id="1a959-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="1a959-111">**Element**</span></span>|<span data-ttu-id="1a959-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="1a959-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1a959-113">Address (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="1a959-113">Address (EmailAddressType)</span></span>](address-emailaddresstype.md) <br/> |<span data-ttu-id="1a959-114">完全に解決された電子メールアドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="1a959-114">Represents a fully resolved e-mail address.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1a959-115">親要素</span><span class="sxs-lookup"><span data-stu-id="1a959-115">Parent elements</span></span>

|<span data-ttu-id="1a959-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="1a959-116">**Element**</span></span>|<span data-ttu-id="1a959-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="1a959-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1a959-118">条件</span><span class="sxs-lookup"><span data-stu-id="1a959-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="1a959-119">ルールのルールの処理を開始するときに実行される条件を表します。</span><span class="sxs-lookup"><span data-stu-id="1a959-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="1a959-120">例外</span><span class="sxs-lookup"><span data-stu-id="1a959-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="1a959-121">受信トレイルールに対して使用可能なすべてのルールの例外条件を表します。</span><span class="sxs-lookup"><span data-stu-id="1a959-121">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1a959-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="1a959-122">Text value</span></span>

<span data-ttu-id="1a959-123">なし。</span><span class="sxs-lookup"><span data-stu-id="1a959-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1a959-124">注釈</span><span class="sxs-lookup"><span data-stu-id="1a959-124">Remarks</span></span>

<span data-ttu-id="1a959-125">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="1a959-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1a959-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="1a959-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1a959-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="1a959-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1a959-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1a959-128">Schema Name</span></span>  <br/> |<span data-ttu-id="1a959-129">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="1a959-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1a959-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1a959-130">Validation File</span></span>  <br/> |<span data-ttu-id="1a959-131">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="1a959-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1a959-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="1a959-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="1a959-133">正しい</span><span class="sxs-lookup"><span data-stu-id="1a959-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1a959-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="1a959-134">See also</span></span>



- [<span data-ttu-id="1a959-135">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="1a959-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

