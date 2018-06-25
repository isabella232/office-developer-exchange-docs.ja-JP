---
title: IncludesLastFolderInRange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IncludesLastFolderInRange
api_type:
- schema
ms.assetid: 95837904-17be-49b7-831c-de4fb20fccfb
description: IncludesLastFolderInRange 要素は、最後の項目を同期するが、応答に含まれているかどうかを示します。
ms.openlocfilehash: 6c4af5b394ee2fab6bc98f7bb6afa9ee80551869
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831908"
---
# <a name="includeslastfolderinrange"></a><span data-ttu-id="cd61d-103">IncludesLastFolderInRange</span><span class="sxs-lookup"><span data-stu-id="cd61d-103">IncludesLastFolderInRange</span></span>

<span data-ttu-id="cd61d-104">**IncludesLastFolderInRange**要素は、最後の項目を同期するが、応答に含まれているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="cd61d-104">The **IncludesLastFolderInRange** element indicates whether the last item to synchronize has been included in the response.</span></span> 
  
[<span data-ttu-id="cd61d-105">SyncFolderHierarchyResponse</span><span class="sxs-lookup"><span data-stu-id="cd61d-105">SyncFolderHierarchyResponse</span></span>](syncfolderhierarchyresponse.md)
  
[<span data-ttu-id="cd61d-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="cd61d-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="cd61d-107">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="cd61d-107">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md)
  
[<span data-ttu-id="cd61d-108">IncludesLastFolderInRange</span><span class="sxs-lookup"><span data-stu-id="cd61d-108">IncludesLastFolderInRange</span></span>](includeslastfolderinrange.md)
  
```xml
<IncludesLastFolderInRange/>
```

 <span data-ttu-id="cd61d-109">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="cd61d-109">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cd61d-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="cd61d-110">Attributes and elements</span></span>

<span data-ttu-id="cd61d-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="cd61d-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cd61d-112">属性</span><span class="sxs-lookup"><span data-stu-id="cd61d-112">Attributes</span></span>

<span data-ttu-id="cd61d-113">なし。</span><span class="sxs-lookup"><span data-stu-id="cd61d-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cd61d-114">子要素</span><span class="sxs-lookup"><span data-stu-id="cd61d-114">Child elements</span></span>

<span data-ttu-id="cd61d-115">なし。</span><span class="sxs-lookup"><span data-stu-id="cd61d-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="cd61d-116">親要素</span><span class="sxs-lookup"><span data-stu-id="cd61d-116">Parent elements</span></span>

|<span data-ttu-id="cd61d-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="cd61d-117">**Element**</span></span>|<span data-ttu-id="cd61d-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="cd61d-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cd61d-119">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="cd61d-119">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md) <br/> |<span data-ttu-id="cd61d-120">SyncFolderHierarchy 要求の結果ステータスを格納します。</span><span class="sxs-lookup"><span data-stu-id="cd61d-120">Contains the status and result of a SyncFolderHierarchy request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="cd61d-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="cd61d-121">Text value</span></span>

<span data-ttu-id="cd61d-122">ブール値を表す文字列値は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="cd61d-122">A text value that represents a Boolean value is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="cd61d-123">備考</span><span class="sxs-lookup"><span data-stu-id="cd61d-123">Remarks</span></span>

<span data-ttu-id="cd61d-124">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="cd61d-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cd61d-125">要素情報</span><span class="sxs-lookup"><span data-stu-id="cd61d-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cd61d-126">名前空間</span><span class="sxs-lookup"><span data-stu-id="cd61d-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="cd61d-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="cd61d-127">Schema name</span></span>  <br/> |<span data-ttu-id="cd61d-128">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="cd61d-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="cd61d-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="cd61d-129">Validation file</span></span>  <br/> |<span data-ttu-id="cd61d-130">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="cd61d-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="cd61d-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="cd61d-131">Can be empty</span></span>  <br/> |<span data-ttu-id="cd61d-132">False</span><span class="sxs-lookup"><span data-stu-id="cd61d-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cd61d-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="cd61d-133">See also</span></span>



[<span data-ttu-id="cd61d-134">SyncFolderHierarchy 操作</span><span class="sxs-lookup"><span data-stu-id="cd61d-134">SyncFolderHierarchy operation</span></span>](syncfolderhierarchy-operation.md)


<span data-ttu-id="cd61d-135">
  [Exchange 用 EWS リファレンス](ews-reference-for-exchange.md)</span><span class="sxs-lookup"><span data-stu-id="cd61d-135">[EWS reference for Exchange](ews-reference-for-exchange.md)</span></span>
  
- [<span data-ttu-id="cd61d-136">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="cd61d-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

