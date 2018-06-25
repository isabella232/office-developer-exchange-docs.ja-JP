---
title: BaseItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- BaseItemId
api_type:
- schema
ms.assetid: c762e60e-08bb-430a-af5e-fa991f33a44f
description: BaseItemId 要素は、id が、メールボックス内のアイテムを表す基本クラスを表します。 これは抽象クラスであり、したがって、インスタンス ドキュメントでは発生しません。
ms.openlocfilehash: 2befcaec905ba269e292cc5d3707f5e75e7633d9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759485"
---
# <a name="baseitemid"></a><span data-ttu-id="5ebfb-104">BaseItemId</span><span class="sxs-lookup"><span data-stu-id="5ebfb-104">BaseItemId</span></span>

<span data-ttu-id="5ebfb-105">**BaseItemId**要素は、id が、メールボックス内のアイテムを表す基本クラスを表します。</span><span class="sxs-lookup"><span data-stu-id="5ebfb-105">The **BaseItemId** element represents the base class for IDs that represent items in a mailbox.</span></span> <span data-ttu-id="5ebfb-106">これは抽象クラスであり、したがって、インスタンス ドキュメントでは発生しません。</span><span class="sxs-lookup"><span data-stu-id="5ebfb-106">This is an abstract class and therefore will not occur in an instance document.</span></span> 
  
```xml
<BaseItemId/>
```

 <span data-ttu-id="5ebfb-107">**BaseItemIdType**</span><span class="sxs-lookup"><span data-stu-id="5ebfb-107">**BaseItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5ebfb-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="5ebfb-108">Attributes and elements</span></span>

<span data-ttu-id="5ebfb-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5ebfb-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5ebfb-110">属性</span><span class="sxs-lookup"><span data-stu-id="5ebfb-110">Attributes</span></span>

<span data-ttu-id="5ebfb-111">なし。</span><span class="sxs-lookup"><span data-stu-id="5ebfb-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5ebfb-112">子要素</span><span class="sxs-lookup"><span data-stu-id="5ebfb-112">Child elements</span></span>

<span data-ttu-id="5ebfb-113">なし。</span><span class="sxs-lookup"><span data-stu-id="5ebfb-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5ebfb-114">親要素</span><span class="sxs-lookup"><span data-stu-id="5ebfb-114">Parent elements</span></span>

<span data-ttu-id="5ebfb-115">なし。</span><span class="sxs-lookup"><span data-stu-id="5ebfb-115">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5ebfb-116">備考</span><span class="sxs-lookup"><span data-stu-id="5ebfb-116">Remarks</span></span>

<span data-ttu-id="5ebfb-117">この要素は、抽象基本型の項目の識別子です。</span><span class="sxs-lookup"><span data-stu-id="5ebfb-117">This element is an abstract base type for item identifiers.</span></span> <span data-ttu-id="5ebfb-118">Web サービスの呼び出しでは、この要素は使用されません。</span><span class="sxs-lookup"><span data-stu-id="5ebfb-118">This element is not used in Web service calls.</span></span>
  
<span data-ttu-id="5ebfb-119">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="5ebfb-119">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5ebfb-120">要素情報</span><span class="sxs-lookup"><span data-stu-id="5ebfb-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5ebfb-121">名前空間</span><span class="sxs-lookup"><span data-stu-id="5ebfb-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5ebfb-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5ebfb-122">Schema name</span></span>  <br/> |<span data-ttu-id="5ebfb-123">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="5ebfb-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="5ebfb-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5ebfb-124">Validation file</span></span>  <br/> |<span data-ttu-id="5ebfb-125">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5ebfb-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5ebfb-126">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="5ebfb-126">Can be empty</span></span>  <br/> |<span data-ttu-id="5ebfb-127">False</span><span class="sxs-lookup"><span data-stu-id="5ebfb-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5ebfb-128">関連項目</span><span class="sxs-lookup"><span data-stu-id="5ebfb-128">See also</span></span>



- [<span data-ttu-id="5ebfb-129">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="5ebfb-129">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

