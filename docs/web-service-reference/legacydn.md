---
title: LegacyDN
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 72cec5ec-8485-431c-95b7-b9c2247669d6
description: LegacyDN 要素では、従来の識別名でメールボックスを識別します。
ms.openlocfilehash: 8cd0aeb3018a6a45a3b7172d83ac0899a012b353
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832238"
---
# <a name="legacydn"></a><span data-ttu-id="89003-103">LegacyDN</span><span class="sxs-lookup"><span data-stu-id="89003-103">LegacyDN</span></span>

<span data-ttu-id="89003-104">**LegacyDN**要素では、従来の識別名でメールボックスを識別します。</span><span class="sxs-lookup"><span data-stu-id="89003-104">The **LegacyDN** element identifies a mailbox by its legacy distinguished name.</span></span> 
  
```XML
<LegacyDN></LegacyDN>
```

<span data-ttu-id="89003-105">**string**</span><span class="sxs-lookup"><span data-stu-id="89003-105">**string**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="89003-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="89003-106">Attributes and elements</span></span>

<span data-ttu-id="89003-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="89003-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="89003-108">属性</span><span class="sxs-lookup"><span data-stu-id="89003-108">Attributes</span></span>

<span data-ttu-id="89003-109">なし。</span><span class="sxs-lookup"><span data-stu-id="89003-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="89003-110">子要素</span><span class="sxs-lookup"><span data-stu-id="89003-110">Child elements</span></span>

<span data-ttu-id="89003-111">なし。</span><span class="sxs-lookup"><span data-stu-id="89003-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="89003-112">親要素</span><span class="sxs-lookup"><span data-stu-id="89003-112">Parent elements</span></span>

[<span data-ttu-id="89003-113">メールボックス (NonEmptyArrayOfLegacyDNsType)</span><span class="sxs-lookup"><span data-stu-id="89003-113">Mailboxes (NonEmptyArrayOfLegacyDNsType)</span></span>](mailboxes-nonemptyarrayoflegacydnstype.md)
  
## <a name="text-value"></a><span data-ttu-id="89003-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="89003-114">Text value</span></span>

<span data-ttu-id="89003-115">**LegacyDN**要素のテキスト値は、移動先のメールボックスの従来の識別名です。</span><span class="sxs-lookup"><span data-stu-id="89003-115">The text value of **LegacyDN** element is the legacy distinguished name of the target mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="89003-116">備考</span><span class="sxs-lookup"><span data-stu-id="89003-116">Remarks</span></span>

<span data-ttu-id="89003-117">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="89003-117">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="89003-118">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="89003-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="89003-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="89003-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="89003-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="89003-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="89003-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="89003-121">Schema name</span></span>  <br/> |<span data-ttu-id="89003-122">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="89003-122">Types schema</span></span>  <br/> |
|<span data-ttu-id="89003-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="89003-123">Validation file</span></span>  <br/> |<span data-ttu-id="89003-124">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="89003-124">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="89003-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="89003-125">Can be empty</span></span>  <br/> ||
   

