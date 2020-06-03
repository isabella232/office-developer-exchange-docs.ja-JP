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
description: FromConnectedAccounts 要素は、条件または例外を適用するために、受信メッセージを集計しておく必要がある電子メールアカウント名を表します。
ms.openlocfilehash: 159ae064827c2f9c2b470580ad5457264e8dae93
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464050"
---
# <a name="fromconnectedaccounts"></a><span data-ttu-id="78079-103">FromConnectedAccounts</span><span class="sxs-lookup"><span data-stu-id="78079-103">FromConnectedAccounts</span></span>

<span data-ttu-id="78079-104">**Fromconnectedaccounts**要素は、条件または例外を適用するために、受信メッセージを集計しておく必要がある電子メールアカウント名を表します。</span><span class="sxs-lookup"><span data-stu-id="78079-104">The **FromConnectedAccounts** element represents the e-mail account names from which incoming messages have to have been aggregated in order for the condition or exception to apply.</span></span> 
  
```XML
<FromConnectedAccounts>
    <String/>
</FromConnectedAccounts>
```

 <span data-ttu-id="78079-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="78079-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="78079-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="78079-106">Attributes and elements</span></span>

<span data-ttu-id="78079-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="78079-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="78079-108">属性</span><span class="sxs-lookup"><span data-stu-id="78079-108">Attributes</span></span>

<span data-ttu-id="78079-109">なし。</span><span class="sxs-lookup"><span data-stu-id="78079-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="78079-110">子要素</span><span class="sxs-lookup"><span data-stu-id="78079-110">Child elements</span></span>

|<span data-ttu-id="78079-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="78079-111">**Element**</span></span>|<span data-ttu-id="78079-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="78079-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="78079-113">String</span><span class="sxs-lookup"><span data-stu-id="78079-113">String</span></span>](string.md) <br/> |<span data-ttu-id="78079-114">条件または例外を適用するために、受信メッセージを集計する必要がある電子メールアカウント名を表します。</span><span class="sxs-lookup"><span data-stu-id="78079-114">Represents an e-mail account name from which incoming messages have to have been aggregated in order for the condition or exception to apply.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="78079-115">親要素</span><span class="sxs-lookup"><span data-stu-id="78079-115">Parent elements</span></span>

|<span data-ttu-id="78079-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="78079-116">**Element**</span></span>|<span data-ttu-id="78079-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="78079-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="78079-118">条件</span><span class="sxs-lookup"><span data-stu-id="78079-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="78079-119">ルールのルールの処理を開始するときに実行される条件を表します。</span><span class="sxs-lookup"><span data-stu-id="78079-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="78079-120">例外</span><span class="sxs-lookup"><span data-stu-id="78079-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="78079-121">受信トレイルールに対して使用可能なルールの例外条件をすべて表す例外を表します。</span><span class="sxs-lookup"><span data-stu-id="78079-121">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="78079-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="78079-122">Text value</span></span>

<span data-ttu-id="78079-123">なし。</span><span class="sxs-lookup"><span data-stu-id="78079-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="78079-124">注釈</span><span class="sxs-lookup"><span data-stu-id="78079-124">Remarks</span></span>

<span data-ttu-id="78079-125">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="78079-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="78079-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="78079-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="78079-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="78079-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="78079-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="78079-128">Schema Name</span></span>  <br/> |<span data-ttu-id="78079-129">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="78079-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="78079-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="78079-130">Validation File</span></span>  <br/> |<span data-ttu-id="78079-131">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="78079-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="78079-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="78079-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="78079-133">正しい</span><span class="sxs-lookup"><span data-stu-id="78079-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="78079-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="78079-134">See also</span></span>



- [<span data-ttu-id="78079-135">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="78079-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

