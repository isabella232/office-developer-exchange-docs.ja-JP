---
title: ErrorMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0cec33a6-4b10-4259-8ac3-3f39a642b34c
description: ErrorMessage 要素は、検証エラーの理由を表します。
ms.openlocfilehash: a35dc6af12e71c8437c13024a254000e8f477a15
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526194"
---
# <a name="errormessage"></a><span data-ttu-id="d9cc9-103">ErrorMessage</span><span class="sxs-lookup"><span data-stu-id="d9cc9-103">ErrorMessage</span></span>

<span data-ttu-id="d9cc9-104">**ErrorMessage**要素は、検証エラーの理由を表します。</span><span class="sxs-lookup"><span data-stu-id="d9cc9-104">The **ErrorMessage** element represents the reason for the validation error.</span></span> 
  
```XML
<ErrorMessage/>
```

 <span data-ttu-id="d9cc9-105">**String**</span><span class="sxs-lookup"><span data-stu-id="d9cc9-105">**String**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d9cc9-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d9cc9-106">Attributes and elements</span></span>

<span data-ttu-id="d9cc9-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d9cc9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d9cc9-108">属性</span><span class="sxs-lookup"><span data-stu-id="d9cc9-108">Attributes</span></span>

<span data-ttu-id="d9cc9-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d9cc9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d9cc9-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d9cc9-110">Child elements</span></span>

<span data-ttu-id="d9cc9-111">なし。</span><span class="sxs-lookup"><span data-stu-id="d9cc9-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d9cc9-112">親要素</span><span class="sxs-lookup"><span data-stu-id="d9cc9-112">Parent elements</span></span>

|<span data-ttu-id="d9cc9-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="d9cc9-113">**Element**</span></span>|<span data-ttu-id="d9cc9-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="d9cc9-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d9cc9-115">Error</span><span class="sxs-lookup"><span data-stu-id="d9cc9-115">Error</span></span>](error.md) <br/> |<span data-ttu-id="d9cc9-116">特定のルールプロパティ値、述語プロパティ値、または action プロパティ値に対する1つの検証エラーを表します。</span><span class="sxs-lookup"><span data-stu-id="d9cc9-116">Represents a single validation error on a particular rule property value, predicate property value, or action property value.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d9cc9-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="d9cc9-117">Text value</span></span>

<span data-ttu-id="d9cc9-118">ルールの検証エラーに関連付けられたエラーメッセージ。</span><span class="sxs-lookup"><span data-stu-id="d9cc9-118">The error message associated with the rule validation error.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d9cc9-119">注釈</span><span class="sxs-lookup"><span data-stu-id="d9cc9-119">Remarks</span></span>

<span data-ttu-id="d9cc9-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="d9cc9-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d9cc9-121">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d9cc9-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d9cc9-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="d9cc9-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d9cc9-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d9cc9-123">Schema Name</span></span>  <br/> |<span data-ttu-id="d9cc9-124">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="d9cc9-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d9cc9-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d9cc9-125">Validation File</span></span>  <br/> |<span data-ttu-id="d9cc9-126">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="d9cc9-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d9cc9-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d9cc9-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="d9cc9-128">正しい</span><span class="sxs-lookup"><span data-stu-id="d9cc9-128">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d9cc9-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="d9cc9-129">See also</span></span>



- [<span data-ttu-id="d9cc9-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="d9cc9-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

