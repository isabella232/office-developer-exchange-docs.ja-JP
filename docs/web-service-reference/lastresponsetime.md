---
title: LastResponseTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- LastResponseTime
api_type:
- schema
ms.assetid: 8e66979e-4e3b-4183-aaf5-a45d8380ede5
description: LastResponseTime 要素は、最新の応答を受信したときの日時を表します。
ms.openlocfilehash: 77f79d87be0b88f8c91c04438a2541643aad8858
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832205"
---
# <a name="lastresponsetime"></a><span data-ttu-id="da94b-103">LastResponseTime</span><span class="sxs-lookup"><span data-stu-id="da94b-103">LastResponseTime</span></span>

<span data-ttu-id="da94b-104">**LastResponseTime**要素は、最新の応答を受信したときの日時を表します。</span><span class="sxs-lookup"><span data-stu-id="da94b-104">The **LastResponseTime** element represents the date and time of the latest response received.</span></span> 
  
```xml
<LastResponseTime/>
```

 <span data-ttu-id="da94b-105">**DateTime**</span><span class="sxs-lookup"><span data-stu-id="da94b-105">**DateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="da94b-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="da94b-106">Attributes and elements</span></span>

<span data-ttu-id="da94b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="da94b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="da94b-108">属性</span><span class="sxs-lookup"><span data-stu-id="da94b-108">Attributes</span></span>

<span data-ttu-id="da94b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="da94b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="da94b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="da94b-110">Child elements</span></span>

<span data-ttu-id="da94b-111">なし。</span><span class="sxs-lookup"><span data-stu-id="da94b-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="da94b-112">親要素</span><span class="sxs-lookup"><span data-stu-id="da94b-112">Parent elements</span></span>

|<span data-ttu-id="da94b-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="da94b-113">**Element**</span></span>|<span data-ttu-id="da94b-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="da94b-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="da94b-115">Attendee</span><span class="sxs-lookup"><span data-stu-id="da94b-115">Attendee</span></span>](attendee.md) <br/> |<span data-ttu-id="da94b-116">出席者および会議のためのリソースを表します。</span><span class="sxs-lookup"><span data-stu-id="da94b-116">Represents attendees and resources for a meeting.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="da94b-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="da94b-117">Text value</span></span>

<span data-ttu-id="da94b-118">最新の応答の時間と日付を表す文字列値は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="da94b-118">A text value that represents the date and time of the latest response is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="da94b-119">備考</span><span class="sxs-lookup"><span data-stu-id="da94b-119">Remarks</span></span>

<span data-ttu-id="da94b-120">MicrosoftExchange 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="da94b-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="da94b-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="da94b-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="da94b-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="da94b-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="da94b-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="da94b-123">Schema name</span></span>  <br/> |<span data-ttu-id="da94b-124">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="da94b-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="da94b-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="da94b-125">Validation file</span></span>  <br/> |<span data-ttu-id="da94b-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="da94b-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="da94b-127">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="da94b-127">Can be empty</span></span>  <br/> |<span data-ttu-id="da94b-128">False</span><span class="sxs-lookup"><span data-stu-id="da94b-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="da94b-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="da94b-129">See also</span></span>



- [<span data-ttu-id="da94b-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="da94b-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

