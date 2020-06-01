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
description: ContentType 要素には、添付ファイルのコンテンツのマルチパーパスインターネットメール拡張 (MIME) の種類が記述されています。
ms.openlocfilehash: cb326bb761ea28e0e9f77501bf754c7c1f0318fb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455227"
---
# <a name="contenttype"></a><span data-ttu-id="d712a-103">ContentType</span><span class="sxs-lookup"><span data-stu-id="d712a-103">ContentType</span></span>

<span data-ttu-id="d712a-104">**ContentType**要素には、添付ファイルのコンテンツのマルチパーパスインターネットメール拡張 (MIME) の種類が記述されています。</span><span class="sxs-lookup"><span data-stu-id="d712a-104">The **ContentType** element describes the Multipurpose Internet Mail Extensions (MIME) type of the attachment content.</span></span> 
  
```xml
<ContentType/>
```

 <span data-ttu-id="d712a-105">**String**</span><span class="sxs-lookup"><span data-stu-id="d712a-105">**String**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d712a-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d712a-106">Attributes and elements</span></span>

<span data-ttu-id="d712a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d712a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d712a-108">属性</span><span class="sxs-lookup"><span data-stu-id="d712a-108">Attributes</span></span>

<span data-ttu-id="d712a-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d712a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d712a-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d712a-110">Child elements</span></span>

<span data-ttu-id="d712a-111">なし。</span><span class="sxs-lookup"><span data-stu-id="d712a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d712a-112">親要素</span><span class="sxs-lookup"><span data-stu-id="d712a-112">Parent elements</span></span>

|<span data-ttu-id="d712a-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="d712a-113">**Element**</span></span>|<span data-ttu-id="d712a-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="d712a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d712a-115">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="d712a-115">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="d712a-116">別の Exchange アイテムに関連付けられている Exchange アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="d712a-116">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="d712a-117">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="d712a-117">FileAttachment</span></span>](fileattachment.md) <br/> |<span data-ttu-id="d712a-118">Exchange ストア内のアイテムに添付されているファイルを表します。</span><span class="sxs-lookup"><span data-stu-id="d712a-118">Represents a file that is attached to an item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d712a-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="d712a-119">Text value</span></span>

<span data-ttu-id="d712a-120">テキスト値は、添付ファイルのコンテンツタイプを表す文字列型 (string) の値です。</span><span class="sxs-lookup"><span data-stu-id="d712a-120">The text value is a string value that represents the content type of the attachment.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d712a-121">注釈</span><span class="sxs-lookup"><span data-stu-id="d712a-121">Remarks</span></span>

<span data-ttu-id="d712a-122">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="d712a-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d712a-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d712a-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d712a-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="d712a-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d712a-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d712a-125">Schema name</span></span>  <br/> |<span data-ttu-id="d712a-126">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="d712a-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="d712a-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d712a-127">Validation file</span></span>  <br/> |<span data-ttu-id="d712a-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="d712a-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d712a-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="d712a-129">Can be empty</span></span>  <br/> |<span data-ttu-id="d712a-130">正しくない</span><span class="sxs-lookup"><span data-stu-id="d712a-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d712a-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="d712a-131">See also</span></span>



- [<span data-ttu-id="d712a-132">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="d712a-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

