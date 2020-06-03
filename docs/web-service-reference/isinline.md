---
title: IsInline
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsInline
api_type:
- schema
ms.assetid: 5e7712c8-372a-4a16-be64-360c5ff3961a
description: IsInline 要素は、添付ファイルがアイテム内にインラインで表示されるかどうかを表します。
ms.openlocfilehash: 2b3b6392fe8867ae9782dcb7211c17f4f4d9becd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464211"
---
# <a name="isinline"></a><span data-ttu-id="431de-103">IsInline</span><span class="sxs-lookup"><span data-stu-id="431de-103">IsInline</span></span>

<span data-ttu-id="431de-104">**Isinline**要素は、添付ファイルがアイテム内にインラインで表示されるかどうかを表します。</span><span class="sxs-lookup"><span data-stu-id="431de-104">The **IsInline** element represents whether the attachment appears inline within an item.</span></span> 
  
```xml
<IsInline>true or false</IsInline>
```

 <span data-ttu-id="431de-105">**boolean**</span><span class="sxs-lookup"><span data-stu-id="431de-105">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="431de-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="431de-106">Attributes and elements</span></span>

<span data-ttu-id="431de-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="431de-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="431de-108">属性</span><span class="sxs-lookup"><span data-stu-id="431de-108">Attributes</span></span>

<span data-ttu-id="431de-109">なし。</span><span class="sxs-lookup"><span data-stu-id="431de-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="431de-110">子要素</span><span class="sxs-lookup"><span data-stu-id="431de-110">Child elements</span></span>

<span data-ttu-id="431de-111">なし。</span><span class="sxs-lookup"><span data-stu-id="431de-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="431de-112">親要素</span><span class="sxs-lookup"><span data-stu-id="431de-112">Parent elements</span></span>

|<span data-ttu-id="431de-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="431de-113">**Element**</span></span>|<span data-ttu-id="431de-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="431de-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="431de-115">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="431de-115">FileAttachment</span></span>](fileattachment.md) <br/> |<span data-ttu-id="431de-116">Exchange ストア内のアイテムに添付されているファイルを表します。</span><span class="sxs-lookup"><span data-stu-id="431de-116">Represents a file that is attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="431de-117">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="431de-117">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="431de-118">別の Exchange アイテムに関連付けられている Exchange アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="431de-118">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="431de-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="431de-119">Text value</span></span>

<span data-ttu-id="431de-120">この要素は、 **true**または**false**のいずれかになります。</span><span class="sxs-lookup"><span data-stu-id="431de-120">This element can be either **true** or **false**.</span></span> <span data-ttu-id="431de-121">既定値は **false** です。</span><span class="sxs-lookup"><span data-stu-id="431de-121">The default value is **false**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="431de-122">注釈</span><span class="sxs-lookup"><span data-stu-id="431de-122">Remarks</span></span>

<span data-ttu-id="431de-123">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="431de-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="431de-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="431de-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="431de-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="431de-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="431de-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="431de-126">Schema Name</span></span>  <br/> |<span data-ttu-id="431de-127">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="431de-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="431de-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="431de-128">Validation File</span></span>  <br/> |<span data-ttu-id="431de-129">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="431de-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="431de-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="431de-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="431de-131">正しくない</span><span class="sxs-lookup"><span data-stu-id="431de-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="431de-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="431de-132">See also</span></span>



- [<span data-ttu-id="431de-133">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="431de-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

