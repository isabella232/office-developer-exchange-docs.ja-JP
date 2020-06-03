---
title: HasLocationChanged
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5fd465b4-6070-4cd0-9ac3-ed9d2bfd5951
description: HasLocationChanged 要素は、会議の場所プロパティが変更されたかどうかを指定します。
ms.openlocfilehash: 4f774adcf4a7666f40524931504f1172e15ba24d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462445"
---
# <a name="haslocationchanged"></a><span data-ttu-id="62598-103">HasLocationChanged</span><span class="sxs-lookup"><span data-stu-id="62598-103">HasLocationChanged</span></span>

<span data-ttu-id="62598-104">**Haslocationchanged**要素は、会議の場所プロパティが変更されたかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="62598-104">The **HasLocationChanged** element specifies whether the location property of a meeting has changed.</span></span> 
  
```XML
<HasLocationChanged> true | false </HasLocationChanged>
```

 <span data-ttu-id="62598-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="62598-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="62598-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="62598-106">Attributes and elements</span></span>

<span data-ttu-id="62598-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="62598-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="62598-108">属性</span><span class="sxs-lookup"><span data-stu-id="62598-108">Attributes</span></span>

<span data-ttu-id="62598-109">なし。</span><span class="sxs-lookup"><span data-stu-id="62598-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="62598-110">子要素</span><span class="sxs-lookup"><span data-stu-id="62598-110">Child elements</span></span>

<span data-ttu-id="62598-111">なし。</span><span class="sxs-lookup"><span data-stu-id="62598-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="62598-112">親要素</span><span class="sxs-lookup"><span data-stu-id="62598-112">Parent elements</span></span>

|<span data-ttu-id="62598-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="62598-113">**Element**</span></span>|<span data-ttu-id="62598-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="62598-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="62598-115">ChangeHighlights 強調表示</span><span class="sxs-lookup"><span data-stu-id="62598-115">ChangeHighlights</span></span>](changehighlights.md) <br/> |<span data-ttu-id="62598-116">2つのバージョンの会議出席依頼メッセージの間で変更されたものを指定します。</span><span class="sxs-lookup"><span data-stu-id="62598-116">Specifies what has changed between two versions of a meeting request message.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="62598-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="62598-117">Text value</span></span>

<span data-ttu-id="62598-118">**Haslocationchanged**要素のテキスト値が**true**の場合は、会議の location プロパティが変更されたことを示します。</span><span class="sxs-lookup"><span data-stu-id="62598-118">A text value of **true** for the **HasLocationChanged** element indicates that the location property of a meeting has changed.</span></span> <span data-ttu-id="62598-119">値が**false**の場合は、会議の location プロパティが変更されていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="62598-119">A value **false** indicates that the location property of a meeting has not changed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="62598-120">注釈</span><span class="sxs-lookup"><span data-stu-id="62598-120">Remarks</span></span>

<span data-ttu-id="62598-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="62598-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="62598-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="62598-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="62598-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="62598-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="62598-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="62598-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="62598-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="62598-125">Schema Name</span></span>  <br/> |<span data-ttu-id="62598-126">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="62598-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="62598-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="62598-127">Validation File</span></span>  <br/> |<span data-ttu-id="62598-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="62598-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="62598-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="62598-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="62598-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="62598-130">See also</span></span>



- [<span data-ttu-id="62598-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="62598-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

