---
title: FieldValue
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8dfda53f-658c-4bc9-8950-f7f572c850eb
description: FieldValue 要素は、検証エラーが発生したフィールドの値を表します。
ms.openlocfilehash: 26517598d49865d2a925b436a0691fe548228955
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760468"
---
# <a name="fieldvalue"></a><span data-ttu-id="f6bff-103">FieldValue</span><span class="sxs-lookup"><span data-stu-id="f6bff-103">FieldValue</span></span>

<span data-ttu-id="f6bff-104">**FieldValue**要素は、検証エラーが発生したフィールドの値を表します。</span><span class="sxs-lookup"><span data-stu-id="f6bff-104">The **FieldValue** element represents the value of the field that caused the validation error.</span></span> 
  
```XML
<FieldValue/>
```

 <span data-ttu-id="f6bff-105">**文字列型 (String)**</span><span class="sxs-lookup"><span data-stu-id="f6bff-105">**String**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f6bff-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="f6bff-106">Attributes and elements</span></span>

<span data-ttu-id="f6bff-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f6bff-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f6bff-108">属性</span><span class="sxs-lookup"><span data-stu-id="f6bff-108">Attributes</span></span>

<span data-ttu-id="f6bff-109">なし。</span><span class="sxs-lookup"><span data-stu-id="f6bff-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f6bff-110">子要素</span><span class="sxs-lookup"><span data-stu-id="f6bff-110">Child elements</span></span>

<span data-ttu-id="f6bff-111">なし。</span><span class="sxs-lookup"><span data-stu-id="f6bff-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f6bff-112">親要素</span><span class="sxs-lookup"><span data-stu-id="f6bff-112">Parent elements</span></span>

|<span data-ttu-id="f6bff-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="f6bff-113">**Element**</span></span>|<span data-ttu-id="f6bff-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="f6bff-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f6bff-115">Error</span><span class="sxs-lookup"><span data-stu-id="f6bff-115">Error</span></span>](error.md) <br/> |<span data-ttu-id="f6bff-116">特定のルールのプロパティの値、述語プロパティの値、またはアクションのプロパティの値の 1 つの検証エラーを表します。</span><span class="sxs-lookup"><span data-stu-id="f6bff-116">Represents a single validation error on a particular rule property value, predicate property value, or action property value.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f6bff-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="f6bff-117">Text value</span></span>

<span data-ttu-id="f6bff-118">なし</span><span class="sxs-lookup"><span data-stu-id="f6bff-118">None</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f6bff-119">解説</span><span class="sxs-lookup"><span data-stu-id="f6bff-119">Remarks</span></span>

<span data-ttu-id="f6bff-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="f6bff-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f6bff-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="f6bff-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f6bff-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="f6bff-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f6bff-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f6bff-123">Schema Name</span></span>  <br/> |<span data-ttu-id="f6bff-124">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="f6bff-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f6bff-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f6bff-125">Validation File</span></span>  <br/> |<span data-ttu-id="f6bff-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f6bff-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f6bff-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="f6bff-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="f6bff-128">True</span><span class="sxs-lookup"><span data-stu-id="f6bff-128">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f6bff-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="f6bff-129">See also</span></span>



- [<span data-ttu-id="f6bff-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="f6bff-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

