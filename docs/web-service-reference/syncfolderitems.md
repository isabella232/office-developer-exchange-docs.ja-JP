---
title: SyncFolderItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncFolderItems
api_type:
- schema
ms.assetid: 463ed78c-bf82-4cd8-971a-d18425e9e7be
description: SyncFolderItems 要素は、Exchange ストアのフォルダーのアイテムを同期するための要求を定義します。
ms.openlocfilehash: 368e19babfccaeab40380103495c63d30647905c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839638"
---
# <a name="syncfolderitems"></a><span data-ttu-id="6d0ca-103">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="6d0ca-103">SyncFolderItems</span></span>

<span data-ttu-id="6d0ca-104">**SyncFolderItems**要素は、Exchange ストアのフォルダーのアイテムを同期するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="6d0ca-104">The **SyncFolderItems** element defines a request to synchronize items in an Exchange store folder.</span></span> 
  
```xml
<SyncFolderItems>
   <ItemShape/>
   <SyncFolderId/>
   <SyncState/>
   <Ignore/>
   <MaxChangesReturned/>   <SyncScope/>
</SyncFolderItems>
```

 <span data-ttu-id="6d0ca-105">**SyncFolderItemsType**</span><span class="sxs-lookup"><span data-stu-id="6d0ca-105">**SyncFolderItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6d0ca-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="6d0ca-106">Attributes and elements</span></span>

<span data-ttu-id="6d0ca-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6d0ca-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6d0ca-108">属性</span><span class="sxs-lookup"><span data-stu-id="6d0ca-108">Attributes</span></span>

<span data-ttu-id="6d0ca-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6d0ca-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6d0ca-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6d0ca-110">Child elements</span></span>

|<span data-ttu-id="6d0ca-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="6d0ca-111">**Element**</span></span>|<span data-ttu-id="6d0ca-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="6d0ca-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6d0ca-113">ItemShape</span><span class="sxs-lookup"><span data-stu-id="6d0ca-113">ItemShape</span></span>](itemshape.md) <br/> |<span data-ttu-id="6d0ca-114">SyncFolderItems の応答に含めるコンテンツ アイテムのプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="6d0ca-114">Identifies the item properties and content to include in a SyncFolderItems response.</span></span> <span data-ttu-id="6d0ca-115">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="6d0ca-115">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="6d0ca-116">SyncFolderId</span><span class="sxs-lookup"><span data-stu-id="6d0ca-116">SyncFolderId</span></span>](syncfolderid.md) <br/> |<span data-ttu-id="6d0ca-117">同期する項目を含むフォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="6d0ca-117">Represents the folder that contains the items to synchronize.</span></span> <span data-ttu-id="6d0ca-118">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="6d0ca-118">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="6d0ca-119">同期状態</span><span class="sxs-lookup"><span data-stu-id="6d0ca-119">SyncState</span></span>](syncstate-ex15websvcsotherref.md) <br/> |<span data-ttu-id="6d0ca-120">各成功した要求の後に更新された同期データの base64 でエンコードされたフォームが含まれています。</span><span class="sxs-lookup"><span data-stu-id="6d0ca-120">Contains a base64-encoded form of the synchronization data that is updated after each successful request.</span></span> <span data-ttu-id="6d0ca-121">これを使用して、同期の状態を識別します。</span><span class="sxs-lookup"><span data-stu-id="6d0ca-121">This is used to identify the synchronization state.</span></span> <span data-ttu-id="6d0ca-122">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="6d0ca-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="6d0ca-123">Ignore</span><span class="sxs-lookup"><span data-stu-id="6d0ca-123">Ignore</span></span>](ignore.md) <br/> |<span data-ttu-id="6d0ca-124">同期中にスキップする項目を識別します。</span><span class="sxs-lookup"><span data-stu-id="6d0ca-124">Identifies items to skip during synchronization.</span></span> <span data-ttu-id="6d0ca-125">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="6d0ca-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="6d0ca-126">MaxChangesReturned</span><span class="sxs-lookup"><span data-stu-id="6d0ca-126">MaxChangesReturned</span></span>](maxchangesreturned.md) <br/> |<span data-ttu-id="6d0ca-127">同期応答で返すことができる変更の最大数について説明します。</span><span class="sxs-lookup"><span data-stu-id="6d0ca-127">Describes the maximum number of changes that can be returned in a synchronization response.</span></span> <span data-ttu-id="6d0ca-128">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="6d0ca-128">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="6d0ca-129">SyncScope</span><span class="sxs-lookup"><span data-stu-id="6d0ca-129">SyncScope</span></span>](syncscope.md) <br/> |<span data-ttu-id="6d0ca-130">同期応答内のアイテムまたはアイテムおよびフォルダーに関連付けられている情報だけを返すかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="6d0ca-130">Specifies whether just items or items and folder associated information are returned in a synchronization response.</span></span> <span data-ttu-id="6d0ca-131">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="6d0ca-131">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6d0ca-132">親要素</span><span class="sxs-lookup"><span data-stu-id="6d0ca-132">Parent elements</span></span>

<span data-ttu-id="6d0ca-133">なし。</span><span class="sxs-lookup"><span data-stu-id="6d0ca-133">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6d0ca-134">備考</span><span class="sxs-lookup"><span data-stu-id="6d0ca-134">Remarks</span></span>

<span data-ttu-id="6d0ca-135">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="6d0ca-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6d0ca-136">要素情報</span><span class="sxs-lookup"><span data-stu-id="6d0ca-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6d0ca-137">名前空間</span><span class="sxs-lookup"><span data-stu-id="6d0ca-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6d0ca-138">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6d0ca-138">Schema name</span></span>  <br/> |<span data-ttu-id="6d0ca-139">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="6d0ca-139">messages schema</span></span>  <br/> |
|<span data-ttu-id="6d0ca-140">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6d0ca-140">Validation file</span></span>  <br/> |<span data-ttu-id="6d0ca-141">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6d0ca-141">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6d0ca-142">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="6d0ca-142">Can be empty</span></span>  <br/> |<span data-ttu-id="6d0ca-143">False</span><span class="sxs-lookup"><span data-stu-id="6d0ca-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6d0ca-144">関連項目</span><span class="sxs-lookup"><span data-stu-id="6d0ca-144">See also</span></span>



[<span data-ttu-id="6d0ca-145">SyncFolderItems の操作</span><span class="sxs-lookup"><span data-stu-id="6d0ca-145">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="6d0ca-146">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="6d0ca-146">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

