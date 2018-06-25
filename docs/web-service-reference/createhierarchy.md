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
ms.openlocfilehash: a5b428fe453dbc31761309b017367a7d25a01b76
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759823"
---
# <a name="createhierarchy"></a><span data-ttu-id="b444b-104">CreateHierarchy</span><span class="sxs-lookup"><span data-stu-id="b444b-104">CreateHierarchy</span></span>

<span data-ttu-id="b444b-105">**CreateHierarchy**要素は、クライアントが階層テーブルを作成できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b444b-105">The **CreateHierarchy** element indicates whether a client can create a hierarchy table.</span></span> <span data-ttu-id="b444b-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="b444b-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<CreateHierarchy>true or false</CreateHierarchy>
```

 <span data-ttu-id="b444b-107">**boolean**</span><span class="sxs-lookup"><span data-stu-id="b444b-107">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b444b-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="b444b-108">Attributes and elements</span></span>

<span data-ttu-id="b444b-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b444b-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b444b-110">属性</span><span class="sxs-lookup"><span data-stu-id="b444b-110">Attributes</span></span>

<span data-ttu-id="b444b-111">なし。</span><span class="sxs-lookup"><span data-stu-id="b444b-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b444b-112">子要素</span><span class="sxs-lookup"><span data-stu-id="b444b-112">Child elements</span></span>

<span data-ttu-id="b444b-113">なし。</span><span class="sxs-lookup"><span data-stu-id="b444b-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b444b-114">親要素</span><span class="sxs-lookup"><span data-stu-id="b444b-114">Parent elements</span></span>

|<span data-ttu-id="b444b-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="b444b-115">**Element**</span></span>|<span data-ttu-id="b444b-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="b444b-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b444b-117">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="b444b-117">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="b444b-118">アイテムまたはフォルダーのアクセス許可の設定に基づいてクライアントの権限が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b444b-118">Contains the rights of the client based on the permission settings for the item or folder.</span></span> <span data-ttu-id="b444b-119">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="b444b-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b444b-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="b444b-120">Text value</span></span>

<span data-ttu-id="b444b-121">**True**の場合、テキスト値は、クライアントが階層テーブルを作成できますを示します。</span><span class="sxs-lookup"><span data-stu-id="b444b-121">A text value of **true** indicates that a client can create a hierarchy table.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="b444b-122">備考</span><span class="sxs-lookup"><span data-stu-id="b444b-122">Remarks</span></span>

<span data-ttu-id="b444b-123">Folder オブジェクトに対してこのプロパティは使用のみ。</span><span class="sxs-lookup"><span data-stu-id="b444b-123">This property is only used on folder objects.</span></span>
  
<span data-ttu-id="b444b-124">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="b444b-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b444b-125">要素情報</span><span class="sxs-lookup"><span data-stu-id="b444b-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b444b-126">名前空間</span><span class="sxs-lookup"><span data-stu-id="b444b-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b444b-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b444b-127">Schema Name</span></span>  <br/> |<span data-ttu-id="b444b-128">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="b444b-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="b444b-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b444b-129">Validation File</span></span>  <br/> |<span data-ttu-id="b444b-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b444b-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b444b-131">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="b444b-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="b444b-132">False</span><span class="sxs-lookup"><span data-stu-id="b444b-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b444b-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="b444b-133">See also</span></span>



- [<span data-ttu-id="b444b-134">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="b444b-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="b444b-135">フォルダー レベルのアクセス許可の設定</span><span class="sxs-lookup"><span data-stu-id="b444b-135">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

