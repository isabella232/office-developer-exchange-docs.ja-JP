---
title: IsMeetingResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsMeetingResponse
api_type:
- schema
ms.assetid: 85090943-81c6-4fbe-a2db-007dced6a4cf
description: IsMeetngResponsequest 要素は、受信メッセージに適用する条件または例外の順序で会議の返信をする必要があるかどうかを示します。
ms.openlocfilehash: 9040859452a48916a969b6d8e4e370b5785c1c1a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832053"
---
# <a name="ismeetingresponse"></a><span data-ttu-id="257a8-103">IsMeetingResponse</span><span class="sxs-lookup"><span data-stu-id="257a8-103">IsMeetingResponse</span></span>

<span data-ttu-id="257a8-104">**IsMeetngResponsequest**要素は、受信メッセージに適用する条件または例外の順序で会議の返信をする必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="257a8-104">The **IsMeetngResponsequest** element indicates whether incoming messages must be a meeting response in order for the condition or exception to apply.</span></span> 
  
```XML
<IsMeetingResponse/>true | false</IsMeetingResponse>
```

 <span data-ttu-id="257a8-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="257a8-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="257a8-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="257a8-106">Attributes and elements</span></span>

<span data-ttu-id="257a8-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="257a8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="257a8-108">属性</span><span class="sxs-lookup"><span data-stu-id="257a8-108">Attributes</span></span>

<span data-ttu-id="257a8-109">なし。</span><span class="sxs-lookup"><span data-stu-id="257a8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="257a8-110">子要素</span><span class="sxs-lookup"><span data-stu-id="257a8-110">Child elements</span></span>

<span data-ttu-id="257a8-111">なし。</span><span class="sxs-lookup"><span data-stu-id="257a8-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="257a8-112">親要素</span><span class="sxs-lookup"><span data-stu-id="257a8-112">Parent elements</span></span>

|<span data-ttu-id="257a8-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="257a8-113">**Element**</span></span>|<span data-ttu-id="257a8-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="257a8-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="257a8-115">条件</span><span class="sxs-lookup"><span data-stu-id="257a8-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="257a8-116">条件を表しますが、満たされるとときに、ルールのルールの処理をトリガーします。</span><span class="sxs-lookup"><span data-stu-id="257a8-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="257a8-117">Exceptions</span><span class="sxs-lookup"><span data-stu-id="257a8-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="257a8-118">受信トレイ ルールの使用可能なルールの例外条件をすべてを表します。</span><span class="sxs-lookup"><span data-stu-id="257a8-118">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="257a8-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="257a8-119">Text value</span></span>

<span data-ttu-id="257a8-120">**True**の場合、テキスト値は、メッセージで会議の返信をするために条件または例外を適用する必要があることを示します。</span><span class="sxs-lookup"><span data-stu-id="257a8-120">A text value of **true** indicates that the message must be a meeting response in order for the condition or exception to apply.</span></span> <span data-ttu-id="257a8-121">**False**のテキスト値は、メッセージでは、会議の返信を適用する場合の条件または例外の順にならないということを示します。</span><span class="sxs-lookup"><span data-stu-id="257a8-121">A text value of **false** indicates that the message must not be a meeting response in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="257a8-122">備考</span><span class="sxs-lookup"><span data-stu-id="257a8-122">Remarks</span></span>

<span data-ttu-id="257a8-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="257a8-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="257a8-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="257a8-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="257a8-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="257a8-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="257a8-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="257a8-126">Schema Name</span></span>  <br/> |<span data-ttu-id="257a8-127">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="257a8-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="257a8-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="257a8-128">Validation File</span></span>  <br/> |<span data-ttu-id="257a8-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="257a8-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="257a8-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="257a8-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="257a8-131">True</span><span class="sxs-lookup"><span data-stu-id="257a8-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="257a8-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="257a8-132">See also</span></span>



- [<span data-ttu-id="257a8-133">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="257a8-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

