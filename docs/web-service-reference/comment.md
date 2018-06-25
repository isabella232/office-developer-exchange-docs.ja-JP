---
title: Comment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Comment
api_type:
- schema
ms.assetid: be7f4b56-a741-46b7-9d72-3604514baac6
description: コメント要素には、管理フォルダーに関連付けられているコメントが含まれています。
ms.openlocfilehash: 02f077c6320acc989bbbd29f7563cdca9e57425e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759631"
---
# <a name="comment"></a><span data-ttu-id="51e99-103">Comment</span><span class="sxs-lookup"><span data-stu-id="51e99-103">Comment</span></span>

<span data-ttu-id="51e99-104">**コメント**要素には、管理フォルダーに関連付けられているコメントが含まれています。</span><span class="sxs-lookup"><span data-stu-id="51e99-104">The **Comment** element contains the comment that is associated with a managed folder.</span></span> 
  
```xml
<Comment/>
```

 <span data-ttu-id="51e99-105">**文字列型 (String)**</span><span class="sxs-lookup"><span data-stu-id="51e99-105">**String**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="51e99-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="51e99-106">Attributes and elements</span></span>

<span data-ttu-id="51e99-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="51e99-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="51e99-108">属性</span><span class="sxs-lookup"><span data-stu-id="51e99-108">Attributes</span></span>

<span data-ttu-id="51e99-109">なし。</span><span class="sxs-lookup"><span data-stu-id="51e99-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="51e99-110">子要素</span><span class="sxs-lookup"><span data-stu-id="51e99-110">Child elements</span></span>

<span data-ttu-id="51e99-111">なし。</span><span class="sxs-lookup"><span data-stu-id="51e99-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="51e99-112">親要素</span><span class="sxs-lookup"><span data-stu-id="51e99-112">Parent elements</span></span>

|<span data-ttu-id="51e99-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="51e99-113">**Element**</span></span>|<span data-ttu-id="51e99-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="51e99-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="51e99-115">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="51e99-115">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="51e99-116">管理フォルダーに関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="51e99-116">Contains information about a managed folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="51e99-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="51e99-117">Text value</span></span>

<span data-ttu-id="51e99-118">テキスト値は、管理フォルダーに関連付けられているコメントを表します。</span><span class="sxs-lookup"><span data-stu-id="51e99-118">The text value represents the comment that is associated with a managed folder.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="51e99-119">備考</span><span class="sxs-lookup"><span data-stu-id="51e99-119">Remarks</span></span>

<span data-ttu-id="51e99-120">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="51e99-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="51e99-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="51e99-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="51e99-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="51e99-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="51e99-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="51e99-123">Schema name</span></span>  <br/> |<span data-ttu-id="51e99-124">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="51e99-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="51e99-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="51e99-125">Validation file</span></span>  <br/> |<span data-ttu-id="51e99-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="51e99-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="51e99-127">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="51e99-127">Can be empty</span></span>  <br/> |<span data-ttu-id="51e99-128">False</span><span class="sxs-lookup"><span data-stu-id="51e99-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="51e99-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="51e99-129">See also</span></span>



- [<span data-ttu-id="51e99-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="51e99-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

