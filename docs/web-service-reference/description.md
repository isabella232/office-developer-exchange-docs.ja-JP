---
title: 説明
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 6e4cd194-0696-4fec-8ab0-e1d349ed0be0
description: Description 要素は、リテンション ・ ポリシーの説明テキストを指定します。
ms.openlocfilehash: e001733e7011610dc09c2cce389104d74894772d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760020"
---
# <a name="description"></a><span data-ttu-id="32576-103">説明</span><span class="sxs-lookup"><span data-stu-id="32576-103">Description</span></span>

<span data-ttu-id="32576-104">**Description**要素は、リテンション ・ ポリシーの説明テキストを指定します。</span><span class="sxs-lookup"><span data-stu-id="32576-104">The **Description** element specifies the descriptive text for the retention policy.</span></span> 
  
```XML
<Description></Description>
```

 <span data-ttu-id="32576-105">**string**</span><span class="sxs-lookup"><span data-stu-id="32576-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="32576-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="32576-106">Attributes and elements</span></span>

<span data-ttu-id="32576-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="32576-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="32576-108">属性</span><span class="sxs-lookup"><span data-stu-id="32576-108">Attributes</span></span>

<span data-ttu-id="32576-109">なし。</span><span class="sxs-lookup"><span data-stu-id="32576-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="32576-110">子要素</span><span class="sxs-lookup"><span data-stu-id="32576-110">Child elements</span></span>

<span data-ttu-id="32576-111">なし。</span><span class="sxs-lookup"><span data-stu-id="32576-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="32576-112">親要素</span><span class="sxs-lookup"><span data-stu-id="32576-112">Parent elements</span></span>

|<span data-ttu-id="32576-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="32576-113">**Element**</span></span>|<span data-ttu-id="32576-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="32576-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="32576-115">RetentionPolicyTag</span><span class="sxs-lookup"><span data-stu-id="32576-115">RetentionPolicyTag</span></span>](retentionpolicytag.md) <br/> |<span data-ttu-id="32576-116">メールボックス アイテムの保持ポリシーを指定します。</span><span class="sxs-lookup"><span data-stu-id="32576-116">Specifies the retention policy for a mailbox item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="32576-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="32576-117">Text value</span></span>

<span data-ttu-id="32576-118">**Description**要素のテキスト値は、リテンション ・ ポリシーを説明する文字列値です。</span><span class="sxs-lookup"><span data-stu-id="32576-118">The text value of the **Description** element is a string value that describes the retention policy.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="32576-119">備考</span><span class="sxs-lookup"><span data-stu-id="32576-119">Remarks</span></span>

<span data-ttu-id="32576-120">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="32576-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="32576-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="32576-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="32576-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="32576-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="32576-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="32576-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="32576-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="32576-124">Schema Name</span></span>  <br/> |<span data-ttu-id="32576-125">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="32576-125">Type schema</span></span>  <br/> |
|<span data-ttu-id="32576-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="32576-126">Validation File</span></span>  <br/> |<span data-ttu-id="32576-127">types.xsd</span><span class="sxs-lookup"><span data-stu-id="32576-127">types.xsd</span></span>  <br/> |
|<span data-ttu-id="32576-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="32576-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="32576-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="32576-129">See also</span></span>

- [<span data-ttu-id="32576-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="32576-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

