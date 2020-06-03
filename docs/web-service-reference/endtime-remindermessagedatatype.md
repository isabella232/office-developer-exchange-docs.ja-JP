---
title: EndTime (ReminderMessageDataType)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 771dce9c-17a7-4c1d-aab2-47b6dd48d795
description: EndTime 要素は、事前通知に対してクエリを実行する時間間隔の終わりを表します。
ms.openlocfilehash: 7a9eac48970d193a1a55a9e4c7934aad56058190
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459659"
---
# <a name="endtime-remindermessagedatatype"></a><span data-ttu-id="cbf0b-103">EndTime (ReminderMessageDataType)</span><span class="sxs-lookup"><span data-stu-id="cbf0b-103">EndTime (ReminderMessageDataType)</span></span>

<span data-ttu-id="cbf0b-104">**EndTime**要素は、事前通知に対してクエリを実行する時間間隔の終わりを表します。</span><span class="sxs-lookup"><span data-stu-id="cbf0b-104">The **EndTime** element represents the end of the time span to query for reminders.</span></span> 
  
```XML
<EndTime/>
```

 <span data-ttu-id="cbf0b-105">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="cbf0b-105">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cbf0b-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="cbf0b-106">Attributes and elements</span></span>

<span data-ttu-id="cbf0b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="cbf0b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cbf0b-108">属性</span><span class="sxs-lookup"><span data-stu-id="cbf0b-108">Attributes</span></span>

<span data-ttu-id="cbf0b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="cbf0b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cbf0b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="cbf0b-110">Child elements</span></span>

<span data-ttu-id="cbf0b-111">なし。</span><span class="sxs-lookup"><span data-stu-id="cbf0b-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="cbf0b-112">親要素</span><span class="sxs-lookup"><span data-stu-id="cbf0b-112">Parent elements</span></span>

[<span data-ttu-id="cbf0b-113">ReminderMessageData</span><span class="sxs-lookup"><span data-stu-id="cbf0b-113">ReminderMessageData</span></span>](remindermessagedata.md)
  
## <a name="text-value"></a><span data-ttu-id="cbf0b-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="cbf0b-114">Text value</span></span>

<span data-ttu-id="cbf0b-115">**EndTime**要素のテキスト値は、事前通知に対してクエリを実行する時間間隔の最後を表します。</span><span class="sxs-lookup"><span data-stu-id="cbf0b-115">The text value of the **EndTime** element represents the end of the time span to query for reminders.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="cbf0b-116">注釈</span><span class="sxs-lookup"><span data-stu-id="cbf0b-116">Remarks</span></span>

<span data-ttu-id="cbf0b-117">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="cbf0b-117">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="cbf0b-118">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="cbf0b-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cbf0b-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="cbf0b-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cbf0b-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="cbf0b-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cbf0b-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="cbf0b-121">Schema Name</span></span>  <br/> |<span data-ttu-id="cbf0b-122">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="cbf0b-122">Types schema</span></span>  <br/> |
|<span data-ttu-id="cbf0b-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="cbf0b-123">Validation File</span></span>  <br/> |<span data-ttu-id="cbf0b-124">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="cbf0b-124">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="cbf0b-125">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="cbf0b-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="cbf0b-126">正しくない</span><span class="sxs-lookup"><span data-stu-id="cbf0b-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cbf0b-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="cbf0b-127">See also</span></span>



[<span data-ttu-id="cbf0b-128">ReminderMessageData</span><span class="sxs-lookup"><span data-stu-id="cbf0b-128">ReminderMessageData</span></span>](remindermessagedata.md)


- [<span data-ttu-id="cbf0b-129">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="cbf0b-129">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

