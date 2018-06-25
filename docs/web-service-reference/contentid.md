---
title: ContentId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContentId
api_type:
- schema
ms.assetid: bc59100d-6079-414b-a6e0-7c15feaa3184
description: ContentId 要素は、添付ファイルの内容の識別子を表します。 ContentId は、任意の文字列値に設定できます。 アプリケーションは、独自の識別メカニズムを実装するために、ContentId を使用できます。
ms.openlocfilehash: dc46ae4b33d435f5d47eb7deb39e92fd0170194b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759737"
---
# <a name="contentid"></a><span data-ttu-id="a495b-105">ContentId</span><span class="sxs-lookup"><span data-stu-id="a495b-105">ContentId</span></span>

<span data-ttu-id="a495b-106">**ContentId**要素は、添付ファイルの内容の識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="a495b-106">The **ContentId** element represents an identifier for the contents of an attachment.</span></span> <span data-ttu-id="a495b-107">**ContentId**は、任意の文字列値に設定できます。</span><span class="sxs-lookup"><span data-stu-id="a495b-107">**ContentId** can be set to any string value.</span></span> <span data-ttu-id="a495b-108">アプリケーションは、独自の識別メカニズムを実装するために、 **ContentId**を使用できます。</span><span class="sxs-lookup"><span data-stu-id="a495b-108">Applications can use **ContentId** to implement their own identification mechanisms.</span></span> 
  
```xml
<ContentId/>
```

 <span data-ttu-id="a495b-109">**文字列型 (String)**</span><span class="sxs-lookup"><span data-stu-id="a495b-109">**String**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a495b-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="a495b-110">Attributes and elements</span></span>

<span data-ttu-id="a495b-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a495b-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a495b-112">属性</span><span class="sxs-lookup"><span data-stu-id="a495b-112">Attributes</span></span>

<span data-ttu-id="a495b-113">なし。</span><span class="sxs-lookup"><span data-stu-id="a495b-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a495b-114">子要素</span><span class="sxs-lookup"><span data-stu-id="a495b-114">Child elements</span></span>

<span data-ttu-id="a495b-115">なし。</span><span class="sxs-lookup"><span data-stu-id="a495b-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a495b-116">親要素</span><span class="sxs-lookup"><span data-stu-id="a495b-116">Parent elements</span></span>

|<span data-ttu-id="a495b-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="a495b-117">**Element**</span></span>|<span data-ttu-id="a495b-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="a495b-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a495b-119">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="a495b-119">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="a495b-120">Exchange の他のアイテムに関連付けられている Exchange アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="a495b-120">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="a495b-121">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="a495b-121">FileAttachment</span></span>](fileattachment.md) <br/> |<span data-ttu-id="a495b-122">Exchange ストア内のアイテムに関連付けられているファイルを表します。</span><span class="sxs-lookup"><span data-stu-id="a495b-122">Represents a file that is attached to an item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a495b-123">テキスト値</span><span class="sxs-lookup"><span data-stu-id="a495b-123">Text value</span></span>

<span data-ttu-id="a495b-124">文字列値は、添付ファイルの内容に識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="a495b-124">The string value represents the identifier to the contents of an attachment.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a495b-125">備考</span><span class="sxs-lookup"><span data-stu-id="a495b-125">Remarks</span></span>

<span data-ttu-id="a495b-126">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="a495b-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a495b-127">要素情報</span><span class="sxs-lookup"><span data-stu-id="a495b-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a495b-128">名前空間</span><span class="sxs-lookup"><span data-stu-id="a495b-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a495b-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a495b-129">Schema name</span></span>  <br/> |<span data-ttu-id="a495b-130">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="a495b-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="a495b-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a495b-131">Validation file</span></span>  <br/> |<span data-ttu-id="a495b-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a495b-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a495b-133">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="a495b-133">Can be empty</span></span>  <br/> |<span data-ttu-id="a495b-134">False</span><span class="sxs-lookup"><span data-stu-id="a495b-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a495b-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="a495b-135">See also</span></span>



- [<span data-ttu-id="a495b-136">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="a495b-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

