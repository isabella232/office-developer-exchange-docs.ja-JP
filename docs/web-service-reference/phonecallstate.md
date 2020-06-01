---
title: PhoneCallState
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PhoneCallState
api_type:
- schema
ms.assetid: ac009eb3-6334-49ce-82be-48fe83577f9c
description: PhoneCallState 要素は、通話の現在の状態を指定します。
ms.openlocfilehash: d2088b9b2811befe80684188d49c8034c577cc55
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468531"
---
# <a name="phonecallstate"></a><span data-ttu-id="18bcc-103">PhoneCallState</span><span class="sxs-lookup"><span data-stu-id="18bcc-103">PhoneCallState</span></span>

<span data-ttu-id="18bcc-104">**PhoneCallState**要素は、通話の現在の状態を指定します。</span><span class="sxs-lookup"><span data-stu-id="18bcc-104">The **PhoneCallState** element specifies the current state for a phone call.</span></span> 
  
```xml
<PhoneCallState>Idle or Connecting or Alerted or Connected or Disconnected or Incoming or Transferring or Forwarding</PhoneCallState>
```

 <span data-ttu-id="18bcc-105">**PhoneCallStateType**</span><span class="sxs-lookup"><span data-stu-id="18bcc-105">**PhoneCallStateType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="18bcc-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="18bcc-106">Attributes and elements</span></span>

<span data-ttu-id="18bcc-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="18bcc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="18bcc-108">属性</span><span class="sxs-lookup"><span data-stu-id="18bcc-108">Attributes</span></span>

<span data-ttu-id="18bcc-109">なし。</span><span class="sxs-lookup"><span data-stu-id="18bcc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="18bcc-110">子要素</span><span class="sxs-lookup"><span data-stu-id="18bcc-110">Child elements</span></span>

<span data-ttu-id="18bcc-111">なし。</span><span class="sxs-lookup"><span data-stu-id="18bcc-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="18bcc-112">親要素</span><span class="sxs-lookup"><span data-stu-id="18bcc-112">Parent elements</span></span>

|<span data-ttu-id="18bcc-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="18bcc-113">**Element**</span></span>|<span data-ttu-id="18bcc-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="18bcc-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="18bcc-115">PhoneCallInformation</span><span class="sxs-lookup"><span data-stu-id="18bcc-115">PhoneCallInformation</span></span>](phonecallinformation.md) <br/> |<span data-ttu-id="18bcc-116">通話の状態情報を指定します。</span><span class="sxs-lookup"><span data-stu-id="18bcc-116">Specifies the state information for a phone call.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="18bcc-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="18bcc-117">Text value</span></span>

<span data-ttu-id="18bcc-118">次の表に、 **PhoneCallState**要素に指定できる値を示します。</span><span class="sxs-lookup"><span data-stu-id="18bcc-118">The following table lists the possible values for the **PhoneCallState** element.</span></span> 
  
<span data-ttu-id="18bcc-119">**PhoneCallState 要素の値**</span><span class="sxs-lookup"><span data-stu-id="18bcc-119">**PhoneCallState element values**</span></span>

|<span data-ttu-id="18bcc-120">**値**</span><span class="sxs-lookup"><span data-stu-id="18bcc-120">**Value**</span></span>|<span data-ttu-id="18bcc-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="18bcc-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="18bcc-122">アイドル</span><span class="sxs-lookup"><span data-stu-id="18bcc-122">Idle</span></span>  <br/> |<span data-ttu-id="18bcc-123">最初の呼び出しの状態。</span><span class="sxs-lookup"><span data-stu-id="18bcc-123">Initial call state.</span></span>  <br/> |
|<span data-ttu-id="18bcc-124">接続中</span><span class="sxs-lookup"><span data-stu-id="18bcc-124">Connecting</span></span>  <br/> |<span data-ttu-id="18bcc-125">システムはこの通話にダイヤルしています。</span><span class="sxs-lookup"><span data-stu-id="18bcc-125">The system is dialing this call.</span></span>  <br/> |
|<span data-ttu-id="18bcc-126">警告</span><span class="sxs-lookup"><span data-stu-id="18bcc-126">Alerted</span></span>  <br/> |<span data-ttu-id="18bcc-127">通話は警告状態にあります (電話は鳴っています)。</span><span class="sxs-lookup"><span data-stu-id="18bcc-127">The call is in alerting state (phone is ringing).</span></span>  <br/> |
|<span data-ttu-id="18bcc-128">Connected</span><span class="sxs-lookup"><span data-stu-id="18bcc-128">Connected</span></span>  <br/> |<span data-ttu-id="18bcc-129">呼び出しは、接続状態です。</span><span class="sxs-lookup"><span data-stu-id="18bcc-129">The call is in the connected state.</span></span>  <br/> |
|<span data-ttu-id="18bcc-130">Disconnected</span><span class="sxs-lookup"><span data-stu-id="18bcc-130">Disconnected</span></span>  <br/> |<span data-ttu-id="18bcc-131">呼び出しは切断されます。</span><span class="sxs-lookup"><span data-stu-id="18bcc-131">The call is disconnected.</span></span>  <br/> |
|<span data-ttu-id="18bcc-132">読み込ま</span><span class="sxs-lookup"><span data-stu-id="18bcc-132">Incoming</span></span>  <br/> |<span data-ttu-id="18bcc-133">通話は受信です。</span><span class="sxs-lookup"><span data-stu-id="18bcc-133">The call is inbound.</span></span>  <br/> |
|<span data-ttu-id="18bcc-134">渡す</span><span class="sxs-lookup"><span data-stu-id="18bcc-134">Transferring</span></span>  <br/> |<span data-ttu-id="18bcc-135">通話は別の宛先に転送されています。</span><span class="sxs-lookup"><span data-stu-id="18bcc-135">The call is being transferred to another destination.</span></span>  <br/> |
|<span data-ttu-id="18bcc-136">しよう</span><span class="sxs-lookup"><span data-stu-id="18bcc-136">Forwarding</span></span>  <br/> |<span data-ttu-id="18bcc-137">通話は別の宛先に転送されています。</span><span class="sxs-lookup"><span data-stu-id="18bcc-137">The call is being forwarded to another destination.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="18bcc-138">注釈</span><span class="sxs-lookup"><span data-stu-id="18bcc-138">Remarks</span></span>

<span data-ttu-id="18bcc-139">この要素を記述するスキーマは、Microsoft Exchange Server 2010 を実行しているコンピューターの/ews/ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="18bcc-139">The schema that describes this element is located in the /ews/ directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="18bcc-140">要素の情報</span><span class="sxs-lookup"><span data-stu-id="18bcc-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="18bcc-141">Namespace</span><span class="sxs-lookup"><span data-stu-id="18bcc-141">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="18bcc-142">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="18bcc-142">Schema Name</span></span>  <br/> |<span data-ttu-id="18bcc-143">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="18bcc-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="18bcc-144">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="18bcc-144">Validation File</span></span>  <br/> |<span data-ttu-id="18bcc-145">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="18bcc-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="18bcc-146">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="18bcc-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="18bcc-147">正しくない</span><span class="sxs-lookup"><span data-stu-id="18bcc-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="18bcc-148">関連項目</span><span class="sxs-lookup"><span data-stu-id="18bcc-148">See also</span></span>



- [<span data-ttu-id="18bcc-149">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="18bcc-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

