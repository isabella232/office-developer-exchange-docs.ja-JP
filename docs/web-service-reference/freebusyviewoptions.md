---
title: FreeBusyViewOptions
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FreeBusyViewOptions
api_type:
- schema
ms.assetid: c07f3ddb-874b-4d30-a60e-7e5c7793bb6f
description: FreeBusyViewOptions 要素は、応答で返される空き時間情報の情報の種類を指定します。
ms.openlocfilehash: 703fc6a3625d24cf874a785600e13ee4505b506f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760605"
---
# <a name="freebusyviewoptions"></a><span data-ttu-id="f3dc2-103">FreeBusyViewOptions</span><span class="sxs-lookup"><span data-stu-id="f3dc2-103">FreeBusyViewOptions</span></span>

<span data-ttu-id="f3dc2-104">**FreeBusyViewOptions**要素は、応答で返される空き時間情報の情報の種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="f3dc2-104">The **FreeBusyViewOptions** element specifies the type of free/busy information returned in the response.</span></span> 
  
[<span data-ttu-id="f3dc2-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="f3dc2-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="f3dc2-106">FreeBusyViewOptions</span><span class="sxs-lookup"><span data-stu-id="f3dc2-106">FreeBusyViewOptions</span></span>](freebusyviewoptions.md)
  
```xml
<FreeBusyViewOptions>
   <TimeWindow>...</TimeWindow>
   <MergedFreeBusyIntervalInMinutes>...</MergedFreeBusyIntervalInMinutes>
<RequestedView>...</RequestedView>
</FreeBusyViewOptions>

```

 <span data-ttu-id="f3dc2-107">**FreeBusyViewOptionsType**</span><span class="sxs-lookup"><span data-stu-id="f3dc2-107">**FreeBusyViewOptionsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f3dc2-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="f3dc2-108">Attributes and elements</span></span>

<span data-ttu-id="f3dc2-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f3dc2-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f3dc2-110">属性</span><span class="sxs-lookup"><span data-stu-id="f3dc2-110">Attributes</span></span>

<span data-ttu-id="f3dc2-111">なし。</span><span class="sxs-lookup"><span data-stu-id="f3dc2-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f3dc2-112">子要素</span><span class="sxs-lookup"><span data-stu-id="f3dc2-112">Child elements</span></span>

|<span data-ttu-id="f3dc2-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="f3dc2-113">**Element**</span></span>|<span data-ttu-id="f3dc2-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="f3dc2-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f3dc2-115">時間</span><span class="sxs-lookup"><span data-stu-id="f3dc2-115">TimeWindow</span></span>](timewindow.md) <br/> |<span data-ttu-id="f3dc2-116">ユーザーの可用性について照会する期間を指定します。</span><span class="sxs-lookup"><span data-stu-id="f3dc2-116">Identifies the time span queried for the user availability information.</span></span>  <br/> |
|[<span data-ttu-id="f3dc2-117">MergedFreeBusyIntervalInMinutes</span><span class="sxs-lookup"><span data-stu-id="f3dc2-117">MergedFreeBusyIntervalInMinutes</span></span>](mergedfreebusyintervalinminutes.md) <br/> |<span data-ttu-id="f3dc2-118">**FreeBusyMerged**ビューで連続する 2 つのスロット間の時間差を表します。</span><span class="sxs-lookup"><span data-stu-id="f3dc2-118">Represents the time difference between two successive slots in the **FreeBusyMerged** view.</span></span>  <br/> |
|[<span data-ttu-id="f3dc2-119">RequestedView</span><span class="sxs-lookup"><span data-stu-id="f3dc2-119">RequestedView</span></span>](requestedview.md) <br/> |<span data-ttu-id="f3dc2-120">クライアントが要求する予定表の情報の種類を定義します。</span><span class="sxs-lookup"><span data-stu-id="f3dc2-120">Defines the type of calendar information that a client requests.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f3dc2-121">親要素</span><span class="sxs-lookup"><span data-stu-id="f3dc2-121">Parent elements</span></span>

|<span data-ttu-id="f3dc2-122">**要素**</span><span class="sxs-lookup"><span data-stu-id="f3dc2-122">**Element**</span></span>|<span data-ttu-id="f3dc2-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="f3dc2-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f3dc2-124">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="f3dc2-124">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md) <br/> |<span data-ttu-id="f3dc2-125">ユーザーの利用可能時間情報を取得するための引数が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f3dc2-125">Contains the arguments used to obtain user availability information.</span></span> <span data-ttu-id="f3dc2-126">これは、ルート要素です。</span><span class="sxs-lookup"><span data-stu-id="f3dc2-126">This is a root element.</span></span>  <br/> <span data-ttu-id="f3dc2-127">以下は、この要素の XPath です。</span><span class="sxs-lookup"><span data-stu-id="f3dc2-127">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f3dc2-128">備考</span><span class="sxs-lookup"><span data-stu-id="f3dc2-128">Remarks</span></span>

<span data-ttu-id="f3dc2-129">この要素は必須ではなく、発生は一度のみを使用する場合。</span><span class="sxs-lookup"><span data-stu-id="f3dc2-129">This element is not required and can only occur once if used.</span></span> <span data-ttu-id="f3dc2-130">[SuggestionsViewOptions](suggestionsviewoptions.md)要素の値が null でない場合、この値を null にすることができます。</span><span class="sxs-lookup"><span data-stu-id="f3dc2-130">This value can be null if the value of the [SuggestionsViewOptions](suggestionsviewoptions.md) element is not null.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="f3dc2-131">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft® Exchange Server 2007 を実行しているコンピューターの/epi/ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="f3dc2-131">The schema that describes this element is located in the /epi/ directory of the computer that is running Microsoft® Exchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="example"></a><span data-ttu-id="f3dc2-132">例</span><span class="sxs-lookup"><span data-stu-id="f3dc2-132">Example</span></span>

<span data-ttu-id="f3dc2-133">次の例では、会議や 60 分間隔で空き/予約済みのストリームの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="f3dc2-133">The following example obtains a list of meetings and a free/busy stream in 60-minute intervals.</span></span>
  
```
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <GetUserAvailabilityRequest xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <TimeZone xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
        <Bias>480</Bias>
        <StandardTime>
          <Bias>0</Bias>
          <Time>02:00:00</Time>
          <DayOrder>5</DayOrder>
          <Month>10</Month>
          <DayOfWeek>Sunday</DayOfWeek>
        </StandardTime>
        <DaylightTime>
          <Bias>-60</Bias>
          <Time>02:00:00</Time>
          <DayOrder>1</DayOrder>
          <Month>4</Month>
          <DayOfWeek>Sunday</DayOfWeek>
        </DaylightTime>
      </TimeZone>
      <MailboxDataArray>
        <MailboxData xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <Email>
            <Name></Name>
            <Address>someone@ExServer.example.com</Address>
            <RoutingType>SMTP</RoutingType>
          </Email>
          <AttendeeType>Organizer</AttendeeType>
          <ExcludeConflicts>false</ExcludeConflicts>
          <ExcludeNonWorkingHours>false</ExcludeNonWorkingHours>
        </MailboxData>
      </MailboxDataArray>
      <FreeBusyViewOptions xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
        <TimeWindow>
          <StartTime>2006-02-06T00:00:00</StartTime>
          <EndTime>2006-02-25T23:59:59</EndTime>
        </TimeWindow>
        <MergedFreeBusyIntervalInMinutes>60</MergedFreeBusyIntervalInMinutes>
        <RequestedView>FreeBusyMerged</RequestedView>
      </FreeBusyViewOptions>
    </GetUserAvailabilityRequest>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a><span data-ttu-id="f3dc2-134">要素情報</span><span class="sxs-lookup"><span data-stu-id="f3dc2-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f3dc2-135">名前空間</span><span class="sxs-lookup"><span data-stu-id="f3dc2-135">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f3dc2-136">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f3dc2-136">Schema Name</span></span>  <br/> |<span data-ttu-id="f3dc2-137">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="f3dc2-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="f3dc2-138">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f3dc2-138">Validation File</span></span>  <br/> |<span data-ttu-id="f3dc2-139">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f3dc2-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f3dc2-140">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="f3dc2-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="f3dc2-141">False</span><span class="sxs-lookup"><span data-stu-id="f3dc2-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f3dc2-142">関連項目</span><span class="sxs-lookup"><span data-stu-id="f3dc2-142">See also</span></span>



[<span data-ttu-id="f3dc2-143">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="f3dc2-143">GetUserAvailability operation</span></span>](getuseravailability-operation.md)


[<span data-ttu-id="f3dc2-144">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="f3dc2-144">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

