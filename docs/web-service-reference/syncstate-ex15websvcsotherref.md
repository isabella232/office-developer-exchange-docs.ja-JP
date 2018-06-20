---
title: 同期状態
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncState
api_type:
- schema
ms.assetid: e5ebaae3-0f07-481d-ac67-d9687a3c7ac3
description: 同期状態の要素には、それぞれの要求が成功した後に更新された同期データの base64 でエンコードされたフォームが含まれています。 これを使用して、同期の状態を識別します。
ms.openlocfilehash: 3c600dde09fd813dcfb1f6e74671ebe9004701a1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839643"
---
# <a name="syncstate"></a><span data-ttu-id="ea152-104">同期状態</span><span class="sxs-lookup"><span data-stu-id="ea152-104">SyncState</span></span>

<span data-ttu-id="ea152-105">**同期状態**の要素には、それぞれの要求が成功した後に更新された同期データの base64 でエンコードされたフォームが含まれています。</span><span class="sxs-lookup"><span data-stu-id="ea152-105">The **SyncState** element contains a base64-encoded form of the synchronization data that is updated after each successful request.</span></span> <span data-ttu-id="ea152-106">これを使用して、同期の状態を識別します。</span><span class="sxs-lookup"><span data-stu-id="ea152-106">This is used to identify the synchronization state.</span></span> 
  
```xml
<SyncState/>
```

 <span data-ttu-id="ea152-107">**文字列型 (String)**</span><span class="sxs-lookup"><span data-stu-id="ea152-107">**String**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ea152-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="ea152-108">Attributes and elements</span></span>

<span data-ttu-id="ea152-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ea152-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ea152-110">属性</span><span class="sxs-lookup"><span data-stu-id="ea152-110">Attributes</span></span>

<span data-ttu-id="ea152-111">なし。</span><span class="sxs-lookup"><span data-stu-id="ea152-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ea152-112">子要素</span><span class="sxs-lookup"><span data-stu-id="ea152-112">Child elements</span></span>

<span data-ttu-id="ea152-113">なし。</span><span class="sxs-lookup"><span data-stu-id="ea152-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ea152-114">親要素</span><span class="sxs-lookup"><span data-stu-id="ea152-114">Parent elements</span></span>

|<span data-ttu-id="ea152-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="ea152-115">**Element**</span></span>|<span data-ttu-id="ea152-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="ea152-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ea152-117">SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="ea152-117">SyncFolderHierarchy</span></span>](syncfolderhierarchy.md) <br/> |<span data-ttu-id="ea152-118">クライアント上のフォルダー階層を同期するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="ea152-118">Defines a request to synchronize a folder hierarchy on a client.</span></span>  <br/> |
|[<span data-ttu-id="ea152-119">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ea152-119">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md) <br/> |<span data-ttu-id="ea152-120">SyncFolderHierarchy 要求の結果ステータスを格納します。</span><span class="sxs-lookup"><span data-stu-id="ea152-120">Contains the status and result of a SyncFolderHierarchy request.</span></span>  <br/> |
|[<span data-ttu-id="ea152-121">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="ea152-121">SyncFolderItems</span></span>](syncfolderitems.md) <br/> |<span data-ttu-id="ea152-122">Exchange ストア フォルダー内のアイテムを同期するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="ea152-122">Defines a request to synchronize items in an Exchange store folder.</span></span>  <br/> |
|[<span data-ttu-id="ea152-123">SyncFolderItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ea152-123">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md) <br/> |<span data-ttu-id="ea152-124">SyncFolderItems 要求の結果ステータスを格納します。</span><span class="sxs-lookup"><span data-stu-id="ea152-124">Contains the status and result of a SyncFolderItems request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ea152-125">テキスト値</span><span class="sxs-lookup"><span data-stu-id="ea152-125">Text value</span></span>

<span data-ttu-id="ea152-126">この要素を使用する場合、テキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="ea152-126">A text value is required when this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ea152-127">備考</span><span class="sxs-lookup"><span data-stu-id="ea152-127">Remarks</span></span>

<span data-ttu-id="ea152-128">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="ea152-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ea152-129">要素情報</span><span class="sxs-lookup"><span data-stu-id="ea152-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ea152-130">名前空間</span><span class="sxs-lookup"><span data-stu-id="ea152-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ea152-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ea152-131">Schema name</span></span>  <br/> |<span data-ttu-id="ea152-132">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="ea152-132">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ea152-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ea152-133">Validation file</span></span>  <br/> |<span data-ttu-id="ea152-134">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ea152-134">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ea152-135">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="ea152-135">Can be empty</span></span>  <br/> |<span data-ttu-id="ea152-136">False</span><span class="sxs-lookup"><span data-stu-id="ea152-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ea152-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="ea152-137">See also</span></span>



[<span data-ttu-id="ea152-138">SyncFolderItems の操作</span><span class="sxs-lookup"><span data-stu-id="ea152-138">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)
  
[<span data-ttu-id="ea152-139">SyncFolderHierarchy 操作</span><span class="sxs-lookup"><span data-stu-id="ea152-139">SyncFolderHierarchy operation</span></span>](syncfolderhierarchy-operation.md)


- [<span data-ttu-id="ea152-140">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="ea152-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

