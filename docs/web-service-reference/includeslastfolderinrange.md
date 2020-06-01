---
title: フォルダーに Lastfolderinrange
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
description: この要素は、最後に同期する項目が応答に含まれているかどうかを示します。
ms.openlocfilehash: 9ba401cf639ef7988fa7a1437a64d09ff54c5960
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466452"
---
# <a name="includeslastfolderinrange"></a><span data-ttu-id="7a9dd-103">フォルダーに Lastfolderinrange</span><span class="sxs-lookup"><span data-stu-id="7a9dd-103">IncludesLastFolderInRange</span></span>

<span data-ttu-id="7a9dd-104">この**要素は**、最後に同期する項目が応答に含まれているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7a9dd-104">The **IncludesLastFolderInRange** element indicates whether the last item to synchronize has been included in the response.</span></span> 
  
[<span data-ttu-id="7a9dd-105">SyncFolderHierarchyResponse</span><span class="sxs-lookup"><span data-stu-id="7a9dd-105">SyncFolderHierarchyResponse</span></span>](syncfolderhierarchyresponse.md)
  
[<span data-ttu-id="7a9dd-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="7a9dd-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="7a9dd-107">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="7a9dd-107">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md)
  
[<span data-ttu-id="7a9dd-108">フォルダーに Lastfolderinrange</span><span class="sxs-lookup"><span data-stu-id="7a9dd-108">IncludesLastFolderInRange</span></span>](includeslastfolderinrange.md)
  
```xml
<IncludesLastFolderInRange/>
```

 <span data-ttu-id="7a9dd-109">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="7a9dd-109">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7a9dd-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="7a9dd-110">Attributes and elements</span></span>

<span data-ttu-id="7a9dd-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7a9dd-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7a9dd-112">属性</span><span class="sxs-lookup"><span data-stu-id="7a9dd-112">Attributes</span></span>

<span data-ttu-id="7a9dd-113">なし。</span><span class="sxs-lookup"><span data-stu-id="7a9dd-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7a9dd-114">子要素</span><span class="sxs-lookup"><span data-stu-id="7a9dd-114">Child elements</span></span>

<span data-ttu-id="7a9dd-115">なし。</span><span class="sxs-lookup"><span data-stu-id="7a9dd-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7a9dd-116">親要素</span><span class="sxs-lookup"><span data-stu-id="7a9dd-116">Parent elements</span></span>

|<span data-ttu-id="7a9dd-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="7a9dd-117">**Element**</span></span>|<span data-ttu-id="7a9dd-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="7a9dd-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7a9dd-119">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="7a9dd-119">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md) <br/> |<span data-ttu-id="7a9dd-120">SyncFolderHierarchy 要求の状態と結果を格納します。</span><span class="sxs-lookup"><span data-stu-id="7a9dd-120">Contains the status and result of a SyncFolderHierarchy request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7a9dd-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="7a9dd-121">Text value</span></span>

<span data-ttu-id="7a9dd-122">ブール値を表すテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="7a9dd-122">A text value that represents a Boolean value is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7a9dd-123">注釈</span><span class="sxs-lookup"><span data-stu-id="7a9dd-123">Remarks</span></span>

<span data-ttu-id="7a9dd-124">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="7a9dd-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7a9dd-125">要素の情報</span><span class="sxs-lookup"><span data-stu-id="7a9dd-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7a9dd-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="7a9dd-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7a9dd-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7a9dd-127">Schema name</span></span>  <br/> |<span data-ttu-id="7a9dd-128">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="7a9dd-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7a9dd-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7a9dd-129">Validation file</span></span>  <br/> |<span data-ttu-id="7a9dd-130">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="7a9dd-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7a9dd-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="7a9dd-131">Can be empty</span></span>  <br/> |<span data-ttu-id="7a9dd-132">正しくない</span><span class="sxs-lookup"><span data-stu-id="7a9dd-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7a9dd-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="7a9dd-133">See also</span></span>



[<span data-ttu-id="7a9dd-134">SyncFolderHierarchy 操作</span><span class="sxs-lookup"><span data-stu-id="7a9dd-134">SyncFolderHierarchy operation</span></span>](syncfolderhierarchy-operation.md)


<span data-ttu-id="7a9dd-135">
  [Exchange 用 EWS リファレンス](ews-reference-for-exchange.md)</span><span class="sxs-lookup"><span data-stu-id="7a9dd-135">[EWS reference for Exchange](ews-reference-for-exchange.md)</span></span>
  
- [<span data-ttu-id="7a9dd-136">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="7a9dd-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

