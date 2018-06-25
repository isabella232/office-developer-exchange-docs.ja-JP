---
title: Modify
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Modify
api_type:
- schema
ms.assetid: 7a51e9e1-addb-4343-8a22-78f23763c0a8
description: 変更要素は、クライアントがフォルダーまたはアイテムを変更できるかどうかを示します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: 29fd2184e83f66a9b7e7db4173a765cee2922be8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832514"
---
# <a name="modify"></a><span data-ttu-id="efc8c-104">Modify</span><span class="sxs-lookup"><span data-stu-id="efc8c-104">Modify</span></span>

<span data-ttu-id="efc8c-105">**変更**要素は、クライアントがフォルダーまたはアイテムを変更できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="efc8c-105">The **Modify** element indicates whether a client can modify a folder or item.</span></span> <span data-ttu-id="efc8c-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="efc8c-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<Modify>true or false</Modify>
```

 <span data-ttu-id="efc8c-107">**boolean**</span><span class="sxs-lookup"><span data-stu-id="efc8c-107">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="efc8c-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="efc8c-108">Attributes and elements</span></span>

<span data-ttu-id="efc8c-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="efc8c-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="efc8c-110">属性</span><span class="sxs-lookup"><span data-stu-id="efc8c-110">Attributes</span></span>

<span data-ttu-id="efc8c-111">なし。</span><span class="sxs-lookup"><span data-stu-id="efc8c-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="efc8c-112">子要素</span><span class="sxs-lookup"><span data-stu-id="efc8c-112">Child elements</span></span>

<span data-ttu-id="efc8c-113">なし。</span><span class="sxs-lookup"><span data-stu-id="efc8c-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="efc8c-114">親要素</span><span class="sxs-lookup"><span data-stu-id="efc8c-114">Parent elements</span></span>

|<span data-ttu-id="efc8c-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="efc8c-115">**Element**</span></span>|<span data-ttu-id="efc8c-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="efc8c-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="efc8c-117">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="efc8c-117">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="efc8c-118">アイテムまたはフォルダーのアクセス許可の設定に基づいてクライアントの権限が含まれています。</span><span class="sxs-lookup"><span data-stu-id="efc8c-118">Contains the rights of the client based on the permission settings for the item or folder.</span></span> <span data-ttu-id="efc8c-119">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="efc8c-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="efc8c-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="efc8c-120">Text value</span></span>

<span data-ttu-id="efc8c-121">**True**の場合、テキスト値は、アイテムまたはフォルダーに、クライアントが変更できることを示します。</span><span class="sxs-lookup"><span data-stu-id="efc8c-121">A text value of **true** indicates that a client can modify an item or folder.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="efc8c-122">備考</span><span class="sxs-lookup"><span data-stu-id="efc8c-122">Remarks</span></span>

<span data-ttu-id="efc8c-123">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="efc8c-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="efc8c-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="efc8c-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="efc8c-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="efc8c-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="efc8c-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="efc8c-126">Schema Name</span></span>  <br/> |<span data-ttu-id="efc8c-127">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="efc8c-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="efc8c-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="efc8c-128">Validation File</span></span>  <br/> |<span data-ttu-id="efc8c-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="efc8c-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="efc8c-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="efc8c-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="efc8c-131">False</span><span class="sxs-lookup"><span data-stu-id="efc8c-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="efc8c-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="efc8c-132">See also</span></span>



- [<span data-ttu-id="efc8c-133">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="efc8c-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="efc8c-134">フォルダー レベルのアクセス許可の設定</span><span class="sxs-lookup"><span data-stu-id="efc8c-134">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

