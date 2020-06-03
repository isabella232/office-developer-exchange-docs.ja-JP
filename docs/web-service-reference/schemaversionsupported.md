---
title: SchemaVersionSupported
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 578b1682-f3e1-4ccc-aa24-d2ca1a9de596
description: SchemaVersionSupported 要素には、クライアントでサポートされているマニフェストスキーマのバージョンが含まれています。
ms.openlocfilehash: df70d8ecf78b4f9b99ceaa3c28d2b1831a1c6171
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465794"
---
# <a name="schemaversionsupported"></a><span data-ttu-id="55f8b-103">SchemaVersionSupported</span><span class="sxs-lookup"><span data-stu-id="55f8b-103">SchemaVersionSupported</span></span>

<span data-ttu-id="55f8b-104">**SchemaVersionSupported**要素には、クライアントでサポートされているマニフェストスキーマのバージョンが含まれています。</span><span class="sxs-lookup"><span data-stu-id="55f8b-104">The **SchemaVersionSupported** element contains the version of the manifest schema supported by the client.</span></span> 
  
```XML
<SchemaVersionSupported />
```

 <span data-ttu-id="55f8b-105">**string**</span><span class="sxs-lookup"><span data-stu-id="55f8b-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="55f8b-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="55f8b-106">Attributes and elements</span></span>

<span data-ttu-id="55f8b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="55f8b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="55f8b-108">属性</span><span class="sxs-lookup"><span data-stu-id="55f8b-108">Attributes</span></span>

<span data-ttu-id="55f8b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="55f8b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="55f8b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="55f8b-110">Child elements</span></span>

<span data-ttu-id="55f8b-111">なし。</span><span class="sxs-lookup"><span data-stu-id="55f8b-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="55f8b-112">親要素</span><span class="sxs-lookup"><span data-stu-id="55f8b-112">Parent elements</span></span>

[<span data-ttu-id="55f8b-113">Getappmanifests が</span><span class="sxs-lookup"><span data-stu-id="55f8b-113">GetAppManifests</span></span>](getappmanifests.md)
  
## <a name="text-value"></a><span data-ttu-id="55f8b-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="55f8b-114">Text value</span></span>

<span data-ttu-id="55f8b-115">**SchemaVersionSupported**要素のテキスト値には、クライアントでサポートされているマニフェストスキーマのバージョンが含まれています。</span><span class="sxs-lookup"><span data-stu-id="55f8b-115">The text value of the **SchemaVersionSupported** element contains the version of the manifest schema supported by the client.</span></span> <span data-ttu-id="55f8b-116">この値は、応答でクライアントに返されるアプリケーションマニフェストを示します。</span><span class="sxs-lookup"><span data-stu-id="55f8b-116">This value indicates which app manifests should be returned to the client in the response.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="55f8b-117">注釈</span><span class="sxs-lookup"><span data-stu-id="55f8b-117">Remarks</span></span>

<span data-ttu-id="55f8b-118">この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="55f8b-118">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="55f8b-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="55f8b-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="55f8b-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="55f8b-120">Namespace</span></span>  <br/> | https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="55f8b-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="55f8b-121">Schema Name</span></span>  <br/> |<span data-ttu-id="55f8b-122">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="55f8b-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="55f8b-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="55f8b-123">Validation File</span></span>  <br/> |<span data-ttu-id="55f8b-124">該当なし</span><span class="sxs-lookup"><span data-stu-id="55f8b-124">Not applicable</span></span>  <br/> |
|<span data-ttu-id="55f8b-125">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="55f8b-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="55f8b-126">正しくない</span><span class="sxs-lookup"><span data-stu-id="55f8b-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="55f8b-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="55f8b-127">See also</span></span>



[<span data-ttu-id="55f8b-128">Getappmanifests が</span><span class="sxs-lookup"><span data-stu-id="55f8b-128">GetAppManifests</span></span>](getappmanifests.md)


- [<span data-ttu-id="55f8b-129">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="55f8b-129">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

