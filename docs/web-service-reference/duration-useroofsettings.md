---
title: 期間 (UserOofSettings)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Duration
api_type:
- schema
ms.assetid: 01d67af3-658e-4acd-93e3-441ae827fdd3
description: 期間要素は、OofState 要素は、[スケジュール済] に設定されている場合に、不在 (oof) の状態が有効になっている期間を指定します。
ms.openlocfilehash: 62a5492372fd80173d58e965376b7c8c466825a6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760177"
---
# <a name="duration-useroofsettings"></a><span data-ttu-id="aa626-103">期間 (UserOofSettings)</span><span class="sxs-lookup"><span data-stu-id="aa626-103">Duration (UserOofSettings)</span></span>

<span data-ttu-id="aa626-104">**期間**要素は、 [OofState](oofstate.md)要素は、**スケジュール**に設定されている場合に、不在 (oof) の状態が有効になっている期間を指定します。</span><span class="sxs-lookup"><span data-stu-id="aa626-104">The **Duration** element specifies the duration that the out of office (OOF) status is enabled if the [OofState](oofstate.md) element is set to **Scheduled**.</span></span>
  
```XML
<Duration>
   <StartTime/>
   <EndTime/> 
</Duration>
```

 <span data-ttu-id="aa626-105">**Duration**</span><span class="sxs-lookup"><span data-stu-id="aa626-105">**Duration**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="aa626-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="aa626-106">Attributes and elements</span></span>

<span data-ttu-id="aa626-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="aa626-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="aa626-108">属性</span><span class="sxs-lookup"><span data-stu-id="aa626-108">Attributes</span></span>

<span data-ttu-id="aa626-109">なし。</span><span class="sxs-lookup"><span data-stu-id="aa626-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="aa626-110">子要素</span><span class="sxs-lookup"><span data-stu-id="aa626-110">Child elements</span></span>

|<span data-ttu-id="aa626-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="aa626-111">**Element**</span></span>|<span data-ttu-id="aa626-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="aa626-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aa626-113">開始時刻</span><span class="sxs-lookup"><span data-stu-id="aa626-113">StartTime</span></span>](starttime.md) <br/> |<span data-ttu-id="aa626-114">不在の状態を設定する期間の開始を表します。</span><span class="sxs-lookup"><span data-stu-id="aa626-114">Represents the start of the time span set with an OOF status.</span></span> <span data-ttu-id="aa626-115">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="aa626-115">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="aa626-116">終了時刻</span><span class="sxs-lookup"><span data-stu-id="aa626-116">EndTime</span></span>](endtime.md) <br/> |<span data-ttu-id="aa626-117">不在の状態を設定する、時間の終了を表します。</span><span class="sxs-lookup"><span data-stu-id="aa626-117">Represents the end of the time span set with an OOF status.</span></span> <span data-ttu-id="aa626-118">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="aa626-118">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="aa626-119">親要素</span><span class="sxs-lookup"><span data-stu-id="aa626-119">Parent elements</span></span>

|<span data-ttu-id="aa626-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="aa626-120">**Element**</span></span>|<span data-ttu-id="aa626-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="aa626-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aa626-122">UserOofSettings</span><span class="sxs-lookup"><span data-stu-id="aa626-122">UserOofSettings</span></span>](useroofsettings.md) <br/> |<span data-ttu-id="aa626-123">不在の設定を指定します。</span><span class="sxs-lookup"><span data-stu-id="aa626-123">Specifies the OOF settings.</span></span>  <br/><br/><span data-ttu-id="aa626-124">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="aa626-124">The following is the XPath expression to this element:</span></span><br/><br/>`/SetUserOofSettingsRequest/UserOofSettings` <br/> |
|[<span data-ttu-id="aa626-125">OofSettings</span><span class="sxs-lookup"><span data-stu-id="aa626-125">OofSettings</span></span>](oofsettings.md) <br/> |<span data-ttu-id="aa626-126">不在の設定が含まれています。</span><span class="sxs-lookup"><span data-stu-id="aa626-126">Contains the OOF settings.</span></span><br/><br/><span data-ttu-id="aa626-127">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="aa626-127">The following is the XPath expression to this element:</span></span><br/><br/>`/GetUserOofSettingsResponse/OofSettings` <br/> |
|[<span data-ttu-id="aa626-128">OutOfOffice</span><span class="sxs-lookup"><span data-stu-id="aa626-128">OutOfOffice</span></span>](outofoffice.md) <br/> |<span data-ttu-id="aa626-129">Office (OOF) の応答メッセージとメールボックスの応答メッセージを送信するための継続時間を定義します。</span><span class="sxs-lookup"><span data-stu-id="aa626-129">Defines the Out of Office (OOF) response message and a duration time for sending the response message for a mailbox.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="aa626-130">備考</span><span class="sxs-lookup"><span data-stu-id="aa626-130">Remarks</span></span>

<span data-ttu-id="aa626-131">**期間**タイプが[DetailedSuggestionsWindow](detailedsuggestionswindow.md)、[時間](timewindow.md)、および[OutOfOffice](outofoffice.md)の要素の型もあります。</span><span class="sxs-lookup"><span data-stu-id="aa626-131">The **Duration** type is also the type for the [DetailedSuggestionsWindow](detailedsuggestionswindow.md), [TimeWindow](timewindow.md), and [OutOfOffice](outofoffice.md) elements.</span></span> 
  
<span data-ttu-id="aa626-132">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="aa626-132">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="example"></a><span data-ttu-id="aa626-133">例</span><span class="sxs-lookup"><span data-stu-id="aa626-133">Example</span></span>

<span data-ttu-id="aa626-134">[SetUserOofSettings 操作](setuseroofsettings-operation.md)要求の次の例では、**有効**、内部と外部の OOF メッセージを[OofState](oofstate.md)を設定し、10 日間の不在時の期間を設定します。</span><span class="sxs-lookup"><span data-stu-id="aa626-134">The following example of a [SetUserOofSettings operation](setuseroofsettings-operation.md) request sets the [OofState](oofstate.md) to **Enabled**, the internal and external OOF messages, and sets the duration of OOF for 10 days.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetUserOofSettingsRequest xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <Mailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
        <Name>David Alexander</Name>
        <Address>someone@example.com</Address>
        <RoutingType>SMTP</RoutingType>
      </Mailbox>
      <UserOofSettings xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
        <OofState>Enabled</OofState>
        <ExternalAudience>All</ExternalAudience>
        <Duration>
          <StartTime>2005-10-05T00:00:00</StartTime>
          <EndTime>2005-10-25T00:00:00</EndTime>
        </Duration>
        <InternalReply>
          <Message>I am out of office.  This is my internal reply.</Message>
        </InternalReply>
        <ExternalReply>
          <Message>I am out of office. This is my external reply.</Message>
        </ExternalReply>
        <SetByLegacyClient>false</SetByLegacyClient>
      </UserOofSettings>
    </SetUserOofSettingsRequest>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a><span data-ttu-id="aa626-135">要素情報</span><span class="sxs-lookup"><span data-stu-id="aa626-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="aa626-136">名前空間</span><span class="sxs-lookup"><span data-stu-id="aa626-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="aa626-137">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="aa626-137">Schema Name</span></span>  <br/> |<span data-ttu-id="aa626-138">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="aa626-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="aa626-139">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="aa626-139">Validation File</span></span>  <br/> |<span data-ttu-id="aa626-140">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="aa626-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="aa626-141">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="aa626-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="aa626-142">False</span><span class="sxs-lookup"><span data-stu-id="aa626-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="aa626-143">関連項目</span><span class="sxs-lookup"><span data-stu-id="aa626-143">See also</span></span>

- [<span data-ttu-id="aa626-144">GetUserOofSettings 操作</span><span class="sxs-lookup"><span data-stu-id="aa626-144">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)  
- [<span data-ttu-id="aa626-145">SetUserOofSettings 操作</span><span class="sxs-lookup"><span data-stu-id="aa626-145">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

