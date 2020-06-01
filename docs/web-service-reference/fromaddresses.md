---
title: FromAddresses
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FromAddresses
api_type:
- schema
ms.assetid: b219f315-c20a-4633-af3e-94bd3e4526b6
description: FromAddresses 要素は、条件または例外を適用するために、受信メッセージを送信する必要がある電子メールアドレスを示します。
ms.openlocfilehash: 4fbb44d02f5010c4395cf691cb6160da4dbb6930
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459540"
---
# <a name="fromaddresses"></a><span data-ttu-id="90c3d-103">FromAddresses</span><span class="sxs-lookup"><span data-stu-id="90c3d-103">FromAddresses</span></span>

<span data-ttu-id="90c3d-104">**Fromaddresses**要素は、条件または例外を適用するために、受信メッセージを送信する必要がある電子メールアドレスを示します。</span><span class="sxs-lookup"><span data-stu-id="90c3d-104">The **FromAddresses** element indicates the e-mail addresses from which incoming messages must be sent in order for the condition or exception to apply.</span></span> 
  
```XML
<FromAddresses>
   <Address/>
</FromAddresses>
```

 <span data-ttu-id="90c3d-105">**ArrayOfEmailAddressesType**</span><span class="sxs-lookup"><span data-stu-id="90c3d-105">**ArrayOfEmailAddressesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="90c3d-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="90c3d-106">Attributes and elements</span></span>

<span data-ttu-id="90c3d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="90c3d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="90c3d-108">属性</span><span class="sxs-lookup"><span data-stu-id="90c3d-108">Attributes</span></span>

<span data-ttu-id="90c3d-109">なし。</span><span class="sxs-lookup"><span data-stu-id="90c3d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="90c3d-110">子要素</span><span class="sxs-lookup"><span data-stu-id="90c3d-110">Child elements</span></span>

|<span data-ttu-id="90c3d-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="90c3d-111">**Element**</span></span>|<span data-ttu-id="90c3d-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="90c3d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="90c3d-113">Address (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="90c3d-113">Address (EmailAddressType)</span></span>](address-emailaddresstype.md) <br/> |<span data-ttu-id="90c3d-114">完全に解決された電子メールアドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="90c3d-114">Represents a fully resolved e-mail address.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="90c3d-115">親要素</span><span class="sxs-lookup"><span data-stu-id="90c3d-115">Parent elements</span></span>

|<span data-ttu-id="90c3d-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="90c3d-116">**Element**</span></span>|<span data-ttu-id="90c3d-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="90c3d-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="90c3d-118">条件</span><span class="sxs-lookup"><span data-stu-id="90c3d-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="90c3d-119">ルールのルールの処理を開始するときに実行される条件を表します。</span><span class="sxs-lookup"><span data-stu-id="90c3d-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="90c3d-120">例外</span><span class="sxs-lookup"><span data-stu-id="90c3d-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="90c3d-121">受信トレイルールに対して使用可能なすべてのルールの例外条件を表します。</span><span class="sxs-lookup"><span data-stu-id="90c3d-121">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="90c3d-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="90c3d-122">Text value</span></span>

<span data-ttu-id="90c3d-123">なし。</span><span class="sxs-lookup"><span data-stu-id="90c3d-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="90c3d-124">注釈</span><span class="sxs-lookup"><span data-stu-id="90c3d-124">Remarks</span></span>

<span data-ttu-id="90c3d-125">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="90c3d-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="90c3d-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="90c3d-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="90c3d-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="90c3d-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="90c3d-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="90c3d-128">Schema Name</span></span>  <br/> |<span data-ttu-id="90c3d-129">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="90c3d-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="90c3d-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="90c3d-130">Validation File</span></span>  <br/> |<span data-ttu-id="90c3d-131">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="90c3d-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="90c3d-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="90c3d-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="90c3d-133">正しい</span><span class="sxs-lookup"><span data-stu-id="90c3d-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="90c3d-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="90c3d-134">See also</span></span>



- [<span data-ttu-id="90c3d-135">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="90c3d-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

