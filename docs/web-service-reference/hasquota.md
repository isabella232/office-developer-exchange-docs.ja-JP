---
title: HasQuota
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- HasQuota
api_type:
- schema
ms.assetid: b6e4fef0-92a9-415f-81ae-0c5ecb7c12ad
description: HasQuota 要素は、管理対象のフォルダーがクォータを持つかどうかを示します。
ms.openlocfilehash: 26f14ee7c9d4de267733bca11f7884d1d391b3dd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831807"
---
# <a name="hasquota"></a><span data-ttu-id="07d9d-103">HasQuota</span><span class="sxs-lookup"><span data-stu-id="07d9d-103">HasQuota</span></span>

<span data-ttu-id="07d9d-104">**HasQuota**要素は、管理対象のフォルダーがクォータを持つかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="07d9d-104">The **HasQuota** element indicates whether the managed folder has a quota.</span></span> 
  
```xml
<HasQuota/>
```

 <span data-ttu-id="07d9d-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="07d9d-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="07d9d-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="07d9d-106">Attributes and elements</span></span>

<span data-ttu-id="07d9d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="07d9d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="07d9d-108">属性</span><span class="sxs-lookup"><span data-stu-id="07d9d-108">Attributes</span></span>

<span data-ttu-id="07d9d-109">なし。</span><span class="sxs-lookup"><span data-stu-id="07d9d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="07d9d-110">子要素</span><span class="sxs-lookup"><span data-stu-id="07d9d-110">Child elements</span></span>

<span data-ttu-id="07d9d-111">なし。</span><span class="sxs-lookup"><span data-stu-id="07d9d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="07d9d-112">親要素</span><span class="sxs-lookup"><span data-stu-id="07d9d-112">Parent elements</span></span>

|<span data-ttu-id="07d9d-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="07d9d-113">**Element**</span></span>|<span data-ttu-id="07d9d-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="07d9d-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="07d9d-115">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="07d9d-115">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="07d9d-116">管理フォルダーに関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="07d9d-116">Contains information about a managed folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="07d9d-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="07d9d-117">Text value</span></span>

<span data-ttu-id="07d9d-118">テキスト値は、ブール値を表します。</span><span class="sxs-lookup"><span data-stu-id="07d9d-118">The text value represents a Boolean value.</span></span> <span data-ttu-id="07d9d-119">**True**の場合は、フォルダーが、クォータを持っていることを示します**false**の値は、フォルダーがクォータを持っていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="07d9d-119">A value of **true** indicates that the folder has a quota; a value of **false** indicates that the folder does not have a quota.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="07d9d-120">備考</span><span class="sxs-lookup"><span data-stu-id="07d9d-120">Remarks</span></span>

<span data-ttu-id="07d9d-121">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="07d9d-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="07d9d-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="07d9d-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="07d9d-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="07d9d-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="07d9d-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="07d9d-124">Schema name</span></span>  <br/> |<span data-ttu-id="07d9d-125">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="07d9d-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="07d9d-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="07d9d-126">Validation file</span></span>  <br/> |<span data-ttu-id="07d9d-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="07d9d-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="07d9d-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="07d9d-128">Can be empty</span></span>  <br/> |<span data-ttu-id="07d9d-129">False</span><span class="sxs-lookup"><span data-stu-id="07d9d-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="07d9d-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="07d9d-130">See also</span></span>



- [<span data-ttu-id="07d9d-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="07d9d-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

