---
title: Generation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Generation
api_type:
- schema
ms.assetid: a4812843-8aec-4fc4-945f-3aeb17a6593a
description: 生成要素では、連絡先の完全な名前を次世代の省略形を表します。
ms.openlocfilehash: 2b6be1a96223da8c70b042475cc7c8f0a67c000b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760621"
---
# <a name="generation"></a><span data-ttu-id="c3868-103">Generation</span><span class="sxs-lookup"><span data-stu-id="c3868-103">Generation</span></span>

<span data-ttu-id="c3868-104">**生成**要素では、連絡先の完全な名前を次世代の省略形を表します。</span><span class="sxs-lookup"><span data-stu-id="c3868-104">The **Generation** element represents a generational abbreviation that follows the full name of a contact.</span></span> 
  
```xml
<Generation/>
```

 <span data-ttu-id="c3868-105">**文字列型 (String)**</span><span class="sxs-lookup"><span data-stu-id="c3868-105">**String**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c3868-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="c3868-106">Attributes and elements</span></span>

<span data-ttu-id="c3868-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c3868-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c3868-108">属性</span><span class="sxs-lookup"><span data-stu-id="c3868-108">Attributes</span></span>

<span data-ttu-id="c3868-109">なし。</span><span class="sxs-lookup"><span data-stu-id="c3868-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c3868-110">子要素</span><span class="sxs-lookup"><span data-stu-id="c3868-110">Child elements</span></span>

<span data-ttu-id="c3868-111">なし。</span><span class="sxs-lookup"><span data-stu-id="c3868-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c3868-112">親要素</span><span class="sxs-lookup"><span data-stu-id="c3868-112">Parent elements</span></span>

|<span data-ttu-id="c3868-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="c3868-113">**Element**</span></span>|<span data-ttu-id="c3868-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="c3868-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c3868-115">Contact</span><span class="sxs-lookup"><span data-stu-id="c3868-115">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="c3868-116">Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="c3868-116">Represents an Exchange contact item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c3868-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="c3868-117">Text value</span></span>

<span data-ttu-id="c3868-118">テキスト値は、この要素が使用される場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="c3868-118">A text value is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c3868-119">備考</span><span class="sxs-lookup"><span data-stu-id="c3868-119">Remarks</span></span>

<span data-ttu-id="c3868-120">この要素は、PR_Generation の MAPI プロパティで表される同じ情報を表します。</span><span class="sxs-lookup"><span data-stu-id="c3868-120">This element represents the same information that is represented by the PR_Generation MAPI property.</span></span>
  
<span data-ttu-id="c3868-121">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="c3868-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c3868-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="c3868-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c3868-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="c3868-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c3868-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c3868-124">Schema name</span></span>  <br/> |<span data-ttu-id="c3868-125">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="c3868-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="c3868-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c3868-126">Validation file</span></span>  <br/> |<span data-ttu-id="c3868-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c3868-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c3868-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="c3868-128">Can be empty</span></span>  <br/> |<span data-ttu-id="c3868-129">False</span><span class="sxs-lookup"><span data-stu-id="c3868-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c3868-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="c3868-130">See also</span></span>



- [<span data-ttu-id="c3868-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="c3868-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="c3868-132">連絡先 (Exchange Web サービス) を作成します。</span><span class="sxs-lookup"><span data-stu-id="c3868-132">Creating Contacts (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)
  
[<span data-ttu-id="c3868-133">連絡先を更新</span><span class="sxs-lookup"><span data-stu-id="c3868-133">Updating Contacts</span></span>](http://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
  
[<span data-ttu-id="c3868-134">連絡先を削除します。</span><span class="sxs-lookup"><span data-stu-id="c3868-134">Deleting Contacts</span></span>](http://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

