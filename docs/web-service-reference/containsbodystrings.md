---
title: 大き Body文字列
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContainsBodyStrings
api_type:
- schema
ms.assetid: 70639472-64bb-456a-8b40-dce727542443
description: 指定した条件または例外を適用するために、受信メッセージの本文に表示する必要がある文字列を指定します。
ms.openlocfilehash: 008261ab94b1bed33cc72cacf7abe7aa58927d1a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463805"
---
# <a name="containsbodystrings"></a><span data-ttu-id="aa7b6-103">大き Body文字列</span><span class="sxs-lookup"><span data-stu-id="aa7b6-103">ContainsBodyStrings</span></span>

<span data-ttu-id="aa7b6-104">指定した条件または例外を適用するために、受信メッセージの本文に表示する必要がある文字列を**指定します**。</span><span class="sxs-lookup"><span data-stu-id="aa7b6-104">The **ContainsBodyStrings** element indicates the strings that must appear in the body of incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<ContainsBodyStrings>
    <String/>
</ContainsBodyStrings>
```

 <span data-ttu-id="aa7b6-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="aa7b6-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="aa7b6-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="aa7b6-106">Attributes and elements</span></span>

<span data-ttu-id="aa7b6-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="aa7b6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="aa7b6-108">属性</span><span class="sxs-lookup"><span data-stu-id="aa7b6-108">Attributes</span></span>

<span data-ttu-id="aa7b6-109">なし。</span><span class="sxs-lookup"><span data-stu-id="aa7b6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="aa7b6-110">子要素</span><span class="sxs-lookup"><span data-stu-id="aa7b6-110">Child elements</span></span>

|<span data-ttu-id="aa7b6-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="aa7b6-111">**Element**</span></span>|<span data-ttu-id="aa7b6-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="aa7b6-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aa7b6-113">String</span><span class="sxs-lookup"><span data-stu-id="aa7b6-113">String</span></span>](string.md) <br/> |<span data-ttu-id="aa7b6-114">条件または例外を適用するために、受信メッセージの本文に表示する必要がある文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="aa7b6-114">Represents a string that must appear in the body of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="aa7b6-115">親要素</span><span class="sxs-lookup"><span data-stu-id="aa7b6-115">Parent elements</span></span>

|<span data-ttu-id="aa7b6-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="aa7b6-116">**Element**</span></span>|<span data-ttu-id="aa7b6-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="aa7b6-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aa7b6-118">条件</span><span class="sxs-lookup"><span data-stu-id="aa7b6-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="aa7b6-119">ルールのルールの処理を開始するときに実行される条件を表します。</span><span class="sxs-lookup"><span data-stu-id="aa7b6-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="aa7b6-120">例外</span><span class="sxs-lookup"><span data-stu-id="aa7b6-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="aa7b6-121">受信トレイルールに対して使用可能なルールの例外条件をすべて表す例外を表します。</span><span class="sxs-lookup"><span data-stu-id="aa7b6-121">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="aa7b6-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="aa7b6-122">Text value</span></span>

<span data-ttu-id="aa7b6-123">なし。</span><span class="sxs-lookup"><span data-stu-id="aa7b6-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="aa7b6-124">注釈</span><span class="sxs-lookup"><span data-stu-id="aa7b6-124">Remarks</span></span>

<span data-ttu-id="aa7b6-125">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="aa7b6-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="aa7b6-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="aa7b6-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="aa7b6-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="aa7b6-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="aa7b6-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="aa7b6-128">Schema Name</span></span>  <br/> |<span data-ttu-id="aa7b6-129">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="aa7b6-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="aa7b6-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="aa7b6-130">Validation File</span></span>  <br/> |<span data-ttu-id="aa7b6-131">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="aa7b6-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="aa7b6-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="aa7b6-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="aa7b6-133">正しい</span><span class="sxs-lookup"><span data-stu-id="aa7b6-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="aa7b6-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="aa7b6-134">See also</span></span>



- [<span data-ttu-id="aa7b6-135">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="aa7b6-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

