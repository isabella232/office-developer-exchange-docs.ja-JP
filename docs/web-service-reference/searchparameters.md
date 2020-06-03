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
ms.openlocfilehash: cd9f255621b17d01113392e67a0301b01b70f326
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466669"
---
# <a name="searchparameters"></a><span data-ttu-id="94a46-103">SearchParameters</span><span class="sxs-lookup"><span data-stu-id="94a46-103">SearchParameters</span></span>

<span data-ttu-id="94a46-104">**Searchparameters**要素は、検索フォルダーを定義するパラメーターを表します。</span><span class="sxs-lookup"><span data-stu-id="94a46-104">The **SearchParameters** element represents the parameters that define a search folder.</span></span> 
  
```xml
<SearchParameters Traversal="">
   <Restriction/>
   <BaseFolderIds/>
</SearchParameters>
```

 <span data-ttu-id="94a46-105">**SearchParametersType**</span><span class="sxs-lookup"><span data-stu-id="94a46-105">**SearchParametersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="94a46-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="94a46-106">Attributes and elements</span></span>

<span data-ttu-id="94a46-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="94a46-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="94a46-108">属性</span><span class="sxs-lookup"><span data-stu-id="94a46-108">Attributes</span></span>

|<span data-ttu-id="94a46-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="94a46-109">**Attribute**</span></span>|<span data-ttu-id="94a46-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="94a46-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="94a46-111">**走査**</span><span class="sxs-lookup"><span data-stu-id="94a46-111">**Traversal**</span></span> <br/> |<span data-ttu-id="94a46-112">検索フォルダーがフォルダー階層をトラバースする方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="94a46-112">Describes how a search folder traverses the folder hierarchy.</span></span> <span data-ttu-id="94a46-113">オプションは、 **Deep**検索または**浅い**検索のどちらかです。</span><span class="sxs-lookup"><span data-stu-id="94a46-113">The options are for either a **Deep** or a **Shallow** search.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="94a46-114">子要素</span><span class="sxs-lookup"><span data-stu-id="94a46-114">Child elements</span></span>

|<span data-ttu-id="94a46-115">**Element**</span><span class="sxs-lookup"><span data-stu-id="94a46-115">**Element**</span></span>|<span data-ttu-id="94a46-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="94a46-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="94a46-117">制限</span><span class="sxs-lookup"><span data-stu-id="94a46-117">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="94a46-118">FindItem/FindFolder および search folder 操作のアイテムまたはフォルダーをフィルター処理するために使用される制限またはクエリを表します。</span><span class="sxs-lookup"><span data-stu-id="94a46-118">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="94a46-119">BaseFolderIds</span><span class="sxs-lookup"><span data-stu-id="94a46-119">BaseFolderIds</span></span>](basefolderids.md) <br/> |<span data-ttu-id="94a46-120">検索フォルダーのコンテンツを特定するためにマイニングされるフォルダーのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="94a46-120">Represents the collection of folders that will be mined to determine the contents of a search folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="94a46-121">親要素</span><span class="sxs-lookup"><span data-stu-id="94a46-121">Parent elements</span></span>

|<span data-ttu-id="94a46-122">**要素**</span><span class="sxs-lookup"><span data-stu-id="94a46-122">**Element**</span></span>|<span data-ttu-id="94a46-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="94a46-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="94a46-124">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="94a46-124">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="94a46-125">メールボックスに含まれている検索フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="94a46-125">Represents a search folder that is contained in a mailbox.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="94a46-126">注釈</span><span class="sxs-lookup"><span data-stu-id="94a46-126">Remarks</span></span>

<span data-ttu-id="94a46-127">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="94a46-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="94a46-128">要素の情報</span><span class="sxs-lookup"><span data-stu-id="94a46-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="94a46-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="94a46-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="94a46-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="94a46-130">Schema Name</span></span>  <br/> |<span data-ttu-id="94a46-131">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="94a46-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="94a46-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="94a46-132">Validation File</span></span>  <br/> |<span data-ttu-id="94a46-133">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="94a46-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="94a46-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="94a46-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="94a46-135">正しくない</span><span class="sxs-lookup"><span data-stu-id="94a46-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="94a46-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="94a46-136">See also</span></span>



- [<span data-ttu-id="94a46-137">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="94a46-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

