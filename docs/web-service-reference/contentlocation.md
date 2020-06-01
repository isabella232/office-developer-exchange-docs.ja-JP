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
description: ContentLocation 要素には、添付ファイルのコンテンツの場所に対応する Uniform Resource Identifier (URI) が含まれています。
ms.openlocfilehash: 01bb95da5f620fddc8777f88b1d3eb1a7e6069b1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461486"
---
# <a name="contentlocation"></a><span data-ttu-id="c5c77-103">ContentLocation</span><span class="sxs-lookup"><span data-stu-id="c5c77-103">ContentLocation</span></span>

<span data-ttu-id="c5c77-104">**Contentlocation**要素には、添付ファイルのコンテンツの場所に対応する Uniform resource IDENTIFIER (URI) が含まれています。</span><span class="sxs-lookup"><span data-stu-id="c5c77-104">The **ContentLocation** element contains the Uniform Resource Identifier (URI) that corresponds to the location of the content of an attachment.</span></span> 
  
```xml
<ContentLocation/>
```

 <span data-ttu-id="c5c77-105">**String**</span><span class="sxs-lookup"><span data-stu-id="c5c77-105">**String**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c5c77-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="c5c77-106">Attributes and elements</span></span>

<span data-ttu-id="c5c77-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c5c77-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c5c77-108">属性</span><span class="sxs-lookup"><span data-stu-id="c5c77-108">Attributes</span></span>

<span data-ttu-id="c5c77-109">なし。</span><span class="sxs-lookup"><span data-stu-id="c5c77-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c5c77-110">子要素</span><span class="sxs-lookup"><span data-stu-id="c5c77-110">Child elements</span></span>

<span data-ttu-id="c5c77-111">なし。</span><span class="sxs-lookup"><span data-stu-id="c5c77-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c5c77-112">親要素</span><span class="sxs-lookup"><span data-stu-id="c5c77-112">Parent elements</span></span>

|<span data-ttu-id="c5c77-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="c5c77-113">**Element**</span></span>|<span data-ttu-id="c5c77-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="c5c77-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c5c77-115">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="c5c77-115">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="c5c77-116">別の Exchange アイテムに関連付けられている Exchange アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="c5c77-116">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="c5c77-117">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="c5c77-117">FileAttachment</span></span>](fileattachment.md) <br/> |<span data-ttu-id="c5c77-118">Exchange ストア内のアイテムに添付されているファイルを表します。</span><span class="sxs-lookup"><span data-stu-id="c5c77-118">Represents a file that is attached to an item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c5c77-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="c5c77-119">Text value</span></span>

<span data-ttu-id="c5c77-120">テキスト値は、URI を表す文字列型 (string) の値です。</span><span class="sxs-lookup"><span data-stu-id="c5c77-120">The text value is a string value that represents a URI.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c5c77-121">注釈</span><span class="sxs-lookup"><span data-stu-id="c5c77-121">Remarks</span></span>

<span data-ttu-id="c5c77-122">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="c5c77-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c5c77-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="c5c77-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c5c77-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="c5c77-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c5c77-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c5c77-125">Schema name</span></span>  <br/> |<span data-ttu-id="c5c77-126">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="c5c77-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="c5c77-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c5c77-127">Validation file</span></span>  <br/> |<span data-ttu-id="c5c77-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="c5c77-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c5c77-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="c5c77-129">Can be empty</span></span>  <br/> |<span data-ttu-id="c5c77-130">正しくない</span><span class="sxs-lookup"><span data-stu-id="c5c77-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c5c77-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="c5c77-131">See also</span></span>



- [<span data-ttu-id="c5c77-132">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="c5c77-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

