---
title: Birthday
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Birthday
api_type:
- schema
ms.assetid: b7529004-46e2-4ac9-b4e4-c8bb6878a7d5
description: 誕生日要素では、取引先担当者の生年月日を表します。
ms.openlocfilehash: 480b922e77f7755932b17e30239ff9d619e555c8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759503"
---
# <a name="birthday"></a><span data-ttu-id="4a9ec-103">Birthday</span><span class="sxs-lookup"><span data-stu-id="4a9ec-103">Birthday</span></span>

<span data-ttu-id="4a9ec-104">**誕生日**要素では、取引先担当者の生年月日を表します。</span><span class="sxs-lookup"><span data-stu-id="4a9ec-104">The **Birthday** element represents the birth date of a contact.</span></span> 
  
```xml
<Birthday/>
```

 <span data-ttu-id="4a9ec-105">**DateTime**</span><span class="sxs-lookup"><span data-stu-id="4a9ec-105">**DateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4a9ec-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="4a9ec-106">Attributes and elements</span></span>

<span data-ttu-id="4a9ec-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4a9ec-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4a9ec-108">属性</span><span class="sxs-lookup"><span data-stu-id="4a9ec-108">Attributes</span></span>

<span data-ttu-id="4a9ec-109">なし。</span><span class="sxs-lookup"><span data-stu-id="4a9ec-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4a9ec-110">子要素</span><span class="sxs-lookup"><span data-stu-id="4a9ec-110">Child elements</span></span>

<span data-ttu-id="4a9ec-111">なし。</span><span class="sxs-lookup"><span data-stu-id="4a9ec-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4a9ec-112">親要素</span><span class="sxs-lookup"><span data-stu-id="4a9ec-112">Parent elements</span></span>

|<span data-ttu-id="4a9ec-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="4a9ec-113">**Element**</span></span>|<span data-ttu-id="4a9ec-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="4a9ec-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4a9ec-115">Contact</span><span class="sxs-lookup"><span data-stu-id="4a9ec-115">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="4a9ec-116">Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="4a9ec-116">Represents an Exchange contact item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4a9ec-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="4a9ec-117">Text value</span></span>

<span data-ttu-id="4a9ec-118">日付と時刻を表す文字列値は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="4a9ec-118">A text value that represents a date and time is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4a9ec-119">備考</span><span class="sxs-lookup"><span data-stu-id="4a9ec-119">Remarks</span></span>

<span data-ttu-id="4a9ec-120">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="4a9ec-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4a9ec-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="4a9ec-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4a9ec-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="4a9ec-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4a9ec-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4a9ec-123">Schema name</span></span>  <br/> |<span data-ttu-id="4a9ec-124">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="4a9ec-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="4a9ec-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4a9ec-125">Validation file</span></span>  <br/> |<span data-ttu-id="4a9ec-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4a9ec-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4a9ec-127">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="4a9ec-127">Can be empty</span></span>  <br/> |<span data-ttu-id="4a9ec-128">False</span><span class="sxs-lookup"><span data-stu-id="4a9ec-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4a9ec-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="4a9ec-129">See also</span></span>



- [<span data-ttu-id="4a9ec-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="4a9ec-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

