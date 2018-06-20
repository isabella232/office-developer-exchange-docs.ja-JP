---
title: OperationIndex
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OperationIndex
api_type:
- schema
ms.assetid: 289f173c-26fa-4981-95dd-652e1921bdc6
description: OperationIndex 要素は、ルールの操作エラーが発生した要求の操作のインデックスを指定します。
ms.openlocfilehash: c13c3a4abebb4938afcd99d5c18bf880a60ff70a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832654"
---
# <a name="operationindex"></a><span data-ttu-id="219d5-103">OperationIndex</span><span class="sxs-lookup"><span data-stu-id="219d5-103">OperationIndex</span></span>

<span data-ttu-id="219d5-104">**OperationIndex**要素は、ルールの操作エラーが発生した要求の操作のインデックスを指定します。</span><span class="sxs-lookup"><span data-stu-id="219d5-104">The **OperationIndex** element specifies the index of the operation in the request that caused the rule operation error.</span></span> 
  
```XML
<OperationIndex/>
```

 <span data-ttu-id="219d5-105">**int**</span><span class="sxs-lookup"><span data-stu-id="219d5-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="219d5-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="219d5-106">Attributes and elements</span></span>

<span data-ttu-id="219d5-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="219d5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="219d5-108">属性</span><span class="sxs-lookup"><span data-stu-id="219d5-108">Attributes</span></span>

<span data-ttu-id="219d5-109">なし。</span><span class="sxs-lookup"><span data-stu-id="219d5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="219d5-110">子要素</span><span class="sxs-lookup"><span data-stu-id="219d5-110">Child elements</span></span>

<span data-ttu-id="219d5-111">なし。</span><span class="sxs-lookup"><span data-stu-id="219d5-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="219d5-112">親要素</span><span class="sxs-lookup"><span data-stu-id="219d5-112">Parent elements</span></span>

|<span data-ttu-id="219d5-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="219d5-113">**Element**</span></span>|<span data-ttu-id="219d5-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="219d5-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="219d5-115">RuleOperationError</span><span class="sxs-lookup"><span data-stu-id="219d5-115">RuleOperationError</span></span>](ruleoperationerror.md) <br/> |<span data-ttu-id="219d5-116">ルール操作のエラーを表します。</span><span class="sxs-lookup"><span data-stu-id="219d5-116">Represents a rule operation error.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="219d5-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="219d5-117">Text value</span></span>

<span data-ttu-id="219d5-118">なし</span><span class="sxs-lookup"><span data-stu-id="219d5-118">None</span></span>
  
## <a name="remarks"></a><span data-ttu-id="219d5-119">解説</span><span class="sxs-lookup"><span data-stu-id="219d5-119">Remarks</span></span>

<span data-ttu-id="219d5-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="219d5-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="219d5-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="219d5-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="219d5-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="219d5-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="219d5-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="219d5-123">Schema Name</span></span>  <br/> |<span data-ttu-id="219d5-124">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="219d5-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="219d5-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="219d5-125">Validation File</span></span>  <br/> |<span data-ttu-id="219d5-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="219d5-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="219d5-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="219d5-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="219d5-128">True</span><span class="sxs-lookup"><span data-stu-id="219d5-128">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="219d5-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="219d5-129">See also</span></span>



- [<span data-ttu-id="219d5-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="219d5-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

