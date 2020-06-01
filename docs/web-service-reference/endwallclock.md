---
title: EndWallClock
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bc04e44e-e6d1-4355-a2b1-feb6663dc647
description: EndWallClock 要素は、会議が開催される場所のタイムゾーンで、会議の終了時刻を指定します。
ms.openlocfilehash: 48b762d0bfe367b966b6f1790230f6a2118c3fd6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462972"
---
# <a name="endwallclock"></a><span data-ttu-id="0e934-103">EndWallClock</span><span class="sxs-lookup"><span data-stu-id="0e934-103">EndWallClock</span></span>

<span data-ttu-id="0e934-104">**EndWallClock**要素は、会議が開催される場所のタイムゾーンで、会議の終了時刻を指定します。</span><span class="sxs-lookup"><span data-stu-id="0e934-104">The **EndWallClock** element specifies the end time of a meeting in the time zone of the location in which the meeting takes place.</span></span> 
  
```XML
<EndWallClock></EndWallClock>
```

 <span data-ttu-id="0e934-105">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="0e934-105">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0e934-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="0e934-106">Attributes and elements</span></span>

<span data-ttu-id="0e934-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0e934-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0e934-108">属性</span><span class="sxs-lookup"><span data-stu-id="0e934-108">Attributes</span></span>

<span data-ttu-id="0e934-109">なし。</span><span class="sxs-lookup"><span data-stu-id="0e934-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0e934-110">子要素</span><span class="sxs-lookup"><span data-stu-id="0e934-110">Child elements</span></span>

<span data-ttu-id="0e934-111">なし。</span><span class="sxs-lookup"><span data-stu-id="0e934-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0e934-112">親要素</span><span class="sxs-lookup"><span data-stu-id="0e934-112">Parent elements</span></span>

|<span data-ttu-id="0e934-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="0e934-113">**Element**</span></span>|<span data-ttu-id="0e934-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="0e934-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0e934-115">ユーザー</span><span class="sxs-lookup"><span data-stu-id="0e934-115">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="0e934-116">**Getpersona**要求によって返される一連のペルソナデータを指定します。</span><span class="sxs-lookup"><span data-stu-id="0e934-116">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0e934-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="0e934-117">Text value</span></span>

<span data-ttu-id="0e934-118">**EndWallClock**要素のテキスト値は、タイムゾーン識別子を指定する文字列型 (string) の値です。</span><span class="sxs-lookup"><span data-stu-id="0e934-118">The text value of the **EndWallClock** element is a string value that specifies the time zone identifier.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="0e934-119">注釈</span><span class="sxs-lookup"><span data-stu-id="0e934-119">Remarks</span></span>

<span data-ttu-id="0e934-120">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="0e934-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="0e934-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="0e934-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0e934-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="0e934-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0e934-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="0e934-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0e934-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0e934-124">Schema Name</span></span>  <br/> |<span data-ttu-id="0e934-125">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="0e934-125">Type schema</span></span>  <br/> |
|<span data-ttu-id="0e934-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0e934-126">Validation File</span></span>  <br/> |<span data-ttu-id="0e934-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="0e934-127">types.xsd</span></span>  <br/> |
|<span data-ttu-id="0e934-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="0e934-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="0e934-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="0e934-129">See also</span></span>



- [<span data-ttu-id="0e934-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="0e934-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

