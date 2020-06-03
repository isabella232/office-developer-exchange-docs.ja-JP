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
description: ReadFlagChange 要素は、アイテムが読み取られたときに、SyncFolderItems 操作の応答で返されます。 このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。
ms.openlocfilehash: 354f8085a6ea5b738d8619e2ffeb0fbccefd51da
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468307"
---
# <a name="readflagchange"></a><span data-ttu-id="ddee8-104">ReadFlagChange</span><span class="sxs-lookup"><span data-stu-id="ddee8-104">ReadFlagChange</span></span>

<span data-ttu-id="ddee8-105">**Readflagchange**要素は、アイテムが読み取られたときに、 [syncfolderitems 操作](syncfolderitems-operation.md)の応答で返されます。</span><span class="sxs-lookup"><span data-stu-id="ddee8-105">The **ReadFlagChange** element is returned in [SyncFolderItems operation](syncfolderitems-operation.md) responses when an item has been read.</span></span> <span data-ttu-id="ddee8-106">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="ddee8-106">This property is read-only.</span></span> 
  
```xml
<ReadFlagChange>
   <ItemId/>
   <IsRead/>
</ReadFlagChange>
```

 <span data-ttu-id="ddee8-107">**SyncFolderItemsReadFlagType**</span><span class="sxs-lookup"><span data-stu-id="ddee8-107">**SyncFolderItemsReadFlagType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ddee8-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="ddee8-108">Attributes and elements</span></span>

<span data-ttu-id="ddee8-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ddee8-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ddee8-110">属性</span><span class="sxs-lookup"><span data-stu-id="ddee8-110">Attributes</span></span>

<span data-ttu-id="ddee8-111">なし。</span><span class="sxs-lookup"><span data-stu-id="ddee8-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ddee8-112">子要素</span><span class="sxs-lookup"><span data-stu-id="ddee8-112">Child elements</span></span>

|<span data-ttu-id="ddee8-113">**Element**</span><span class="sxs-lookup"><span data-stu-id="ddee8-113">**Element**</span></span>|<span data-ttu-id="ddee8-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="ddee8-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ddee8-115">ItemId</span><span class="sxs-lookup"><span data-stu-id="ddee8-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="ddee8-116">読み取りフラグが変更されたアイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="ddee8-116">Identifies the item for which the read-flag has been changed.</span></span>  <br/> |
|[<span data-ttu-id="ddee8-117">IsRead</span><span class="sxs-lookup"><span data-stu-id="ddee8-117">IsRead</span></span>](isread.md) <br/> |<span data-ttu-id="ddee8-118">読み取りフラグが**true**に設定されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ddee8-118">Indicates whether the read-flag has been set to **true**.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ddee8-119">親要素</span><span class="sxs-lookup"><span data-stu-id="ddee8-119">Parent elements</span></span>

|<span data-ttu-id="ddee8-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="ddee8-120">**Element**</span></span>|<span data-ttu-id="ddee8-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="ddee8-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ddee8-122">変更 (アイテム)</span><span class="sxs-lookup"><span data-stu-id="ddee8-122">Changes (Items)</span></span>](changes-items.md) <br/> |<span data-ttu-id="ddee8-123">クライアント上のアイテムと Exchange サーバー上のアイテムの間の相違点の種類を表す、変更の種類のシーケンス配列を含みます。</span><span class="sxs-lookup"><span data-stu-id="ddee8-123">Contains a sequence array of change types that represent the types of differences between the items on the client and the items on the Exchange server.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ddee8-124">注釈</span><span class="sxs-lookup"><span data-stu-id="ddee8-124">Remarks</span></span>

<span data-ttu-id="ddee8-125">この要素を記述するスキーマは、Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="ddee8-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ddee8-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="ddee8-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ddee8-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="ddee8-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ddee8-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ddee8-128">Schema Name</span></span>  <br/> |<span data-ttu-id="ddee8-129">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="ddee8-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="ddee8-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ddee8-130">Validation File</span></span>  <br/> |<span data-ttu-id="ddee8-131">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="ddee8-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ddee8-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="ddee8-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="ddee8-133">正しくない</span><span class="sxs-lookup"><span data-stu-id="ddee8-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ddee8-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="ddee8-134">See also</span></span>



- [<span data-ttu-id="ddee8-135">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="ddee8-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

