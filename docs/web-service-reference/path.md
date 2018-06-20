---
title: パス
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Path
api_type:
- schema
ms.assetid: 5829149e-7bfe-4820-bcc6-910e9264acc9
description: Path 要素は、プロパティ識別子のすべてのスキーマの基本型です。 この型は抽象であり、インスタンス ドキュメント内で直接発生ことはありません。
ms.openlocfilehash: a5a1ca5179ccf339e5a1f15621c92e2870f4f2d9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832700"
---
# <a name="path"></a><span data-ttu-id="403f0-104">パス</span><span class="sxs-lookup"><span data-stu-id="403f0-104">Path</span></span>

<span data-ttu-id="403f0-105">**Path**要素は、プロパティ識別子のすべてのスキーマの基本型です。</span><span class="sxs-lookup"><span data-stu-id="403f0-105">The **Path** element is the base schema type for all property identifiers.</span></span> <span data-ttu-id="403f0-106">この型は抽象であり、インスタンス ドキュメント内で直接発生ことはありません。</span><span class="sxs-lookup"><span data-stu-id="403f0-106">This type is abstract and will never occur directly within instance documents.</span></span> 
  
```xml
<Path/>
```

 <span data-ttu-id="403f0-107">**BasePathToElementType**</span><span class="sxs-lookup"><span data-stu-id="403f0-107">**BasePathToElementType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="403f0-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="403f0-108">Attributes and elements</span></span>

<span data-ttu-id="403f0-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="403f0-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="403f0-110">属性</span><span class="sxs-lookup"><span data-stu-id="403f0-110">Attributes</span></span>

<span data-ttu-id="403f0-111">なし。</span><span class="sxs-lookup"><span data-stu-id="403f0-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="403f0-112">子要素</span><span class="sxs-lookup"><span data-stu-id="403f0-112">Child elements</span></span>

<span data-ttu-id="403f0-113">なし。</span><span class="sxs-lookup"><span data-stu-id="403f0-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="403f0-114">親要素</span><span class="sxs-lookup"><span data-stu-id="403f0-114">Parent elements</span></span>

<span data-ttu-id="403f0-115">なし。</span><span class="sxs-lookup"><span data-stu-id="403f0-115">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="403f0-116">備考</span><span class="sxs-lookup"><span data-stu-id="403f0-116">Remarks</span></span>

<span data-ttu-id="403f0-117">次の要素は、**パス**要素の代わりに使用されます。</span><span class="sxs-lookup"><span data-stu-id="403f0-117">The following elements are used to substitute for the **Path** element:</span></span> 
  
- [<span data-ttu-id="403f0-118">FieldURI</span><span class="sxs-lookup"><span data-stu-id="403f0-118">FieldURI</span></span>](fielduri.md)
    
- [<span data-ttu-id="403f0-119">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="403f0-119">IndexedFieldURI</span></span>](indexedfielduri.md)
    
- [<span data-ttu-id="403f0-120">ExceptionFieldURI</span><span class="sxs-lookup"><span data-stu-id="403f0-120">ExceptionFieldURI</span></span>](exceptionfielduri.md)
    
- [<span data-ttu-id="403f0-121">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="403f0-121">ExtendedFieldURI</span></span>](extendedfielduri.md)
    
<span data-ttu-id="403f0-122">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="403f0-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="403f0-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="403f0-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="403f0-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="403f0-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="403f0-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="403f0-125">Schema Name</span></span>  <br/> |<span data-ttu-id="403f0-126">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="403f0-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="403f0-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="403f0-127">Validation File</span></span>  <br/> |<span data-ttu-id="403f0-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="403f0-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="403f0-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="403f0-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="403f0-130">False</span><span class="sxs-lookup"><span data-stu-id="403f0-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="403f0-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="403f0-131">See also</span></span>



- [<span data-ttu-id="403f0-132">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="403f0-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

