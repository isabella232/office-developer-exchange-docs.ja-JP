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
description: Path 要素は、すべてのプロパティ識別子の基本スキーマの種類です。 この型は abstract で、インスタンスドキュメント内で直接発生することはありません。
ms.openlocfilehash: 5ba18084243e9720a76b9ac28023778c6d546bc4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529015"
---
# <a name="path"></a><span data-ttu-id="2c331-104">パス</span><span class="sxs-lookup"><span data-stu-id="2c331-104">Path</span></span>

<span data-ttu-id="2c331-105">**Path**要素は、すべてのプロパティ識別子の基本スキーマの種類です。</span><span class="sxs-lookup"><span data-stu-id="2c331-105">The **Path** element is the base schema type for all property identifiers.</span></span> <span data-ttu-id="2c331-106">この型は abstract で、インスタンスドキュメント内で直接発生することはありません。</span><span class="sxs-lookup"><span data-stu-id="2c331-106">This type is abstract and will never occur directly within instance documents.</span></span> 
  
```xml
<Path/>
```

 <span data-ttu-id="2c331-107">**BasePathToElementType**</span><span class="sxs-lookup"><span data-stu-id="2c331-107">**BasePathToElementType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2c331-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="2c331-108">Attributes and elements</span></span>

<span data-ttu-id="2c331-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2c331-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2c331-110">属性</span><span class="sxs-lookup"><span data-stu-id="2c331-110">Attributes</span></span>

<span data-ttu-id="2c331-111">なし。</span><span class="sxs-lookup"><span data-stu-id="2c331-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2c331-112">子要素</span><span class="sxs-lookup"><span data-stu-id="2c331-112">Child elements</span></span>

<span data-ttu-id="2c331-113">なし。</span><span class="sxs-lookup"><span data-stu-id="2c331-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2c331-114">親要素</span><span class="sxs-lookup"><span data-stu-id="2c331-114">Parent elements</span></span>

<span data-ttu-id="2c331-115">なし。</span><span class="sxs-lookup"><span data-stu-id="2c331-115">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2c331-116">注釈</span><span class="sxs-lookup"><span data-stu-id="2c331-116">Remarks</span></span>

<span data-ttu-id="2c331-117">**Path**要素を置き換えるには、次の要素を使用します。</span><span class="sxs-lookup"><span data-stu-id="2c331-117">The following elements are used to substitute for the **Path** element:</span></span> 
  
- [<span data-ttu-id="2c331-118">FieldURI</span><span class="sxs-lookup"><span data-stu-id="2c331-118">FieldURI</span></span>](fielduri.md)
    
- [<span data-ttu-id="2c331-119">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="2c331-119">IndexedFieldURI</span></span>](indexedfielduri.md)
    
- [<span data-ttu-id="2c331-120">ExceptionFieldURI</span><span class="sxs-lookup"><span data-stu-id="2c331-120">ExceptionFieldURI</span></span>](exceptionfielduri.md)
    
- [<span data-ttu-id="2c331-121">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="2c331-121">ExtendedFieldURI</span></span>](extendedfielduri.md)
    
<span data-ttu-id="2c331-122">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="2c331-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2c331-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="2c331-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2c331-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="2c331-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2c331-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2c331-125">Schema Name</span></span>  <br/> |<span data-ttu-id="2c331-126">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="2c331-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="2c331-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2c331-127">Validation File</span></span>  <br/> |<span data-ttu-id="2c331-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="2c331-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2c331-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="2c331-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="2c331-130">正しくない</span><span class="sxs-lookup"><span data-stu-id="2c331-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2c331-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="2c331-131">See also</span></span>



- [<span data-ttu-id="2c331-132">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="2c331-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

