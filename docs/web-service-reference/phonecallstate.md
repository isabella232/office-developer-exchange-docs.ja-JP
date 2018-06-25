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
description: PhoneCallState 要素は、電話の呼び出しの現在の状態を指定します。
ms.openlocfilehash: 184a7400810711442e565d1ef37094bd63b00914
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832761"
---
# <a name="phonecallstate"></a><span data-ttu-id="510d6-103">PhoneCallState</span><span class="sxs-lookup"><span data-stu-id="510d6-103">PhoneCallState</span></span>

<span data-ttu-id="510d6-104">**PhoneCallState**要素は、電話の呼び出しの現在の状態を指定します。</span><span class="sxs-lookup"><span data-stu-id="510d6-104">The **PhoneCallState** element specifies the current state for a phone call.</span></span> 
  
```xml
<PhoneCallState>Idle or Connecting or Alerted or Connected or Disconnected or Incoming or Transferring or Forwarding</PhoneCallState>
```

 <span data-ttu-id="510d6-105">**PhoneCallStateType**</span><span class="sxs-lookup"><span data-stu-id="510d6-105">**PhoneCallStateType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="510d6-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="510d6-106">Attributes and elements</span></span>

<span data-ttu-id="510d6-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="510d6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="510d6-108">属性</span><span class="sxs-lookup"><span data-stu-id="510d6-108">Attributes</span></span>

<span data-ttu-id="510d6-109">なし。</span><span class="sxs-lookup"><span data-stu-id="510d6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="510d6-110">子要素</span><span class="sxs-lookup"><span data-stu-id="510d6-110">Child elements</span></span>

<span data-ttu-id="510d6-111">なし。</span><span class="sxs-lookup"><span data-stu-id="510d6-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="510d6-112">親要素</span><span class="sxs-lookup"><span data-stu-id="510d6-112">Parent elements</span></span>

|<span data-ttu-id="510d6-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="510d6-113">**Element**</span></span>|<span data-ttu-id="510d6-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="510d6-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="510d6-115">PhoneCallInformation</span><span class="sxs-lookup"><span data-stu-id="510d6-115">PhoneCallInformation</span></span>](phonecallinformation.md) <br/> |<span data-ttu-id="510d6-116">電話の状態情報を指定します。</span><span class="sxs-lookup"><span data-stu-id="510d6-116">Specifies the state information for a phone call.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="510d6-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="510d6-117">Text value</span></span>

<span data-ttu-id="510d6-118">次の表は、 **PhoneCallState**要素の値を一覧します。</span><span class="sxs-lookup"><span data-stu-id="510d6-118">The following table lists the possible values for the **PhoneCallState** element.</span></span> 
  
<span data-ttu-id="510d6-119">**PhoneCallState 要素の値**</span><span class="sxs-lookup"><span data-stu-id="510d6-119">**PhoneCallState element values**</span></span>

|<span data-ttu-id="510d6-120">**値**</span><span class="sxs-lookup"><span data-stu-id="510d6-120">**Value**</span></span>|<span data-ttu-id="510d6-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="510d6-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="510d6-122">アイドル</span><span class="sxs-lookup"><span data-stu-id="510d6-122">Idle</span></span>  <br/> |<span data-ttu-id="510d6-123">最初の呼び出しの状態です。</span><span class="sxs-lookup"><span data-stu-id="510d6-123">Initial call state.</span></span>  <br/> |
|<span data-ttu-id="510d6-124">Connecting</span><span class="sxs-lookup"><span data-stu-id="510d6-124">Connecting</span></span>  <br/> |<span data-ttu-id="510d6-125">システムがこの呼び出しをダイヤルします。</span><span class="sxs-lookup"><span data-stu-id="510d6-125">The system is dialing this call.</span></span>  <br/> |
|<span data-ttu-id="510d6-126">警告を表示</span><span class="sxs-lookup"><span data-stu-id="510d6-126">Alerted</span></span>  <br/> |<span data-ttu-id="510d6-127">状態の警告では、呼び出し (電話が鳴って)。</span><span class="sxs-lookup"><span data-stu-id="510d6-127">The call is in alerting state (phone is ringing).</span></span>  <br/> |
|<span data-ttu-id="510d6-128">Connected</span><span class="sxs-lookup"><span data-stu-id="510d6-128">Connected</span></span>  <br/> |<span data-ttu-id="510d6-129">呼び出しは、接続されている状態です。</span><span class="sxs-lookup"><span data-stu-id="510d6-129">The call is in the connected state.</span></span>  <br/> |
|<span data-ttu-id="510d6-130">Disconnected</span><span class="sxs-lookup"><span data-stu-id="510d6-130">Disconnected</span></span>  <br/> |<span data-ttu-id="510d6-131">呼び出しは切断されます。</span><span class="sxs-lookup"><span data-stu-id="510d6-131">The call is disconnected.</span></span>  <br/> |
|<span data-ttu-id="510d6-132">受信</span><span class="sxs-lookup"><span data-stu-id="510d6-132">Incoming</span></span>  <br/> |<span data-ttu-id="510d6-133">呼び出しのバインドが解除されます。</span><span class="sxs-lookup"><span data-stu-id="510d6-133">The call is inbound.</span></span>  <br/> |
|<span data-ttu-id="510d6-134">転送します。</span><span class="sxs-lookup"><span data-stu-id="510d6-134">Transferring</span></span>  <br/> |<span data-ttu-id="510d6-135">呼び出しが別の宛先に転送されます。</span><span class="sxs-lookup"><span data-stu-id="510d6-135">The call is being transferred to another destination.</span></span>  <br/> |
|<span data-ttu-id="510d6-136">転送</span><span class="sxs-lookup"><span data-stu-id="510d6-136">Forwarding</span></span>  <br/> |<span data-ttu-id="510d6-137">呼び出しを別の宛先に転送されているが。</span><span class="sxs-lookup"><span data-stu-id="510d6-137">The call is being forwarded to another destination.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="510d6-138">備考</span><span class="sxs-lookup"><span data-stu-id="510d6-138">Remarks</span></span>

<span data-ttu-id="510d6-139">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの/ews/ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="510d6-139">The schema that describes this element is located in the /ews/ directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="510d6-140">要素情報</span><span class="sxs-lookup"><span data-stu-id="510d6-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="510d6-141">名前空間</span><span class="sxs-lookup"><span data-stu-id="510d6-141">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="510d6-142">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="510d6-142">Schema Name</span></span>  <br/> |<span data-ttu-id="510d6-143">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="510d6-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="510d6-144">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="510d6-144">Validation File</span></span>  <br/> |<span data-ttu-id="510d6-145">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="510d6-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="510d6-146">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="510d6-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="510d6-147">False</span><span class="sxs-lookup"><span data-stu-id="510d6-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="510d6-148">関連項目</span><span class="sxs-lookup"><span data-stu-id="510d6-148">See also</span></span>



- [<span data-ttu-id="510d6-149">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="510d6-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

