---
title: SyncFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncFolderId
api_type:
- schema
ms.assetid: 3645fa03-236d-4e5f-b8b9-5d98f7f35fa2
description: SyncFolderId 要素は、[同期する項目を含むフォルダーを表します。
ms.openlocfilehash: 45a4a62c7d269861555089019db259eacab26ef0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839635"
---
# <a name="syncfolderid"></a><span data-ttu-id="2701b-103">SyncFolderId</span><span class="sxs-lookup"><span data-stu-id="2701b-103">SyncFolderId</span></span>

<span data-ttu-id="2701b-104">**SyncFolderId**要素は、[同期する項目を含むフォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="2701b-104">The **SyncFolderId** element represents the folder that contains the items to synchronize.</span></span> 
  
```xml
<SyncFolderId>
   <FolderId/>
</SyncFolderId>
```

 <span data-ttu-id="2701b-105">**TargetFolderIdType**</span><span class="sxs-lookup"><span data-stu-id="2701b-105">**TargetFolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2701b-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="2701b-106">Attributes and elements</span></span>

<span data-ttu-id="2701b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2701b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2701b-108">属性</span><span class="sxs-lookup"><span data-stu-id="2701b-108">Attributes</span></span>

<span data-ttu-id="2701b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="2701b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2701b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="2701b-110">Child elements</span></span>

|<span data-ttu-id="2701b-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="2701b-111">**Element**</span></span>|<span data-ttu-id="2701b-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="2701b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2701b-113">フォルダー Id</span><span class="sxs-lookup"><span data-stu-id="2701b-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="2701b-114">フォルダーの識別子と変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="2701b-114">Contains the identifier and change key of a folder.</span></span>  <br/> |
|[<span data-ttu-id="2701b-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="2701b-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="2701b-116">名前で参照することができます MicrosoftExchange Server 2007 フォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="2701b-116">Identifies MicrosoftExchange Server 2007 folders that can be referenced by name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2701b-117">親要素</span><span class="sxs-lookup"><span data-stu-id="2701b-117">Parent elements</span></span>

|<span data-ttu-id="2701b-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="2701b-118">**Element**</span></span>|<span data-ttu-id="2701b-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="2701b-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2701b-120">SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="2701b-120">SyncFolderHierarchy</span></span>](syncfolderhierarchy.md) <br/> |<span data-ttu-id="2701b-121">Exchange ストア内のフォルダー階層を同期するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="2701b-121">Defines a request to synchronize a folder hierarchy in an Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2701b-122">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="2701b-122">SyncFolderItems</span></span>](syncfolderitems.md) <br/> |<span data-ttu-id="2701b-123">Exchange ストア フォルダー内のアイテムを同期するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="2701b-123">Defines a request to synchronize items in an Exchange store folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2701b-124">備考</span><span class="sxs-lookup"><span data-stu-id="2701b-124">Remarks</span></span>

<span data-ttu-id="2701b-125">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="2701b-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2701b-126">要素情報</span><span class="sxs-lookup"><span data-stu-id="2701b-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2701b-127">名前空間</span><span class="sxs-lookup"><span data-stu-id="2701b-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2701b-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2701b-128">Schema name</span></span>  <br/> |<span data-ttu-id="2701b-129">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="2701b-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="2701b-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2701b-130">Validation file</span></span>  <br/> |<span data-ttu-id="2701b-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="2701b-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2701b-132">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="2701b-132">Can be empty</span></span>  <br/> |<span data-ttu-id="2701b-133">False</span><span class="sxs-lookup"><span data-stu-id="2701b-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2701b-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="2701b-134">See also</span></span>



[<span data-ttu-id="2701b-135">SyncFolderItems の操作</span><span class="sxs-lookup"><span data-stu-id="2701b-135">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="2701b-136">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="2701b-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

