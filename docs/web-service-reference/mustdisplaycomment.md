---
title: MustDisplayComment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MustDisplayComment
api_type:
- schema
ms.assetid: 11d4d3c3-4652-4ed4-9b29-a0b5f85b82b7
description: MustDisplayComment 要素は、管理フォルダーのコメントを表示する必要があるかどうかを示します。
ms.openlocfilehash: 9a7e6a88b77ff9f1fd82507b8320898c195cd190
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832502"
---
# <a name="mustdisplaycomment"></a><span data-ttu-id="d4560-103">MustDisplayComment</span><span class="sxs-lookup"><span data-stu-id="d4560-103">MustDisplayComment</span></span>

<span data-ttu-id="d4560-104">**MustDisplayComment**要素は、管理フォルダーのコメントを表示する必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d4560-104">The **MustDisplayComment** element indicates whether the managed folder comment must be displayed.</span></span> 
  
```xml
<MustDisplayComment/>
```

 <span data-ttu-id="d4560-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="d4560-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d4560-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="d4560-106">Attributes and elements</span></span>

<span data-ttu-id="d4560-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d4560-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d4560-108">属性</span><span class="sxs-lookup"><span data-stu-id="d4560-108">Attributes</span></span>

<span data-ttu-id="d4560-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d4560-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d4560-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d4560-110">Child elements</span></span>

<span data-ttu-id="d4560-111">なし。</span><span class="sxs-lookup"><span data-stu-id="d4560-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d4560-112">親要素</span><span class="sxs-lookup"><span data-stu-id="d4560-112">Parent elements</span></span>

|<span data-ttu-id="d4560-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="d4560-113">**Element**</span></span>|<span data-ttu-id="d4560-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="d4560-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d4560-115">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="d4560-115">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="d4560-116">管理フォルダーに関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="d4560-116">Contains information about a managed folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d4560-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="d4560-117">Text value</span></span>

<span data-ttu-id="d4560-118">テキスト値は、ブール値を表します。</span><span class="sxs-lookup"><span data-stu-id="d4560-118">The text value represents a Boolean value.</span></span> <span data-ttu-id="d4560-119">**True**の場合は、コメントを表示する必要がありますようにことを示します**false**の値は、表示するコメントがないことを示します。</span><span class="sxs-lookup"><span data-stu-id="d4560-119">A value of **true** indicates that the comment must be displayed; a value of **false** indicates that the comment does not have to be displayed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="d4560-120">備考</span><span class="sxs-lookup"><span data-stu-id="d4560-120">Remarks</span></span>

<span data-ttu-id="d4560-121">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="d4560-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d4560-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="d4560-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d4560-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="d4560-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d4560-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d4560-124">Schema name</span></span>  <br/> |<span data-ttu-id="d4560-125">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="d4560-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="d4560-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d4560-126">Validation file</span></span>  <br/> |<span data-ttu-id="d4560-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d4560-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d4560-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="d4560-128">Can be empty</span></span>  <br/> |<span data-ttu-id="d4560-129">False</span><span class="sxs-lookup"><span data-stu-id="d4560-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d4560-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="d4560-130">See also</span></span>



[<span data-ttu-id="d4560-131">CreateManagedFolder 操作</span><span class="sxs-lookup"><span data-stu-id="d4560-131">CreateManagedFolder operation</span></span>](createmanagedfolder-operation.md)


- [<span data-ttu-id="d4560-132">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="d4560-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

