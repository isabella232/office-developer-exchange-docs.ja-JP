---
title: MaxItems
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4ddba6b8-0f38-42cd-96a1-0d4283f6375b
description: MaxItems 要素は、要求で返されるアイテムの最大数を指定します。
ms.openlocfilehash: f16e9d46b59c0f562aabd5383f7f445d93414f68
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461745"
---
# <a name="maxitems"></a><span data-ttu-id="2bdf3-103">MaxItems</span><span class="sxs-lookup"><span data-stu-id="2bdf3-103">MaxItems</span></span>

<span data-ttu-id="2bdf3-104">**MaxItems**要素は、要求で返されるアイテムの最大数を指定します。</span><span class="sxs-lookup"><span data-stu-id="2bdf3-104">The **MaxItems** element specifies the maximum number of items to return in the request.</span></span> 
  
```XML
<MaxItems/>
```

 <span data-ttu-id="2bdf3-105">**int**</span><span class="sxs-lookup"><span data-stu-id="2bdf3-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2bdf3-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="2bdf3-106">Attributes and elements</span></span>

<span data-ttu-id="2bdf3-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2bdf3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2bdf3-108">属性</span><span class="sxs-lookup"><span data-stu-id="2bdf3-108">Attributes</span></span>

<span data-ttu-id="2bdf3-109">なし。</span><span class="sxs-lookup"><span data-stu-id="2bdf3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2bdf3-110">子要素</span><span class="sxs-lookup"><span data-stu-id="2bdf3-110">Child elements</span></span>

<span data-ttu-id="2bdf3-111">なし。</span><span class="sxs-lookup"><span data-stu-id="2bdf3-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2bdf3-112">親要素</span><span class="sxs-lookup"><span data-stu-id="2bdf3-112">Parent elements</span></span>

[<span data-ttu-id="2bdf3-113">GetReminders</span><span class="sxs-lookup"><span data-stu-id="2bdf3-113">GetReminders</span></span>](getreminders.md)
  
## <a name="text-value"></a><span data-ttu-id="2bdf3-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="2bdf3-114">Text value</span></span>

<span data-ttu-id="2bdf3-115">**MaxItems**要素のテキスト値は、要求で返される項目の最大数です。</span><span class="sxs-lookup"><span data-stu-id="2bdf3-115">The text value of the **MaxItems** element is the maximum number of items to return in the request.</span></span> <span data-ttu-id="2bdf3-116">この数値は、0より小さくする必要があります。または、200を超えることはできません。</span><span class="sxs-lookup"><span data-stu-id="2bdf3-116">This number cannot be less than zero or greater than 200.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="2bdf3-117">注釈</span><span class="sxs-lookup"><span data-stu-id="2bdf3-117">Remarks</span></span>

<span data-ttu-id="2bdf3-118">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="2bdf3-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="2bdf3-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="2bdf3-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2bdf3-120">要素の情報</span><span class="sxs-lookup"><span data-stu-id="2bdf3-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2bdf3-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="2bdf3-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2bdf3-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2bdf3-122">Schema Name</span></span>  <br/> |<span data-ttu-id="2bdf3-123">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="2bdf3-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="2bdf3-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2bdf3-124">Validation File</span></span>  <br/> |<span data-ttu-id="2bdf3-125">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="2bdf3-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2bdf3-126">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="2bdf3-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="2bdf3-127">正しくない</span><span class="sxs-lookup"><span data-stu-id="2bdf3-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2bdf3-128">関連項目</span><span class="sxs-lookup"><span data-stu-id="2bdf3-128">See also</span></span>



[<span data-ttu-id="2bdf3-129">GetReminders</span><span class="sxs-lookup"><span data-stu-id="2bdf3-129">GetReminders</span></span>](getreminders.md)


- [<span data-ttu-id="2bdf3-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="2bdf3-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

