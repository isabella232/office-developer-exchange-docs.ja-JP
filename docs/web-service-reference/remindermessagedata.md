---
title: ReminderMessageData
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 04dd4987-baaf-4ebe-ae58-ad962c2f8fa1
description: ReminderMessageData 要素は、アラーム メッセージのデータを指定します。
ms.openlocfilehash: a1d01dd24030b047bd8ad025f3e1cebed0da8e29
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833067"
---
# <a name="remindermessagedata"></a><span data-ttu-id="ea740-103">ReminderMessageData</span><span class="sxs-lookup"><span data-stu-id="ea740-103">ReminderMessageData</span></span>

<span data-ttu-id="ea740-104">**ReminderMessageData**要素は、アラーム メッセージのデータを指定します。</span><span class="sxs-lookup"><span data-stu-id="ea740-104">The **ReminderMessageData** element specifies the data in a reminder message.</span></span> 
  
```XML
<ReminderMessageData>
   <ReminderText></ReminderText>
   <Location></Location>
   <StartTime></StartTime>
   <EndTime></EndTime>
   <AssociatedCalendarItemId></AssociatedCalendarItemId>
</ReminderMessageData>

```

 <span data-ttu-id="ea740-105">**ReminderMessageDataType**</span><span class="sxs-lookup"><span data-stu-id="ea740-105">**ReminderMessageDataType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ea740-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="ea740-106">Attributes and elements</span></span>

<span data-ttu-id="ea740-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ea740-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ea740-108">属性</span><span class="sxs-lookup"><span data-stu-id="ea740-108">Attributes</span></span>

<span data-ttu-id="ea740-109">なし。</span><span class="sxs-lookup"><span data-stu-id="ea740-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ea740-110">子要素</span><span class="sxs-lookup"><span data-stu-id="ea740-110">Child elements</span></span>

<span data-ttu-id="ea740-111">[ReminderText](remindertext.md) | [の場所](location.md) | [開始時刻 (ReminderMessageDataType)](starttime-remindermessagedatatype.md) | [終了時刻 (ReminderMessageDataType)](endtime-remindermessagedatatype.md) | [AssociatedCalendarItemId](associatedcalendaritemid.md)</span><span class="sxs-lookup"><span data-stu-id="ea740-111">[ReminderText](remindertext.md) | [Location](location.md) | [StartTime (ReminderMessageDataType)](starttime-remindermessagedatatype.md) | [EndTime (ReminderMessageDataType)](endtime-remindermessagedatatype.md) | [AssociatedCalendarItemId](associatedcalendaritemid.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ea740-112">親要素</span><span class="sxs-lookup"><span data-stu-id="ea740-112">Parent elements</span></span>

[<span data-ttu-id="ea740-113">Message</span><span class="sxs-lookup"><span data-stu-id="ea740-113">Message</span></span>](message-ex15websvcsotherref.md)
  
## <a name="remarks"></a><span data-ttu-id="ea740-114">備考</span><span class="sxs-lookup"><span data-stu-id="ea740-114">Remarks</span></span>

<span data-ttu-id="ea740-115">この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="ea740-115">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="ea740-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="ea740-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="ea740-117">Exchange のビルド番号 15.00.0913.09 以降のバージョンでは、 **ReminderMessageData**要素の子要素として**AssociatedCalendarItemId**の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="ea740-117">Versions of Exchange starting with build number 15.00.0913.09 can include the **AssociatedCalendarItemId** element as a child element of the **ReminderMessageData** element.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="ea740-118">要素情報</span><span class="sxs-lookup"><span data-stu-id="ea740-118">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ea740-119">名前空間</span><span class="sxs-lookup"><span data-stu-id="ea740-119">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ea740-120">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ea740-120">Schema Name</span></span>  <br/> |<span data-ttu-id="ea740-121">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="ea740-121">Types schema</span></span>  <br/> |
|<span data-ttu-id="ea740-122">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ea740-122">Validation File</span></span>  <br/> |<span data-ttu-id="ea740-123">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ea740-123">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ea740-124">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="ea740-124">Can be Empty</span></span>  <br/> |<span data-ttu-id="ea740-125">True</span><span class="sxs-lookup"><span data-stu-id="ea740-125">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ea740-126">関連項目</span><span class="sxs-lookup"><span data-stu-id="ea740-126">See also</span></span>



[<span data-ttu-id="ea740-127">Message</span><span class="sxs-lookup"><span data-stu-id="ea740-127">Message</span></span>](message-ex15websvcsotherref.md)


- [<span data-ttu-id="ea740-128">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="ea740-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

