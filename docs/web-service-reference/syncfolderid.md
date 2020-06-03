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
description: SyncFolderId 要素は、同期するアイテムを含むフォルダーを表します。
ms.openlocfilehash: 35b66579116a00d27df722629ff980471ca0272e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530297"
---
# <a name="syncfolderid"></a><span data-ttu-id="5f046-103">SyncFolderId</span><span class="sxs-lookup"><span data-stu-id="5f046-103">SyncFolderId</span></span>

<span data-ttu-id="5f046-104">**SyncFolderId**要素は、同期するアイテムを含むフォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="5f046-104">The **SyncFolderId** element represents the folder that contains the items to synchronize.</span></span> 
  
```xml
<SyncFolderId>
   <FolderId/>
</SyncFolderId>
```

```xml
<SyncFolderId>
   <DistinguishedFolderId/> 
</SyncFolderId>
```

<span data-ttu-id="5f046-105">**TargetFolderIdType**</span><span class="sxs-lookup"><span data-stu-id="5f046-105">**TargetFolderIdType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="5f046-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="5f046-106">Attributes and elements</span></span>

<span data-ttu-id="5f046-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5f046-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5f046-108">属性</span><span class="sxs-lookup"><span data-stu-id="5f046-108">Attributes</span></span>

<span data-ttu-id="5f046-109">なし。</span><span class="sxs-lookup"><span data-stu-id="5f046-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5f046-110">子要素</span><span class="sxs-lookup"><span data-stu-id="5f046-110">Child elements</span></span>

|<span data-ttu-id="5f046-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="5f046-111">**Element**</span></span>|<span data-ttu-id="5f046-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="5f046-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5f046-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="5f046-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="5f046-114">フォルダーの識別子と変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="5f046-114">Contains the identifier and change key of a folder.</span></span>  <br/> |
|[<span data-ttu-id="5f046-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="5f046-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="5f046-116">名前で参照できる Microsoft Exchange Server 2007 フォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="5f046-116">Identifies MicrosoftExchange Server 2007 folders that can be referenced by name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5f046-117">親要素</span><span class="sxs-lookup"><span data-stu-id="5f046-117">Parent elements</span></span>

|<span data-ttu-id="5f046-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="5f046-118">**Element**</span></span>|<span data-ttu-id="5f046-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="5f046-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5f046-120">SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="5f046-120">SyncFolderHierarchy</span></span>](syncfolderhierarchy.md) <br/> |<span data-ttu-id="5f046-121">Exchange ストア内のフォルダー階層を同期する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="5f046-121">Defines a request to synchronize a folder hierarchy in an Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5f046-122">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="5f046-122">SyncFolderItems</span></span>](syncfolderitems.md) <br/> |<span data-ttu-id="5f046-123">Exchange ストアフォルダー内のアイテムを同期する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="5f046-123">Defines a request to synchronize items in an Exchange store folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5f046-124">注釈</span><span class="sxs-lookup"><span data-stu-id="5f046-124">Remarks</span></span>

<span data-ttu-id="5f046-125">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="5f046-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5f046-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="5f046-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5f046-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="5f046-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5f046-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5f046-128">Schema name</span></span>  <br/> |<span data-ttu-id="5f046-129">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="5f046-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5f046-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5f046-130">Validation file</span></span>  <br/> |<span data-ttu-id="5f046-131">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="5f046-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5f046-132">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="5f046-132">Can be empty</span></span>  <br/> |<span data-ttu-id="5f046-133">正しくない</span><span class="sxs-lookup"><span data-stu-id="5f046-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5f046-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="5f046-134">See also</span></span>

- [<span data-ttu-id="5f046-135">SyncFolderItems 操作</span><span class="sxs-lookup"><span data-stu-id="5f046-135">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)
- [<span data-ttu-id="5f046-136">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="5f046-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

