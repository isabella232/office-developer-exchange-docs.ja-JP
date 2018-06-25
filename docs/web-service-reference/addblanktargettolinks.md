---
title: AddBlankTargetToLinks
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 30180298-2501-4369-9b8f-2f7663f02336
description: AddBlankTargetToLinks 要素は、新しいウィンドウを開くに HTML リンクの target 属性を設定することを指定します。
ms.openlocfilehash: 8a47e44d89bcc84bc0e8b61d45f18ff3182f7870
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759274"
---
# <a name="addblanktargettolinks"></a><span data-ttu-id="4c44a-103">AddBlankTargetToLinks</span><span class="sxs-lookup"><span data-stu-id="4c44a-103">AddBlankTargetToLinks</span></span>

<span data-ttu-id="4c44a-104">**AddBlankTargetToLinks**要素は、新しいウィンドウを開くに HTML リンクの target 属性を設定することを指定します。</span><span class="sxs-lookup"><span data-stu-id="4c44a-104">The **AddBlankTargetToLinks** element specifies that the target attribute in HTML links are set to open a new window.</span></span> 
  
```XML
<AddBlankTargetToLinks> true | false </AddBlankTargetToLinks>
```

<span data-ttu-id="4c44a-105">**xs:Boolean**</span><span class="sxs-lookup"><span data-stu-id="4c44a-105">**xs:Boolean**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="4c44a-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="4c44a-106">Attributes and elements</span></span>

<span data-ttu-id="4c44a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4c44a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4c44a-108">属性</span><span class="sxs-lookup"><span data-stu-id="4c44a-108">Attributes</span></span>

<span data-ttu-id="4c44a-109">なし。</span><span class="sxs-lookup"><span data-stu-id="4c44a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4c44a-110">子要素</span><span class="sxs-lookup"><span data-stu-id="4c44a-110">Child elements</span></span>

<span data-ttu-id="4c44a-111">なし。</span><span class="sxs-lookup"><span data-stu-id="4c44a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4c44a-112">親要素</span><span class="sxs-lookup"><span data-stu-id="4c44a-112">Parent elements</span></span>

|<span data-ttu-id="4c44a-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="4c44a-113">**Element**</span></span>|<span data-ttu-id="4c44a-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="4c44a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4c44a-115">ItemShape</span><span class="sxs-lookup"><span data-stu-id="4c44a-115">ItemShape</span></span>](itemshape.md) <br/> | <span data-ttu-id="4c44a-116">**GetItem**、 **FindItem**、 **GetConversationItems**または**SyncFolderItems**の応答に含めるコンテンツ アイテムのプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="4c44a-116">Identifies the item properties and content to include in a **GetItem**, **FindItem**, **GetConversationItems** or **SyncFolderItems** response.</span></span><br/><br/>  <span data-ttu-id="4c44a-117">この要素への XPath 式は、次のように。</span><span class="sxs-lookup"><span data-stu-id="4c44a-117">The following are the XPath expressions to this element:</span></span><br/><br/>  `/GetItem/ItemShape` <br/>  `/FindItem/ItemShape` <br/>  `/SyncFolderItems/ItemShape` <br/>  `/GetConversationItems/ItemShape` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4c44a-118">テキスト値</span><span class="sxs-lookup"><span data-stu-id="4c44a-118">Text value</span></span>

<span data-ttu-id="4c44a-119">の**場合は true** 、 **AddBlankTargetToLinks**要素のテキスト値は、すべての HTML リンクを新しいウィンドウを開くに設定されることを示します。</span><span class="sxs-lookup"><span data-stu-id="4c44a-119">A text value of **true** for the **AddBlankTargetToLinks** element indicates that all HTML links will be set to open a new window.</span></span> <span data-ttu-id="4c44a-120">**False**の値は、現在のウィンドウで HTML リンクが開かれることを示します。</span><span class="sxs-lookup"><span data-stu-id="4c44a-120">A value of **false** indicates that HTML links will open in the current window.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="4c44a-121">備考</span><span class="sxs-lookup"><span data-stu-id="4c44a-121">Remarks</span></span>

<span data-ttu-id="4c44a-122">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="4c44a-122">This element is optional.</span></span>
  
<span data-ttu-id="4c44a-123">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="4c44a-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4c44a-124">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="4c44a-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4c44a-125">要素情報</span><span class="sxs-lookup"><span data-stu-id="4c44a-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4c44a-126">名前空間</span><span class="sxs-lookup"><span data-stu-id="4c44a-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4c44a-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4c44a-127">Schema Name</span></span>  <br/> |<span data-ttu-id="4c44a-128">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="4c44a-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="4c44a-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4c44a-129">Validation File</span></span>  <br/> |<span data-ttu-id="4c44a-130">types.xsd</span><span class="sxs-lookup"><span data-stu-id="4c44a-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="4c44a-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="4c44a-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="4c44a-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="4c44a-132">See also</span></span>

- [<span data-ttu-id="4c44a-133">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="4c44a-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

