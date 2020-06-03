---
title: Read
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
description: Read 要素は、クライアントがフォルダーまたはアイテムを読み取ることができるかどうかを示します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: d75285e0ab14c4f53d73cb7f4349196e07c3c521
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468314"
---
# <a name="read"></a><span data-ttu-id="29443-104">Read</span><span class="sxs-lookup"><span data-stu-id="29443-104">Read</span></span>

<span data-ttu-id="29443-105">**Read**要素は、クライアントがフォルダーまたはアイテムを読み取ることができるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="29443-105">The **Read** element indicates whether a client can read a folder or item.</span></span> <span data-ttu-id="29443-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="29443-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<Read>true or false</Read>
```

 <span data-ttu-id="29443-107">**boolean**</span><span class="sxs-lookup"><span data-stu-id="29443-107">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="29443-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="29443-108">Attributes and elements</span></span>

<span data-ttu-id="29443-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="29443-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="29443-110">属性</span><span class="sxs-lookup"><span data-stu-id="29443-110">Attributes</span></span>

<span data-ttu-id="29443-111">なし。</span><span class="sxs-lookup"><span data-stu-id="29443-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="29443-112">子要素</span><span class="sxs-lookup"><span data-stu-id="29443-112">Child elements</span></span>

<span data-ttu-id="29443-113">なし。</span><span class="sxs-lookup"><span data-stu-id="29443-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="29443-114">親要素</span><span class="sxs-lookup"><span data-stu-id="29443-114">Parent elements</span></span>

|<span data-ttu-id="29443-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="29443-115">**Element**</span></span>|<span data-ttu-id="29443-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="29443-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="29443-117">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="29443-117">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="29443-118">アイテムまたはフォルダーのアクセス許可の設定に基づいて、クライアントの権限が含まれています。</span><span class="sxs-lookup"><span data-stu-id="29443-118">Contains the rights of the client based on the permission settings for the item or folder.</span></span> <span data-ttu-id="29443-119">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="29443-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="29443-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="29443-120">Text value</span></span>

<span data-ttu-id="29443-121">テキスト値が**true の場合**は、クライアントがフォルダーのアイテムを読み取ることができることを示します。</span><span class="sxs-lookup"><span data-stu-id="29443-121">A text value of **true** indicates that a client can read an item of folder.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="29443-122">注釈</span><span class="sxs-lookup"><span data-stu-id="29443-122">Remarks</span></span>

<span data-ttu-id="29443-123">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="29443-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="29443-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="29443-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="29443-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="29443-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="29443-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="29443-126">Schema Name</span></span>  <br/> |<span data-ttu-id="29443-127">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="29443-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="29443-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="29443-128">Validation File</span></span>  <br/> |<span data-ttu-id="29443-129">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="29443-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="29443-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="29443-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="29443-131">正しくない</span><span class="sxs-lookup"><span data-stu-id="29443-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="29443-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="29443-132">See also</span></span>



- [<span data-ttu-id="29443-133">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="29443-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="29443-134">フォルダーレベルのアクセス許可を設定する</span><span class="sxs-lookup"><span data-stu-id="29443-134">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

