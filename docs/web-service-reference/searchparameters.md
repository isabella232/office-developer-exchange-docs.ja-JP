---
title: SearchParameters
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SearchParameters
api_type:
- schema
ms.assetid: 34602cb1-dc33-4552-a98c-3e77f614daa3
description: SearchParameters 要素は、検索フォルダーを定義するパラメーターを表します。
ms.openlocfilehash: b534574a1292d78c8df99f5186990b114fc4e70a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833299"
---
# <a name="searchparameters"></a><span data-ttu-id="f711f-103">SearchParameters</span><span class="sxs-lookup"><span data-stu-id="f711f-103">SearchParameters</span></span>

<span data-ttu-id="f711f-104">**SearchParameters**要素は、検索フォルダーを定義するパラメーターを表します。</span><span class="sxs-lookup"><span data-stu-id="f711f-104">The **SearchParameters** element represents the parameters that define a search folder.</span></span> 
  
```xml
<SearchParameters Traversal="">
   <Restriction/>
   <BaseFolderIds/>
</SearchParameters>
```

 <span data-ttu-id="f711f-105">**SearchParametersType**</span><span class="sxs-lookup"><span data-stu-id="f711f-105">**SearchParametersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f711f-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="f711f-106">Attributes and elements</span></span>

<span data-ttu-id="f711f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f711f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f711f-108">属性</span><span class="sxs-lookup"><span data-stu-id="f711f-108">Attributes</span></span>

|<span data-ttu-id="f711f-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="f711f-109">**Attribute**</span></span>|<span data-ttu-id="f711f-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="f711f-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f711f-111">**トラバーサル**</span><span class="sxs-lookup"><span data-stu-id="f711f-111">**Traversal**</span></span> <br/> |<span data-ttu-id="f711f-112">検索フォルダーがフォルダー階層を走査する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="f711f-112">Describes how a search folder traverses the folder hierarchy.</span></span> <span data-ttu-id="f711f-113">オプションは、**深い**または**簡易**検索のいずれかのです。</span><span class="sxs-lookup"><span data-stu-id="f711f-113">The options are for either a **Deep** or a **Shallow** search.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="f711f-114">子要素</span><span class="sxs-lookup"><span data-stu-id="f711f-114">Child elements</span></span>

|<span data-ttu-id="f711f-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="f711f-115">**Element**</span></span>|<span data-ttu-id="f711f-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="f711f-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f711f-117">Restriction</span><span class="sxs-lookup"><span data-stu-id="f711f-117">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="f711f-118">制限またはアイテムまたはフォルダーの FindItem/FindFolder、検索フォルダーの操作にフィルターを適用するために使用するクエリを表します。</span><span class="sxs-lookup"><span data-stu-id="f711f-118">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="f711f-119">BaseFolderIds</span><span class="sxs-lookup"><span data-stu-id="f711f-119">BaseFolderIds</span></span>](basefolderids.md) <br/> |<span data-ttu-id="f711f-120">検索フォルダーの内容を判断するためにマイニングするフォルダーのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="f711f-120">Represents the collection of folders that will be mined to determine the contents of a search folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f711f-121">親要素</span><span class="sxs-lookup"><span data-stu-id="f711f-121">Parent elements</span></span>

|<span data-ttu-id="f711f-122">**要素**</span><span class="sxs-lookup"><span data-stu-id="f711f-122">**Element**</span></span>|<span data-ttu-id="f711f-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="f711f-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f711f-124">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="f711f-124">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="f711f-125">メールボックスに格納されている検索フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="f711f-125">Represents a search folder that is contained in a mailbox.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f711f-126">備考</span><span class="sxs-lookup"><span data-stu-id="f711f-126">Remarks</span></span>

<span data-ttu-id="f711f-127">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="f711f-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f711f-128">要素情報</span><span class="sxs-lookup"><span data-stu-id="f711f-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f711f-129">名前空間</span><span class="sxs-lookup"><span data-stu-id="f711f-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f711f-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f711f-130">Schema Name</span></span>  <br/> |<span data-ttu-id="f711f-131">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="f711f-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="f711f-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f711f-132">Validation File</span></span>  <br/> |<span data-ttu-id="f711f-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f711f-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f711f-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="f711f-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="f711f-135">False</span><span class="sxs-lookup"><span data-stu-id="f711f-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f711f-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="f711f-136">See also</span></span>



- [<span data-ttu-id="f711f-137">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="f711f-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

