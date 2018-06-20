---
title: ContainsSubjectStrings
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContainsSubjectStrings
api_type:
- schema
ms.assetid: c6ec1d8d-8dd8-4c9a-a3e1-50e24958eb0d
description: ContainsSubjectStrings 要素を適用する場合の条件または例外の順序で受信したメッセージの件名に表示される文字列を示します。
ms.openlocfilehash: a266855effaeb34aa232305db970f97c309a2e4c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759728"
---
# <a name="containssubjectstrings"></a><span data-ttu-id="32aec-103">ContainsSubjectStrings</span><span class="sxs-lookup"><span data-stu-id="32aec-103">ContainsSubjectStrings</span></span>

<span data-ttu-id="32aec-104">**ContainsSubjectStrings**要素を適用する場合の条件または例外の順序で受信したメッセージの件名に表示される文字列を示します。</span><span class="sxs-lookup"><span data-stu-id="32aec-104">The **ContainsSubjectStrings** element indicates the strings that must appear in the subject of incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<ContainsSubjectStrings>
    <String/>
</ContainsSubjectStrings>
```

 <span data-ttu-id="32aec-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="32aec-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="32aec-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="32aec-106">Attributes and elements</span></span>

<span data-ttu-id="32aec-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="32aec-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="32aec-108">属性</span><span class="sxs-lookup"><span data-stu-id="32aec-108">Attributes</span></span>

<span data-ttu-id="32aec-109">なし。</span><span class="sxs-lookup"><span data-stu-id="32aec-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="32aec-110">子要素</span><span class="sxs-lookup"><span data-stu-id="32aec-110">Child elements</span></span>

|<span data-ttu-id="32aec-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="32aec-111">**Element**</span></span>|<span data-ttu-id="32aec-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="32aec-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="32aec-113">String</span><span class="sxs-lookup"><span data-stu-id="32aec-113">String</span></span>](string.md) <br/> |<span data-ttu-id="32aec-114">適用する場合の条件または例外の順序で受信したメッセージの件名に表示される文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="32aec-114">Represents a string that must appear in the subject of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="32aec-115">親要素</span><span class="sxs-lookup"><span data-stu-id="32aec-115">Parent elements</span></span>

|<span data-ttu-id="32aec-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="32aec-116">**Element**</span></span>|<span data-ttu-id="32aec-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="32aec-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="32aec-118">条件</span><span class="sxs-lookup"><span data-stu-id="32aec-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="32aec-119">条件を表しますが、満たされるとときに、ルールのルールの処理をトリガーします。</span><span class="sxs-lookup"><span data-stu-id="32aec-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="32aec-120">Exceptions</span><span class="sxs-lookup"><span data-stu-id="32aec-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="32aec-121">受信トレイ ルールの使用可能なルールの例外条件をすべてを表す例外を表します。</span><span class="sxs-lookup"><span data-stu-id="32aec-121">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="32aec-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="32aec-122">Text value</span></span>

<span data-ttu-id="32aec-123">なし。</span><span class="sxs-lookup"><span data-stu-id="32aec-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="32aec-124">備考</span><span class="sxs-lookup"><span data-stu-id="32aec-124">Remarks</span></span>

<span data-ttu-id="32aec-125">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="32aec-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="32aec-126">要素情報</span><span class="sxs-lookup"><span data-stu-id="32aec-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="32aec-127">名前空間</span><span class="sxs-lookup"><span data-stu-id="32aec-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="32aec-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="32aec-128">Schema Name</span></span>  <br/> |<span data-ttu-id="32aec-129">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="32aec-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="32aec-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="32aec-130">Validation File</span></span>  <br/> |<span data-ttu-id="32aec-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="32aec-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="32aec-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="32aec-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="32aec-133">True</span><span class="sxs-lookup"><span data-stu-id="32aec-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="32aec-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="32aec-134">See also</span></span>



- [<span data-ttu-id="32aec-135">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="32aec-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

