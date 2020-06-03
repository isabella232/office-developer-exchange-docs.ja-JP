---
title: LegacyDN
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 72cec5ec-8485-431c-95b7-b9c2247669d6
description: LegacyDN 要素は、従来の識別名でメールボックスを識別します。
ms.openlocfilehash: b5eb23d285925f97cc25f53b56bca669bbbb5840
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463238"
---
# <a name="legacydn"></a><span data-ttu-id="75dc4-103">LegacyDN</span><span class="sxs-lookup"><span data-stu-id="75dc4-103">LegacyDN</span></span>

<span data-ttu-id="75dc4-104">**LegacyDN**要素は、従来の識別名でメールボックスを識別します。</span><span class="sxs-lookup"><span data-stu-id="75dc4-104">The **LegacyDN** element identifies a mailbox by its legacy distinguished name.</span></span> 
  
```XML
<LegacyDN></LegacyDN>
```

<span data-ttu-id="75dc4-105">**string**</span><span class="sxs-lookup"><span data-stu-id="75dc4-105">**string**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="75dc4-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="75dc4-106">Attributes and elements</span></span>

<span data-ttu-id="75dc4-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="75dc4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="75dc4-108">属性</span><span class="sxs-lookup"><span data-stu-id="75dc4-108">Attributes</span></span>

<span data-ttu-id="75dc4-109">なし。</span><span class="sxs-lookup"><span data-stu-id="75dc4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="75dc4-110">子要素</span><span class="sxs-lookup"><span data-stu-id="75dc4-110">Child elements</span></span>

<span data-ttu-id="75dc4-111">なし。</span><span class="sxs-lookup"><span data-stu-id="75dc4-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="75dc4-112">親要素</span><span class="sxs-lookup"><span data-stu-id="75dc4-112">Parent elements</span></span>

[<span data-ttu-id="75dc4-113">メールボックス (NonEmptyArrayOfLegacyDNsType)</span><span class="sxs-lookup"><span data-stu-id="75dc4-113">Mailboxes (NonEmptyArrayOfLegacyDNsType)</span></span>](mailboxes-nonemptyarrayoflegacydnstype.md)
  
## <a name="text-value"></a><span data-ttu-id="75dc4-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="75dc4-114">Text value</span></span>

<span data-ttu-id="75dc4-115">**LegacyDN**要素のテキスト値は、ターゲットメールボックスの従来の識別名です。</span><span class="sxs-lookup"><span data-stu-id="75dc4-115">The text value of **LegacyDN** element is the legacy distinguished name of the target mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="75dc4-116">注釈</span><span class="sxs-lookup"><span data-stu-id="75dc4-116">Remarks</span></span>

<span data-ttu-id="75dc4-117">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="75dc4-117">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="75dc4-118">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="75dc4-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="75dc4-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="75dc4-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="75dc4-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="75dc4-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="75dc4-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="75dc4-121">Schema name</span></span>  <br/> |<span data-ttu-id="75dc4-122">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="75dc4-122">Types schema</span></span>  <br/> |
|<span data-ttu-id="75dc4-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="75dc4-123">Validation file</span></span>  <br/> |<span data-ttu-id="75dc4-124">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="75dc4-124">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="75dc4-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="75dc4-125">Can be empty</span></span>  <br/> ||
   

