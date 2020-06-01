---
title: 大き Subjectstrings
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
description: 指定した条件または例外を適用するために、受信メッセージの件名に表示する必要がある文字列を指定します。
ms.openlocfilehash: 8b078f61d08864970a123f81688981ffba2864ff
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458958"
---
# <a name="containssubjectstrings"></a><span data-ttu-id="36eda-103">大き Subjectstrings</span><span class="sxs-lookup"><span data-stu-id="36eda-103">ContainsSubjectStrings</span></span>

<span data-ttu-id="36eda-104">指定した条件または例外を適用するために、受信メッセージの件名に表示する必要がある文字列を**指定します**。</span><span class="sxs-lookup"><span data-stu-id="36eda-104">The **ContainsSubjectStrings** element indicates the strings that must appear in the subject of incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<ContainsSubjectStrings>
    <String/>
</ContainsSubjectStrings>
```

 <span data-ttu-id="36eda-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="36eda-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="36eda-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="36eda-106">Attributes and elements</span></span>

<span data-ttu-id="36eda-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="36eda-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="36eda-108">属性</span><span class="sxs-lookup"><span data-stu-id="36eda-108">Attributes</span></span>

<span data-ttu-id="36eda-109">なし。</span><span class="sxs-lookup"><span data-stu-id="36eda-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="36eda-110">子要素</span><span class="sxs-lookup"><span data-stu-id="36eda-110">Child elements</span></span>

|<span data-ttu-id="36eda-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="36eda-111">**Element**</span></span>|<span data-ttu-id="36eda-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="36eda-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="36eda-113">String</span><span class="sxs-lookup"><span data-stu-id="36eda-113">String</span></span>](string.md) <br/> |<span data-ttu-id="36eda-114">条件または例外を適用するために、受信メッセージの件名に表示する必要がある文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="36eda-114">Represents a string that must appear in the subject of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="36eda-115">親要素</span><span class="sxs-lookup"><span data-stu-id="36eda-115">Parent elements</span></span>

|<span data-ttu-id="36eda-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="36eda-116">**Element**</span></span>|<span data-ttu-id="36eda-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="36eda-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="36eda-118">条件</span><span class="sxs-lookup"><span data-stu-id="36eda-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="36eda-119">ルールのルールの処理を開始するときに実行される条件を表します。</span><span class="sxs-lookup"><span data-stu-id="36eda-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="36eda-120">例外</span><span class="sxs-lookup"><span data-stu-id="36eda-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="36eda-121">受信トレイルールに対して使用可能なルールの例外条件をすべて表す例外を表します。</span><span class="sxs-lookup"><span data-stu-id="36eda-121">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="36eda-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="36eda-122">Text value</span></span>

<span data-ttu-id="36eda-123">なし。</span><span class="sxs-lookup"><span data-stu-id="36eda-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="36eda-124">注釈</span><span class="sxs-lookup"><span data-stu-id="36eda-124">Remarks</span></span>

<span data-ttu-id="36eda-125">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="36eda-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="36eda-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="36eda-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="36eda-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="36eda-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="36eda-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="36eda-128">Schema Name</span></span>  <br/> |<span data-ttu-id="36eda-129">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="36eda-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="36eda-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="36eda-130">Validation File</span></span>  <br/> |<span data-ttu-id="36eda-131">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="36eda-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="36eda-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="36eda-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="36eda-133">正しい</span><span class="sxs-lookup"><span data-stu-id="36eda-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="36eda-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="36eda-134">See also</span></span>



- [<span data-ttu-id="36eda-135">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="36eda-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

