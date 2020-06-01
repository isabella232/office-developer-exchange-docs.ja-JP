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
description: SourceIds 要素は、変換するソース識別子を含みます。
ms.openlocfilehash: 1c4990f2185788c5cfaab5483cb6a54a0d850596
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466109"
---
# <a name="sourceids"></a><span data-ttu-id="47608-103">SourceIds</span><span class="sxs-lookup"><span data-stu-id="47608-103">SourceIds</span></span>

<span data-ttu-id="47608-104">**SourceIds**要素は、変換するソース識別子を含みます。</span><span class="sxs-lookup"><span data-stu-id="47608-104">The **SourceIds** element contains the source identifiers to convert.</span></span> 
  
[<span data-ttu-id="47608-105">ConvertId</span><span class="sxs-lookup"><span data-stu-id="47608-105">ConvertId</span></span>](convertid.md)
  
[<span data-ttu-id="47608-106">SourceIds</span><span class="sxs-lookup"><span data-stu-id="47608-106">SourceIds</span></span>](sourceids.md)
  
```xml
<SourceIds>
   <AlternateId/>
   <AlternatePublicFolderId/>
   <AlternatePublicFolderItemId/>
</SourceIds>
```

 <span data-ttu-id="47608-107">**NonEmptyArrayOfAlternateIdsType**</span><span class="sxs-lookup"><span data-stu-id="47608-107">**NonEmptyArrayOfAlternateIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="47608-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="47608-108">Attributes and elements</span></span>

<span data-ttu-id="47608-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="47608-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="47608-110">属性</span><span class="sxs-lookup"><span data-stu-id="47608-110">Attributes</span></span>

<span data-ttu-id="47608-111">なし。</span><span class="sxs-lookup"><span data-stu-id="47608-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="47608-112">子要素</span><span class="sxs-lookup"><span data-stu-id="47608-112">Child elements</span></span>

|<span data-ttu-id="47608-113">**Element**</span><span class="sxs-lookup"><span data-stu-id="47608-113">**Element**</span></span>|<span data-ttu-id="47608-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="47608-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="47608-115">AlternateId</span><span class="sxs-lookup"><span data-stu-id="47608-115">AlternateId</span></span>](alternateid.md) <br/> |<span data-ttu-id="47608-116">変換するアイテムまたはフォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="47608-116">Describes an item or folder identifier to convert.</span></span>  <br/> |
|[<span data-ttu-id="47608-117">AlternatePublicFolderId</span><span class="sxs-lookup"><span data-stu-id="47608-117">AlternatePublicFolderId</span></span>](alternatepublicfolderid.md) <br/> |<span data-ttu-id="47608-118">変換するパブリックフォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="47608-118">Describes a public folder identifier to convert.</span></span>  <br/> |
|[<span data-ttu-id="47608-119">AlternatePublicFolderItemId</span><span class="sxs-lookup"><span data-stu-id="47608-119">AlternatePublicFolderItemId</span></span>](alternatepublicfolderitemid.md) <br/> |<span data-ttu-id="47608-120">変換するパブリックフォルダーのアイテム識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="47608-120">Describes a public folder item identifier to convert.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="47608-121">親要素</span><span class="sxs-lookup"><span data-stu-id="47608-121">Parent elements</span></span>

|<span data-ttu-id="47608-122">**要素**</span><span class="sxs-lookup"><span data-stu-id="47608-122">**Element**</span></span>|<span data-ttu-id="47608-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="47608-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="47608-124">ConvertId</span><span class="sxs-lookup"><span data-stu-id="47608-124">ConvertId</span></span>](convertid.md) <br/> |<span data-ttu-id="47608-125">Exchange でサポートされている形式の間でアイテムとフォルダーの識別子を変換する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="47608-125">Defines a request to convert item and folder identifiers between Exchange supported formats.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="47608-126">注釈</span><span class="sxs-lookup"><span data-stu-id="47608-126">Remarks</span></span>

<span data-ttu-id="47608-127">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="47608-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="47608-128">要素の情報</span><span class="sxs-lookup"><span data-stu-id="47608-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="47608-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="47608-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="47608-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="47608-130">Schema Name</span></span>  <br/> |<span data-ttu-id="47608-131">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="47608-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="47608-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="47608-132">Validation File</span></span>  <br/> |<span data-ttu-id="47608-133">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="47608-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="47608-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="47608-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="47608-135">正しくない</span><span class="sxs-lookup"><span data-stu-id="47608-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="47608-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="47608-136">See also</span></span>



[<span data-ttu-id="47608-137">ConvertId 操作</span><span class="sxs-lookup"><span data-stu-id="47608-137">ConvertId operation</span></span>](convertid-operation.md)


- [<span data-ttu-id="47608-138">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="47608-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="47608-139">識別子の変換</span><span class="sxs-lookup"><span data-stu-id="47608-139">Converting Identifiers</span></span>](https://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

