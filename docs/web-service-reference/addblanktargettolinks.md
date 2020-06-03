---
title: Add空白 Targettolインク
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 30180298-2501-4369-9b8f-2f7663f02336
description: AddBlankTargetToLinks 要素は、HTML リンクの target 属性が新しいウィンドウを開くように設定されていることを示します。
ms.openlocfilehash: 1d4d36c1f4b98ebee96baea683c40527d2a9ec27
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465044"
---
# <a name="addblanktargettolinks"></a><span data-ttu-id="879f6-103">Add空白 Targettolインク</span><span class="sxs-lookup"><span data-stu-id="879f6-103">AddBlankTargetToLinks</span></span>

<span data-ttu-id="879f6-104">**Addblanktargettolinks**要素は、HTML リンクの target 属性が新しいウィンドウを開くように設定されていることを示します。</span><span class="sxs-lookup"><span data-stu-id="879f6-104">The **AddBlankTargetToLinks** element specifies that the target attribute in HTML links are set to open a new window.</span></span> 
  
```XML
<AddBlankTargetToLinks> true | false </AddBlankTargetToLinks>
```

<span data-ttu-id="879f6-105">**xs: Boolean**</span><span class="sxs-lookup"><span data-stu-id="879f6-105">**xs:Boolean**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="879f6-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="879f6-106">Attributes and elements</span></span>

<span data-ttu-id="879f6-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="879f6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="879f6-108">属性</span><span class="sxs-lookup"><span data-stu-id="879f6-108">Attributes</span></span>

<span data-ttu-id="879f6-109">なし。</span><span class="sxs-lookup"><span data-stu-id="879f6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="879f6-110">子要素</span><span class="sxs-lookup"><span data-stu-id="879f6-110">Child elements</span></span>

<span data-ttu-id="879f6-111">なし。</span><span class="sxs-lookup"><span data-stu-id="879f6-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="879f6-112">親要素</span><span class="sxs-lookup"><span data-stu-id="879f6-112">Parent elements</span></span>

|<span data-ttu-id="879f6-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="879f6-113">**Element**</span></span>|<span data-ttu-id="879f6-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="879f6-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="879f6-115">ItemShape</span><span class="sxs-lookup"><span data-stu-id="879f6-115">ItemShape</span></span>](itemshape.md) <br/> | <span data-ttu-id="879f6-116">**GetItem**、 **FindItem**、 **GetConversationItems** 、または**syncfolderitems**応答に含めるアイテムのプロパティとコンテンツを識別します。</span><span class="sxs-lookup"><span data-stu-id="879f6-116">Identifies the item properties and content to include in a **GetItem**, **FindItem**, **GetConversationItems** or **SyncFolderItems** response.</span></span><br/><br/>  <span data-ttu-id="879f6-117">この要素の XPath 式は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="879f6-117">The following are the XPath expressions to this element:</span></span><br/><br/>  `/GetItem/ItemShape` <br/>  `/FindItem/ItemShape` <br/>  `/SyncFolderItems/ItemShape` <br/>  `/GetConversationItems/ItemShape` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="879f6-118">テキスト値</span><span class="sxs-lookup"><span data-stu-id="879f6-118">Text value</span></span>

<span data-ttu-id="879f6-119">**Addblanktargettolinks**要素のテキスト値が**true の場合**は、すべての HTML リンクが新しいウィンドウを開くように設定されていることを示します。</span><span class="sxs-lookup"><span data-stu-id="879f6-119">A text value of **true** for the **AddBlankTargetToLinks** element indicates that all HTML links will be set to open a new window.</span></span> <span data-ttu-id="879f6-120">**False**を指定すると、現在のウィンドウで HTML リンクが開きます。</span><span class="sxs-lookup"><span data-stu-id="879f6-120">A value of **false** indicates that HTML links will open in the current window.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="879f6-121">注釈</span><span class="sxs-lookup"><span data-stu-id="879f6-121">Remarks</span></span>

<span data-ttu-id="879f6-122">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="879f6-122">This element is optional.</span></span>
  
<span data-ttu-id="879f6-123">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="879f6-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="879f6-124">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="879f6-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="879f6-125">要素の情報</span><span class="sxs-lookup"><span data-stu-id="879f6-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="879f6-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="879f6-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="879f6-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="879f6-127">Schema Name</span></span>  <br/> |<span data-ttu-id="879f6-128">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="879f6-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="879f6-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="879f6-129">Validation File</span></span>  <br/> |<span data-ttu-id="879f6-130">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="879f6-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="879f6-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="879f6-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="879f6-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="879f6-132">See also</span></span>

- [<span data-ttu-id="879f6-133">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="879f6-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

