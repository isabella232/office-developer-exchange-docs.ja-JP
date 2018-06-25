---
title: SyncFolderHierarchy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncFolderHierarchy
api_type:
- schema
ms.assetid: 55df4d01-e48e-4263-a851-78a66ad1093a
description: SyncFolderHierarchy 要素は、クライアント上のフォルダー階層を同期するための要求を定義します。
ms.openlocfilehash: f72640e5605dd83e92cd323cb00e4d2f64406245
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839634"
---
# <a name="syncfolderhierarchy"></a><span data-ttu-id="3a0a0-103">SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="3a0a0-103">SyncFolderHierarchy</span></span>

<span data-ttu-id="3a0a0-104">**SyncFolderHierarchy**要素は、クライアント上のフォルダー階層を同期するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="3a0a0-104">The **SyncFolderHierarchy** element defines a request to synchronize a folder hierarchy on a client.</span></span> 
  
```xml
<SyncFolderHierarchy>
   <FolderShape/>   <SyncFolderId/>
   <SyncState/>
</SyncFolderHierarchy>
```

 <span data-ttu-id="3a0a0-105">**SyncFolderHierarchyType**</span><span class="sxs-lookup"><span data-stu-id="3a0a0-105">**SyncFolderHierarchyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3a0a0-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="3a0a0-106">Attributes and elements</span></span>

<span data-ttu-id="3a0a0-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3a0a0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3a0a0-108">属性</span><span class="sxs-lookup"><span data-stu-id="3a0a0-108">Attributes</span></span>

<span data-ttu-id="3a0a0-109">なし。</span><span class="sxs-lookup"><span data-stu-id="3a0a0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3a0a0-110">子要素</span><span class="sxs-lookup"><span data-stu-id="3a0a0-110">Child elements</span></span>

|<span data-ttu-id="3a0a0-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="3a0a0-111">**Element**</span></span>|<span data-ttu-id="3a0a0-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="3a0a0-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3a0a0-113">FolderShape</span><span class="sxs-lookup"><span data-stu-id="3a0a0-113">FolderShape</span></span>](foldershape.md) <br/> |<span data-ttu-id="3a0a0-114">[SyncFolderHierarchy](syncfolderhierarchy.md)の応答に含めるフォルダーのプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="3a0a0-114">Identifies the folder properties to include in a [SyncFolderHierarchy](syncfolderhierarchy.md) response.</span></span>  <br/> |
|[<span data-ttu-id="3a0a0-115">SyncFolderId</span><span class="sxs-lookup"><span data-stu-id="3a0a0-115">SyncFolderId</span></span>](syncfolderid.md) <br/> |<span data-ttu-id="3a0a0-116">同期する項目を含むフォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="3a0a0-116">Represents the folder that contains the items to synchronize.</span></span> <span data-ttu-id="3a0a0-117">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="3a0a0-117">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="3a0a0-118">同期状態</span><span class="sxs-lookup"><span data-stu-id="3a0a0-118">SyncState</span></span>](syncstate-ex15websvcsotherref.md) <br/> |<span data-ttu-id="3a0a0-119">各成功した要求の後に更新された同期データの base64 でエンコードされたフォームが含まれています。</span><span class="sxs-lookup"><span data-stu-id="3a0a0-119">Contains a base64-encoded form of the synchronization data that is updated after each successful request.</span></span> <span data-ttu-id="3a0a0-120">これを使用して、同期の状態を識別します。</span><span class="sxs-lookup"><span data-stu-id="3a0a0-120">This is used to identify the synchronization state.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3a0a0-121">親要素</span><span class="sxs-lookup"><span data-stu-id="3a0a0-121">Parent elements</span></span>

<span data-ttu-id="3a0a0-122">なし。</span><span class="sxs-lookup"><span data-stu-id="3a0a0-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3a0a0-123">備考</span><span class="sxs-lookup"><span data-stu-id="3a0a0-123">Remarks</span></span>

<span data-ttu-id="3a0a0-124">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="3a0a0-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3a0a0-125">要素情報</span><span class="sxs-lookup"><span data-stu-id="3a0a0-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3a0a0-126">名前空間</span><span class="sxs-lookup"><span data-stu-id="3a0a0-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3a0a0-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3a0a0-127">Schema name</span></span>  <br/> |<span data-ttu-id="3a0a0-128">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="3a0a0-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3a0a0-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3a0a0-129">Validation file</span></span>  <br/> |<span data-ttu-id="3a0a0-130">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="3a0a0-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3a0a0-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="3a0a0-131">Can be empty</span></span>  <br/> |<span data-ttu-id="3a0a0-132">False</span><span class="sxs-lookup"><span data-stu-id="3a0a0-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3a0a0-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="3a0a0-133">See also</span></span>



[<span data-ttu-id="3a0a0-134">SyncFolderHierarchy 操作</span><span class="sxs-lookup"><span data-stu-id="3a0a0-134">SyncFolderHierarchy operation</span></span>](syncfolderhierarchy-operation.md)


- [<span data-ttu-id="3a0a0-135">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="3a0a0-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

