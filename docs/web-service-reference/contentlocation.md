---
title: ContentLocation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContentLocation
api_type:
- schema
ms.assetid: d91cf587-24e3-4c13-8784-5ca29787cca7
description: ContentLocation 要素には、統一リソース識別子 (URI) の添付ファイルのコンテンツの場所に対応するが含まれています。
ms.openlocfilehash: 060dab2da653637420d5900bad3b95823c2e6ea3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759740"
---
# <a name="contentlocation"></a><span data-ttu-id="1a645-103">ContentLocation</span><span class="sxs-lookup"><span data-stu-id="1a645-103">ContentLocation</span></span>

<span data-ttu-id="1a645-104">**ContentLocation**要素には、統一リソース識別子 (URI) の添付ファイルのコンテンツの場所に対応するが含まれています。</span><span class="sxs-lookup"><span data-stu-id="1a645-104">The **ContentLocation** element contains the Uniform Resource Identifier (URI) that corresponds to the location of the content of an attachment.</span></span> 
  
```xml
<ContentLocation/>
```

 <span data-ttu-id="1a645-105">**文字列型 (String)**</span><span class="sxs-lookup"><span data-stu-id="1a645-105">**String**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1a645-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="1a645-106">Attributes and elements</span></span>

<span data-ttu-id="1a645-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1a645-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1a645-108">属性</span><span class="sxs-lookup"><span data-stu-id="1a645-108">Attributes</span></span>

<span data-ttu-id="1a645-109">なし。</span><span class="sxs-lookup"><span data-stu-id="1a645-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1a645-110">子要素</span><span class="sxs-lookup"><span data-stu-id="1a645-110">Child elements</span></span>

<span data-ttu-id="1a645-111">なし。</span><span class="sxs-lookup"><span data-stu-id="1a645-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1a645-112">親要素</span><span class="sxs-lookup"><span data-stu-id="1a645-112">Parent elements</span></span>

|<span data-ttu-id="1a645-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="1a645-113">**Element**</span></span>|<span data-ttu-id="1a645-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="1a645-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1a645-115">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="1a645-115">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="1a645-116">Exchange の他のアイテムに関連付けられている Exchange アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="1a645-116">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="1a645-117">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="1a645-117">FileAttachment</span></span>](fileattachment.md) <br/> |<span data-ttu-id="1a645-118">Exchange ストア内のアイテムに関連付けられているファイルを表します。</span><span class="sxs-lookup"><span data-stu-id="1a645-118">Represents a file that is attached to an item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1a645-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="1a645-119">Text value</span></span>

<span data-ttu-id="1a645-120">テキスト値は、URI を表す文字列値です。</span><span class="sxs-lookup"><span data-stu-id="1a645-120">The text value is a string value that represents a URI.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1a645-121">備考</span><span class="sxs-lookup"><span data-stu-id="1a645-121">Remarks</span></span>

<span data-ttu-id="1a645-122">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="1a645-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1a645-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="1a645-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1a645-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="1a645-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1a645-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1a645-125">Schema name</span></span>  <br/> |<span data-ttu-id="1a645-126">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="1a645-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="1a645-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1a645-127">Validation file</span></span>  <br/> |<span data-ttu-id="1a645-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1a645-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1a645-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="1a645-129">Can be empty</span></span>  <br/> |<span data-ttu-id="1a645-130">False</span><span class="sxs-lookup"><span data-stu-id="1a645-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1a645-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="1a645-131">See also</span></span>



- [<span data-ttu-id="1a645-132">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="1a645-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

