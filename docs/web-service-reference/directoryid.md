---
title: DirectoryId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4958764f-64dd-4ae7-ade1-0255cb414fcc
description: DirectoryId 要素には、連絡先のディレクトリ ID が含まれています。
ms.openlocfilehash: b94e53cdb1b82edf0094ffa1ec5cf73dcca75257
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760049"
---
# <a name="directoryid"></a><span data-ttu-id="31526-103">DirectoryId</span><span class="sxs-lookup"><span data-stu-id="31526-103">DirectoryId</span></span>

<span data-ttu-id="31526-104">**DirectoryId**要素には、連絡先のディレクトリ ID が含まれています。</span><span class="sxs-lookup"><span data-stu-id="31526-104">The **DirectoryId** element contains the directory ID of a contact.</span></span> 
  
```XML
<DirectoryId/>
```

 <span data-ttu-id="31526-105">**string**</span><span class="sxs-lookup"><span data-stu-id="31526-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="31526-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="31526-106">Attributes and elements</span></span>

<span data-ttu-id="31526-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="31526-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="31526-108">属性</span><span class="sxs-lookup"><span data-stu-id="31526-108">Attributes</span></span>

<span data-ttu-id="31526-109">なし。</span><span class="sxs-lookup"><span data-stu-id="31526-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="31526-110">子要素</span><span class="sxs-lookup"><span data-stu-id="31526-110">Child elements</span></span>

<span data-ttu-id="31526-111">なし。</span><span class="sxs-lookup"><span data-stu-id="31526-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="31526-112">親要素</span><span class="sxs-lookup"><span data-stu-id="31526-112">Parent elements</span></span>

|<span data-ttu-id="31526-113">**要素名**</span><span class="sxs-lookup"><span data-stu-id="31526-113">**Element name**</span></span>|<span data-ttu-id="31526-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="31526-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="31526-115">Contact</span><span class="sxs-lookup"><span data-stu-id="31526-115">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="31526-116">Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="31526-116">Represents an Exchange contact item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="31526-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="31526-117">Text value</span></span>

<span data-ttu-id="31526-118">テキスト値は、連絡先のディレクトリ ID を表す文字列です。</span><span class="sxs-lookup"><span data-stu-id="31526-118">The text value is a string that represents the directory ID of the contact.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="31526-119">備考</span><span class="sxs-lookup"><span data-stu-id="31526-119">Remarks</span></span>

<span data-ttu-id="31526-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="31526-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="31526-121">この要素は Exchange Server 2010 Service Pack 2 (SP2) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="31526-121">This element was introduced in Exchange Server 2010 Service Pack 2 (SP2).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="31526-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="31526-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="31526-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="31526-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="31526-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="31526-124">Schema name</span></span>  <br/> |<span data-ttu-id="31526-125">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="31526-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="31526-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="31526-126">Validation file</span></span>  <br/> |<span data-ttu-id="31526-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="31526-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="31526-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="31526-128">Can be empty</span></span>  <br/> |<span data-ttu-id="31526-129">False</span><span class="sxs-lookup"><span data-stu-id="31526-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="31526-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="31526-130">See also</span></span>

- [<span data-ttu-id="31526-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="31526-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="31526-132">連絡先 (Exchange Web サービス) を作成します。</span><span class="sxs-lookup"><span data-stu-id="31526-132">Creating Contacts (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)

