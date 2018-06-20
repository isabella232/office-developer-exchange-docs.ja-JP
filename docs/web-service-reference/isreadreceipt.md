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
description: IsReadReceipt 要素は、あるかどうかの受信メッセージ読み取る必要があります適用の条件または例外のために領収書を示します。
ms.openlocfilehash: 78714aafb116a609a69d77b3b4f0fd15695bda34
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832094"
---
# <a name="isreadreceipt"></a><span data-ttu-id="bcbc6-103">IsReadReceipt</span><span class="sxs-lookup"><span data-stu-id="bcbc6-103">IsReadReceipt</span></span>

<span data-ttu-id="bcbc6-104">**IsReadReceipt**要素は、あるかどうかの受信メッセージ読み取る必要があります適用の条件または例外のために領収書を示します。</span><span class="sxs-lookup"><span data-stu-id="bcbc6-104">The **IsReadReceipt** element indicates whether incoming messages must be read receipts in order for the condition or exception to apply.</span></span> 
  
```XML
<IsReadReceipt> true | false</IsReadReceipt>
```

 <span data-ttu-id="bcbc6-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="bcbc6-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bcbc6-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="bcbc6-106">Attributes and elements</span></span>

<span data-ttu-id="bcbc6-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="bcbc6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bcbc6-108">属性</span><span class="sxs-lookup"><span data-stu-id="bcbc6-108">Attributes</span></span>

<span data-ttu-id="bcbc6-109">なし。</span><span class="sxs-lookup"><span data-stu-id="bcbc6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bcbc6-110">子要素</span><span class="sxs-lookup"><span data-stu-id="bcbc6-110">Child elements</span></span>

<span data-ttu-id="bcbc6-111">なし。</span><span class="sxs-lookup"><span data-stu-id="bcbc6-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bcbc6-112">親要素</span><span class="sxs-lookup"><span data-stu-id="bcbc6-112">Parent elements</span></span>

|<span data-ttu-id="bcbc6-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="bcbc6-113">**Element**</span></span>|<span data-ttu-id="bcbc6-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="bcbc6-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bcbc6-115">条件</span><span class="sxs-lookup"><span data-stu-id="bcbc6-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="bcbc6-116">条件を表しますが、満たされるとときに、そのルールのルールの処理をトリガーします。</span><span class="sxs-lookup"><span data-stu-id="bcbc6-116">Represents the conditions that, when fulfilled, will trigger the rule actions for that rule.</span></span>  <br/> |
|[<span data-ttu-id="bcbc6-117">Exceptions</span><span class="sxs-lookup"><span data-stu-id="bcbc6-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="bcbc6-118">受信トレイ ルールの使用可能なルールの例外条件をすべてを表します。</span><span class="sxs-lookup"><span data-stu-id="bcbc6-118">Represents all the available rule exception conditions for the Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bcbc6-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="bcbc6-119">Text value</span></span>

<span data-ttu-id="bcbc6-120">**True**の場合、テキスト値は、メッセージは開封済みメッセージを適用する場合の条件または例外の順序である必要があることを示します。</span><span class="sxs-lookup"><span data-stu-id="bcbc6-120">A text value of **true** indicates that the message must be a read receipt in order for the condition or exception to apply.</span></span> <span data-ttu-id="bcbc6-121">メッセージが開封済みの条件または例外を適用する、値が**false**にします。</span><span class="sxs-lookup"><span data-stu-id="bcbc6-121">If the message does not have to be a read receipt for the condition or exception to apply, the value is **false**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bcbc6-122">備考</span><span class="sxs-lookup"><span data-stu-id="bcbc6-122">Remarks</span></span>

<span data-ttu-id="bcbc6-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="bcbc6-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bcbc6-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="bcbc6-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bcbc6-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="bcbc6-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="bcbc6-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="bcbc6-126">Schema Name</span></span>  <br/> |<span data-ttu-id="bcbc6-127">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="bcbc6-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="bcbc6-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="bcbc6-128">Validation File</span></span>  <br/> |<span data-ttu-id="bcbc6-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="bcbc6-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="bcbc6-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="bcbc6-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="bcbc6-131">True</span><span class="sxs-lookup"><span data-stu-id="bcbc6-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bcbc6-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="bcbc6-132">See also</span></span>



- [<span data-ttu-id="bcbc6-133">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="bcbc6-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

