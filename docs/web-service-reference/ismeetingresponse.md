---
title: Is会議の応答
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
description: IsMeetngResponsequest 要素は、条件または例外を適用するために、受信メッセージが会議の応答である必要があるかどうかを示します。
ms.openlocfilehash: 40714b7e926768f55207d870b79f21f07163bb37
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465934"
---
# <a name="ismeetingresponse"></a><span data-ttu-id="21f03-103">Is会議の応答</span><span class="sxs-lookup"><span data-stu-id="21f03-103">IsMeetingResponse</span></span>

<span data-ttu-id="21f03-104">**IsMeetngResponsequest**要素は、条件または例外を適用するために、受信メッセージが会議の応答である必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="21f03-104">The **IsMeetngResponsequest** element indicates whether incoming messages must be a meeting response in order for the condition or exception to apply.</span></span> 
  
```XML
<IsMeetingResponse/>true | false</IsMeetingResponse>
```

 <span data-ttu-id="21f03-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="21f03-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="21f03-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="21f03-106">Attributes and elements</span></span>

<span data-ttu-id="21f03-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="21f03-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="21f03-108">属性</span><span class="sxs-lookup"><span data-stu-id="21f03-108">Attributes</span></span>

<span data-ttu-id="21f03-109">なし。</span><span class="sxs-lookup"><span data-stu-id="21f03-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="21f03-110">子要素</span><span class="sxs-lookup"><span data-stu-id="21f03-110">Child elements</span></span>

<span data-ttu-id="21f03-111">なし。</span><span class="sxs-lookup"><span data-stu-id="21f03-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="21f03-112">親要素</span><span class="sxs-lookup"><span data-stu-id="21f03-112">Parent elements</span></span>

|<span data-ttu-id="21f03-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="21f03-113">**Element**</span></span>|<span data-ttu-id="21f03-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="21f03-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="21f03-115">条件</span><span class="sxs-lookup"><span data-stu-id="21f03-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="21f03-116">ルールのルールの処理を開始するときに実行される条件を表します。</span><span class="sxs-lookup"><span data-stu-id="21f03-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="21f03-117">例外</span><span class="sxs-lookup"><span data-stu-id="21f03-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="21f03-118">受信トレイルールに対して使用可能なすべてのルールの例外条件を表します。</span><span class="sxs-lookup"><span data-stu-id="21f03-118">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="21f03-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="21f03-119">Text value</span></span>

<span data-ttu-id="21f03-120">**True**のテキスト値は、条件または例外を適用するために、メッセージが会議の応答である必要があることを示します。</span><span class="sxs-lookup"><span data-stu-id="21f03-120">A text value of **true** indicates that the message must be a meeting response in order for the condition or exception to apply.</span></span> <span data-ttu-id="21f03-121">テキスト値が**false**の場合は、条件または例外を適用するために、メッセージが会議出席依頼の返信ではない必要があることを示します。</span><span class="sxs-lookup"><span data-stu-id="21f03-121">A text value of **false** indicates that the message must not be a meeting response in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="21f03-122">注釈</span><span class="sxs-lookup"><span data-stu-id="21f03-122">Remarks</span></span>

<span data-ttu-id="21f03-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="21f03-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="21f03-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="21f03-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="21f03-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="21f03-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="21f03-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="21f03-126">Schema Name</span></span>  <br/> |<span data-ttu-id="21f03-127">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="21f03-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="21f03-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="21f03-128">Validation File</span></span>  <br/> |<span data-ttu-id="21f03-129">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="21f03-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="21f03-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="21f03-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="21f03-131">正しい</span><span class="sxs-lookup"><span data-stu-id="21f03-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="21f03-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="21f03-132">See also</span></span>



- [<span data-ttu-id="21f03-133">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="21f03-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

