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
description: コンテンツ要素には、Base64 でエンコードされた添付ファイルの内容が含まれています。
ms.openlocfilehash: 20afe6286d3efaa5da6cdc88e397e88fddb1d8c6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759730"
---
# <a name="content"></a><span data-ttu-id="e8875-103">コンテンツ</span><span class="sxs-lookup"><span data-stu-id="e8875-103">Content</span></span>

<span data-ttu-id="e8875-104">**コンテンツ**要素には、Base64 でエンコードされた添付ファイルの内容が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e8875-104">The **Content** element contains the Base64-encoded contents of a file attachment.</span></span> 
  
```xml
<Content/>
```

 <span data-ttu-id="e8875-105">**Base64Binary**</span><span class="sxs-lookup"><span data-stu-id="e8875-105">**Base64Binary**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e8875-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="e8875-106">Attributes and elements</span></span>

<span data-ttu-id="e8875-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e8875-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e8875-108">属性</span><span class="sxs-lookup"><span data-stu-id="e8875-108">Attributes</span></span>

<span data-ttu-id="e8875-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e8875-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e8875-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e8875-110">Child elements</span></span>

<span data-ttu-id="e8875-111">なし。</span><span class="sxs-lookup"><span data-stu-id="e8875-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e8875-112">親要素</span><span class="sxs-lookup"><span data-stu-id="e8875-112">Parent elements</span></span>

|<span data-ttu-id="e8875-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="e8875-113">**Element**</span></span>|<span data-ttu-id="e8875-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="e8875-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e8875-115">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="e8875-115">FileAttachment</span></span>](fileattachment.md) <br/> |<span data-ttu-id="e8875-116">T のファイルを表しますが、Exchange ストア内の項目に thattached です。</span><span class="sxs-lookup"><span data-stu-id="e8875-116">Represents a file t is thattached to an item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e8875-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="e8875-117">Text value</span></span>

<span data-ttu-id="e8875-118">文字列値は、添付ファイルの Base64 でエンコードされたバイナリ データを表します。</span><span class="sxs-lookup"><span data-stu-id="e8875-118">The string value represents the Base64-encoded binary data of the file attachment.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e8875-119">備考</span><span class="sxs-lookup"><span data-stu-id="e8875-119">Remarks</span></span>

<span data-ttu-id="e8875-120">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="e8875-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e8875-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="e8875-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e8875-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="e8875-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e8875-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e8875-123">Schema name</span></span>  <br/> |<span data-ttu-id="e8875-124">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="e8875-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="e8875-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e8875-125">Validation file</span></span>  <br/> |<span data-ttu-id="e8875-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e8875-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e8875-127">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="e8875-127">Can be empty</span></span>  <br/> |<span data-ttu-id="e8875-128">False</span><span class="sxs-lookup"><span data-stu-id="e8875-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e8875-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="e8875-129">See also</span></span>



- [<span data-ttu-id="e8875-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="e8875-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

