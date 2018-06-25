---
title: CanRenameOrMove
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CanRenameOrMove
api_type:
- schema
ms.assetid: fe0cdb04-5f2b-4f1d-9d12-7ace0883cd86
description: CanRenameOrMove 要素は、管理対象のフォルダーの名前の変更やお客様が移動するかどうかを示します。
ms.openlocfilehash: 0303499f5cd54d4a52222e43c2c5f0b389fbcf53
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759613"
---
# <a name="canrenameormove"></a><span data-ttu-id="6a7ba-103">CanRenameOrMove</span><span class="sxs-lookup"><span data-stu-id="6a7ba-103">CanRenameOrMove</span></span>

<span data-ttu-id="6a7ba-104">**CanRenameOrMove**要素は、管理対象のフォルダーの名前の変更やお客様が移動するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6a7ba-104">The **CanRenameOrMove** element indicates whether a managed folder can be renamed or moved by the customer.</span></span> 
  
```xml
<CanRenameOrMove/>
```

 <span data-ttu-id="6a7ba-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="6a7ba-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6a7ba-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="6a7ba-106">Attributes and elements</span></span>

<span data-ttu-id="6a7ba-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6a7ba-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6a7ba-108">属性</span><span class="sxs-lookup"><span data-stu-id="6a7ba-108">Attributes</span></span>

<span data-ttu-id="6a7ba-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6a7ba-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6a7ba-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6a7ba-110">Child elements</span></span>

<span data-ttu-id="6a7ba-111">なし。</span><span class="sxs-lookup"><span data-stu-id="6a7ba-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6a7ba-112">親要素</span><span class="sxs-lookup"><span data-stu-id="6a7ba-112">Parent elements</span></span>

|<span data-ttu-id="6a7ba-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="6a7ba-113">**Element**</span></span>|<span data-ttu-id="6a7ba-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="6a7ba-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6a7ba-115">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="6a7ba-115">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="6a7ba-116">管理フォルダーに関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6a7ba-116">Contains information about a managed folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6a7ba-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="6a7ba-117">Text value</span></span>

<span data-ttu-id="6a7ba-118">テキスト値は、ブール値を表します。</span><span class="sxs-lookup"><span data-stu-id="6a7ba-118">The text value represents a Boolean value.</span></span> <span data-ttu-id="6a7ba-119">**True**の場合は、フォルダーの名前変更または移動することを示します。**false**の値は、フォルダーの名前変更または移動できないことを示します。</span><span class="sxs-lookup"><span data-stu-id="6a7ba-119">A value of **true** indicates that the folder can be renamed or moved; a value of **false** indicates that the folder cannot be renamed or moved.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="6a7ba-120">備考</span><span class="sxs-lookup"><span data-stu-id="6a7ba-120">Remarks</span></span>

<span data-ttu-id="6a7ba-121">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="6a7ba-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6a7ba-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="6a7ba-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6a7ba-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="6a7ba-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6a7ba-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6a7ba-124">Schema name</span></span>  <br/> |<span data-ttu-id="6a7ba-125">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="6a7ba-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="6a7ba-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6a7ba-126">Validation file</span></span>  <br/> |<span data-ttu-id="6a7ba-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6a7ba-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6a7ba-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="6a7ba-128">Can be empty</span></span>  <br/> |<span data-ttu-id="6a7ba-129">False</span><span class="sxs-lookup"><span data-stu-id="6a7ba-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6a7ba-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="6a7ba-130">See also</span></span>



- [<span data-ttu-id="6a7ba-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="6a7ba-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

