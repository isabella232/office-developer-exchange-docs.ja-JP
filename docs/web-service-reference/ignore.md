---
title: 無視します。
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Ignore
api_type:
- schema
ms.assetid: 7789eec5-ceec-43f2-84d5-d0d15b734076
description: 無視する要素では、同期中にスキップする項目を識別します。
ms.openlocfilehash: 0ecff9bfeb1257552b7e52c0115e9e814edecd4b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831858"
---
# <a name="ignore"></a><span data-ttu-id="4d3ad-103">無視します。</span><span class="sxs-lookup"><span data-stu-id="4d3ad-103">Ignore</span></span>

<span data-ttu-id="4d3ad-104">**無視する**要素では、同期中にスキップする項目を識別します。</span><span class="sxs-lookup"><span data-stu-id="4d3ad-104">The **Ignore** element identifies items to skip during synchronization.</span></span> 
  
[<span data-ttu-id="4d3ad-105">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="4d3ad-105">SyncFolderItems</span></span>](syncfolderitems.md)
  
[<span data-ttu-id="4d3ad-106">Ignore</span><span class="sxs-lookup"><span data-stu-id="4d3ad-106">Ignore</span></span>](ignore.md)
  
```xml
<Ignore>
   <ItemId/>
</Ignore>
```

 <span data-ttu-id="4d3ad-107">**ArrayOfBaseItemIdsType**</span><span class="sxs-lookup"><span data-stu-id="4d3ad-107">**ArrayOfBaseItemIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4d3ad-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="4d3ad-108">Attributes and elements</span></span>

<span data-ttu-id="4d3ad-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4d3ad-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4d3ad-110">属性</span><span class="sxs-lookup"><span data-stu-id="4d3ad-110">Attributes</span></span>

<span data-ttu-id="4d3ad-111">なし。</span><span class="sxs-lookup"><span data-stu-id="4d3ad-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4d3ad-112">子要素</span><span class="sxs-lookup"><span data-stu-id="4d3ad-112">Child elements</span></span>

|<span data-ttu-id="4d3ad-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="4d3ad-113">**Element**</span></span>|<span data-ttu-id="4d3ad-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="4d3ad-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4d3ad-115">ItemId</span><span class="sxs-lookup"><span data-stu-id="4d3ad-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="4d3ad-116">Exchange ストア内のアイテムの一意の識別子と変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="4d3ad-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4d3ad-117">親要素</span><span class="sxs-lookup"><span data-stu-id="4d3ad-117">Parent elements</span></span>

|<span data-ttu-id="4d3ad-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="4d3ad-118">**Element**</span></span>|<span data-ttu-id="4d3ad-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="4d3ad-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4d3ad-120">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="4d3ad-120">SyncFolderItems</span></span>](syncfolderitems.md) <br/> |<span data-ttu-id="4d3ad-121">Exchange ストア フォルダー内のアイテムを同期するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="4d3ad-121">Defines a request to synchronize items in an Exchange store folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4d3ad-122">備考</span><span class="sxs-lookup"><span data-stu-id="4d3ad-122">Remarks</span></span>

<span data-ttu-id="4d3ad-123">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="4d3ad-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4d3ad-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="4d3ad-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4d3ad-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="4d3ad-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4d3ad-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4d3ad-126">Schema name</span></span>  <br/> |<span data-ttu-id="4d3ad-127">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="4d3ad-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4d3ad-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4d3ad-128">Validation file</span></span>  <br/> |<span data-ttu-id="4d3ad-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="4d3ad-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4d3ad-130">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="4d3ad-130">Can be empty</span></span>  <br/> |<span data-ttu-id="4d3ad-131">False</span><span class="sxs-lookup"><span data-stu-id="4d3ad-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4d3ad-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="4d3ad-132">See also</span></span>



[<span data-ttu-id="4d3ad-133">SyncFolderItems の操作</span><span class="sxs-lookup"><span data-stu-id="4d3ad-133">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="4d3ad-134">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="4d3ad-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

