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
description: BaseFolderIds 要素は、検索フォルダーの内容を判断するためにマイニングするフォルダーのコレクションを表します。
ms.openlocfilehash: 960e4d9c1d6eb37bf988bf163e696cbba3e1ef6f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759482"
---
# <a name="basefolderids"></a><span data-ttu-id="260fd-103">BaseFolderIds</span><span class="sxs-lookup"><span data-stu-id="260fd-103">BaseFolderIds</span></span>

<span data-ttu-id="260fd-104">**BaseFolderIds**要素は、検索フォルダーの内容を判断するためにマイニングするフォルダーのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="260fd-104">The **BaseFolderIds** element represents the collection of folders that will be mined to determine the contents of a search folder.</span></span> 
  
```xml
<BaseFolderIds>
   <FolderId/>
   <DistinguishedFolderId/>
</BaseFolderIds>
```

 <span data-ttu-id="260fd-105">**NonEmptyArrayOfBaseFolderIdsType**</span><span class="sxs-lookup"><span data-stu-id="260fd-105">**NonEmptyArrayOfBaseFolderIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="260fd-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="260fd-106">Attributes and elements</span></span>

<span data-ttu-id="260fd-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="260fd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="260fd-108">属性</span><span class="sxs-lookup"><span data-stu-id="260fd-108">Attributes</span></span>

<span data-ttu-id="260fd-109">なし。</span><span class="sxs-lookup"><span data-stu-id="260fd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="260fd-110">子要素</span><span class="sxs-lookup"><span data-stu-id="260fd-110">Child elements</span></span>

|<span data-ttu-id="260fd-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="260fd-111">**Element**</span></span>|<span data-ttu-id="260fd-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="260fd-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="260fd-113">フォルダー Id</span><span class="sxs-lookup"><span data-stu-id="260fd-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="260fd-114">フォルダーの識別子と変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="260fd-114">Contains the identifier and change key of a folder.</span></span>  <br/> |
|[<span data-ttu-id="260fd-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="260fd-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="260fd-116">名前で参照することができます MicrosoftExchange Server 2007 フォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="260fd-116">Identifies MicrosoftExchange Server 2007 folders that can be referenced by name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="260fd-117">親要素</span><span class="sxs-lookup"><span data-stu-id="260fd-117">Parent elements</span></span>

|<span data-ttu-id="260fd-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="260fd-118">**Element**</span></span>|<span data-ttu-id="260fd-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="260fd-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="260fd-120">SearchParameters</span><span class="sxs-lookup"><span data-stu-id="260fd-120">SearchParameters</span></span>](searchparameters.md) <br/> |<span data-ttu-id="260fd-121">検索フォルダーを定義するパラメーターを表します。</span><span class="sxs-lookup"><span data-stu-id="260fd-121">Represents the parameters that define a search folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="260fd-122">備考</span><span class="sxs-lookup"><span data-stu-id="260fd-122">Remarks</span></span>

<span data-ttu-id="260fd-123">**BaseFolderIds**要素は、少なくとも 1 つの[フォルダー Id](folderid.md)または[DistinguishedFolderId](distinguishedfolderid.md)の要素を含める必要があります。</span><span class="sxs-lookup"><span data-stu-id="260fd-123">The **BaseFolderIds** element must contain at least one [FolderId](folderid.md) or [DistinguishedFolderId](distinguishedfolderid.md) element.</span></span> 
  
<span data-ttu-id="260fd-124">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="260fd-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="260fd-125">要素情報</span><span class="sxs-lookup"><span data-stu-id="260fd-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="260fd-126">名前空間</span><span class="sxs-lookup"><span data-stu-id="260fd-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="260fd-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="260fd-127">Schema name</span></span>  <br/> |<span data-ttu-id="260fd-128">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="260fd-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="260fd-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="260fd-129">Validation file</span></span>  <br/> |<span data-ttu-id="260fd-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="260fd-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="260fd-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="260fd-131">Can be empty</span></span>  <br/> |<span data-ttu-id="260fd-132">False</span><span class="sxs-lookup"><span data-stu-id="260fd-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="260fd-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="260fd-133">See also</span></span>



- [<span data-ttu-id="260fd-134">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="260fd-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

