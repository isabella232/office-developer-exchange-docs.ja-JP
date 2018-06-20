---
title: State
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- State
api_type:
- schema
ms.assetid: bcce7b0e-d504-4a1f-a530-db80b207f201
description: 状態の要素は、連絡先アイテムの居住地の状態を表します。
ms.openlocfilehash: caa9541d30eaa04cc3f2dda0ebbf687b156c4f64
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833565"
---
# <a name="state"></a><span data-ttu-id="b9a65-103">State</span><span class="sxs-lookup"><span data-stu-id="b9a65-103">State</span></span>

<span data-ttu-id="b9a65-104">**状態**の要素は、連絡先アイテムの居住地の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="b9a65-104">The **State** element represents the state of residence for a contact item.</span></span> 
  
```xml
<State/>
```

<span data-ttu-id="b9a65-105">**string**</span><span class="sxs-lookup"><span data-stu-id="b9a65-105">**string**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="b9a65-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="b9a65-106">Attributes and elements</span></span>

<span data-ttu-id="b9a65-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b9a65-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b9a65-108">属性</span><span class="sxs-lookup"><span data-stu-id="b9a65-108">Attributes</span></span>

<span data-ttu-id="b9a65-109">なし。</span><span class="sxs-lookup"><span data-stu-id="b9a65-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b9a65-110">子要素</span><span class="sxs-lookup"><span data-stu-id="b9a65-110">Child elements</span></span>

<span data-ttu-id="b9a65-111">なし。</span><span class="sxs-lookup"><span data-stu-id="b9a65-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b9a65-112">親要素</span><span class="sxs-lookup"><span data-stu-id="b9a65-112">Parent elements</span></span>

|<span data-ttu-id="b9a65-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="b9a65-113">**Element**</span></span>|<span data-ttu-id="b9a65-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="b9a65-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b9a65-115">エントリ (PhysicalAddress)</span><span class="sxs-lookup"><span data-stu-id="b9a65-115">Entry (PhysicalAddress)</span></span>](entry-physicaladdress.md) <br/> |<span data-ttu-id="b9a65-116">連絡先アイテムの 1 つの物理アドレスをについて説明します。</span><span class="sxs-lookup"><span data-stu-id="b9a65-116">Describes a single physical address for a contact item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b9a65-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="b9a65-117">Text value</span></span>

<span data-ttu-id="b9a65-118">状態の名前を表す文字列値は、この要素が使用される場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="b9a65-118">A string value that represents the name of a state is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b9a65-119">備考</span><span class="sxs-lookup"><span data-stu-id="b9a65-119">Remarks</span></span>

<span data-ttu-id="b9a65-120">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="b9a65-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b9a65-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="b9a65-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b9a65-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="b9a65-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b9a65-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b9a65-123">Schema name</span></span>  <br/> |<span data-ttu-id="b9a65-124">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="b9a65-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="b9a65-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b9a65-125">Validation file</span></span>  <br/> |<span data-ttu-id="b9a65-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b9a65-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b9a65-127">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="b9a65-127">Can be empty</span></span>  <br/> |<span data-ttu-id="b9a65-128">False</span><span class="sxs-lookup"><span data-stu-id="b9a65-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b9a65-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="b9a65-129">See also</span></span>

- [<span data-ttu-id="b9a65-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="b9a65-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="b9a65-131">連絡先 (Exchange Web サービス) を作成します。</span><span class="sxs-lookup"><span data-stu-id="b9a65-131">Creating Contacts (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)
- [<span data-ttu-id="b9a65-132">連絡先を更新</span><span class="sxs-lookup"><span data-stu-id="b9a65-132">Updating Contacts</span></span>](http://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
- [<span data-ttu-id="b9a65-133">連絡先を削除します。</span><span class="sxs-lookup"><span data-stu-id="b9a65-133">Deleting Contacts</span></span>](http://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

