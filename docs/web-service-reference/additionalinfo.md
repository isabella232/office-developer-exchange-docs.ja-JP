---
title: AdditionalInfo
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 50bebbab-2fef-4a27-a5a9-32d7200820b6
description: AdditionalInfo 要素は、メールボックスの保留中の状態に関する追加情報を指定します。
ms.openlocfilehash: 6fbe24d5d3e41f2ba9c81657b2c38240d10eefed
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759289"
---
# <a name="additionalinfo"></a><span data-ttu-id="5d177-103">AdditionalInfo</span><span class="sxs-lookup"><span data-stu-id="5d177-103">AdditionalInfo</span></span>

<span data-ttu-id="5d177-104">**AdditionalInfo**要素は、メールボックスの保留中の状態に関する追加情報を指定します。</span><span class="sxs-lookup"><span data-stu-id="5d177-104">The **AdditionalInfo** element specifies additional information about the hold status of a mailbox.</span></span> 
  
```XML
<AdditionalInfo></AdditionalInfo>
```

 <span data-ttu-id="5d177-105">**使用されています**</span><span class="sxs-lookup"><span data-stu-id="5d177-105">**xs:string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5d177-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="5d177-106">Attributes and elements</span></span>

<span data-ttu-id="5d177-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5d177-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5d177-108">属性</span><span class="sxs-lookup"><span data-stu-id="5d177-108">Attributes</span></span>

<span data-ttu-id="5d177-109">なし。</span><span class="sxs-lookup"><span data-stu-id="5d177-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5d177-110">子要素</span><span class="sxs-lookup"><span data-stu-id="5d177-110">Child elements</span></span>

<span data-ttu-id="5d177-111">なし。</span><span class="sxs-lookup"><span data-stu-id="5d177-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5d177-112">親要素</span><span class="sxs-lookup"><span data-stu-id="5d177-112">Parent elements</span></span>

|<span data-ttu-id="5d177-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="5d177-113">**Element**</span></span>|<span data-ttu-id="5d177-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="5d177-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5d177-115">MailboxHoldStatus</span><span class="sxs-lookup"><span data-stu-id="5d177-115">MailboxHoldStatus</span></span>](mailboxholdstatus.md) <br/> |<span data-ttu-id="5d177-116">メールボックスの保留状態を指定します。</span><span class="sxs-lookup"><span data-stu-id="5d177-116">Specifies the hold status of the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="5d177-117">NonIndexableItemDetail</span><span class="sxs-lookup"><span data-stu-id="5d177-117">NonIndexableItemDetail</span></span>](nonindexableitemdetail.md) <br/> |<span data-ttu-id="5d177-118">インデックスを作成できないアイテムの詳細を指定します。</span><span class="sxs-lookup"><span data-stu-id="5d177-118">Specifies detail for an item that cannot be indexed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5d177-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="5d177-119">Text value</span></span>

<span data-ttu-id="5d177-120">AdditionalInfo 要素のテキスト値は、メールボックスの保留中の状態に関する追加情報です。</span><span class="sxs-lookup"><span data-stu-id="5d177-120">The text value of the AdditionalInfo element is additional information about the hold status of a mailbox.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5d177-121">備考</span><span class="sxs-lookup"><span data-stu-id="5d177-121">Remarks</span></span>

<span data-ttu-id="5d177-122">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="5d177-122">This element is optional.</span></span>
  
<span data-ttu-id="5d177-123">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="5d177-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="5d177-124">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="5d177-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5d177-125">要素情報</span><span class="sxs-lookup"><span data-stu-id="5d177-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5d177-126">名前空間</span><span class="sxs-lookup"><span data-stu-id="5d177-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5d177-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5d177-127">Schema Name</span></span>  <br/> |<span data-ttu-id="5d177-128">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="5d177-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="5d177-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5d177-129">Validation File</span></span>  <br/> |<span data-ttu-id="5d177-130">types.xsd</span><span class="sxs-lookup"><span data-stu-id="5d177-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="5d177-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="5d177-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="5d177-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="5d177-132">See also</span></span>

- [<span data-ttu-id="5d177-133">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="5d177-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

