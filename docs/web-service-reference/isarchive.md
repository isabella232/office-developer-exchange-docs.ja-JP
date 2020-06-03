---
title: IsArchive
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b89d8a78-5c18-4547-aaf4-4b16a93190a7
description: IsArchive 要素は、メールボックスがアーカイブメールボックスであるかどうかを示すブール値を指定します。
ms.openlocfilehash: 6d0be0eb283de3f4d8f786ff96f4a0d4f49e2009
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526516"
---
# <a name="isarchive"></a><span data-ttu-id="dc47b-103">IsArchive</span><span class="sxs-lookup"><span data-stu-id="dc47b-103">IsArchive</span></span>

<span data-ttu-id="dc47b-104">**Isarchive**要素は、メールボックスがアーカイブメールボックスであるかどうかを示すブール値を指定します。</span><span class="sxs-lookup"><span data-stu-id="dc47b-104">The **IsArchive** element specifies a Boolean value that indicates whether the mailbox is an archive mailbox.</span></span> 
  
```XML
<IsArchive>true | false</IsArchive>
```

 <span data-ttu-id="dc47b-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="dc47b-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dc47b-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="dc47b-106">Attributes and elements</span></span>

<span data-ttu-id="dc47b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="dc47b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dc47b-108">属性</span><span class="sxs-lookup"><span data-stu-id="dc47b-108">Attributes</span></span>

<span data-ttu-id="dc47b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="dc47b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dc47b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="dc47b-110">Child elements</span></span>

<span data-ttu-id="dc47b-111">なし。</span><span class="sxs-lookup"><span data-stu-id="dc47b-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="dc47b-112">親要素</span><span class="sxs-lookup"><span data-stu-id="dc47b-112">Parent elements</span></span>

<span data-ttu-id="dc47b-113">[失敗したメールボックス](failedmailbox.md)  | [New-retentionpolicytag](retentionpolicytag.md)</span><span class="sxs-lookup"><span data-stu-id="dc47b-113">[FailedMailbox](failedmailbox.md) | [RetentionPolicyTag](retentionpolicytag.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="dc47b-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="dc47b-114">Text value</span></span>

<span data-ttu-id="dc47b-115">**Isarchive**要素のテキスト値が**true の場合**は、ターゲットメールボックスがアーカイブメールボックスであることを示します。</span><span class="sxs-lookup"><span data-stu-id="dc47b-115">A text value of **true** for the **IsArchive** element indicates that the target mailbox is an archive mailbox.</span></span> <span data-ttu-id="dc47b-116">値が**false**の場合、ターゲットメールボックスがアーカイブメールボックスではないことを示します。</span><span class="sxs-lookup"><span data-stu-id="dc47b-116">A value of **false** indicates that the target mailbox is not an archive mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="dc47b-117">注釈</span><span class="sxs-lookup"><span data-stu-id="dc47b-117">Remarks</span></span>

<span data-ttu-id="dc47b-118">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="dc47b-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="dc47b-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="dc47b-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dc47b-120">要素の情報</span><span class="sxs-lookup"><span data-stu-id="dc47b-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dc47b-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="dc47b-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="dc47b-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="dc47b-122">Schema Name</span></span>  <br/> |<span data-ttu-id="dc47b-123">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="dc47b-123">Type schema</span></span>  <br/> |
|<span data-ttu-id="dc47b-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="dc47b-124">Validation File</span></span>  <br/> |<span data-ttu-id="dc47b-125">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="dc47b-125">types.xsd</span></span>  <br/> |
|<span data-ttu-id="dc47b-126">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="dc47b-126">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="dc47b-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="dc47b-127">See also</span></span>



- [<span data-ttu-id="dc47b-128">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="dc47b-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

