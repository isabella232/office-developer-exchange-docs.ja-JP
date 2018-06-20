---
title: エラー メッセージ
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0cec33a6-4b10-4259-8ac3-3f39a642b34c
description: エラー メッセージ要素は、検証エラーの原因を表します。
ms.openlocfilehash: d1869041254ef7c661fb2acb7c9c2ccaf628b394
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760332"
---
# <a name="errormessage"></a><span data-ttu-id="e28f6-103">エラー メッセージ</span><span class="sxs-lookup"><span data-stu-id="e28f6-103">ErrorMessage</span></span>

<span data-ttu-id="e28f6-104">**エラー メッセージ**要素は、検証エラーの原因を表します。</span><span class="sxs-lookup"><span data-stu-id="e28f6-104">The **ErrorMessage** element represents the reason for the validation error.</span></span> 
  
```XML
<ErrorMessage/>
```

 <span data-ttu-id="e28f6-105">**文字列型 (String)**</span><span class="sxs-lookup"><span data-stu-id="e28f6-105">**String**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e28f6-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="e28f6-106">Attributes and elements</span></span>

<span data-ttu-id="e28f6-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e28f6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e28f6-108">属性</span><span class="sxs-lookup"><span data-stu-id="e28f6-108">Attributes</span></span>

<span data-ttu-id="e28f6-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e28f6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e28f6-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e28f6-110">Child elements</span></span>

<span data-ttu-id="e28f6-111">なし。</span><span class="sxs-lookup"><span data-stu-id="e28f6-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e28f6-112">親要素</span><span class="sxs-lookup"><span data-stu-id="e28f6-112">Parent elements</span></span>

|<span data-ttu-id="e28f6-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="e28f6-113">**Element**</span></span>|<span data-ttu-id="e28f6-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="e28f6-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e28f6-115">Error</span><span class="sxs-lookup"><span data-stu-id="e28f6-115">Error</span></span>](error.md) <br/> |<span data-ttu-id="e28f6-116">特定のルールのプロパティの値、述語プロパティの値、またはアクションのプロパティの値の 1 つの検証エラーを表します。</span><span class="sxs-lookup"><span data-stu-id="e28f6-116">Represents a single validation error on a particular rule property value, predicate property value, or action property value.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e28f6-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="e28f6-117">Text value</span></span>

<span data-ttu-id="e28f6-118">ルールの検証エラーに関連付けられているエラー メッセージです。</span><span class="sxs-lookup"><span data-stu-id="e28f6-118">The error message associated with the rule validation error.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e28f6-119">備考</span><span class="sxs-lookup"><span data-stu-id="e28f6-119">Remarks</span></span>

<span data-ttu-id="e28f6-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="e28f6-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e28f6-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="e28f6-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e28f6-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="e28f6-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e28f6-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e28f6-123">Schema Name</span></span>  <br/> |<span data-ttu-id="e28f6-124">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="e28f6-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e28f6-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e28f6-125">Validation File</span></span>  <br/> |<span data-ttu-id="e28f6-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e28f6-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e28f6-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="e28f6-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="e28f6-128">True</span><span class="sxs-lookup"><span data-stu-id="e28f6-128">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e28f6-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="e28f6-129">See also</span></span>



- [<span data-ttu-id="e28f6-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="e28f6-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

