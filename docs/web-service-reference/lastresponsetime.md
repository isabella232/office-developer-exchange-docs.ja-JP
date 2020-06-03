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
description: LastResponseTime 要素は、最新の応答を受信した日付と時刻を表します。
ms.openlocfilehash: 45740d1a31d9b04bbc5062e7ff8b05629abd84c4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455381"
---
# <a name="lastresponsetime"></a><span data-ttu-id="97fb8-103">LastResponseTime</span><span class="sxs-lookup"><span data-stu-id="97fb8-103">LastResponseTime</span></span>

<span data-ttu-id="97fb8-104">**LastResponseTime**要素は、最新の応答を受信した日付と時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="97fb8-104">The **LastResponseTime** element represents the date and time of the latest response received.</span></span> 
  
```xml
<LastResponseTime/>
```

 <span data-ttu-id="97fb8-105">**DateTime**</span><span class="sxs-lookup"><span data-stu-id="97fb8-105">**DateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="97fb8-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="97fb8-106">Attributes and elements</span></span>

<span data-ttu-id="97fb8-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="97fb8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="97fb8-108">属性</span><span class="sxs-lookup"><span data-stu-id="97fb8-108">Attributes</span></span>

<span data-ttu-id="97fb8-109">なし。</span><span class="sxs-lookup"><span data-stu-id="97fb8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="97fb8-110">子要素</span><span class="sxs-lookup"><span data-stu-id="97fb8-110">Child elements</span></span>

<span data-ttu-id="97fb8-111">なし。</span><span class="sxs-lookup"><span data-stu-id="97fb8-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="97fb8-112">親要素</span><span class="sxs-lookup"><span data-stu-id="97fb8-112">Parent elements</span></span>

|<span data-ttu-id="97fb8-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="97fb8-113">**Element**</span></span>|<span data-ttu-id="97fb8-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="97fb8-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="97fb8-115">出席者</span><span class="sxs-lookup"><span data-stu-id="97fb8-115">Attendee</span></span>](attendee.md) <br/> |<span data-ttu-id="97fb8-116">会議の出席者とリソースを表します。</span><span class="sxs-lookup"><span data-stu-id="97fb8-116">Represents attendees and resources for a meeting.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="97fb8-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="97fb8-117">Text value</span></span>

<span data-ttu-id="97fb8-118">最新の応答の日付と時刻を表すテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="97fb8-118">A text value that represents the date and time of the latest response is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="97fb8-119">注釈</span><span class="sxs-lookup"><span data-stu-id="97fb8-119">Remarks</span></span>

<span data-ttu-id="97fb8-120">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="97fb8-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="97fb8-121">要素の情報</span><span class="sxs-lookup"><span data-stu-id="97fb8-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="97fb8-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="97fb8-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="97fb8-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="97fb8-123">Schema name</span></span>  <br/> |<span data-ttu-id="97fb8-124">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="97fb8-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="97fb8-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="97fb8-125">Validation file</span></span>  <br/> |<span data-ttu-id="97fb8-126">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="97fb8-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="97fb8-127">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="97fb8-127">Can be empty</span></span>  <br/> |<span data-ttu-id="97fb8-128">正しくない</span><span class="sxs-lookup"><span data-stu-id="97fb8-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="97fb8-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="97fb8-129">See also</span></span>



- [<span data-ttu-id="97fb8-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="97fb8-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

