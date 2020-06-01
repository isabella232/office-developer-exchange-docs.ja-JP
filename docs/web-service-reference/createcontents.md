---
title: CreateContents
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateContents
api_type:
- schema
ms.assetid: 8a9cd241-0d73-4be8-a563-a945898d1a0e
description: CreateContents 要素は、クライアントがコンテンツテーブルを作成できるかどうかを示します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: 409e0e566c5fa39830707c199f8e3783411c7334
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458916"
---
# <a name="createcontents"></a><span data-ttu-id="1fefd-104">CreateContents</span><span class="sxs-lookup"><span data-stu-id="1fefd-104">CreateContents</span></span>

<span data-ttu-id="1fefd-105">**CreateContents**要素は、クライアントがコンテンツテーブルを作成できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1fefd-105">The **CreateContents** element indicates whether a client can create a contents table.</span></span> <span data-ttu-id="1fefd-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="1fefd-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<CreateContents>true or false</CreateContents>
```

 <span data-ttu-id="1fefd-107">**boolean**</span><span class="sxs-lookup"><span data-stu-id="1fefd-107">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1fefd-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="1fefd-108">Attributes and elements</span></span>

<span data-ttu-id="1fefd-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1fefd-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1fefd-110">属性</span><span class="sxs-lookup"><span data-stu-id="1fefd-110">Attributes</span></span>

<span data-ttu-id="1fefd-111">なし。</span><span class="sxs-lookup"><span data-stu-id="1fefd-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1fefd-112">子要素</span><span class="sxs-lookup"><span data-stu-id="1fefd-112">Child elements</span></span>

<span data-ttu-id="1fefd-113">なし。</span><span class="sxs-lookup"><span data-stu-id="1fefd-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1fefd-114">親要素</span><span class="sxs-lookup"><span data-stu-id="1fefd-114">Parent elements</span></span>

|<span data-ttu-id="1fefd-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="1fefd-115">**Element**</span></span>|<span data-ttu-id="1fefd-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="1fefd-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1fefd-117">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="1fefd-117">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="1fefd-118">アイテムまたはフォルダーのアクセス許可の設定に基づいて、クライアントの権限が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1fefd-118">Contains the rights of the client based on the permission settings for the item or folder.</span></span> <span data-ttu-id="1fefd-119">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="1fefd-119">This element was introduced inExchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1fefd-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="1fefd-120">Text value</span></span>

<span data-ttu-id="1fefd-121">テキスト値が**true の場合**は、クライアントがコンテンツテーブルを作成できることを示します。</span><span class="sxs-lookup"><span data-stu-id="1fefd-121">A text value of **true** indicates that a client can create a contents table.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="1fefd-122">注釈</span><span class="sxs-lookup"><span data-stu-id="1fefd-122">Remarks</span></span>

<span data-ttu-id="1fefd-123">このプロパティは、folder オブジェクトに対してのみ使用されます。</span><span class="sxs-lookup"><span data-stu-id="1fefd-123">This property is only used on folder objects.</span></span>
  
<span data-ttu-id="1fefd-124">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="1fefd-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1fefd-125">要素の情報</span><span class="sxs-lookup"><span data-stu-id="1fefd-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1fefd-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="1fefd-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1fefd-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1fefd-127">Schema Name</span></span>  <br/> |<span data-ttu-id="1fefd-128">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="1fefd-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="1fefd-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1fefd-129">Validation File</span></span>  <br/> |<span data-ttu-id="1fefd-130">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="1fefd-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1fefd-131">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="1fefd-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="1fefd-132">正しくない</span><span class="sxs-lookup"><span data-stu-id="1fefd-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1fefd-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="1fefd-133">See also</span></span>



- [<span data-ttu-id="1fefd-134">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="1fefd-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="1fefd-135">フォルダーレベルのアクセス許可を設定する</span><span class="sxs-lookup"><span data-stu-id="1fefd-135">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

