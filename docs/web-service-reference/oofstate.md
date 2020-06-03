---
title: OofState
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OofState
api_type:
- schema
ms.assetid: 3c486a38-06da-4382-ad20-664d067d76ac
description: OofState 要素は、ユーザーの不在時 (OOF) の状態を取得または設定するために使用されます。
ms.openlocfilehash: 6aef7d989ee6978019a483f2673895e68a88a7c5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459736"
---
# <a name="oofstate"></a><span data-ttu-id="3159d-103">OofState</span><span class="sxs-lookup"><span data-stu-id="3159d-103">OofState</span></span>

<span data-ttu-id="3159d-104">**Oofstate**要素は、ユーザーの不在時 (OOF) の状態を取得または設定するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="3159d-104">The **OofState** element is used to get or set the user's Out of Office (OOF) state.</span></span> 
  
```xml
<OofState>Disabled or Enabled or Scheduled</OofState>
```

 <span data-ttu-id="3159d-105">**OofState**</span><span class="sxs-lookup"><span data-stu-id="3159d-105">**OofState**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3159d-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="3159d-106">Attributes and elements</span></span>

<span data-ttu-id="3159d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3159d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3159d-108">属性</span><span class="sxs-lookup"><span data-stu-id="3159d-108">Attributes</span></span>

<span data-ttu-id="3159d-109">なし。</span><span class="sxs-lookup"><span data-stu-id="3159d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3159d-110">子要素</span><span class="sxs-lookup"><span data-stu-id="3159d-110">Child elements</span></span>

<span data-ttu-id="3159d-111">なし。</span><span class="sxs-lookup"><span data-stu-id="3159d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3159d-112">親要素</span><span class="sxs-lookup"><span data-stu-id="3159d-112">Parent elements</span></span>

|<span data-ttu-id="3159d-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="3159d-113">**Element**</span></span>|<span data-ttu-id="3159d-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="3159d-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3159d-115">UserOofSettings</span><span class="sxs-lookup"><span data-stu-id="3159d-115">UserOofSettings</span></span>](useroofsettings.md) <br/> |<span data-ttu-id="3159d-116">OOF 設定を指定します。</span><span class="sxs-lookup"><span data-stu-id="3159d-116">Specifies the OOF settings.</span></span>  <br/> <span data-ttu-id="3159d-117">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3159d-117">The following is the XPath expression to this element:</span></span>  <br/>  `/SetUserOofSettingsRequest/UserOofSettings` <br/> |
|[<span data-ttu-id="3159d-118">OofSettings</span><span class="sxs-lookup"><span data-stu-id="3159d-118">OofSettings</span></span>](oofsettings.md) <br/> |<span data-ttu-id="3159d-119">不在時の設定が含まれます。</span><span class="sxs-lookup"><span data-stu-id="3159d-119">Contains the OOF settings.</span></span>  <br/> <span data-ttu-id="3159d-120">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3159d-120">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserOofSettingsResponse/OofSettings` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3159d-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="3159d-121">Text value</span></span>

<span data-ttu-id="3159d-122">**Oofstate**要素にはテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="3159d-122">A text value is required for the **OofState** element.</span></span> <span data-ttu-id="3159d-123">次の一覧に、この要素に使用できる値を示します。</span><span class="sxs-lookup"><span data-stu-id="3159d-123">The following list contains the possible values for this element:</span></span> 
  
- <span data-ttu-id="3159d-124">**Disabled**</span><span class="sxs-lookup"><span data-stu-id="3159d-124">**Disabled**</span></span>
    
- <span data-ttu-id="3159d-125">**Enabled**</span><span class="sxs-lookup"><span data-stu-id="3159d-125">**Enabled**</span></span>
    
- <span data-ttu-id="3159d-126">**スケジュール済み**</span><span class="sxs-lookup"><span data-stu-id="3159d-126">**Scheduled**</span></span>
    
<span data-ttu-id="3159d-127">[**スケジュール**] の値は、[期間 (UserOofSettings)](duration-useroofsettings.md)要素で指定された期間中に OOF の状態が [**有効**] に設定されていることを示します。</span><span class="sxs-lookup"><span data-stu-id="3159d-127">A value of **Scheduled** indicates that the OOF status is set to **Enabled** during a time period identified by the [Duration (UserOofSettings)](duration-useroofsettings.md) element.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="3159d-128">注釈</span><span class="sxs-lookup"><span data-stu-id="3159d-128">Remarks</span></span>

<span data-ttu-id="3159d-129">この要素は、SetUsersOofSettingRequest メッセージと GetUserOofSettingResponse メッセージの両方に必要です。</span><span class="sxs-lookup"><span data-stu-id="3159d-129">This element is required in both the SetUsersOofSettingRequest message and the GetUserOofSettingResponse message.</span></span>
  
<span data-ttu-id="3159d-130">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="3159d-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="3159d-131">例</span><span class="sxs-lookup"><span data-stu-id="3159d-131">Example</span></span>

<span data-ttu-id="3159d-132">SetUserOofSettings 要求の次の例では、 **Oofstate**を有効にします。</span><span class="sxs-lookup"><span data-stu-id="3159d-132">The following example of a SetUserOofSettings request enables the **OofState**.</span></span>
  
```
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
      </UserOofSettings>
    </SetUserOofSettingsRequest>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a><span data-ttu-id="3159d-133">要素の情報</span><span class="sxs-lookup"><span data-stu-id="3159d-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3159d-134">Namespace</span><span class="sxs-lookup"><span data-stu-id="3159d-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3159d-135">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3159d-135">Schema Name</span></span>  <br/> |<span data-ttu-id="3159d-136">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="3159d-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="3159d-137">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3159d-137">Validation File</span></span>  <br/> |<span data-ttu-id="3159d-138">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="3159d-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3159d-139">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="3159d-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="3159d-140">正しくない</span><span class="sxs-lookup"><span data-stu-id="3159d-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3159d-141">関連項目</span><span class="sxs-lookup"><span data-stu-id="3159d-141">See also</span></span>



[<span data-ttu-id="3159d-142">GetUserOofSettings 操作</span><span class="sxs-lookup"><span data-stu-id="3159d-142">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)
  
[<span data-ttu-id="3159d-143">SetUserOofSettings 操作</span><span class="sxs-lookup"><span data-stu-id="3159d-143">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

