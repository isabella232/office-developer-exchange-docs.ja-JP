---
title: ReminderMessageData
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 04dd4987-baaf-4ebe-ae58-ad962c2f8fa1
description: ReminderMessageData 要素は、アラームメッセージのデータを指定します。
ms.openlocfilehash: f2632062cd02581c426f7dbfa2a33d53e5594d72
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458552"
---
# <a name="remindermessagedata"></a><span data-ttu-id="8dbf0-103">ReminderMessageData</span><span class="sxs-lookup"><span data-stu-id="8dbf0-103">ReminderMessageData</span></span>

<span data-ttu-id="8dbf0-104">**ReminderMessageData**要素は、アラームメッセージのデータを指定します。</span><span class="sxs-lookup"><span data-stu-id="8dbf0-104">The **ReminderMessageData** element specifies the data in a reminder message.</span></span> 
  
```XML
<ReminderMessageData>
   <ReminderText></ReminderText>
   <Location></Location>
   <StartTime></StartTime>
   <EndTime></EndTime>
   <AssociatedCalendarItemId></AssociatedCalendarItemId>
</ReminderMessageData>

```

 <span data-ttu-id="8dbf0-105">**ReminderMessageDataType**</span><span class="sxs-lookup"><span data-stu-id="8dbf0-105">**ReminderMessageDataType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8dbf0-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="8dbf0-106">Attributes and elements</span></span>

<span data-ttu-id="8dbf0-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8dbf0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8dbf0-108">属性</span><span class="sxs-lookup"><span data-stu-id="8dbf0-108">Attributes</span></span>

<span data-ttu-id="8dbf0-109">なし。</span><span class="sxs-lookup"><span data-stu-id="8dbf0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8dbf0-110">子要素</span><span class="sxs-lookup"><span data-stu-id="8dbf0-110">Child elements</span></span>

<span data-ttu-id="8dbf0-111">[ReminderText](remindertext.md)  | [場所](location.md)  | [StartTime (ReminderMessageDataType)](starttime-remindermessagedatatype.md)  | [EndTime (ReminderMessageDataType)](endtime-remindermessagedatatype.md)  | [AssociatedCalendarItemId](associatedcalendaritemid.md)</span><span class="sxs-lookup"><span data-stu-id="8dbf0-111">[ReminderText](remindertext.md) | [Location](location.md) | [StartTime (ReminderMessageDataType)](starttime-remindermessagedatatype.md) | [EndTime (ReminderMessageDataType)](endtime-remindermessagedatatype.md) | [AssociatedCalendarItemId](associatedcalendaritemid.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8dbf0-112">親要素</span><span class="sxs-lookup"><span data-stu-id="8dbf0-112">Parent elements</span></span>

[<span data-ttu-id="8dbf0-113">Message</span><span class="sxs-lookup"><span data-stu-id="8dbf0-113">Message</span></span>](message-ex15websvcsotherref.md)
  
## <a name="remarks"></a><span data-ttu-id="8dbf0-114">注釈</span><span class="sxs-lookup"><span data-stu-id="8dbf0-114">Remarks</span></span>

<span data-ttu-id="8dbf0-115">この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="8dbf0-115">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="8dbf0-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="8dbf0-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="8dbf0-117">ビルド番号15.00.0913.09 以降のバージョンの Exchange では、 **ReminderMessageData**要素の子要素として**AssociatedCalendarItemId**要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="8dbf0-117">Versions of Exchange starting with build number 15.00.0913.09 can include the **AssociatedCalendarItemId** element as a child element of the **ReminderMessageData** element.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="8dbf0-118">要素の情報</span><span class="sxs-lookup"><span data-stu-id="8dbf0-118">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8dbf0-119">Namespace</span><span class="sxs-lookup"><span data-stu-id="8dbf0-119">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8dbf0-120">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8dbf0-120">Schema Name</span></span>  <br/> |<span data-ttu-id="8dbf0-121">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="8dbf0-121">Types schema</span></span>  <br/> |
|<span data-ttu-id="8dbf0-122">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8dbf0-122">Validation File</span></span>  <br/> |<span data-ttu-id="8dbf0-123">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="8dbf0-123">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8dbf0-124">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="8dbf0-124">Can be Empty</span></span>  <br/> |<span data-ttu-id="8dbf0-125">正しい</span><span class="sxs-lookup"><span data-stu-id="8dbf0-125">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8dbf0-126">関連項目</span><span class="sxs-lookup"><span data-stu-id="8dbf0-126">See also</span></span>



[<span data-ttu-id="8dbf0-127">Message</span><span class="sxs-lookup"><span data-stu-id="8dbf0-127">Message</span></span>](message-ex15websvcsotherref.md)


- [<span data-ttu-id="8dbf0-128">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="8dbf0-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

