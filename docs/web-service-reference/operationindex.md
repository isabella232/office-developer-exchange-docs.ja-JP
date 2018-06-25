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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832654"
---
# <a name="operationindex"></a><span data-ttu-id="96a6a-103">OperationIndex</span><span class="sxs-lookup"><span data-stu-id="96a6a-103">OperationIndex</span></span>

<span data-ttu-id="96a6a-104">**OperationIndex**要素は、ルールの操作エラーが発生した要求の操作のインデックスを指定します。</span><span class="sxs-lookup"><span data-stu-id="96a6a-104">The **OperationIndex** element specifies the index of the operation in the request that caused the rule operation error.</span></span> 
  
```XML
<OperationIndex/>
```

 <span data-ttu-id="96a6a-105">**int**</span><span class="sxs-lookup"><span data-stu-id="96a6a-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="96a6a-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="96a6a-106">Attributes and elements</span></span>

<span data-ttu-id="96a6a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="96a6a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="96a6a-108">属性</span><span class="sxs-lookup"><span data-stu-id="96a6a-108">Attributes</span></span>

<span data-ttu-id="96a6a-109">なし。</span><span class="sxs-lookup"><span data-stu-id="96a6a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="96a6a-110">子要素</span><span class="sxs-lookup"><span data-stu-id="96a6a-110">Child elements</span></span>

<span data-ttu-id="96a6a-111">なし。</span><span class="sxs-lookup"><span data-stu-id="96a6a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="96a6a-112">親要素</span><span class="sxs-lookup"><span data-stu-id="96a6a-112">Parent elements</span></span>

|<span data-ttu-id="96a6a-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="96a6a-113">**Element**</span></span>|<span data-ttu-id="96a6a-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="96a6a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="96a6a-115">RuleOperationError</span><span class="sxs-lookup"><span data-stu-id="96a6a-115">RuleOperationError</span></span>](ruleoperationerror.md) <br/> |<span data-ttu-id="96a6a-116">ルール操作のエラーを表します。</span><span class="sxs-lookup"><span data-stu-id="96a6a-116">Represents a rule operation error.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="96a6a-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="96a6a-117">Text value</span></span>

<span data-ttu-id="96a6a-118">なし</span><span class="sxs-lookup"><span data-stu-id="96a6a-118">None</span></span>
  
## <a name="remarks"></a><span data-ttu-id="96a6a-119">解説</span><span class="sxs-lookup"><span data-stu-id="96a6a-119">Remarks</span></span>

<span data-ttu-id="96a6a-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="96a6a-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="96a6a-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="96a6a-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="96a6a-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="96a6a-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="96a6a-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="96a6a-123">Schema Name</span></span>  <br/> |<span data-ttu-id="96a6a-124">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="96a6a-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="96a6a-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="96a6a-125">Validation File</span></span>  <br/> |<span data-ttu-id="96a6a-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="96a6a-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="96a6a-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="96a6a-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="96a6a-128">True</span><span class="sxs-lookup"><span data-stu-id="96a6a-128">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="96a6a-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="96a6a-129">See also</span></span>



- [<span data-ttu-id="96a6a-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="96a6a-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

