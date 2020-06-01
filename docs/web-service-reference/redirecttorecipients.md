---
title: RedirectToRecipients
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RedirectToRecipients
api_type:
- schema
ms.assetid: 00ef4a84-76d2-4669-b597-f52abbbc34f5
description: RedirectToRecipients 要素は、メッセージがリダイレクトされる電子メールアドレスを示します。
ms.openlocfilehash: ebc0e0abe88d1e364dee94cc24313879458778d0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462193"
---
# <a name="redirecttorecipients"></a><span data-ttu-id="3e177-103">RedirectToRecipients</span><span class="sxs-lookup"><span data-stu-id="3e177-103">RedirectToRecipients</span></span>

<span data-ttu-id="3e177-104">**Redirecttorecipients**要素は、メッセージがリダイレクトされる電子メールアドレスを示します。</span><span class="sxs-lookup"><span data-stu-id="3e177-104">The **RedirectToRecipients** element indicates the e-mail addresses to which messages are to be redirected.</span></span> 
  
```XML
<RedirectToRecipients>
   <Address/>
</RedirectToRecipients>
```

 <span data-ttu-id="3e177-105">**ArrayOfEmailAddressesType**</span><span class="sxs-lookup"><span data-stu-id="3e177-105">**ArrayOfEmailAddressesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3e177-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="3e177-106">Attributes and elements</span></span>

<span data-ttu-id="3e177-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3e177-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3e177-108">属性</span><span class="sxs-lookup"><span data-stu-id="3e177-108">Attributes</span></span>

<span data-ttu-id="3e177-109">なし。</span><span class="sxs-lookup"><span data-stu-id="3e177-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3e177-110">子要素</span><span class="sxs-lookup"><span data-stu-id="3e177-110">Child elements</span></span>

|<span data-ttu-id="3e177-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="3e177-111">**Element**</span></span>|<span data-ttu-id="3e177-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="3e177-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3e177-113">Address (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="3e177-113">Address (EmailAddressType)</span></span>](address-emailaddresstype.md) <br/> |<span data-ttu-id="3e177-114">完全に解決された電子メールアドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="3e177-114">Represents a fully resolved e-mail address.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3e177-115">親要素</span><span class="sxs-lookup"><span data-stu-id="3e177-115">Parent elements</span></span>

|<span data-ttu-id="3e177-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="3e177-116">**Element**</span></span>|<span data-ttu-id="3e177-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="3e177-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3e177-118">Actions</span><span class="sxs-lookup"><span data-stu-id="3e177-118">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="3e177-119">条件が満たされたときに、メッセージに対して実行できるアクションのセットを表します。</span><span class="sxs-lookup"><span data-stu-id="3e177-119">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3e177-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="3e177-120">Text value</span></span>

<span data-ttu-id="3e177-121">なし。</span><span class="sxs-lookup"><span data-stu-id="3e177-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3e177-122">注釈</span><span class="sxs-lookup"><span data-stu-id="3e177-122">Remarks</span></span>

<span data-ttu-id="3e177-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="3e177-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3e177-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="3e177-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3e177-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="3e177-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3e177-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3e177-126">Schema Name</span></span>  <br/> |<span data-ttu-id="3e177-127">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="3e177-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3e177-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3e177-128">Validation File</span></span>  <br/> |<span data-ttu-id="3e177-129">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="3e177-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3e177-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="3e177-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="3e177-131">正しい</span><span class="sxs-lookup"><span data-stu-id="3e177-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3e177-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="3e177-132">See also</span></span>



- [<span data-ttu-id="3e177-133">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="3e177-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

