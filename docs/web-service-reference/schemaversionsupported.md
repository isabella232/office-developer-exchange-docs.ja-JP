---
title: SchemaVersionSupported
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 578b1682-f3e1-4ccc-aa24-d2ca1a9de596
description: SchemaVersionSupported 要素には、クライアントでサポートされるマニフェストのスキーマのバージョンが含まれています。
ms.openlocfilehash: 0b27a6f16f310ffe10ab819fc1046d4b0b6ecaa2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833272"
---
# <a name="schemaversionsupported"></a><span data-ttu-id="59656-103">SchemaVersionSupported</span><span class="sxs-lookup"><span data-stu-id="59656-103">SchemaVersionSupported</span></span>

<span data-ttu-id="59656-104">**SchemaVersionSupported**要素には、クライアントでサポートされるマニフェストのスキーマのバージョンが含まれています。</span><span class="sxs-lookup"><span data-stu-id="59656-104">The **SchemaVersionSupported** element contains the version of the manifest schema supported by the client.</span></span> 
  
```XML
<SchemaVersionSupported />
```

 <span data-ttu-id="59656-105">**string**</span><span class="sxs-lookup"><span data-stu-id="59656-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="59656-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="59656-106">Attributes and elements</span></span>

<span data-ttu-id="59656-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="59656-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="59656-108">属性</span><span class="sxs-lookup"><span data-stu-id="59656-108">Attributes</span></span>

<span data-ttu-id="59656-109">なし。</span><span class="sxs-lookup"><span data-stu-id="59656-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="59656-110">子要素</span><span class="sxs-lookup"><span data-stu-id="59656-110">Child elements</span></span>

<span data-ttu-id="59656-111">なし。</span><span class="sxs-lookup"><span data-stu-id="59656-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="59656-112">親要素</span><span class="sxs-lookup"><span data-stu-id="59656-112">Parent elements</span></span>

[<span data-ttu-id="59656-113">GetAppManifests</span><span class="sxs-lookup"><span data-stu-id="59656-113">GetAppManifests</span></span>](getappmanifests.md)
  
## <a name="text-value"></a><span data-ttu-id="59656-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="59656-114">Text value</span></span>

<span data-ttu-id="59656-115">**SchemaVersionSupported**要素のテキスト値には、クライアントでサポートされるマニフェストのスキーマのバージョンが含まれています。</span><span class="sxs-lookup"><span data-stu-id="59656-115">The text value of the **SchemaVersionSupported** element contains the version of the manifest schema supported by the client.</span></span> <span data-ttu-id="59656-116">この値は、アプリケーション マニフェストは、応答でクライアントに返される必要がありますを示します。</span><span class="sxs-lookup"><span data-stu-id="59656-116">This value indicates which app manifests should be returned to the client in the response.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="59656-117">備考</span><span class="sxs-lookup"><span data-stu-id="59656-117">Remarks</span></span>

<span data-ttu-id="59656-118">この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="59656-118">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="59656-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="59656-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="59656-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="59656-120">Namespace</span></span>  <br/> | http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="59656-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="59656-121">Schema Name</span></span>  <br/> |<span data-ttu-id="59656-122">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="59656-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="59656-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="59656-123">Validation File</span></span>  <br/> |<span data-ttu-id="59656-124">該当しない</span><span class="sxs-lookup"><span data-stu-id="59656-124">Not applicable</span></span>  <br/> |
|<span data-ttu-id="59656-125">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="59656-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="59656-126">False</span><span class="sxs-lookup"><span data-stu-id="59656-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="59656-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="59656-127">See also</span></span>



[<span data-ttu-id="59656-128">GetAppManifests</span><span class="sxs-lookup"><span data-stu-id="59656-128">GetAppManifests</span></span>](getappmanifests.md)


- [<span data-ttu-id="59656-129">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="59656-129">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

