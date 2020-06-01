---
title: AdditionalInfo
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 50bebbab-2fef-4a27-a5a9-32d7200820b6
description: AdditionalInfo 要素は、メールボックスの保留状態に関する追加情報を指定します。
ms.openlocfilehash: 1911ff3ac0baf7a8854c0609e08959a54cc27b6d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455822"
---
# <a name="additionalinfo"></a><span data-ttu-id="30d7a-103">AdditionalInfo</span><span class="sxs-lookup"><span data-stu-id="30d7a-103">AdditionalInfo</span></span>

<span data-ttu-id="30d7a-104">**Additionalinfo**要素は、メールボックスの保留状態に関する追加情報を指定します。</span><span class="sxs-lookup"><span data-stu-id="30d7a-104">The **AdditionalInfo** element specifies additional information about the hold status of a mailbox.</span></span> 
  
```XML
<AdditionalInfo></AdditionalInfo>
```

 <span data-ttu-id="30d7a-105">**xs: 文字列**</span><span class="sxs-lookup"><span data-stu-id="30d7a-105">**xs:string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="30d7a-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="30d7a-106">Attributes and elements</span></span>

<span data-ttu-id="30d7a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="30d7a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="30d7a-108">属性</span><span class="sxs-lookup"><span data-stu-id="30d7a-108">Attributes</span></span>

<span data-ttu-id="30d7a-109">なし。</span><span class="sxs-lookup"><span data-stu-id="30d7a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="30d7a-110">子要素</span><span class="sxs-lookup"><span data-stu-id="30d7a-110">Child elements</span></span>

<span data-ttu-id="30d7a-111">なし。</span><span class="sxs-lookup"><span data-stu-id="30d7a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="30d7a-112">親要素</span><span class="sxs-lookup"><span data-stu-id="30d7a-112">Parent elements</span></span>

|<span data-ttu-id="30d7a-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="30d7a-113">**Element**</span></span>|<span data-ttu-id="30d7a-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="30d7a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="30d7a-115">MailboxHoldStatus</span><span class="sxs-lookup"><span data-stu-id="30d7a-115">MailboxHoldStatus</span></span>](mailboxholdstatus.md) <br/> |<span data-ttu-id="30d7a-116">メールボックスの保持状態を指定します。</span><span class="sxs-lookup"><span data-stu-id="30d7a-116">Specifies the hold status of the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="30d7a-117">NonIndexableItemDetail</span><span class="sxs-lookup"><span data-stu-id="30d7a-117">NonIndexableItemDetail</span></span>](nonindexableitemdetail.md) <br/> |<span data-ttu-id="30d7a-118">インデックスを作成できないアイテムの詳細を指定します。</span><span class="sxs-lookup"><span data-stu-id="30d7a-118">Specifies detail for an item that cannot be indexed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="30d7a-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="30d7a-119">Text value</span></span>

<span data-ttu-id="30d7a-120">AdditionalInfo 要素のテキスト値は、メールボックスの保持状態に関する追加情報です。</span><span class="sxs-lookup"><span data-stu-id="30d7a-120">The text value of the AdditionalInfo element is additional information about the hold status of a mailbox.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="30d7a-121">注釈</span><span class="sxs-lookup"><span data-stu-id="30d7a-121">Remarks</span></span>

<span data-ttu-id="30d7a-122">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="30d7a-122">This element is optional.</span></span>
  
<span data-ttu-id="30d7a-123">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="30d7a-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="30d7a-124">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="30d7a-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="30d7a-125">要素の情報</span><span class="sxs-lookup"><span data-stu-id="30d7a-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="30d7a-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="30d7a-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="30d7a-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="30d7a-127">Schema Name</span></span>  <br/> |<span data-ttu-id="30d7a-128">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="30d7a-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="30d7a-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="30d7a-129">Validation File</span></span>  <br/> |<span data-ttu-id="30d7a-130">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="30d7a-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="30d7a-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="30d7a-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="30d7a-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="30d7a-132">See also</span></span>

- [<span data-ttu-id="30d7a-133">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="30d7a-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

