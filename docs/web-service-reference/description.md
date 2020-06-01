---
title: 説明
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 6e4cd194-0696-4fec-8ab0-e1d349ed0be0
description: Description 要素は、アイテム保持ポリシーの説明テキストを指定します。
ms.openlocfilehash: a399d4072220e3fa9199f0a3eb760e886b7b4ee6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467887"
---
# <a name="description"></a><span data-ttu-id="eda46-103">説明</span><span class="sxs-lookup"><span data-stu-id="eda46-103">Description</span></span>

<span data-ttu-id="eda46-104">**Description**要素は、アイテム保持ポリシーの説明テキストを指定します。</span><span class="sxs-lookup"><span data-stu-id="eda46-104">The **Description** element specifies the descriptive text for the retention policy.</span></span> 
  
```XML
<Description></Description>
```

 <span data-ttu-id="eda46-105">**string**</span><span class="sxs-lookup"><span data-stu-id="eda46-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="eda46-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="eda46-106">Attributes and elements</span></span>

<span data-ttu-id="eda46-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="eda46-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="eda46-108">属性</span><span class="sxs-lookup"><span data-stu-id="eda46-108">Attributes</span></span>

<span data-ttu-id="eda46-109">なし。</span><span class="sxs-lookup"><span data-stu-id="eda46-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="eda46-110">子要素</span><span class="sxs-lookup"><span data-stu-id="eda46-110">Child elements</span></span>

<span data-ttu-id="eda46-111">なし。</span><span class="sxs-lookup"><span data-stu-id="eda46-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="eda46-112">親要素</span><span class="sxs-lookup"><span data-stu-id="eda46-112">Parent elements</span></span>

|<span data-ttu-id="eda46-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="eda46-113">**Element**</span></span>|<span data-ttu-id="eda46-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="eda46-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eda46-115">New-retentionpolicytag</span><span class="sxs-lookup"><span data-stu-id="eda46-115">RetentionPolicyTag</span></span>](retentionpolicytag.md) <br/> |<span data-ttu-id="eda46-116">メールボックスアイテムのアイテム保持ポリシーを指定します。</span><span class="sxs-lookup"><span data-stu-id="eda46-116">Specifies the retention policy for a mailbox item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="eda46-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="eda46-117">Text value</span></span>

<span data-ttu-id="eda46-118">**Description**要素のテキスト値は、アイテム保持ポリシーを説明する文字列型 (string) の値です。</span><span class="sxs-lookup"><span data-stu-id="eda46-118">The text value of the **Description** element is a string value that describes the retention policy.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="eda46-119">注釈</span><span class="sxs-lookup"><span data-stu-id="eda46-119">Remarks</span></span>

<span data-ttu-id="eda46-120">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="eda46-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="eda46-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="eda46-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="eda46-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="eda46-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="eda46-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="eda46-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="eda46-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="eda46-124">Schema Name</span></span>  <br/> |<span data-ttu-id="eda46-125">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="eda46-125">Type schema</span></span>  <br/> |
|<span data-ttu-id="eda46-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="eda46-126">Validation File</span></span>  <br/> |<span data-ttu-id="eda46-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="eda46-127">types.xsd</span></span>  <br/> |
|<span data-ttu-id="eda46-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="eda46-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="eda46-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="eda46-129">See also</span></span>

- [<span data-ttu-id="eda46-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="eda46-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

