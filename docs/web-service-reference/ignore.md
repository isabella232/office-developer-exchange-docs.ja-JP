---
title: 無視
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
description: Ignore 要素は、同期中にスキップするアイテムを識別します。
ms.openlocfilehash: b65d11d8c7655279dac0e7d3cbd13f8a9317540c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458573"
---
# <a name="ignore"></a><span data-ttu-id="2d849-103">無視</span><span class="sxs-lookup"><span data-stu-id="2d849-103">Ignore</span></span>

<span data-ttu-id="2d849-104">**Ignore**要素は、同期中にスキップするアイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="2d849-104">The **Ignore** element identifies items to skip during synchronization.</span></span> 
  
[<span data-ttu-id="2d849-105">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="2d849-105">SyncFolderItems</span></span>](syncfolderitems.md)
  
[<span data-ttu-id="2d849-106">無視</span><span class="sxs-lookup"><span data-stu-id="2d849-106">Ignore</span></span>](ignore.md)
  
```xml
<Ignore>
   <ItemId/>
</Ignore>
```

 <span data-ttu-id="2d849-107">**ArrayOfBaseItemIdsType**</span><span class="sxs-lookup"><span data-stu-id="2d849-107">**ArrayOfBaseItemIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2d849-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="2d849-108">Attributes and elements</span></span>

<span data-ttu-id="2d849-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2d849-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2d849-110">属性</span><span class="sxs-lookup"><span data-stu-id="2d849-110">Attributes</span></span>

<span data-ttu-id="2d849-111">なし。</span><span class="sxs-lookup"><span data-stu-id="2d849-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2d849-112">子要素</span><span class="sxs-lookup"><span data-stu-id="2d849-112">Child elements</span></span>

|<span data-ttu-id="2d849-113">**Element**</span><span class="sxs-lookup"><span data-stu-id="2d849-113">**Element**</span></span>|<span data-ttu-id="2d849-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="2d849-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2d849-115">ItemId</span><span class="sxs-lookup"><span data-stu-id="2d849-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="2d849-116">Exchange ストア内のアイテムの一意識別子および変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="2d849-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2d849-117">親要素</span><span class="sxs-lookup"><span data-stu-id="2d849-117">Parent elements</span></span>

|<span data-ttu-id="2d849-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="2d849-118">**Element**</span></span>|<span data-ttu-id="2d849-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="2d849-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2d849-120">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="2d849-120">SyncFolderItems</span></span>](syncfolderitems.md) <br/> |<span data-ttu-id="2d849-121">Exchange ストアフォルダー内のアイテムを同期する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="2d849-121">Defines a request to synchronize items in an Exchange store folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2d849-122">注釈</span><span class="sxs-lookup"><span data-stu-id="2d849-122">Remarks</span></span>

<span data-ttu-id="2d849-123">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="2d849-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2d849-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="2d849-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2d849-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="2d849-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2d849-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2d849-126">Schema name</span></span>  <br/> |<span data-ttu-id="2d849-127">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="2d849-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="2d849-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2d849-128">Validation file</span></span>  <br/> |<span data-ttu-id="2d849-129">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="2d849-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2d849-130">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="2d849-130">Can be empty</span></span>  <br/> |<span data-ttu-id="2d849-131">正しくない</span><span class="sxs-lookup"><span data-stu-id="2d849-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2d849-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="2d849-132">See also</span></span>



[<span data-ttu-id="2d849-133">SyncFolderItems 操作</span><span class="sxs-lookup"><span data-stu-id="2d849-133">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="2d849-134">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="2d849-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

