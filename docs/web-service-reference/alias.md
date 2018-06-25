---
title: Alias
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 18aafbcd-a221-463a-935c-bc7c3fdbb08f
description: エイリアスの要素には、連絡先の電子メール エイリアスが含まれています。
ms.openlocfilehash: 6f93cdf3594a8426827ca53cae770df089dd6eef
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759307"
---
# <a name="alias"></a><span data-ttu-id="90887-103">Alias</span><span class="sxs-lookup"><span data-stu-id="90887-103">Alias</span></span>

<span data-ttu-id="90887-104">**エイリアス**の要素には、連絡先の電子メール エイリアスが含まれています。</span><span class="sxs-lookup"><span data-stu-id="90887-104">The **Alias** element contains the email alias of a contact.</span></span> 
  
```XML
<Alias/>
```

 <span data-ttu-id="90887-105">**string**</span><span class="sxs-lookup"><span data-stu-id="90887-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="90887-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="90887-106">Attributes and elements</span></span>

<span data-ttu-id="90887-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="90887-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="90887-108">属性</span><span class="sxs-lookup"><span data-stu-id="90887-108">Attributes</span></span>

<span data-ttu-id="90887-109">なし。</span><span class="sxs-lookup"><span data-stu-id="90887-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="90887-110">子要素</span><span class="sxs-lookup"><span data-stu-id="90887-110">Child elements</span></span>

<span data-ttu-id="90887-111">なし。</span><span class="sxs-lookup"><span data-stu-id="90887-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="90887-112">親要素</span><span class="sxs-lookup"><span data-stu-id="90887-112">Parent elements</span></span>

|<span data-ttu-id="90887-113">**要素名**</span><span class="sxs-lookup"><span data-stu-id="90887-113">**Element name**</span></span>|<span data-ttu-id="90887-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="90887-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="90887-115">Contact</span><span class="sxs-lookup"><span data-stu-id="90887-115">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="90887-116">Exchange ストア内の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="90887-116">Represents a contact item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="90887-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="90887-117">Text value</span></span>

<span data-ttu-id="90887-118">テキスト値は、連絡先の電子メール エイリアスを表す文字列です。</span><span class="sxs-lookup"><span data-stu-id="90887-118">The text value is a string that represents the email alias of a contact.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="90887-119">備考</span><span class="sxs-lookup"><span data-stu-id="90887-119">Remarks</span></span>

<span data-ttu-id="90887-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="90887-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="90887-121">この要素は Exchange Server 2010 Service Pack 2 (SP2) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="90887-121">This element was introduced in Exchange Server 2010 Service Pack 2 (SP2).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="90887-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="90887-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="90887-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="90887-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="90887-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="90887-124">Schema name</span></span>  <br/> |<span data-ttu-id="90887-125">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="90887-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="90887-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="90887-126">Validation file</span></span>  <br/> |<span data-ttu-id="90887-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="90887-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="90887-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="90887-128">Can be empty</span></span>  <br/> |<span data-ttu-id="90887-129">False</span><span class="sxs-lookup"><span data-stu-id="90887-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="90887-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="90887-130">See also</span></span>

- [<span data-ttu-id="90887-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="90887-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="90887-132">連絡先 (Exchange Web サービス) を作成します。</span><span class="sxs-lookup"><span data-stu-id="90887-132">Creating Contacts (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)

