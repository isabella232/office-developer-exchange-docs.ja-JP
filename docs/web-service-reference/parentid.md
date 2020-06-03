---
title: ParentId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bb7aaa46-3a04-4197-aebb-8881ff10603f
description: ParentId 要素は、検索プレビューで親アイテムの識別子を指定します。
ms.openlocfilehash: e09b5f9e463c7ecdfc595c87a84584f69cab3f2c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529022"
---
# <a name="parentid"></a><span data-ttu-id="8311a-103">ParentId</span><span class="sxs-lookup"><span data-stu-id="8311a-103">ParentId</span></span>

<span data-ttu-id="8311a-104">**ParentId**要素は、検索プレビューで親アイテムの識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="8311a-104">The **ParentId** element specifies the identifier of the parent item in a search preview.</span></span> 
  
```XML
<ParentId Id="" ChangeKey=""/>
```

<span data-ttu-id="8311a-105">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="8311a-105">**ItemIdType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="8311a-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="8311a-106">Attributes and elements</span></span>

<span data-ttu-id="8311a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8311a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8311a-108">属性</span><span class="sxs-lookup"><span data-stu-id="8311a-108">Attributes</span></span>

|<span data-ttu-id="8311a-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="8311a-109">**Attribute**</span></span>|<span data-ttu-id="8311a-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="8311a-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8311a-111">ID</span><span class="sxs-lookup"><span data-stu-id="8311a-111">Id</span></span>  <br/> |<span data-ttu-id="8311a-112">**Id**属性のテキスト値は、親アイテムの識別子です。</span><span class="sxs-lookup"><span data-stu-id="8311a-112">The text value of the **Id** attribute is the identifier of the parent item.</span></span>  <br/> |
|<span data-ttu-id="8311a-113">ChangeKey</span><span class="sxs-lookup"><span data-stu-id="8311a-113">ChangeKey</span></span>  <br/> |<span data-ttu-id="8311a-114">**Changekey**属性のテキスト値は、親アイテムの変更キーです。</span><span class="sxs-lookup"><span data-stu-id="8311a-114">The text value of the **ChangeKey** attribute is the change key of the parent item.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="8311a-115">子要素</span><span class="sxs-lookup"><span data-stu-id="8311a-115">Child elements</span></span>

<span data-ttu-id="8311a-116">なし。</span><span class="sxs-lookup"><span data-stu-id="8311a-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8311a-117">親要素</span><span class="sxs-lookup"><span data-stu-id="8311a-117">Parent elements</span></span>

[<span data-ttu-id="8311a-118">Searchプレビューアイテム</span><span class="sxs-lookup"><span data-stu-id="8311a-118">SearchPreviewItem</span></span>](searchpreviewitem.md)
  
## <a name="remarks"></a><span data-ttu-id="8311a-119">注釈</span><span class="sxs-lookup"><span data-stu-id="8311a-119">Remarks</span></span>

<span data-ttu-id="8311a-120">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="8311a-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="8311a-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="8311a-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8311a-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="8311a-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8311a-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="8311a-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8311a-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8311a-124">Schema name</span></span>  <br/> |<span data-ttu-id="8311a-125">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="8311a-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="8311a-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8311a-126">Validation file</span></span>  <br/> |<span data-ttu-id="8311a-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="8311a-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8311a-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="8311a-128">Can be empty</span></span>  <br/> |<span data-ttu-id="8311a-129">true</span><span class="sxs-lookup"><span data-stu-id="8311a-129">true</span></span>  <br/> |
   

