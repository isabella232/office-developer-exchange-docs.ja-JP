---
title: 「Orccme」
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SentToOrCcMe
api_type:
- schema
ms.assetid: ca43e05d-df37-485b-9276-34678025f2b7
description: 送信 Toorccme 要素は、条件または例外を適用するために、メールボックスの所有者が受信メッセージの ToRecipients または CcRecipients いずれかのプロパティに含まれている必要があるかどうかを示します。
ms.openlocfilehash: 906e5d9fd405b9aa6f772bcedbd1869b5023a05e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462081"
---
# <a name="senttoorccme"></a><span data-ttu-id="60c54-103">「Orccme」</span><span class="sxs-lookup"><span data-stu-id="60c54-103">SentToOrCcMe</span></span>

<span data-ttu-id="60c54-104">送信**Toorccme**要素は、条件または例外を適用するために、メールボックスの所有者が受信メッセージの**torecipients**または**ccrecipients**いずれかのプロパティに含まれている必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="60c54-104">The **SentToOrCcMe** element indicates whether the owner of the mailbox has to be in either a **ToRecipients** or **CcRecipients** property of incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<SentToOrCcMe>true | false</SentToOrCcMe>
```

 <span data-ttu-id="60c54-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="60c54-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="60c54-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="60c54-106">Attributes and elements</span></span>

<span data-ttu-id="60c54-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="60c54-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="60c54-108">属性</span><span class="sxs-lookup"><span data-stu-id="60c54-108">Attributes</span></span>

<span data-ttu-id="60c54-109">なし。</span><span class="sxs-lookup"><span data-stu-id="60c54-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="60c54-110">子要素</span><span class="sxs-lookup"><span data-stu-id="60c54-110">Child elements</span></span>

<span data-ttu-id="60c54-111">なし。</span><span class="sxs-lookup"><span data-stu-id="60c54-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="60c54-112">親要素</span><span class="sxs-lookup"><span data-stu-id="60c54-112">Parent elements</span></span>

|<span data-ttu-id="60c54-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="60c54-113">**Element**</span></span>|<span data-ttu-id="60c54-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="60c54-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="60c54-115">条件</span><span class="sxs-lookup"><span data-stu-id="60c54-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="60c54-116">ルールのルールの処理を開始するときに実行される条件を表します。</span><span class="sxs-lookup"><span data-stu-id="60c54-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="60c54-117">例外</span><span class="sxs-lookup"><span data-stu-id="60c54-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="60c54-118">受信トレイルールに対して使用可能なすべてのルールの例外条件を表します。</span><span class="sxs-lookup"><span data-stu-id="60c54-118">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="60c54-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="60c54-119">Text value</span></span>

<span data-ttu-id="60c54-120">テキスト値が**true の場合**は、条件または例外を適用するために、メールボックスの所有者が受信メッセージの**torecipients** **イベントプロパティに**含まれている必要があることを示します。</span><span class="sxs-lookup"><span data-stu-id="60c54-120">A text value of **true** indicates that the owner of the mailbox must be in the **ToRecipients** or **CcRecipients** property of the incoming messages in order for the condition or exception to apply.</span></span> <span data-ttu-id="60c54-121">値が**false**の場合は、条件または例外を適用するために、メールボックスの所有者が、受信メッセージの**torecipients**所有者または**ccrecipients**プロパティに含まれていない必要があることを示します。</span><span class="sxs-lookup"><span data-stu-id="60c54-121">A value of **false** indicates that the owner of the mailbox must not be in the **ToRecipients** or **CcRecipients** property of the incoming messages in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="60c54-122">注釈</span><span class="sxs-lookup"><span data-stu-id="60c54-122">Remarks</span></span>

<span data-ttu-id="60c54-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="60c54-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="60c54-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="60c54-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="60c54-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="60c54-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="60c54-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="60c54-126">Schema Name</span></span>  <br/> |<span data-ttu-id="60c54-127">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="60c54-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="60c54-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="60c54-128">Validation File</span></span>  <br/> |<span data-ttu-id="60c54-129">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="60c54-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="60c54-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="60c54-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="60c54-131">正しい</span><span class="sxs-lookup"><span data-stu-id="60c54-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="60c54-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="60c54-132">See also</span></span>



- [<span data-ttu-id="60c54-133">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="60c54-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

