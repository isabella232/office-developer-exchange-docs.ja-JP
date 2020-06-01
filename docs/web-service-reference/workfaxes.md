---
title: ファックス
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 95d115a1-2743-4416-af6f-1ef1be8c4e93
description: 仕事用の Fax 要素は、勤務先の fax 番号の配列と、関連付けられたペルソナのソース attributions の識別子を指定します。
ms.openlocfilehash: d0da5fc2e1b26d14ef3c07f876174da6ccacd016
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459687"
---
# <a name="workfaxes"></a><span data-ttu-id="8cc29-103">ファックス</span><span class="sxs-lookup"><span data-stu-id="8cc29-103">WorkFaxes</span></span>

<span data-ttu-id="8cc29-104">仕事用の**fax**要素は、勤務先の fax 番号の配列と、関連付けられたペルソナのソース attributions の識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="8cc29-104">The **WorkFaxes** element specifies an array of work fax numbers and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<WorkFaxes>
   <PhoneNumberAttributedValue/>
</WorkFaxes>
```

 <span data-ttu-id="8cc29-105">**ArrayOfPhoneNumberAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="8cc29-105">**ArrayOfPhoneNumberAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8cc29-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="8cc29-106">Attributes and elements</span></span>

<span data-ttu-id="8cc29-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8cc29-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8cc29-108">属性</span><span class="sxs-lookup"><span data-stu-id="8cc29-108">Attributes</span></span>

<span data-ttu-id="8cc29-109">なし。</span><span class="sxs-lookup"><span data-stu-id="8cc29-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8cc29-110">子要素</span><span class="sxs-lookup"><span data-stu-id="8cc29-110">Child elements</span></span>

[<span data-ttu-id="8cc29-111">PhoneNumberAttributedValue</span><span class="sxs-lookup"><span data-stu-id="8cc29-111">PhoneNumberAttributedValue</span></span>](phonenumberattributedvalue.md)
  
### <a name="parent-elements"></a><span data-ttu-id="8cc29-112">親要素</span><span class="sxs-lookup"><span data-stu-id="8cc29-112">Parent elements</span></span>

[<span data-ttu-id="8cc29-113">ユーザー</span><span class="sxs-lookup"><span data-stu-id="8cc29-113">Persona</span></span>](persona.md)
  
## <a name="remarks"></a><span data-ttu-id="8cc29-114">注釈</span><span class="sxs-lookup"><span data-stu-id="8cc29-114">Remarks</span></span>

<span data-ttu-id="8cc29-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="8cc29-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="8cc29-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="8cc29-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8cc29-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="8cc29-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8cc29-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="8cc29-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8cc29-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8cc29-119">Schema name</span></span>  <br/> |<span data-ttu-id="8cc29-120">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="8cc29-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="8cc29-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8cc29-121">Validation file</span></span>  <br/> |<span data-ttu-id="8cc29-122">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="8cc29-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8cc29-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="8cc29-123">Can be empty</span></span>  <br/> ||
   

