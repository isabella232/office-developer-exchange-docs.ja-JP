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
description: Generation 要素は、連絡先の完全な名前の後の省略形を表します。
ms.openlocfilehash: 75246153d19632c1a0ad245a460584731275565e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463021"
---
# <a name="generation"></a><span data-ttu-id="6af1e-103">Generation</span><span class="sxs-lookup"><span data-stu-id="6af1e-103">Generation</span></span>

<span data-ttu-id="6af1e-104">**Generation**要素は、連絡先の完全な名前の後の省略形を表します。</span><span class="sxs-lookup"><span data-stu-id="6af1e-104">The **Generation** element represents a generational abbreviation that follows the full name of a contact.</span></span> 
  
```xml
<Generation/>
```

 <span data-ttu-id="6af1e-105">**String**</span><span class="sxs-lookup"><span data-stu-id="6af1e-105">**String**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6af1e-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="6af1e-106">Attributes and elements</span></span>

<span data-ttu-id="6af1e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6af1e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6af1e-108">属性</span><span class="sxs-lookup"><span data-stu-id="6af1e-108">Attributes</span></span>

<span data-ttu-id="6af1e-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6af1e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6af1e-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6af1e-110">Child elements</span></span>

<span data-ttu-id="6af1e-111">なし。</span><span class="sxs-lookup"><span data-stu-id="6af1e-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6af1e-112">親要素</span><span class="sxs-lookup"><span data-stu-id="6af1e-112">Parent elements</span></span>

|<span data-ttu-id="6af1e-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="6af1e-113">**Element**</span></span>|<span data-ttu-id="6af1e-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="6af1e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6af1e-115">連絡先</span><span class="sxs-lookup"><span data-stu-id="6af1e-115">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="6af1e-116">Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="6af1e-116">Represents an Exchange contact item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6af1e-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="6af1e-117">Text value</span></span>

<span data-ttu-id="6af1e-118">この要素を使用する場合は、テキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="6af1e-118">A text value is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6af1e-119">注釈</span><span class="sxs-lookup"><span data-stu-id="6af1e-119">Remarks</span></span>

<span data-ttu-id="6af1e-120">この要素は、PR_Generation MAPI プロパティによって表される同じ情報を表します。</span><span class="sxs-lookup"><span data-stu-id="6af1e-120">This element represents the same information that is represented by the PR_Generation MAPI property.</span></span>
  
<span data-ttu-id="6af1e-121">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="6af1e-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6af1e-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="6af1e-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6af1e-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="6af1e-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6af1e-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6af1e-124">Schema name</span></span>  <br/> |<span data-ttu-id="6af1e-125">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="6af1e-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="6af1e-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6af1e-126">Validation file</span></span>  <br/> |<span data-ttu-id="6af1e-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="6af1e-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6af1e-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="6af1e-128">Can be empty</span></span>  <br/> |<span data-ttu-id="6af1e-129">正しくない</span><span class="sxs-lookup"><span data-stu-id="6af1e-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6af1e-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="6af1e-130">See also</span></span>



- [<span data-ttu-id="6af1e-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="6af1e-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="6af1e-132">連絡先の作成 (Exchange Web サービス)</span><span class="sxs-lookup"><span data-stu-id="6af1e-132">Creating Contacts (Exchange Web Services)</span></span>](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)
  
[<span data-ttu-id="6af1e-133">連絡先の更新</span><span class="sxs-lookup"><span data-stu-id="6af1e-133">Updating Contacts</span></span>](https://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
  
[<span data-ttu-id="6af1e-134">連絡先の削除</span><span class="sxs-lookup"><span data-stu-id="6af1e-134">Deleting Contacts</span></span>](https://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

