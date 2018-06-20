---
title: SourceIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SourceIds
api_type:
- schema
ms.assetid: 0043abd5-ba9c-4d67-8832-325f32bf7651
description: SourceIds 要素には、変換するソース識別子が含まれています。
ms.openlocfilehash: c9ee9fd01367f714e1cb3770e2be5161cb45d98f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833522"
---
# <a name="sourceids"></a><span data-ttu-id="592e4-103">SourceIds</span><span class="sxs-lookup"><span data-stu-id="592e4-103">SourceIds</span></span>

<span data-ttu-id="592e4-104">**SourceIds**要素には、変換するソース識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="592e4-104">The **SourceIds** element contains the source identifiers to convert.</span></span> 
  
[<span data-ttu-id="592e4-105">ConvertId</span><span class="sxs-lookup"><span data-stu-id="592e4-105">ConvertId</span></span>](convertid.md)
  
[<span data-ttu-id="592e4-106">SourceIds</span><span class="sxs-lookup"><span data-stu-id="592e4-106">SourceIds</span></span>](sourceids.md)
  
```xml
<SourceIds>
   <AlternateId/>
   <AlternatePublicFolderId/>
   <AlternatePublicFolderItemId/>
</SourceIds>
```

 <span data-ttu-id="592e4-107">**NonEmptyArrayOfAlternateIdsType**</span><span class="sxs-lookup"><span data-stu-id="592e4-107">**NonEmptyArrayOfAlternateIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="592e4-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="592e4-108">Attributes and elements</span></span>

<span data-ttu-id="592e4-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="592e4-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="592e4-110">属性</span><span class="sxs-lookup"><span data-stu-id="592e4-110">Attributes</span></span>

<span data-ttu-id="592e4-111">なし。</span><span class="sxs-lookup"><span data-stu-id="592e4-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="592e4-112">子要素</span><span class="sxs-lookup"><span data-stu-id="592e4-112">Child elements</span></span>

|<span data-ttu-id="592e4-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="592e4-113">**Element**</span></span>|<span data-ttu-id="592e4-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="592e4-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="592e4-115">AlternateId</span><span class="sxs-lookup"><span data-stu-id="592e4-115">AlternateId</span></span>](alternateid.md) <br/> |<span data-ttu-id="592e4-116">アイテムまたはフォルダーの識別子を変換について説明します。</span><span class="sxs-lookup"><span data-stu-id="592e4-116">Describes an item or folder identifier to convert.</span></span>  <br/> |
|[<span data-ttu-id="592e4-117">AlternatePublicFolderId</span><span class="sxs-lookup"><span data-stu-id="592e4-117">AlternatePublicFolderId</span></span>](alternatepublicfolderid.md) <br/> |<span data-ttu-id="592e4-118">変換するパブリック フォルダーの識別子について説明します。</span><span class="sxs-lookup"><span data-stu-id="592e4-118">Describes a public folder identifier to convert.</span></span>  <br/> |
|[<span data-ttu-id="592e4-119">AlternatePublicFolderItemId</span><span class="sxs-lookup"><span data-stu-id="592e4-119">AlternatePublicFolderItemId</span></span>](alternatepublicfolderitemid.md) <br/> |<span data-ttu-id="592e4-120">変換するパブリック フォルダーの項目識別子をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="592e4-120">Describes a public folder item identifier to convert.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="592e4-121">親要素</span><span class="sxs-lookup"><span data-stu-id="592e4-121">Parent elements</span></span>

|<span data-ttu-id="592e4-122">**要素**</span><span class="sxs-lookup"><span data-stu-id="592e4-122">**Element**</span></span>|<span data-ttu-id="592e4-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="592e4-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="592e4-124">ConvertId</span><span class="sxs-lookup"><span data-stu-id="592e4-124">ConvertId</span></span>](convertid.md) <br/> |<span data-ttu-id="592e4-125">Exchange がサポートされている形式の間でのアイテムおよびフォルダーの識別子を変換するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="592e4-125">Defines a request to convert item and folder identifiers between Exchange supported formats.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="592e4-126">備考</span><span class="sxs-lookup"><span data-stu-id="592e4-126">Remarks</span></span>

<span data-ttu-id="592e4-127">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="592e4-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="592e4-128">要素情報</span><span class="sxs-lookup"><span data-stu-id="592e4-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="592e4-129">名前空間</span><span class="sxs-lookup"><span data-stu-id="592e4-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="592e4-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="592e4-130">Schema Name</span></span>  <br/> |<span data-ttu-id="592e4-131">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="592e4-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="592e4-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="592e4-132">Validation File</span></span>  <br/> |<span data-ttu-id="592e4-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="592e4-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="592e4-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="592e4-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="592e4-135">False</span><span class="sxs-lookup"><span data-stu-id="592e4-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="592e4-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="592e4-136">See also</span></span>



[<span data-ttu-id="592e4-137">ConvertId 操作</span><span class="sxs-lookup"><span data-stu-id="592e4-137">ConvertId operation</span></span>](convertid-operation.md)


- [<span data-ttu-id="592e4-138">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="592e4-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="592e4-139">識別子に変換します。</span><span class="sxs-lookup"><span data-stu-id="592e4-139">Converting Identifiers</span></span>](http://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

