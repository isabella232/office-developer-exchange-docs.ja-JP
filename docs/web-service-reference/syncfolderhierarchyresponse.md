---
title: SyncFolderHierarchyResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncFolderHierarchyResponse
api_type:
- schema
ms.assetid: 7e6061d2-bbce-4864-a7bb-a6457628cb7c
description: SyncFolderHierarchyResponse 要素は、SyncFolderHierarchy 要求への応答を定義します。
ms.openlocfilehash: aee70603b84dfdf5f7f580fd2566f7ebfbbce383
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839636"
---
# <a name="syncfolderhierarchyresponse"></a><span data-ttu-id="83c76-103">SyncFolderHierarchyResponse</span><span class="sxs-lookup"><span data-stu-id="83c76-103">SyncFolderHierarchyResponse</span></span>

<span data-ttu-id="83c76-104">**SyncFolderHierarchyResponse**要素は、SyncFolderHierarchy 要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="83c76-104">The **SyncFolderHierarchyResponse** element defines a response to a SyncFolderHierarchy request.</span></span> 
  
```xml
<SyncFolderHierarchyResponse>
   <ResponseMessages/>
</SyncFolderHierarchyResponse>
```

 <span data-ttu-id="83c76-105">**SyncFolderHierarchyResponseType**</span><span class="sxs-lookup"><span data-stu-id="83c76-105">**SyncFolderHierarchyResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="83c76-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="83c76-106">Attributes and elements</span></span>

<span data-ttu-id="83c76-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="83c76-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="83c76-108">属性</span><span class="sxs-lookup"><span data-stu-id="83c76-108">Attributes</span></span>

<span data-ttu-id="83c76-109">なし。</span><span class="sxs-lookup"><span data-stu-id="83c76-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="83c76-110">子要素</span><span class="sxs-lookup"><span data-stu-id="83c76-110">Child elements</span></span>

|<span data-ttu-id="83c76-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="83c76-111">**Element**</span></span>|<span data-ttu-id="83c76-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="83c76-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="83c76-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="83c76-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="83c76-114">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="83c76-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="83c76-115">親要素</span><span class="sxs-lookup"><span data-stu-id="83c76-115">Parent elements</span></span>

<span data-ttu-id="83c76-116">なし。</span><span class="sxs-lookup"><span data-stu-id="83c76-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="83c76-117">備考</span><span class="sxs-lookup"><span data-stu-id="83c76-117">Remarks</span></span>

<span data-ttu-id="83c76-118">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="83c76-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="83c76-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="83c76-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="83c76-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="83c76-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="83c76-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="83c76-121">Schema name</span></span>  <br/> |<span data-ttu-id="83c76-122">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="83c76-122">messages schema</span></span>  <br/> |
|<span data-ttu-id="83c76-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="83c76-123">Validation file</span></span>  <br/> |<span data-ttu-id="83c76-124">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="83c76-124">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="83c76-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="83c76-125">Can be empty</span></span>  <br/> |<span data-ttu-id="83c76-126">False</span><span class="sxs-lookup"><span data-stu-id="83c76-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="83c76-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="83c76-127">See also</span></span>



[<span data-ttu-id="83c76-128">SyncFolderHierarchy 操作</span><span class="sxs-lookup"><span data-stu-id="83c76-128">SyncFolderHierarchy operation</span></span>](syncfolderhierarchy-operation.md)


- [<span data-ttu-id="83c76-129">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="83c76-129">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

