---
title: ContainsSubjectOrBodyStrings
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContainsSubjectOrBodyStrings
api_type:
- schema
ms.assetid: 22aebf31-d9f4-4e03-bbff-c675409518d1
description: ContainsSubjectOrBodyStrings 要素は、条件または例外を適用するために、受信メッセージの本文または件名に表示する必要がある文字列を示します。
ms.openlocfilehash: 6f9c7862912632e7e86a0b704e760c7fd0f5f14c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466823"
---
# <a name="containssubjectorbodystrings"></a><span data-ttu-id="18523-103">ContainsSubjectOrBodyStrings</span><span class="sxs-lookup"><span data-stu-id="18523-103">ContainsSubjectOrBodyStrings</span></span>

<span data-ttu-id="18523-104">**ContainsSubjectOrBodyStrings**要素は、条件または例外を適用するために、受信メッセージの本文または件名に表示する必要がある文字列を示します。</span><span class="sxs-lookup"><span data-stu-id="18523-104">The **ContainsSubjectOrBodyStrings** element indicates the strings that must appear in either the body or the subject of incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<ContainsSubjectOrBodyStrings>
    <String/>
</ContainsSubjectOrBodyStrings>
```

 <span data-ttu-id="18523-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="18523-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="18523-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="18523-106">Attributes and elements</span></span>

<span data-ttu-id="18523-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="18523-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="18523-108">属性</span><span class="sxs-lookup"><span data-stu-id="18523-108">Attributes</span></span>

<span data-ttu-id="18523-109">なし。</span><span class="sxs-lookup"><span data-stu-id="18523-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="18523-110">子要素</span><span class="sxs-lookup"><span data-stu-id="18523-110">Child elements</span></span>

|<span data-ttu-id="18523-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="18523-111">**Element**</span></span>|<span data-ttu-id="18523-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="18523-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="18523-113">String</span><span class="sxs-lookup"><span data-stu-id="18523-113">String</span></span>](string.md) <br/> |<span data-ttu-id="18523-114">条件または例外を適用するために、受信メッセージの本文または件名のどちらかに表示される文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="18523-114">Represents a string that must appear in either the body or the subject of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="18523-115">親要素</span><span class="sxs-lookup"><span data-stu-id="18523-115">Parent elements</span></span>

|<span data-ttu-id="18523-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="18523-116">**Element**</span></span>|<span data-ttu-id="18523-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="18523-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="18523-118">条件</span><span class="sxs-lookup"><span data-stu-id="18523-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="18523-119">ルールのルールの処理を開始するときに実行される条件を表します。</span><span class="sxs-lookup"><span data-stu-id="18523-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="18523-120">例外</span><span class="sxs-lookup"><span data-stu-id="18523-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="18523-121">受信トレイルールに対して使用可能なルールの例外条件をすべて表す例外を表します。</span><span class="sxs-lookup"><span data-stu-id="18523-121">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="18523-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="18523-122">Text value</span></span>

<span data-ttu-id="18523-123">なし。</span><span class="sxs-lookup"><span data-stu-id="18523-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="18523-124">注釈</span><span class="sxs-lookup"><span data-stu-id="18523-124">Remarks</span></span>

<span data-ttu-id="18523-125">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="18523-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="18523-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="18523-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="18523-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="18523-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="18523-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="18523-128">Schema Name</span></span>  <br/> |<span data-ttu-id="18523-129">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="18523-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="18523-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="18523-130">Validation File</span></span>  <br/> |<span data-ttu-id="18523-131">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="18523-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="18523-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="18523-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="18523-133">正しい</span><span class="sxs-lookup"><span data-stu-id="18523-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="18523-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="18523-134">See also</span></span>



- [<span data-ttu-id="18523-135">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="18523-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

