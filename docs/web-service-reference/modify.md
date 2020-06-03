---
title: 変更
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
description: Modify 要素は、クライアントがフォルダーまたはアイテムを変更できるかどうかを示します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: e7712644ac9c32afab06be49b438ad83bbb31058
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530416"
---
# <a name="modify"></a><span data-ttu-id="5a866-104">変更</span><span class="sxs-lookup"><span data-stu-id="5a866-104">Modify</span></span>

<span data-ttu-id="5a866-105">**Modify**要素は、クライアントがフォルダーまたはアイテムを変更できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5a866-105">The **Modify** element indicates whether a client can modify a folder or item.</span></span> <span data-ttu-id="5a866-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="5a866-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<Modify>true or false</Modify>
```

 <span data-ttu-id="5a866-107">**boolean**</span><span class="sxs-lookup"><span data-stu-id="5a866-107">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5a866-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="5a866-108">Attributes and elements</span></span>

<span data-ttu-id="5a866-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5a866-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5a866-110">属性</span><span class="sxs-lookup"><span data-stu-id="5a866-110">Attributes</span></span>

<span data-ttu-id="5a866-111">なし。</span><span class="sxs-lookup"><span data-stu-id="5a866-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5a866-112">子要素</span><span class="sxs-lookup"><span data-stu-id="5a866-112">Child elements</span></span>

<span data-ttu-id="5a866-113">なし。</span><span class="sxs-lookup"><span data-stu-id="5a866-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5a866-114">親要素</span><span class="sxs-lookup"><span data-stu-id="5a866-114">Parent elements</span></span>

|<span data-ttu-id="5a866-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="5a866-115">**Element**</span></span>|<span data-ttu-id="5a866-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="5a866-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5a866-117">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="5a866-117">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="5a866-118">アイテムまたはフォルダーのアクセス許可の設定に基づいて、クライアントの権限が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5a866-118">Contains the rights of the client based on the permission settings for the item or folder.</span></span> <span data-ttu-id="5a866-119">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="5a866-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5a866-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="5a866-120">Text value</span></span>

<span data-ttu-id="5a866-121">テキスト値が**true の場合**は、クライアントがアイテムまたはフォルダーを変更できることを示します。</span><span class="sxs-lookup"><span data-stu-id="5a866-121">A text value of **true** indicates that a client can modify an item or folder.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="5a866-122">注釈</span><span class="sxs-lookup"><span data-stu-id="5a866-122">Remarks</span></span>

<span data-ttu-id="5a866-123">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="5a866-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5a866-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="5a866-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5a866-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="5a866-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5a866-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5a866-126">Schema Name</span></span>  <br/> |<span data-ttu-id="5a866-127">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="5a866-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="5a866-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5a866-128">Validation File</span></span>  <br/> |<span data-ttu-id="5a866-129">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="5a866-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5a866-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="5a866-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="5a866-131">正しくない</span><span class="sxs-lookup"><span data-stu-id="5a866-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5a866-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="5a866-132">See also</span></span>



- [<span data-ttu-id="5a866-133">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="5a866-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="5a866-134">フォルダーレベルのアクセス許可を設定する</span><span class="sxs-lookup"><span data-stu-id="5a866-134">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

