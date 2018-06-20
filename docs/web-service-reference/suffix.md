---
title: Suffix
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Suffix
api_type:
- schema
ms.assetid: ead92079-c4a7-4f54-a132-86653b488bdb
description: サフィックスの要素は、連絡先の名前にサフィックスを表します。
ms.openlocfilehash: 4d5bde0ca68769cf63b2bb4f00c5b68b316169a9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839620"
---
# <a name="suffix"></a><span data-ttu-id="e9379-103">Suffix</span><span class="sxs-lookup"><span data-stu-id="e9379-103">Suffix</span></span>

<span data-ttu-id="e9379-104">**サフィックス**の要素は、連絡先の名前にサフィックスを表します。</span><span class="sxs-lookup"><span data-stu-id="e9379-104">The **Suffix** element represents a suffix to a contact's name.</span></span> 
  
```xml
<Suffix/>
```

 <span data-ttu-id="e9379-105">**string**</span><span class="sxs-lookup"><span data-stu-id="e9379-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e9379-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="e9379-106">Attributes and elements</span></span>

<span data-ttu-id="e9379-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e9379-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e9379-108">属性</span><span class="sxs-lookup"><span data-stu-id="e9379-108">Attributes</span></span>

<span data-ttu-id="e9379-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e9379-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e9379-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e9379-110">Child elements</span></span>

<span data-ttu-id="e9379-111">なし。</span><span class="sxs-lookup"><span data-stu-id="e9379-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e9379-112">親要素</span><span class="sxs-lookup"><span data-stu-id="e9379-112">Parent elements</span></span>

|<span data-ttu-id="e9379-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="e9379-113">**Element**</span></span>|<span data-ttu-id="e9379-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="e9379-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e9379-115">CompleteName</span><span class="sxs-lookup"><span data-stu-id="e9379-115">CompleteName</span></span>](completename.md) <br/> |<span data-ttu-id="e9379-116">連絡先の完全な名前を表します。</span><span class="sxs-lookup"><span data-stu-id="e9379-116">Represents the complete name of a contact.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e9379-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="e9379-117">Text value</span></span>

<span data-ttu-id="e9379-118">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="e9379-118">A text value is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e9379-119">備考</span><span class="sxs-lookup"><span data-stu-id="e9379-119">Remarks</span></span>

<span data-ttu-id="e9379-120">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="e9379-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e9379-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="e9379-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e9379-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="e9379-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e9379-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e9379-123">Schema name</span></span>  <br/> |<span data-ttu-id="e9379-124">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="e9379-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="e9379-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e9379-125">Validation file</span></span>  <br/> |<span data-ttu-id="e9379-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e9379-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e9379-127">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="e9379-127">Can be empty</span></span>  <br/> |<span data-ttu-id="e9379-128">False</span><span class="sxs-lookup"><span data-stu-id="e9379-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e9379-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="e9379-129">See also</span></span>



- [<span data-ttu-id="e9379-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="e9379-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="e9379-131">連絡先 (Exchange Web サービス) を作成します。</span><span class="sxs-lookup"><span data-stu-id="e9379-131">Creating Contacts (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)

