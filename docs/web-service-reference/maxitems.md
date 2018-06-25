---
title: MaxItems
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4ddba6b8-0f38-42cd-96a1-0d4283f6375b
description: MaxItems 要素は、要求で取得するアイテムの最大数を指定します。
ms.openlocfilehash: dffb9ba4e29915a65fe2a57b6e7a7b4468028fa1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832384"
---
# <a name="maxitems"></a><span data-ttu-id="f37f4-103">MaxItems</span><span class="sxs-lookup"><span data-stu-id="f37f4-103">MaxItems</span></span>

<span data-ttu-id="f37f4-104">**MaxItems**要素は、要求で取得するアイテムの最大数を指定します。</span><span class="sxs-lookup"><span data-stu-id="f37f4-104">The **MaxItems** element specifies the maximum number of items to return in the request.</span></span> 
  
```XML
<MaxItems/>
```

 <span data-ttu-id="f37f4-105">**int**</span><span class="sxs-lookup"><span data-stu-id="f37f4-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f37f4-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="f37f4-106">Attributes and elements</span></span>

<span data-ttu-id="f37f4-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f37f4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f37f4-108">属性</span><span class="sxs-lookup"><span data-stu-id="f37f4-108">Attributes</span></span>

<span data-ttu-id="f37f4-109">なし。</span><span class="sxs-lookup"><span data-stu-id="f37f4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f37f4-110">子要素</span><span class="sxs-lookup"><span data-stu-id="f37f4-110">Child elements</span></span>

<span data-ttu-id="f37f4-111">なし。</span><span class="sxs-lookup"><span data-stu-id="f37f4-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f37f4-112">親要素</span><span class="sxs-lookup"><span data-stu-id="f37f4-112">Parent elements</span></span>

[<span data-ttu-id="f37f4-113">GetReminders</span><span class="sxs-lookup"><span data-stu-id="f37f4-113">GetReminders</span></span>](getreminders.md)
  
## <a name="text-value"></a><span data-ttu-id="f37f4-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="f37f4-114">Text value</span></span>

<span data-ttu-id="f37f4-115">**MaxItems**要素のテキスト値は、要求で取得するアイテムの最大数です。</span><span class="sxs-lookup"><span data-stu-id="f37f4-115">The text value of the **MaxItems** element is the maximum number of items to return in the request.</span></span> <span data-ttu-id="f37f4-116">この数には、0 以上 200 より大きい値を指定できません。</span><span class="sxs-lookup"><span data-stu-id="f37f4-116">This number cannot be less than zero or greater than 200.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="f37f4-117">備考</span><span class="sxs-lookup"><span data-stu-id="f37f4-117">Remarks</span></span>

<span data-ttu-id="f37f4-118">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="f37f4-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f37f4-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="f37f4-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f37f4-120">要素情報</span><span class="sxs-lookup"><span data-stu-id="f37f4-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f37f4-121">名前空間</span><span class="sxs-lookup"><span data-stu-id="f37f4-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f37f4-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f37f4-122">Schema Name</span></span>  <br/> |<span data-ttu-id="f37f4-123">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="f37f4-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f37f4-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f37f4-124">Validation File</span></span>  <br/> |<span data-ttu-id="f37f4-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f37f4-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f37f4-126">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="f37f4-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="f37f4-127">False</span><span class="sxs-lookup"><span data-stu-id="f37f4-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f37f4-128">関連項目</span><span class="sxs-lookup"><span data-stu-id="f37f4-128">See also</span></span>



[<span data-ttu-id="f37f4-129">GetReminders</span><span class="sxs-lookup"><span data-stu-id="f37f4-129">GetReminders</span></span>](getreminders.md)


- [<span data-ttu-id="f37f4-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="f37f4-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

