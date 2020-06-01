---
title: BaseFolderIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- BaseFolderIds
api_type:
- schema
ms.assetid: bdaa6093-f960-469a-b338-0e75aaa536c6
description: BaseFolderIds 要素は、検索フォルダーの内容を確認するためにマイニングされるフォルダーのコレクションを表します。
ms.openlocfilehash: 97159ec1ded685e63aafedfaf90a06eff39adaab
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460268"
---
# <a name="basefolderids"></a><span data-ttu-id="95628-103">BaseFolderIds</span><span class="sxs-lookup"><span data-stu-id="95628-103">BaseFolderIds</span></span>

<span data-ttu-id="95628-104">**BaseFolderIds**要素は、検索フォルダーの内容を確認するためにマイニングされるフォルダーのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="95628-104">The **BaseFolderIds** element represents the collection of folders that will be mined to determine the contents of a search folder.</span></span> 
  
```xml
<BaseFolderIds>
   <FolderId/>
   <DistinguishedFolderId/>
</BaseFolderIds>
```

 <span data-ttu-id="95628-105">**非 Emptyarrayofbasefolderidstype**</span><span class="sxs-lookup"><span data-stu-id="95628-105">**NonEmptyArrayOfBaseFolderIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="95628-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="95628-106">Attributes and elements</span></span>

<span data-ttu-id="95628-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="95628-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="95628-108">属性</span><span class="sxs-lookup"><span data-stu-id="95628-108">Attributes</span></span>

<span data-ttu-id="95628-109">なし。</span><span class="sxs-lookup"><span data-stu-id="95628-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="95628-110">子要素</span><span class="sxs-lookup"><span data-stu-id="95628-110">Child elements</span></span>

|<span data-ttu-id="95628-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="95628-111">**Element**</span></span>|<span data-ttu-id="95628-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="95628-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="95628-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="95628-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="95628-114">フォルダーの識別子と変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="95628-114">Contains the identifier and change key of a folder.</span></span>  <br/> |
|[<span data-ttu-id="95628-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="95628-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="95628-116">名前で参照できる Microsoft Exchange Server 2007 フォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="95628-116">Identifies MicrosoftExchange Server 2007 folders that can be referenced by name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="95628-117">親要素</span><span class="sxs-lookup"><span data-stu-id="95628-117">Parent elements</span></span>

|<span data-ttu-id="95628-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="95628-118">**Element**</span></span>|<span data-ttu-id="95628-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="95628-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="95628-120">SearchParameters</span><span class="sxs-lookup"><span data-stu-id="95628-120">SearchParameters</span></span>](searchparameters.md) <br/> |<span data-ttu-id="95628-121">検索フォルダーを定義するパラメーターを表します。</span><span class="sxs-lookup"><span data-stu-id="95628-121">Represents the parameters that define a search folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="95628-122">注釈</span><span class="sxs-lookup"><span data-stu-id="95628-122">Remarks</span></span>

<span data-ttu-id="95628-123">**BaseFolderIds**要素には、少なくとも1つの[FolderId](folderid.md)または[DistinguishedFolderId](distinguishedfolderid.md)要素が含まれている必要があります。</span><span class="sxs-lookup"><span data-stu-id="95628-123">The **BaseFolderIds** element must contain at least one [FolderId](folderid.md) or [DistinguishedFolderId](distinguishedfolderid.md) element.</span></span> 
  
<span data-ttu-id="95628-124">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="95628-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="95628-125">要素の情報</span><span class="sxs-lookup"><span data-stu-id="95628-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="95628-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="95628-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="95628-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="95628-127">Schema name</span></span>  <br/> |<span data-ttu-id="95628-128">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="95628-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="95628-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="95628-129">Validation file</span></span>  <br/> |<span data-ttu-id="95628-130">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="95628-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="95628-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="95628-131">Can be empty</span></span>  <br/> |<span data-ttu-id="95628-132">正しくない</span><span class="sxs-lookup"><span data-stu-id="95628-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="95628-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="95628-133">See also</span></span>



- [<span data-ttu-id="95628-134">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="95628-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

