---
title: CreateAssociated
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateAssociated
api_type:
- schema
ms.assetid: 742a6136-6015-4924-bae4-f3868127e966
description: CreateAssociated 要素は、クライアントが関連するコンテンツテーブルを作成できるかどうかを示します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: e88d7670fd9ef848221dab8cc145395bcb11e5bf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460793"
---
# <a name="createassociated"></a><span data-ttu-id="36655-104">CreateAssociated</span><span class="sxs-lookup"><span data-stu-id="36655-104">CreateAssociated</span></span>

<span data-ttu-id="36655-105">**Createassociated**要素は、クライアントが関連するコンテンツテーブルを作成できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="36655-105">The **CreateAssociated** element indicates whether a client can create an associated contents table.</span></span> <span data-ttu-id="36655-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="36655-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<CreateAssociated>true or false</CreateAssociated>
```

 <span data-ttu-id="36655-107">**boolean**</span><span class="sxs-lookup"><span data-stu-id="36655-107">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="36655-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="36655-108">Attributes and elements</span></span>

<span data-ttu-id="36655-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="36655-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="36655-110">属性</span><span class="sxs-lookup"><span data-stu-id="36655-110">Attributes</span></span>

<span data-ttu-id="36655-111">なし。</span><span class="sxs-lookup"><span data-stu-id="36655-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="36655-112">子要素</span><span class="sxs-lookup"><span data-stu-id="36655-112">Child elements</span></span>

<span data-ttu-id="36655-113">なし。</span><span class="sxs-lookup"><span data-stu-id="36655-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="36655-114">親要素</span><span class="sxs-lookup"><span data-stu-id="36655-114">Parent elements</span></span>

|<span data-ttu-id="36655-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="36655-115">**Element**</span></span>|<span data-ttu-id="36655-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="36655-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="36655-117">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="36655-117">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="36655-118">アイテムまたはフォルダーのアクセス許可の設定に基づいて、クライアントの権限が含まれています。</span><span class="sxs-lookup"><span data-stu-id="36655-118">Contains the rights of the client based on the permission settings for the item or folder.</span></span> <span data-ttu-id="36655-119">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="36655-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="36655-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="36655-120">Text value</span></span>

<span data-ttu-id="36655-121">テキスト値が**true の場合**は、クライアントが関連するコンテンツテーブルを作成できることを示します。</span><span class="sxs-lookup"><span data-stu-id="36655-121">A text value of **true** indicates that a client can create an associated contents table.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="36655-122">注釈</span><span class="sxs-lookup"><span data-stu-id="36655-122">Remarks</span></span>

<span data-ttu-id="36655-123">このプロパティは、folder オブジェクトに対してのみ使用されます。</span><span class="sxs-lookup"><span data-stu-id="36655-123">This property is only used on folder objects.</span></span>
  
<span data-ttu-id="36655-124">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="36655-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="36655-125">要素の情報</span><span class="sxs-lookup"><span data-stu-id="36655-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="36655-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="36655-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="36655-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="36655-127">Schema Name</span></span>  <br/> |<span data-ttu-id="36655-128">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="36655-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="36655-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="36655-129">Validation File</span></span>  <br/> |<span data-ttu-id="36655-130">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="36655-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="36655-131">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="36655-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="36655-132">正しくない</span><span class="sxs-lookup"><span data-stu-id="36655-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="36655-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="36655-133">See also</span></span>



- [<span data-ttu-id="36655-134">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="36655-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="36655-135">フォルダーレベルのアクセス許可を設定する</span><span class="sxs-lookup"><span data-stu-id="36655-135">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

