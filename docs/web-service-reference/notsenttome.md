---
title: NotSentToMe
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NotSentToMe
api_type:
- schema
ms.assetid: 7cb63269-622c-4198-9a21-f5a021bf6901
description: NotSentToMe 要素は、条件または例外を適用するために、メールボックスの所有者が受信メッセージの Tor プロパティにない必要があるかどうかを示します。
ms.openlocfilehash: 58efe4381fe0c9f5bd0645a9eba471a13b5e4064
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462613"
---
# <a name="notsenttome"></a><span data-ttu-id="1585e-103">NotSentToMe</span><span class="sxs-lookup"><span data-stu-id="1585e-103">NotSentToMe</span></span>

<span data-ttu-id="1585e-104">**NotSentToMe**要素は、条件または例外を適用するために、メールボックスの所有者が受信メッセージの**tor**プロパティにない必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1585e-104">The **NotSentToMe** element indicates whether the owner of the mailbox must not be in the **ToRecipients** property of the incoming messages in order for the condition or exception to apply.</span></span> 
  
```xml
<NotSentToMe>true | false</NotSentToMe>
```

 <span data-ttu-id="1585e-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="1585e-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1585e-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="1585e-106">Attributes and elements</span></span>

<span data-ttu-id="1585e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1585e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1585e-108">属性</span><span class="sxs-lookup"><span data-stu-id="1585e-108">Attributes</span></span>

<span data-ttu-id="1585e-109">なし。</span><span class="sxs-lookup"><span data-stu-id="1585e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1585e-110">子要素</span><span class="sxs-lookup"><span data-stu-id="1585e-110">Child elements</span></span>

<span data-ttu-id="1585e-111">なし。</span><span class="sxs-lookup"><span data-stu-id="1585e-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1585e-112">親要素</span><span class="sxs-lookup"><span data-stu-id="1585e-112">Parent elements</span></span>

|<span data-ttu-id="1585e-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="1585e-113">**Element**</span></span>|<span data-ttu-id="1585e-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="1585e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1585e-115">条件</span><span class="sxs-lookup"><span data-stu-id="1585e-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="1585e-116">ルールのルールの処理を開始するときに実行される条件を表します。</span><span class="sxs-lookup"><span data-stu-id="1585e-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="1585e-117">例外</span><span class="sxs-lookup"><span data-stu-id="1585e-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="1585e-118">受信トレイルールに対して使用可能なルールの例外条件をすべて表す例外を表します。</span><span class="sxs-lookup"><span data-stu-id="1585e-118">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1585e-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="1585e-119">Text value</span></span>

<span data-ttu-id="1585e-120">テキスト値が**true の場合**は、条件または例外を適用するために、メールボックスの所有者が受信メッセージの**トーラス**プロパティに含まれていてはならないことを示します。</span><span class="sxs-lookup"><span data-stu-id="1585e-120">A text value of **true** indicates that the owner of the mailbox must not be in the **ToRecipients** property of the incoming messages in order for the condition or exception to apply.</span></span> <span data-ttu-id="1585e-121">値が**false**の場合は、条件または例外を適用するために、メールボックスの所有者が受信メッセージの**torecipients**プロパティにある必要があることを示します。</span><span class="sxs-lookup"><span data-stu-id="1585e-121">A value of **false** indicates that the owner of the mailbox must be in the **ToRecipients** property of the incoming message in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="1585e-122">注釈</span><span class="sxs-lookup"><span data-stu-id="1585e-122">Remarks</span></span>

<span data-ttu-id="1585e-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="1585e-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1585e-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="1585e-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1585e-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="1585e-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1585e-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1585e-126">Schema Name</span></span>  <br/> |<span data-ttu-id="1585e-127">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="1585e-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1585e-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1585e-128">Validation File</span></span>  <br/> |<span data-ttu-id="1585e-129">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="1585e-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1585e-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="1585e-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="1585e-131">正しい</span><span class="sxs-lookup"><span data-stu-id="1585e-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1585e-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="1585e-132">See also</span></span>



- [<span data-ttu-id="1585e-133">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="1585e-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

