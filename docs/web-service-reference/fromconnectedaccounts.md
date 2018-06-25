---
title: FromConnectedAccounts
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FromConnectedAccounts
api_type:
- schema
ms.assetid: d4d7ddd7-078d-4f1a-a26b-22dce0c49f3a
description: FromConnectedAccounts 要素は、受信メッセージの適用の条件または例外のために集められたを持つ必要がある電子メール アカウントの名前を表します。
ms.openlocfilehash: 426e81bbbe96fb5fb4b36506438dc4af4f560eef
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760604"
---
# <a name="fromconnectedaccounts"></a><span data-ttu-id="d41dc-103">FromConnectedAccounts</span><span class="sxs-lookup"><span data-stu-id="d41dc-103">FromConnectedAccounts</span></span>

<span data-ttu-id="d41dc-104">**FromConnectedAccounts**要素は、受信メッセージの適用の条件または例外のために集められたを持つ必要がある電子メール アカウントの名前を表します。</span><span class="sxs-lookup"><span data-stu-id="d41dc-104">The **FromConnectedAccounts** element represents the e-mail account names from which incoming messages have to have been aggregated in order for the condition or exception to apply.</span></span> 
  
```XML
<FromConnectedAccounts>
    <String/>
</FromConnectedAccounts>
```

 <span data-ttu-id="d41dc-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="d41dc-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d41dc-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="d41dc-106">Attributes and elements</span></span>

<span data-ttu-id="d41dc-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d41dc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d41dc-108">属性</span><span class="sxs-lookup"><span data-stu-id="d41dc-108">Attributes</span></span>

<span data-ttu-id="d41dc-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d41dc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d41dc-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d41dc-110">Child elements</span></span>

|<span data-ttu-id="d41dc-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="d41dc-111">**Element**</span></span>|<span data-ttu-id="d41dc-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="d41dc-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d41dc-113">String</span><span class="sxs-lookup"><span data-stu-id="d41dc-113">String</span></span>](string.md) <br/> |<span data-ttu-id="d41dc-114">受信メッセージの適用の条件または例外のために集められたを持つ必要がある電子メール アカウント名を表します。</span><span class="sxs-lookup"><span data-stu-id="d41dc-114">Represents an e-mail account name from which incoming messages have to have been aggregated in order for the condition or exception to apply.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d41dc-115">親要素</span><span class="sxs-lookup"><span data-stu-id="d41dc-115">Parent elements</span></span>

|<span data-ttu-id="d41dc-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="d41dc-116">**Element**</span></span>|<span data-ttu-id="d41dc-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="d41dc-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d41dc-118">条件</span><span class="sxs-lookup"><span data-stu-id="d41dc-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="d41dc-119">条件を表しますが、満たされるとときに、ルールのルールの処理をトリガーします。</span><span class="sxs-lookup"><span data-stu-id="d41dc-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="d41dc-120">Exceptions</span><span class="sxs-lookup"><span data-stu-id="d41dc-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="d41dc-121">受信トレイ ルールの使用可能なルールの例外条件をすべてを表す例外を表します。</span><span class="sxs-lookup"><span data-stu-id="d41dc-121">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d41dc-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="d41dc-122">Text value</span></span>

<span data-ttu-id="d41dc-123">なし。</span><span class="sxs-lookup"><span data-stu-id="d41dc-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d41dc-124">備考</span><span class="sxs-lookup"><span data-stu-id="d41dc-124">Remarks</span></span>

<span data-ttu-id="d41dc-125">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="d41dc-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d41dc-126">要素情報</span><span class="sxs-lookup"><span data-stu-id="d41dc-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d41dc-127">名前空間</span><span class="sxs-lookup"><span data-stu-id="d41dc-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d41dc-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d41dc-128">Schema Name</span></span>  <br/> |<span data-ttu-id="d41dc-129">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="d41dc-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d41dc-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d41dc-130">Validation File</span></span>  <br/> |<span data-ttu-id="d41dc-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d41dc-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d41dc-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d41dc-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="d41dc-133">True</span><span class="sxs-lookup"><span data-stu-id="d41dc-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d41dc-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="d41dc-134">See also</span></span>



- [<span data-ttu-id="d41dc-135">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="d41dc-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

