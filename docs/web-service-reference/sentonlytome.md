---
title: SentOnlyToMe
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SentOnlyToMe
api_type:
- schema
ms.assetid: b6d4dea5-812d-4b29-917d-071ebd7ddd92
description: SentOnlyToMe 要素は、メールボックスの所有者が ToRecipients プロパティを適用する場合の条件または例外の順序で受信メッセージの 1 つだけにするかどうかを示します。
ms.openlocfilehash: 91c31069652a35dc7a38ad6b6e1512cc07d67a98
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833353"
---
# <a name="sentonlytome"></a><span data-ttu-id="9951b-103">SentOnlyToMe</span><span class="sxs-lookup"><span data-stu-id="9951b-103">SentOnlyToMe</span></span>

<span data-ttu-id="9951b-104">**SentOnlyToMe**要素は、メールボックスの所有者が**ToRecipients**プロパティを適用する場合の条件または例外の順序で受信メッセージの 1 つだけにするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9951b-104">The **SentOnlyToMe** element indicates whether the owner of the mailbox has to be the only one in the **ToRecipients** property of incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<SentOnlyToMe/>true | false</SentOnlyToMe>
```

 <span data-ttu-id="9951b-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="9951b-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9951b-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="9951b-106">Attributes and elements</span></span>

<span data-ttu-id="9951b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9951b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9951b-108">属性</span><span class="sxs-lookup"><span data-stu-id="9951b-108">Attributes</span></span>

<span data-ttu-id="9951b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9951b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9951b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9951b-110">Child elements</span></span>

<span data-ttu-id="9951b-111">なし。</span><span class="sxs-lookup"><span data-stu-id="9951b-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9951b-112">親要素</span><span class="sxs-lookup"><span data-stu-id="9951b-112">Parent elements</span></span>

|<span data-ttu-id="9951b-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="9951b-113">**Element**</span></span>|<span data-ttu-id="9951b-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="9951b-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9951b-115">条件</span><span class="sxs-lookup"><span data-stu-id="9951b-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="9951b-116">条件を表しますが、満たされるとときに、ルールのルールの処理をトリガーします。</span><span class="sxs-lookup"><span data-stu-id="9951b-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="9951b-117">Exceptions</span><span class="sxs-lookup"><span data-stu-id="9951b-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="9951b-118">受信トレイ ルールの使用可能なルールの例外条件をすべてを表します。</span><span class="sxs-lookup"><span data-stu-id="9951b-118">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9951b-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="9951b-119">Text value</span></span>

<span data-ttu-id="9951b-120">**True**の場合、テキスト値は、メールボックスの所有者は**ToRecipients**プロパティを適用する場合の条件または例外の順序で受信メッセージの 1 つのみである必要があることを示します。</span><span class="sxs-lookup"><span data-stu-id="9951b-120">A text value of **true** indicates that the owner of the mailbox must be the only one in the **ToRecipients** property of the incoming messages in order for the condition or exception to apply.</span></span> <span data-ttu-id="9951b-121">**False**の値では、メールボックスの所有者では、 **ToRecipients**プロパティを適用する場合の条件または例外の順序で受信メッセージの 1 つにしかならないということを示します。</span><span class="sxs-lookup"><span data-stu-id="9951b-121">A value of **false** indicates that the owner of the mailbox must not be the only one in the **ToRecipients** property of the incoming messages in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="9951b-122">備考</span><span class="sxs-lookup"><span data-stu-id="9951b-122">Remarks</span></span>

<span data-ttu-id="9951b-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="9951b-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9951b-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="9951b-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9951b-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="9951b-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9951b-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9951b-126">Schema Name</span></span>  <br/> |<span data-ttu-id="9951b-127">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="9951b-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9951b-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9951b-128">Validation File</span></span>  <br/> |<span data-ttu-id="9951b-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9951b-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9951b-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="9951b-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="9951b-131">True</span><span class="sxs-lookup"><span data-stu-id="9951b-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9951b-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="9951b-132">See also</span></span>



- [<span data-ttu-id="9951b-133">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="9951b-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

