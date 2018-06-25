---
title: IsArchive
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b89d8a78-5c18-4547-aaf4-4b16a93190a7
description: IsArchive 要素は、メールボックスが、アーカイブ メールボックスであるかどうかを示すブール値を指定します。
ms.openlocfilehash: 417afd1afc25e5872d1f511feff34494fe6b7b62
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831990"
---
# <a name="isarchive"></a><span data-ttu-id="e7426-103">IsArchive</span><span class="sxs-lookup"><span data-stu-id="e7426-103">IsArchive</span></span>

<span data-ttu-id="e7426-104">**IsArchive**要素は、メールボックスが、アーカイブ メールボックスであるかどうかを示すブール値を指定します。</span><span class="sxs-lookup"><span data-stu-id="e7426-104">The **IsArchive** element specifies a Boolean value that indicates whether the mailbox is an archive mailbox.</span></span> 
  
```XML
<IsArchive>true | false</IsArchive>
```

 <span data-ttu-id="e7426-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="e7426-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e7426-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="e7426-106">Attributes and elements</span></span>

<span data-ttu-id="e7426-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e7426-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e7426-108">属性</span><span class="sxs-lookup"><span data-stu-id="e7426-108">Attributes</span></span>

<span data-ttu-id="e7426-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e7426-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e7426-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e7426-110">Child elements</span></span>

<span data-ttu-id="e7426-111">なし。</span><span class="sxs-lookup"><span data-stu-id="e7426-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e7426-112">親要素</span><span class="sxs-lookup"><span data-stu-id="e7426-112">Parent elements</span></span>

<span data-ttu-id="e7426-113">[FailedMailbox](failedmailbox.md) | [RetentionPolicyTag](retentionpolicytag.md)</span><span class="sxs-lookup"><span data-stu-id="e7426-113">[FailedMailbox](failedmailbox.md) | [RetentionPolicyTag](retentionpolicytag.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="e7426-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="e7426-114">Text value</span></span>

<span data-ttu-id="e7426-115">テキストの値**は true** **IsArchive**要素の移動先のメールボックスが、アーカイブ メールボックスであることを示します。</span><span class="sxs-lookup"><span data-stu-id="e7426-115">A text value of **true** for the **IsArchive** element indicates that the target mailbox is an archive mailbox.</span></span> <span data-ttu-id="e7426-116">**False**の値は、移動先のメールボックスは、アーカイブ メールボックスではないことを示します。</span><span class="sxs-lookup"><span data-stu-id="e7426-116">A value of **false** indicates that the target mailbox is not an archive mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="e7426-117">備考</span><span class="sxs-lookup"><span data-stu-id="e7426-117">Remarks</span></span>

<span data-ttu-id="e7426-118">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="e7426-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e7426-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="e7426-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e7426-120">要素情報</span><span class="sxs-lookup"><span data-stu-id="e7426-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e7426-121">名前空間</span><span class="sxs-lookup"><span data-stu-id="e7426-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e7426-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e7426-122">Schema Name</span></span>  <br/> |<span data-ttu-id="e7426-123">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="e7426-123">Type schema</span></span>  <br/> |
|<span data-ttu-id="e7426-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e7426-124">Validation File</span></span>  <br/> |<span data-ttu-id="e7426-125">types.xsd</span><span class="sxs-lookup"><span data-stu-id="e7426-125">types.xsd</span></span>  <br/> |
|<span data-ttu-id="e7426-126">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="e7426-126">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="e7426-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="e7426-127">See also</span></span>



- [<span data-ttu-id="e7426-128">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="e7426-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

