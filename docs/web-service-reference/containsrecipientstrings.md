---
title: ContainsRecipientStrings
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContainsRecipientStrings
api_type:
- schema
ms.assetid: a7fd13ac-0f13-4610-ac9b-98e27ac3940b
description: ContainsRecipientStrings 要素は、ToRecipients または CcRecipients のいずれかのプロパティを適用する場合の条件または例外の順序で受信メッセージの [表示する文字列を示します。
ms.openlocfilehash: 861aba22c9474caf02f9c50d8a7b65b9cc8a2eda
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759701"
---
# <a name="containsrecipientstrings"></a><span data-ttu-id="b01d3-103">ContainsRecipientStrings</span><span class="sxs-lookup"><span data-stu-id="b01d3-103">ContainsRecipientStrings</span></span>

<span data-ttu-id="b01d3-104">**ContainsRecipientStrings**要素は、 **ToRecipients**または**CcRecipients**のいずれかの条件または例外を適用する順序で受信メッセージのプロパティに表示される文字列を示します。</span><span class="sxs-lookup"><span data-stu-id="b01d3-104">The **ContainsRecipientStrings** element indicates the strings that must appear in either the **ToRecipients** or **CcRecipients** properties of incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<ContainsRecipientStrings>
    <String/>
</ContainsRecipientStrings>
```

 <span data-ttu-id="b01d3-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="b01d3-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b01d3-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="b01d3-106">Attributes and elements</span></span>

<span data-ttu-id="b01d3-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b01d3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b01d3-108">属性</span><span class="sxs-lookup"><span data-stu-id="b01d3-108">Attributes</span></span>

<span data-ttu-id="b01d3-109">なし。</span><span class="sxs-lookup"><span data-stu-id="b01d3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b01d3-110">子要素</span><span class="sxs-lookup"><span data-stu-id="b01d3-110">Child elements</span></span>

|<span data-ttu-id="b01d3-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="b01d3-111">**Element**</span></span>|<span data-ttu-id="b01d3-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="b01d3-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b01d3-113">String</span><span class="sxs-lookup"><span data-stu-id="b01d3-113">String</span></span>](string.md) <br/> |<span data-ttu-id="b01d3-114">**ToRecipients**または**CcRecipients**のいずれかの条件または例外を適用する順序で受信メッセージのプロパティに表示される文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="b01d3-114">Represents a string that must appear in either the **ToRecipients** or **CcRecipients** properties of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b01d3-115">親要素</span><span class="sxs-lookup"><span data-stu-id="b01d3-115">Parent elements</span></span>

|<span data-ttu-id="b01d3-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="b01d3-116">**Element**</span></span>|<span data-ttu-id="b01d3-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="b01d3-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b01d3-118">条件</span><span class="sxs-lookup"><span data-stu-id="b01d3-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="b01d3-119">条件を表しますが、満たされるとときに、ルールのルールの処理をトリガーします。</span><span class="sxs-lookup"><span data-stu-id="b01d3-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="b01d3-120">Exceptions</span><span class="sxs-lookup"><span data-stu-id="b01d3-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="b01d3-121">受信トレイ ルールの使用可能なルールの例外条件をすべてを表す例外を表します。</span><span class="sxs-lookup"><span data-stu-id="b01d3-121">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b01d3-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="b01d3-122">Text value</span></span>

<span data-ttu-id="b01d3-123">なし。</span><span class="sxs-lookup"><span data-stu-id="b01d3-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b01d3-124">備考</span><span class="sxs-lookup"><span data-stu-id="b01d3-124">Remarks</span></span>

<span data-ttu-id="b01d3-125">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="b01d3-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b01d3-126">要素情報</span><span class="sxs-lookup"><span data-stu-id="b01d3-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b01d3-127">名前空間</span><span class="sxs-lookup"><span data-stu-id="b01d3-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b01d3-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b01d3-128">Schema Name</span></span>  <br/> |<span data-ttu-id="b01d3-129">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="b01d3-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b01d3-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b01d3-130">Validation File</span></span>  <br/> |<span data-ttu-id="b01d3-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b01d3-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b01d3-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="b01d3-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="b01d3-133">True</span><span class="sxs-lookup"><span data-stu-id="b01d3-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b01d3-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="b01d3-134">See also</span></span>



- [<span data-ttu-id="b01d3-135">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="b01d3-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

