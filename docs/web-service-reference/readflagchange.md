---
title: ReadFlagChange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ReadFlagChange
api_type:
- schema
ms.assetid: 527bfe90-63d0-4b2f-97f7-7875b3a516b2
description: ReadFlagChange 要素が返されます SyncFolderItems の操作の応答アイテムを開封したとき。 このプロパティは値の取得のみ可能です。
ms.openlocfilehash: 28ef0267e8308ba58057bec01ab2672a19ee94a1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832953"
---
# <a name="readflagchange"></a><span data-ttu-id="38866-104">ReadFlagChange</span><span class="sxs-lookup"><span data-stu-id="38866-104">ReadFlagChange</span></span>

<span data-ttu-id="38866-105">**ReadFlagChange**要素は、アイテムを開封したとき、 [SyncFolderItems 操作](syncfolderitems-operation.md)の応答で返されます。</span><span class="sxs-lookup"><span data-stu-id="38866-105">The **ReadFlagChange** element is returned in [SyncFolderItems operation](syncfolderitems-operation.md) responses when an item has been read.</span></span> <span data-ttu-id="38866-106">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="38866-106">This property is read-only.</span></span> 
  
```xml
<ReadFlagChange>
   <ItemId/>
   <IsRead/>
</ReadFlagChange>
```

 <span data-ttu-id="38866-107">**SyncFolderItemsReadFlagType**</span><span class="sxs-lookup"><span data-stu-id="38866-107">**SyncFolderItemsReadFlagType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="38866-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="38866-108">Attributes and elements</span></span>

<span data-ttu-id="38866-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="38866-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="38866-110">属性</span><span class="sxs-lookup"><span data-stu-id="38866-110">Attributes</span></span>

<span data-ttu-id="38866-111">なし。</span><span class="sxs-lookup"><span data-stu-id="38866-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="38866-112">子要素</span><span class="sxs-lookup"><span data-stu-id="38866-112">Child elements</span></span>

|<span data-ttu-id="38866-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="38866-113">**Element**</span></span>|<span data-ttu-id="38866-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="38866-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="38866-115">ItemId</span><span class="sxs-lookup"><span data-stu-id="38866-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="38866-116">Read フラグが変更された項目を識別します。</span><span class="sxs-lookup"><span data-stu-id="38866-116">Identifies the item for which the read-flag has been changed.</span></span>  <br/> |
|[<span data-ttu-id="38866-117">IsRead</span><span class="sxs-lookup"><span data-stu-id="38866-117">IsRead</span></span>](isread.md) <br/> |<span data-ttu-id="38866-118">Read フラグが**true**に設定されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="38866-118">Indicates whether the read-flag has been set to **true**.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="38866-119">親要素</span><span class="sxs-lookup"><span data-stu-id="38866-119">Parent elements</span></span>

|<span data-ttu-id="38866-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="38866-120">**Element**</span></span>|<span data-ttu-id="38866-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="38866-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="38866-122">変更 (アイテム)</span><span class="sxs-lookup"><span data-stu-id="38866-122">Changes (Items)</span></span>](changes-items.md) <br/> |<span data-ttu-id="38866-123">クライアント上のアイテムと、Exchange サーバー上のアイテム間の相違点の種類を表すの種類の変更の順序の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="38866-123">Contains a sequence array of change types that represent the types of differences between the items on the client and the items on the Exchange server.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="38866-124">備考</span><span class="sxs-lookup"><span data-stu-id="38866-124">Remarks</span></span>

<span data-ttu-id="38866-125">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="38866-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="38866-126">要素情報</span><span class="sxs-lookup"><span data-stu-id="38866-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="38866-127">名前空間</span><span class="sxs-lookup"><span data-stu-id="38866-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="38866-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="38866-128">Schema Name</span></span>  <br/> |<span data-ttu-id="38866-129">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="38866-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="38866-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="38866-130">Validation File</span></span>  <br/> |<span data-ttu-id="38866-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="38866-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="38866-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="38866-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="38866-133">False</span><span class="sxs-lookup"><span data-stu-id="38866-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="38866-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="38866-134">See also</span></span>



- [<span data-ttu-id="38866-135">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="38866-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

