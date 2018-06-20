---
title: IsManagedFoldersRoot
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsManagedFoldersRoot
api_type:
- schema
ms.assetid: 00823fb9-bf8b-49bb-8e1b-d698c6d4063f
description: IsManagedFoldersRoot 要素は、管理フォルダーがすべての管理フォルダーのルートかどうかを示します。
ms.openlocfilehash: 3484a3fef56545a9a8d56af65f56f75205918ec7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832044"
---
# <a name="ismanagedfoldersroot"></a><span data-ttu-id="8f985-103">IsManagedFoldersRoot</span><span class="sxs-lookup"><span data-stu-id="8f985-103">IsManagedFoldersRoot</span></span>

<span data-ttu-id="8f985-104">**IsManagedFoldersRoot**要素は、管理フォルダーがすべての管理フォルダーのルートかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8f985-104">The **IsManagedFoldersRoot** element indicates whether the managed folder is the root for all managed folders.</span></span> 
  
```xml
<IsManagedFoldersRoot/>
```

 <span data-ttu-id="8f985-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="8f985-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8f985-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="8f985-106">Attributes and elements</span></span>

<span data-ttu-id="8f985-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8f985-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8f985-108">属性</span><span class="sxs-lookup"><span data-stu-id="8f985-108">Attributes</span></span>

<span data-ttu-id="8f985-109">なし。</span><span class="sxs-lookup"><span data-stu-id="8f985-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8f985-110">子要素</span><span class="sxs-lookup"><span data-stu-id="8f985-110">Child elements</span></span>

<span data-ttu-id="8f985-111">なし。</span><span class="sxs-lookup"><span data-stu-id="8f985-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8f985-112">親要素</span><span class="sxs-lookup"><span data-stu-id="8f985-112">Parent elements</span></span>

|<span data-ttu-id="8f985-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="8f985-113">**Element**</span></span>|<span data-ttu-id="8f985-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="8f985-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8f985-115">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="8f985-115">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="8f985-116">管理フォルダーに関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="8f985-116">Contains information about a managed folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8f985-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="8f985-117">Text value</span></span>

<span data-ttu-id="8f985-118">ブール値を表す文字列値は、この要素が存在する場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="8f985-118">A text value that represents a Boolean value is required if this element is present.</span></span> <span data-ttu-id="8f985-119">**True**の値の場合、フォルダーが、管理対象フォルダーのルート フォルダーであることを示します**false**の値は、フォルダーは、管理フォルダーのルート フォルダーではありませんを示します。</span><span class="sxs-lookup"><span data-stu-id="8f985-119">A value of **true** indicates that the folder is the root folder of the managed folder; a value of **false** indicates that the folder is not the root folder of the managed folder.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="8f985-120">備考</span><span class="sxs-lookup"><span data-stu-id="8f985-120">Remarks</span></span>

<span data-ttu-id="8f985-121">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="8f985-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8f985-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="8f985-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8f985-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="8f985-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8f985-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8f985-124">Schema name</span></span>  <br/> |<span data-ttu-id="8f985-125">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="8f985-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="8f985-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8f985-126">Validation file</span></span>  <br/> |<span data-ttu-id="8f985-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8f985-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8f985-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="8f985-128">Can be empty</span></span>  <br/> |<span data-ttu-id="8f985-129">False</span><span class="sxs-lookup"><span data-stu-id="8f985-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8f985-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="8f985-130">See also</span></span>



- [<span data-ttu-id="8f985-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="8f985-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

