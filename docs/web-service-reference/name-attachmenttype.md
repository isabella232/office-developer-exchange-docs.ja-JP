---
title: 名 (AttachmentType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Name
api_type:
- schema
ms.assetid: 8ee00842-2d59-4346-9659-fa105bee747b
description: Name 要素は、添付ファイルの名前を表します。
ms.openlocfilehash: 5991874d784425efe3d9fc886c48dac2116e6edb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832499"
---
# <a name="name-attachmenttype"></a><span data-ttu-id="78db0-103">名 (AttachmentType)</span><span class="sxs-lookup"><span data-stu-id="78db0-103">Name (AttachmentType)</span></span>

<span data-ttu-id="78db0-104">**Name**要素は、添付ファイルの名前を表します。</span><span class="sxs-lookup"><span data-stu-id="78db0-104">The **Name** element represents the name of the attachment.</span></span> 
  
```xml
<Name/>
```

<span data-ttu-id="78db0-105">**string**</span><span class="sxs-lookup"><span data-stu-id="78db0-105">**string**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="78db0-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="78db0-106">Attributes and elements</span></span>

<span data-ttu-id="78db0-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="78db0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="78db0-108">属性</span><span class="sxs-lookup"><span data-stu-id="78db0-108">Attributes</span></span>

<span data-ttu-id="78db0-109">なし。</span><span class="sxs-lookup"><span data-stu-id="78db0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="78db0-110">子要素</span><span class="sxs-lookup"><span data-stu-id="78db0-110">Child elements</span></span>

<span data-ttu-id="78db0-111">なし。</span><span class="sxs-lookup"><span data-stu-id="78db0-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="78db0-112">親要素</span><span class="sxs-lookup"><span data-stu-id="78db0-112">Parent elements</span></span>

|<span data-ttu-id="78db0-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="78db0-113">**Element**</span></span>|<span data-ttu-id="78db0-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="78db0-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="78db0-115">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="78db0-115">FileAttachment</span></span>](fileattachment.md) <br/> |<span data-ttu-id="78db0-116">Exchange ストア内のアイテムに関連付けられているファイルを表します。</span><span class="sxs-lookup"><span data-stu-id="78db0-116">Represents a file that is attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="78db0-117">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="78db0-117">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="78db0-118">Exchange の他のアイテムに関連付けられている Exchange アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="78db0-118">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="78db0-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="78db0-119">Text value</span></span>

<span data-ttu-id="78db0-120">テキスト値は、添付ファイルの名前を表す文字列値です。</span><span class="sxs-lookup"><span data-stu-id="78db0-120">The text value is a string value that represents the name of the attachment.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="78db0-121">備考</span><span class="sxs-lookup"><span data-stu-id="78db0-121">Remarks</span></span>

<span data-ttu-id="78db0-122">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="78db0-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="78db0-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="78db0-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="78db0-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="78db0-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="78db0-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="78db0-125">Schema name</span></span>  <br/> |<span data-ttu-id="78db0-126">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="78db0-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="78db0-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="78db0-127">Validation file</span></span>  <br/> |<span data-ttu-id="78db0-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="78db0-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="78db0-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="78db0-129">Can be empty</span></span>  <br/> |<span data-ttu-id="78db0-130">False</span><span class="sxs-lookup"><span data-stu-id="78db0-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="78db0-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="78db0-131">See also</span></span>

- [<span data-ttu-id="78db0-132">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="78db0-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

