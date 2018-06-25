---
title: 読み取り
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Read
api_type:
- schema
ms.assetid: b14637e9-1695-4b7e-b078-ae527c2e4303
description: 読み取り要素は、クライアントがフォルダーまたはアイテムを読み取ることができるかどうかを示します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: cd9c2c9802c78b202418e3947f5b5718b0f676cc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832948"
---
# <a name="read"></a><span data-ttu-id="4ad39-104">読み取り</span><span class="sxs-lookup"><span data-stu-id="4ad39-104">Read</span></span>

<span data-ttu-id="4ad39-105">**読み取り**要素は、クライアントがフォルダーまたはアイテムを読み取ることができるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4ad39-105">The **Read** element indicates whether a client can read a folder or item.</span></span> <span data-ttu-id="4ad39-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="4ad39-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<Read>true or false</Read>
```

 <span data-ttu-id="4ad39-107">**boolean**</span><span class="sxs-lookup"><span data-stu-id="4ad39-107">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4ad39-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="4ad39-108">Attributes and elements</span></span>

<span data-ttu-id="4ad39-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4ad39-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4ad39-110">属性</span><span class="sxs-lookup"><span data-stu-id="4ad39-110">Attributes</span></span>

<span data-ttu-id="4ad39-111">なし。</span><span class="sxs-lookup"><span data-stu-id="4ad39-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4ad39-112">子要素</span><span class="sxs-lookup"><span data-stu-id="4ad39-112">Child elements</span></span>

<span data-ttu-id="4ad39-113">なし。</span><span class="sxs-lookup"><span data-stu-id="4ad39-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4ad39-114">親要素</span><span class="sxs-lookup"><span data-stu-id="4ad39-114">Parent elements</span></span>

|<span data-ttu-id="4ad39-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="4ad39-115">**Element**</span></span>|<span data-ttu-id="4ad39-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="4ad39-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4ad39-117">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="4ad39-117">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="4ad39-118">アイテムまたはフォルダーのアクセス許可の設定に基づいてクライアントの権限が含まれています。</span><span class="sxs-lookup"><span data-stu-id="4ad39-118">Contains the rights of the client based on the permission settings for the item or folder.</span></span> <span data-ttu-id="4ad39-119">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="4ad39-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4ad39-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="4ad39-120">Text value</span></span>

<span data-ttu-id="4ad39-121">**True**の場合、テキスト値は、クライアントがフォルダーのアイテムを読み取ることができますを示します。</span><span class="sxs-lookup"><span data-stu-id="4ad39-121">A text value of **true** indicates that a client can read an item of folder.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="4ad39-122">備考</span><span class="sxs-lookup"><span data-stu-id="4ad39-122">Remarks</span></span>

<span data-ttu-id="4ad39-123">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="4ad39-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4ad39-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="4ad39-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4ad39-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="4ad39-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4ad39-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4ad39-126">Schema Name</span></span>  <br/> |<span data-ttu-id="4ad39-127">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="4ad39-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="4ad39-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4ad39-128">Validation File</span></span>  <br/> |<span data-ttu-id="4ad39-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4ad39-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4ad39-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="4ad39-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="4ad39-131">False</span><span class="sxs-lookup"><span data-stu-id="4ad39-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4ad39-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="4ad39-132">See also</span></span>



- [<span data-ttu-id="4ad39-133">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="4ad39-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="4ad39-134">フォルダー レベルのアクセス許可の設定</span><span class="sxs-lookup"><span data-stu-id="4ad39-134">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

