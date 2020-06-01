---
title: CreateHierarchy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateHierarchy
api_type:
- schema
ms.assetid: 630b5610-1c19-4d4a-a5df-8cebb9afd2f4
description: CreateHierarchy 要素は、クライアントが階層テーブルを作成できるかどうかを示します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: 3fb0c34a8a148cc8336c70d643a21ecb6fef30b5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457523"
---
# <a name="createhierarchy"></a><span data-ttu-id="99875-104">CreateHierarchy</span><span class="sxs-lookup"><span data-stu-id="99875-104">CreateHierarchy</span></span>

<span data-ttu-id="99875-105">**Createhierarchy**要素は、クライアントが階層テーブルを作成できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="99875-105">The **CreateHierarchy** element indicates whether a client can create a hierarchy table.</span></span> <span data-ttu-id="99875-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="99875-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<CreateHierarchy>true or false</CreateHierarchy>
```

 <span data-ttu-id="99875-107">**boolean**</span><span class="sxs-lookup"><span data-stu-id="99875-107">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="99875-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="99875-108">Attributes and elements</span></span>

<span data-ttu-id="99875-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="99875-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="99875-110">属性</span><span class="sxs-lookup"><span data-stu-id="99875-110">Attributes</span></span>

<span data-ttu-id="99875-111">なし。</span><span class="sxs-lookup"><span data-stu-id="99875-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="99875-112">子要素</span><span class="sxs-lookup"><span data-stu-id="99875-112">Child elements</span></span>

<span data-ttu-id="99875-113">なし。</span><span class="sxs-lookup"><span data-stu-id="99875-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="99875-114">親要素</span><span class="sxs-lookup"><span data-stu-id="99875-114">Parent elements</span></span>

|<span data-ttu-id="99875-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="99875-115">**Element**</span></span>|<span data-ttu-id="99875-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="99875-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="99875-117">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="99875-117">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="99875-118">アイテムまたはフォルダーのアクセス許可の設定に基づいて、クライアントの権限が含まれています。</span><span class="sxs-lookup"><span data-stu-id="99875-118">Contains the rights of the client based on the permission settings for the item or folder.</span></span> <span data-ttu-id="99875-119">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="99875-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="99875-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="99875-120">Text value</span></span>

<span data-ttu-id="99875-121">テキスト値が**true の場合**は、クライアントが階層テーブルを作成できることを示します。</span><span class="sxs-lookup"><span data-stu-id="99875-121">A text value of **true** indicates that a client can create a hierarchy table.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="99875-122">注釈</span><span class="sxs-lookup"><span data-stu-id="99875-122">Remarks</span></span>

<span data-ttu-id="99875-123">このプロパティは、folder オブジェクトに対してのみ使用されます。</span><span class="sxs-lookup"><span data-stu-id="99875-123">This property is only used on folder objects.</span></span>
  
<span data-ttu-id="99875-124">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="99875-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="99875-125">要素の情報</span><span class="sxs-lookup"><span data-stu-id="99875-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="99875-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="99875-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="99875-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="99875-127">Schema Name</span></span>  <br/> |<span data-ttu-id="99875-128">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="99875-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="99875-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="99875-129">Validation File</span></span>  <br/> |<span data-ttu-id="99875-130">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="99875-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="99875-131">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="99875-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="99875-132">正しくない</span><span class="sxs-lookup"><span data-stu-id="99875-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="99875-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="99875-133">See also</span></span>



- [<span data-ttu-id="99875-134">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="99875-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="99875-135">フォルダーレベルのアクセス許可を設定する</span><span class="sxs-lookup"><span data-stu-id="99875-135">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

