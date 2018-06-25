---
title: IsSigned
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsSigned
api_type:
- schema
ms.assetid: a4f90fe5-2834-4621-9aa3-b561f74d4674
description: IsSigned 要素を適用する場合の条件または例外の順序で受信したメッセージに署名が必要かどうかを示します。
ms.openlocfilehash: 33ff204260465490c701c6573ff4140967ac625a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832105"
---
# <a name="issigned"></a><span data-ttu-id="4eb4a-103">IsSigned</span><span class="sxs-lookup"><span data-stu-id="4eb4a-103">IsSigned</span></span>

<span data-ttu-id="4eb4a-104">**IsSigned**要素を適用する場合の条件または例外の順序で受信したメッセージに署名が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4eb4a-104">The **IsSigned** element indicates whether incoming messages must be signed in order for the condition or exception to apply.</span></span> 
  
```XML
<IsSigned>true | false</IsSigned>
```

 <span data-ttu-id="4eb4a-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="4eb4a-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4eb4a-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="4eb4a-106">Attributes and elements</span></span>

<span data-ttu-id="4eb4a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4eb4a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4eb4a-108">属性</span><span class="sxs-lookup"><span data-stu-id="4eb4a-108">Attributes</span></span>

<span data-ttu-id="4eb4a-109">なし。</span><span class="sxs-lookup"><span data-stu-id="4eb4a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4eb4a-110">子要素</span><span class="sxs-lookup"><span data-stu-id="4eb4a-110">Child elements</span></span>

<span data-ttu-id="4eb4a-111">なし。</span><span class="sxs-lookup"><span data-stu-id="4eb4a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4eb4a-112">親要素</span><span class="sxs-lookup"><span data-stu-id="4eb4a-112">Parent elements</span></span>

|<span data-ttu-id="4eb4a-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="4eb4a-113">**Element**</span></span>|<span data-ttu-id="4eb4a-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="4eb4a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4eb4a-115">条件</span><span class="sxs-lookup"><span data-stu-id="4eb4a-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="4eb4a-116">条件を表しますが、満たされるとときに、ルールのルールの処理をトリガーします。</span><span class="sxs-lookup"><span data-stu-id="4eb4a-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="4eb4a-117">Exceptions</span><span class="sxs-lookup"><span data-stu-id="4eb4a-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="4eb4a-118">受信トレイ ルールの使用可能なルールの例外条件をすべてを表す例外を表します。</span><span class="sxs-lookup"><span data-stu-id="4eb4a-118">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4eb4a-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="4eb4a-119">Text value</span></span>

<span data-ttu-id="4eb4a-120">**True**の場合、テキスト値を適用する場合の条件または例外の順序でメッセージを署名する必要があることを示します。</span><span class="sxs-lookup"><span data-stu-id="4eb4a-120">A text value of **true** indicates that the message must be signed in order for the condition or exception to apply.</span></span> <span data-ttu-id="4eb4a-121">**False**のテキスト値は、メッセージに適用する条件または例外の署名がないことを示します。</span><span class="sxs-lookup"><span data-stu-id="4eb4a-121">A text value of **false** indicates that the message does not have to be signed for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="4eb4a-122">備考</span><span class="sxs-lookup"><span data-stu-id="4eb4a-122">Remarks</span></span>

<span data-ttu-id="4eb4a-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="4eb4a-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4eb4a-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="4eb4a-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4eb4a-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="4eb4a-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4eb4a-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4eb4a-126">Schema Name</span></span>  <br/> |<span data-ttu-id="4eb4a-127">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="4eb4a-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4eb4a-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4eb4a-128">Validation File</span></span>  <br/> |<span data-ttu-id="4eb4a-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="4eb4a-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4eb4a-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="4eb4a-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="4eb4a-131">True</span><span class="sxs-lookup"><span data-stu-id="4eb4a-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4eb4a-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="4eb4a-132">See also</span></span>



- [<span data-ttu-id="4eb4a-133">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="4eb4a-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

