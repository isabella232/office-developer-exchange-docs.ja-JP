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
ms.openlocfilehash: bf17ee9080405d308328197f7cbeb92e9b1e02d3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456424"
---
# <a name="syncfolderhierarchyresponse"></a><span data-ttu-id="2042a-103">SyncFolderHierarchyResponse</span><span class="sxs-lookup"><span data-stu-id="2042a-103">SyncFolderHierarchyResponse</span></span>

<span data-ttu-id="2042a-104">**SyncFolderHierarchyResponse**要素は、SyncFolderHierarchy 要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="2042a-104">The **SyncFolderHierarchyResponse** element defines a response to a SyncFolderHierarchy request.</span></span> 
  
```xml
<SyncFolderHierarchyResponse>
   <ResponseMessages/>
</SyncFolderHierarchyResponse>
```

 <span data-ttu-id="2042a-105">**SyncFolderHierarchyResponseType**</span><span class="sxs-lookup"><span data-stu-id="2042a-105">**SyncFolderHierarchyResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2042a-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="2042a-106">Attributes and elements</span></span>

<span data-ttu-id="2042a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2042a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2042a-108">属性</span><span class="sxs-lookup"><span data-stu-id="2042a-108">Attributes</span></span>

<span data-ttu-id="2042a-109">なし。</span><span class="sxs-lookup"><span data-stu-id="2042a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2042a-110">子要素</span><span class="sxs-lookup"><span data-stu-id="2042a-110">Child elements</span></span>

|<span data-ttu-id="2042a-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="2042a-111">**Element**</span></span>|<span data-ttu-id="2042a-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="2042a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2042a-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="2042a-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="2042a-114">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="2042a-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2042a-115">親要素</span><span class="sxs-lookup"><span data-stu-id="2042a-115">Parent elements</span></span>

<span data-ttu-id="2042a-116">なし。</span><span class="sxs-lookup"><span data-stu-id="2042a-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2042a-117">注釈</span><span class="sxs-lookup"><span data-stu-id="2042a-117">Remarks</span></span>

<span data-ttu-id="2042a-118">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="2042a-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2042a-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="2042a-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2042a-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="2042a-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2042a-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2042a-121">Schema name</span></span>  <br/> |<span data-ttu-id="2042a-122">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="2042a-122">messages schema</span></span>  <br/> |
|<span data-ttu-id="2042a-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2042a-123">Validation file</span></span>  <br/> |<span data-ttu-id="2042a-124">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="2042a-124">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2042a-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="2042a-125">Can be empty</span></span>  <br/> |<span data-ttu-id="2042a-126">正しくない</span><span class="sxs-lookup"><span data-stu-id="2042a-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2042a-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="2042a-127">See also</span></span>



[<span data-ttu-id="2042a-128">SyncFolderHierarchy 操作</span><span class="sxs-lookup"><span data-stu-id="2042a-128">SyncFolderHierarchy operation</span></span>](syncfolderhierarchy-operation.md)


- [<span data-ttu-id="2042a-129">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="2042a-129">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

