---
title: ContentType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContentType
api_type:
- schema
ms.assetid: f91ff0df-0d8a-43ea-a188-d80f0e885f19
description: ContentType 要素では、添付ファイルのコンテンツの多目的インターネット メール拡張 (MIME) の種類について説明します。
ms.openlocfilehash: 489df47343051623d5b6a98557f2bd434a5dad52
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759745"
---
# <a name="contenttype"></a><span data-ttu-id="f2ac4-103">ContentType</span><span class="sxs-lookup"><span data-stu-id="f2ac4-103">ContentType</span></span>

<span data-ttu-id="f2ac4-104">**ContentType**要素では、添付ファイルのコンテンツの多目的インターネット メール拡張 (MIME) の種類について説明します。</span><span class="sxs-lookup"><span data-stu-id="f2ac4-104">The **ContentType** element describes the Multipurpose Internet Mail Extensions (MIME) type of the attachment content.</span></span> 
  
```xml
<ContentType/>
```

 <span data-ttu-id="f2ac4-105">**文字列型 (String)**</span><span class="sxs-lookup"><span data-stu-id="f2ac4-105">**String**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f2ac4-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="f2ac4-106">Attributes and elements</span></span>

<span data-ttu-id="f2ac4-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f2ac4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f2ac4-108">属性</span><span class="sxs-lookup"><span data-stu-id="f2ac4-108">Attributes</span></span>

<span data-ttu-id="f2ac4-109">なし。</span><span class="sxs-lookup"><span data-stu-id="f2ac4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f2ac4-110">子要素</span><span class="sxs-lookup"><span data-stu-id="f2ac4-110">Child elements</span></span>

<span data-ttu-id="f2ac4-111">なし。</span><span class="sxs-lookup"><span data-stu-id="f2ac4-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f2ac4-112">親要素</span><span class="sxs-lookup"><span data-stu-id="f2ac4-112">Parent elements</span></span>

|<span data-ttu-id="f2ac4-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="f2ac4-113">**Element**</span></span>|<span data-ttu-id="f2ac4-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="f2ac4-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f2ac4-115">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="f2ac4-115">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="f2ac4-116">Exchange の他のアイテムに関連付けられている Exchange アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="f2ac4-116">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="f2ac4-117">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="f2ac4-117">FileAttachment</span></span>](fileattachment.md) <br/> |<span data-ttu-id="f2ac4-118">Exchange ストア内のアイテムに関連付けられているファイルを表します。</span><span class="sxs-lookup"><span data-stu-id="f2ac4-118">Represents a file that is attached to an item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f2ac4-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="f2ac4-119">Text value</span></span>

<span data-ttu-id="f2ac4-120">テキスト値は、添付ファイルのコンテンツ タイプを表す文字列値です。</span><span class="sxs-lookup"><span data-stu-id="f2ac4-120">The text value is a string value that represents the content type of the attachment.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f2ac4-121">備考</span><span class="sxs-lookup"><span data-stu-id="f2ac4-121">Remarks</span></span>

<span data-ttu-id="f2ac4-122">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="f2ac4-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f2ac4-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="f2ac4-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f2ac4-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="f2ac4-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f2ac4-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f2ac4-125">Schema name</span></span>  <br/> |<span data-ttu-id="f2ac4-126">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="f2ac4-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="f2ac4-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f2ac4-127">Validation file</span></span>  <br/> |<span data-ttu-id="f2ac4-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f2ac4-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f2ac4-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="f2ac4-129">Can be empty</span></span>  <br/> |<span data-ttu-id="f2ac4-130">False</span><span class="sxs-lookup"><span data-stu-id="f2ac4-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f2ac4-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="f2ac4-131">See also</span></span>



- [<span data-ttu-id="f2ac4-132">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="f2ac4-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

