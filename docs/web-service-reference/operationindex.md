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
description: OperationIndex 要素は、ルールの操作エラーの原因となった、要求内の操作のインデックスを指定します。
ms.openlocfilehash: a95f194231200520d2f3feb328b3608e2921826c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462494"
---
# <a name="operationindex"></a><span data-ttu-id="4ed69-103">OperationIndex</span><span class="sxs-lookup"><span data-stu-id="4ed69-103">OperationIndex</span></span>

<span data-ttu-id="4ed69-104">**Operationindex**要素は、ルールの操作エラーの原因となった、要求内の操作のインデックスを指定します。</span><span class="sxs-lookup"><span data-stu-id="4ed69-104">The **OperationIndex** element specifies the index of the operation in the request that caused the rule operation error.</span></span> 
  
```XML
<OperationIndex/>
```

 <span data-ttu-id="4ed69-105">**int**</span><span class="sxs-lookup"><span data-stu-id="4ed69-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4ed69-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="4ed69-106">Attributes and elements</span></span>

<span data-ttu-id="4ed69-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4ed69-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4ed69-108">属性</span><span class="sxs-lookup"><span data-stu-id="4ed69-108">Attributes</span></span>

<span data-ttu-id="4ed69-109">なし。</span><span class="sxs-lookup"><span data-stu-id="4ed69-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4ed69-110">子要素</span><span class="sxs-lookup"><span data-stu-id="4ed69-110">Child elements</span></span>

<span data-ttu-id="4ed69-111">なし。</span><span class="sxs-lookup"><span data-stu-id="4ed69-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4ed69-112">親要素</span><span class="sxs-lookup"><span data-stu-id="4ed69-112">Parent elements</span></span>

|<span data-ttu-id="4ed69-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="4ed69-113">**Element**</span></span>|<span data-ttu-id="4ed69-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="4ed69-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4ed69-115">RuleOperationError</span><span class="sxs-lookup"><span data-stu-id="4ed69-115">RuleOperationError</span></span>](ruleoperationerror.md) <br/> |<span data-ttu-id="4ed69-116">ルール操作エラーを表します。</span><span class="sxs-lookup"><span data-stu-id="4ed69-116">Represents a rule operation error.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4ed69-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="4ed69-117">Text value</span></span>

<span data-ttu-id="4ed69-118">なし</span><span class="sxs-lookup"><span data-stu-id="4ed69-118">None</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4ed69-119">注釈</span><span class="sxs-lookup"><span data-stu-id="4ed69-119">Remarks</span></span>

<span data-ttu-id="4ed69-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="4ed69-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4ed69-121">要素の情報</span><span class="sxs-lookup"><span data-stu-id="4ed69-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4ed69-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="4ed69-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4ed69-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4ed69-123">Schema Name</span></span>  <br/> |<span data-ttu-id="4ed69-124">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="4ed69-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4ed69-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4ed69-125">Validation File</span></span>  <br/> |<span data-ttu-id="4ed69-126">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="4ed69-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4ed69-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="4ed69-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="4ed69-128">正しい</span><span class="sxs-lookup"><span data-stu-id="4ed69-128">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4ed69-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="4ed69-129">See also</span></span>



- [<span data-ttu-id="4ed69-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="4ed69-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

