---
title: Duration (UserOofSettings)
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
description: Duration 要素は、OofState 要素が [スケジュール済み] に設定されている場合に、不在時 (OOF) の状態が有効である期間を指定します。
ms.openlocfilehash: 0ba0f1ea7498781c0cccb072c7ea0fa05414764c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457299"
---
# <a name="duration-useroofsettings"></a><span data-ttu-id="cb01d-103">Duration (UserOofSettings)</span><span class="sxs-lookup"><span data-stu-id="cb01d-103">Duration (UserOofSettings)</span></span>

<span data-ttu-id="cb01d-104">**Duration**要素は、 [oofstate](oofstate.md)要素が [**スケジュール済み**] に設定されている場合に、不在時 (OOF) の状態が有効である期間を指定します。</span><span class="sxs-lookup"><span data-stu-id="cb01d-104">The **Duration** element specifies the duration that the out of office (OOF) status is enabled if the [OofState](oofstate.md) element is set to **Scheduled**.</span></span>
  
```XML
<Duration>
   <StartTime/>
   <EndTime/> 
</Duration>
```

 <span data-ttu-id="cb01d-105">**Duration**</span><span class="sxs-lookup"><span data-stu-id="cb01d-105">**Duration**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cb01d-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="cb01d-106">Attributes and elements</span></span>

<span data-ttu-id="cb01d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="cb01d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cb01d-108">属性</span><span class="sxs-lookup"><span data-stu-id="cb01d-108">Attributes</span></span>

<span data-ttu-id="cb01d-109">なし。</span><span class="sxs-lookup"><span data-stu-id="cb01d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cb01d-110">子要素</span><span class="sxs-lookup"><span data-stu-id="cb01d-110">Child elements</span></span>

|<span data-ttu-id="cb01d-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="cb01d-111">**Element**</span></span>|<span data-ttu-id="cb01d-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="cb01d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cb01d-113">StartTime</span><span class="sxs-lookup"><span data-stu-id="cb01d-113">StartTime</span></span>](starttime.md) <br/> |<span data-ttu-id="cb01d-114">OOF 状態で設定された時間間隔の開始を表します。</span><span class="sxs-lookup"><span data-stu-id="cb01d-114">Represents the start of the time span set with an OOF status.</span></span> <span data-ttu-id="cb01d-115">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="cb01d-115">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="cb01d-116">EndTime</span><span class="sxs-lookup"><span data-stu-id="cb01d-116">EndTime</span></span>](endtime.md) <br/> |<span data-ttu-id="cb01d-117">不在時の状態で設定された時間間隔の最後の部分を表します。</span><span class="sxs-lookup"><span data-stu-id="cb01d-117">Represents the end of the time span set with an OOF status.</span></span> <span data-ttu-id="cb01d-118">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="cb01d-118">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cb01d-119">親要素</span><span class="sxs-lookup"><span data-stu-id="cb01d-119">Parent elements</span></span>

|<span data-ttu-id="cb01d-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="cb01d-120">**Element**</span></span>|<span data-ttu-id="cb01d-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="cb01d-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cb01d-122">UserOofSettings</span><span class="sxs-lookup"><span data-stu-id="cb01d-122">UserOofSettings</span></span>](useroofsettings.md) <br/> |<span data-ttu-id="cb01d-123">OOF 設定を指定します。</span><span class="sxs-lookup"><span data-stu-id="cb01d-123">Specifies the OOF settings.</span></span>  <br/><br/><span data-ttu-id="cb01d-124">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cb01d-124">The following is the XPath expression to this element:</span></span><br/><br/>`/SetUserOofSettingsRequest/UserOofSettings` <br/> |
|[<span data-ttu-id="cb01d-125">OofSettings</span><span class="sxs-lookup"><span data-stu-id="cb01d-125">OofSettings</span></span>](oofsettings.md) <br/> |<span data-ttu-id="cb01d-126">不在時の設定が含まれます。</span><span class="sxs-lookup"><span data-stu-id="cb01d-126">Contains the OOF settings.</span></span><br/><br/><span data-ttu-id="cb01d-127">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cb01d-127">The following is the XPath expression to this element:</span></span><br/><br/>`/GetUserOofSettingsResponse/OofSettings` <br/> |
|[<span data-ttu-id="cb01d-128">不在</span><span class="sxs-lookup"><span data-stu-id="cb01d-128">OutOfOffice</span></span>](outofoffice.md) <br/> |<span data-ttu-id="cb01d-129">不在 (OOF) 応答メッセージと、メールボックスの応答メッセージを送信する時間を定義します。</span><span class="sxs-lookup"><span data-stu-id="cb01d-129">Defines the Out of Office (OOF) response message and a duration time for sending the response message for a mailbox.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="cb01d-130">注釈</span><span class="sxs-lookup"><span data-stu-id="cb01d-130">Remarks</span></span>

<span data-ttu-id="cb01d-131">**期間**の種類は、 [DetailedSuggestionsWindow](detailedsuggestionswindow.md)、 [TimeWindow](timewindow.md)、および[不在](outofoffice.md)要素の型でもあります。</span><span class="sxs-lookup"><span data-stu-id="cb01d-131">The **Duration** type is also the type for the [DetailedSuggestionsWindow](detailedsuggestionswindow.md), [TimeWindow](timewindow.md), and [OutOfOffice](outofoffice.md) elements.</span></span> 
  
<span data-ttu-id="cb01d-132">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="cb01d-132">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="example"></a><span data-ttu-id="cb01d-133">例</span><span class="sxs-lookup"><span data-stu-id="cb01d-133">Example</span></span>

<span data-ttu-id="cb01d-134">[Setuseroofsettings 操作](setuseroofsettings-operation.md)要求の次の例では、 [Oofstate](oofstate.md)を**有効**にし、内部および外部の OOF メッセージを設定し、不在時の時間を10日間に設定します。</span><span class="sxs-lookup"><span data-stu-id="cb01d-134">The following example of a [SetUserOofSettings operation](setuseroofsettings-operation.md) request sets the [OofState](oofstate.md) to **Enabled**, the internal and external OOF messages, and sets the duration of OOF for 10 days.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetUserOofSettingsRequest xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <Mailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
        <Name>David Alexander</Name>
        <Address>someone@example.com</Address>
        <RoutingType>SMTP</RoutingType>
      </Mailbox>
      <UserOofSettings xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="element-information"></a><span data-ttu-id="cb01d-135">要素の情報</span><span class="sxs-lookup"><span data-stu-id="cb01d-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cb01d-136">Namespace</span><span class="sxs-lookup"><span data-stu-id="cb01d-136">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cb01d-137">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="cb01d-137">Schema Name</span></span>  <br/> |<span data-ttu-id="cb01d-138">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="cb01d-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="cb01d-139">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="cb01d-139">Validation File</span></span>  <br/> |<span data-ttu-id="cb01d-140">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="cb01d-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="cb01d-141">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="cb01d-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="cb01d-142">正しくない</span><span class="sxs-lookup"><span data-stu-id="cb01d-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cb01d-143">関連項目</span><span class="sxs-lookup"><span data-stu-id="cb01d-143">See also</span></span>

- [<span data-ttu-id="cb01d-144">GetUserOofSettings 操作</span><span class="sxs-lookup"><span data-stu-id="cb01d-144">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)  
- [<span data-ttu-id="cb01d-145">SetUserOofSettings 操作</span><span class="sxs-lookup"><span data-stu-id="cb01d-145">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

