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
description: CreateAssociated 要素は、クライアントが、関連付けられている内容のテーブルを作成できるかどうかを示します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: ec6e55ed2423ff5849f6d19aee29f790572ddda6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759796"
---
# <a name="createassociated"></a><span data-ttu-id="b4b6e-104">CreateAssociated</span><span class="sxs-lookup"><span data-stu-id="b4b6e-104">CreateAssociated</span></span>

<span data-ttu-id="b4b6e-105">**CreateAssociated**要素は、クライアントが、関連付けられている内容のテーブルを作成できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b4b6e-105">The **CreateAssociated** element indicates whether a client can create an associated contents table.</span></span> <span data-ttu-id="b4b6e-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="b4b6e-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<CreateAssociated>true or false</CreateAssociated>
```

 <span data-ttu-id="b4b6e-107">**boolean**</span><span class="sxs-lookup"><span data-stu-id="b4b6e-107">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b4b6e-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="b4b6e-108">Attributes and elements</span></span>

<span data-ttu-id="b4b6e-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b4b6e-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b4b6e-110">属性</span><span class="sxs-lookup"><span data-stu-id="b4b6e-110">Attributes</span></span>

<span data-ttu-id="b4b6e-111">なし。</span><span class="sxs-lookup"><span data-stu-id="b4b6e-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b4b6e-112">子要素</span><span class="sxs-lookup"><span data-stu-id="b4b6e-112">Child elements</span></span>

<span data-ttu-id="b4b6e-113">なし。</span><span class="sxs-lookup"><span data-stu-id="b4b6e-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b4b6e-114">親要素</span><span class="sxs-lookup"><span data-stu-id="b4b6e-114">Parent elements</span></span>

|<span data-ttu-id="b4b6e-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="b4b6e-115">**Element**</span></span>|<span data-ttu-id="b4b6e-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="b4b6e-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b4b6e-117">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="b4b6e-117">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="b4b6e-118">アイテムまたはフォルダーのアクセス許可の設定に基づいてクライアントの権限が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b4b6e-118">Contains the rights of the client based on the permission settings for the item or folder.</span></span> <span data-ttu-id="b4b6e-119">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="b4b6e-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b4b6e-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="b4b6e-120">Text value</span></span>

<span data-ttu-id="b4b6e-121">**True**の場合、テキスト値は、クライアントが、関連付けられている内容のテーブルを作成できますを示します。</span><span class="sxs-lookup"><span data-stu-id="b4b6e-121">A text value of **true** indicates that a client can create an associated contents table.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="b4b6e-122">備考</span><span class="sxs-lookup"><span data-stu-id="b4b6e-122">Remarks</span></span>

<span data-ttu-id="b4b6e-123">Folder オブジェクトに対してこのプロパティは使用のみ。</span><span class="sxs-lookup"><span data-stu-id="b4b6e-123">This property is only used on folder objects.</span></span>
  
<span data-ttu-id="b4b6e-124">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="b4b6e-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b4b6e-125">要素情報</span><span class="sxs-lookup"><span data-stu-id="b4b6e-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b4b6e-126">名前空間</span><span class="sxs-lookup"><span data-stu-id="b4b6e-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b4b6e-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b4b6e-127">Schema Name</span></span>  <br/> |<span data-ttu-id="b4b6e-128">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="b4b6e-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="b4b6e-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b4b6e-129">Validation File</span></span>  <br/> |<span data-ttu-id="b4b6e-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b4b6e-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b4b6e-131">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="b4b6e-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="b4b6e-132">False</span><span class="sxs-lookup"><span data-stu-id="b4b6e-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b4b6e-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="b4b6e-133">See also</span></span>



- [<span data-ttu-id="b4b6e-134">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="b4b6e-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="b4b6e-135">フォルダー レベルのアクセス許可の設定</span><span class="sxs-lookup"><span data-stu-id="b4b6e-135">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

