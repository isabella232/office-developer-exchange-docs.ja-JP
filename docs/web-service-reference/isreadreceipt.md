---
title: IsReadReceipt
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsReadReceipt
api_type:
- schema
ms.assetid: e60e525f-c136-469a-b68b-b3dc01f400a6
description: IsReadReceipt 要素は、条件または例外を適用するために、受信メッセージが開封確認である必要があるかどうかを示します。
ms.openlocfilehash: e86a7776bc43204dae9fc92f21d4304255ddb888
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463903"
---
# <a name="isreadreceipt"></a><span data-ttu-id="06fe0-103">IsReadReceipt</span><span class="sxs-lookup"><span data-stu-id="06fe0-103">IsReadReceipt</span></span>

<span data-ttu-id="06fe0-104">**Isreadreceipt**要素は、条件または例外を適用するために、受信メッセージが開封確認である必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="06fe0-104">The **IsReadReceipt** element indicates whether incoming messages must be read receipts in order for the condition or exception to apply.</span></span> 
  
```XML
<IsReadReceipt> true | false</IsReadReceipt>
```

 <span data-ttu-id="06fe0-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="06fe0-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="06fe0-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="06fe0-106">Attributes and elements</span></span>

<span data-ttu-id="06fe0-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="06fe0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="06fe0-108">属性</span><span class="sxs-lookup"><span data-stu-id="06fe0-108">Attributes</span></span>

<span data-ttu-id="06fe0-109">なし。</span><span class="sxs-lookup"><span data-stu-id="06fe0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="06fe0-110">子要素</span><span class="sxs-lookup"><span data-stu-id="06fe0-110">Child elements</span></span>

<span data-ttu-id="06fe0-111">なし。</span><span class="sxs-lookup"><span data-stu-id="06fe0-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="06fe0-112">親要素</span><span class="sxs-lookup"><span data-stu-id="06fe0-112">Parent elements</span></span>

|<span data-ttu-id="06fe0-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="06fe0-113">**Element**</span></span>|<span data-ttu-id="06fe0-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="06fe0-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="06fe0-115">条件</span><span class="sxs-lookup"><span data-stu-id="06fe0-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="06fe0-116">そのルールのルールの処理を開始するときに実行される条件を表します。</span><span class="sxs-lookup"><span data-stu-id="06fe0-116">Represents the conditions that, when fulfilled, will trigger the rule actions for that rule.</span></span>  <br/> |
|[<span data-ttu-id="06fe0-117">例外</span><span class="sxs-lookup"><span data-stu-id="06fe0-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="06fe0-118">受信トレイルールの利用可能なすべてのルールの例外条件を表します。</span><span class="sxs-lookup"><span data-stu-id="06fe0-118">Represents all the available rule exception conditions for the Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="06fe0-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="06fe0-119">Text value</span></span>

<span data-ttu-id="06fe0-120">テキスト値が**true の場合**、条件または例外を適用するには、メッセージが開封確認メッセージである必要があることを示します。</span><span class="sxs-lookup"><span data-stu-id="06fe0-120">A text value of **true** indicates that the message must be a read receipt in order for the condition or exception to apply.</span></span> <span data-ttu-id="06fe0-121">条件または例外を適用するために、メッセージが開封確認を必要としない場合、値は**false**になります。</span><span class="sxs-lookup"><span data-stu-id="06fe0-121">If the message does not have to be a read receipt for the condition or exception to apply, the value is **false**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="06fe0-122">注釈</span><span class="sxs-lookup"><span data-stu-id="06fe0-122">Remarks</span></span>

<span data-ttu-id="06fe0-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="06fe0-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="06fe0-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="06fe0-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="06fe0-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="06fe0-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="06fe0-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="06fe0-126">Schema Name</span></span>  <br/> |<span data-ttu-id="06fe0-127">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="06fe0-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="06fe0-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="06fe0-128">Validation File</span></span>  <br/> |<span data-ttu-id="06fe0-129">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="06fe0-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="06fe0-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="06fe0-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="06fe0-131">正しい</span><span class="sxs-lookup"><span data-stu-id="06fe0-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="06fe0-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="06fe0-132">See also</span></span>



- [<span data-ttu-id="06fe0-133">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="06fe0-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

