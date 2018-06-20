---
title: YomiLastNames
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 893409f1-fe76-40a4-ad7b-8a6bbc2bce12
description: YomiLastNames 要素は、ルビ日本語姓と名の配列と関連付けられているペルソナにそのソースの帰属の識別子を指定します。
ms.openlocfilehash: 8b413c20b50e4ccd6b4dc427e70b921ad34c7949
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840059"
---
# <a name="yomilastnames"></a><span data-ttu-id="2c204-103">YomiLastNames</span><span class="sxs-lookup"><span data-stu-id="2c204-103">YomiLastNames</span></span>

<span data-ttu-id="2c204-104">**YomiLastNames**要素は、ルビ日本語姓と名の配列と関連付けられているペルソナにそのソースの帰属の識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="2c204-104">The **YomiLastNames** element specifies an array of phonetic Japanese last names and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<YomiLastNames>
   <StringAttributedValue/>
</YomiLastNames>
```

 <span data-ttu-id="2c204-105">**ArrayOfStringAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="2c204-105">**ArrayOfStringAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2c204-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="2c204-106">Attributes and elements</span></span>

<span data-ttu-id="2c204-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2c204-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2c204-108">属性</span><span class="sxs-lookup"><span data-stu-id="2c204-108">Attributes</span></span>

<span data-ttu-id="2c204-109">なし。</span><span class="sxs-lookup"><span data-stu-id="2c204-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2c204-110">子要素</span><span class="sxs-lookup"><span data-stu-id="2c204-110">Child elements</span></span>

[<span data-ttu-id="2c204-111">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="2c204-111">StringAttributedValue</span></span>](stringattributedvalue.md)
  
### <a name="parent-elements"></a><span data-ttu-id="2c204-112">親要素</span><span class="sxs-lookup"><span data-stu-id="2c204-112">Parent elements</span></span>

[<span data-ttu-id="2c204-113">ペルソナ</span><span class="sxs-lookup"><span data-stu-id="2c204-113">Persona</span></span>](persona.md)
  
## <a name="remarks"></a><span data-ttu-id="2c204-114">備考</span><span class="sxs-lookup"><span data-stu-id="2c204-114">Remarks</span></span>

<span data-ttu-id="2c204-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="2c204-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="2c204-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="2c204-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2c204-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="2c204-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2c204-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="2c204-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2c204-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2c204-119">Schema name</span></span>  <br/> |<span data-ttu-id="2c204-120">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="2c204-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="2c204-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2c204-121">Validation file</span></span>  <br/> |<span data-ttu-id="2c204-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2c204-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2c204-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="2c204-123">Can be empty</span></span>  <br/> ||
   

