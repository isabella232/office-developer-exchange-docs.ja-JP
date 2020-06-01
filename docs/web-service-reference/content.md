---
title: コンテンツ
manager: sethgros
ms.date: 09/17/2015
ms.audience: ITPro
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Content
api_type:
- schema
ms.assetid: 24f8c54a-505f-4fc0-b7e7-93ad50b97070
description: Content 要素には、ファイル添付の Base64 でエンコードされたコンテンツが含まれています。
ms.openlocfilehash: 81f6acf69ff702bd0645663cb2e499ee5b45ea78
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458951"
---
# <a name="content"></a><span data-ttu-id="06453-103">コンテンツ</span><span class="sxs-lookup"><span data-stu-id="06453-103">Content</span></span>

<span data-ttu-id="06453-104">**Content**要素には、ファイル添付の Base64 でエンコードされたコンテンツが含まれています。</span><span class="sxs-lookup"><span data-stu-id="06453-104">The **Content** element contains the Base64-encoded contents of a file attachment.</span></span> 
  
```xml
<Content/>
```

 <span data-ttu-id="06453-105">**Base64Binary**</span><span class="sxs-lookup"><span data-stu-id="06453-105">**Base64Binary**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="06453-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="06453-106">Attributes and elements</span></span>

<span data-ttu-id="06453-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="06453-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="06453-108">属性</span><span class="sxs-lookup"><span data-stu-id="06453-108">Attributes</span></span>

<span data-ttu-id="06453-109">なし。</span><span class="sxs-lookup"><span data-stu-id="06453-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="06453-110">子要素</span><span class="sxs-lookup"><span data-stu-id="06453-110">Child elements</span></span>

<span data-ttu-id="06453-111">なし。</span><span class="sxs-lookup"><span data-stu-id="06453-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="06453-112">親要素</span><span class="sxs-lookup"><span data-stu-id="06453-112">Parent elements</span></span>

|<span data-ttu-id="06453-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="06453-113">**Element**</span></span>|<span data-ttu-id="06453-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="06453-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="06453-115">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="06453-115">FileAttachment</span></span>](fileattachment.md) <br/> |<span data-ttu-id="06453-116">Exchange ストア内のアイテムに関連付けられているファイル t を表します。</span><span class="sxs-lookup"><span data-stu-id="06453-116">Represents a file t is thattached to an item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="06453-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="06453-117">Text value</span></span>

<span data-ttu-id="06453-118">文字列型 (string) の値は、添付ファイルの Base64 でエンコードされたバイナリデータを表します。</span><span class="sxs-lookup"><span data-stu-id="06453-118">The string value represents the Base64-encoded binary data of the file attachment.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="06453-119">注釈</span><span class="sxs-lookup"><span data-stu-id="06453-119">Remarks</span></span>

<span data-ttu-id="06453-120">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="06453-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="06453-121">要素の情報</span><span class="sxs-lookup"><span data-stu-id="06453-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="06453-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="06453-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="06453-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="06453-123">Schema name</span></span>  <br/> |<span data-ttu-id="06453-124">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="06453-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="06453-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="06453-125">Validation file</span></span>  <br/> |<span data-ttu-id="06453-126">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="06453-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="06453-127">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="06453-127">Can be empty</span></span>  <br/> |<span data-ttu-id="06453-128">正しくない</span><span class="sxs-lookup"><span data-stu-id="06453-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="06453-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="06453-129">See also</span></span>



- [<span data-ttu-id="06453-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="06453-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

