---
title: PhoneCallInformation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PhoneCallInformation
api_type:
- schema
ms.assetid: a0363c42-6d35-4074-bc17-946eb12736ff
description: PhoneCallInformation 要素は、電話の状態情報を指定します。
ms.openlocfilehash: e64e7b38b3801c60df8a966e95d980746533d3a4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832758"
---
# <a name="phonecallinformation"></a><span data-ttu-id="c5d78-103">PhoneCallInformation</span><span class="sxs-lookup"><span data-stu-id="c5d78-103">PhoneCallInformation</span></span>

<span data-ttu-id="c5d78-104">**PhoneCallInformation**要素は、電話の状態情報を指定します。</span><span class="sxs-lookup"><span data-stu-id="c5d78-104">The **PhoneCallInformation** element specifies the state information for a phone call.</span></span> 
  
```XML
<PhoneCallInformation>
   <PhoneCallState/>
   <ConnectionFailureCause/>
   <SIPResponseText/>
   <SIPResponseCode/>
</PhoneCallInformation>
```

 <span data-ttu-id="c5d78-105">**PhoneCallInformationType**</span><span class="sxs-lookup"><span data-stu-id="c5d78-105">**PhoneCallInformationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c5d78-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="c5d78-106">Attributes and elements</span></span>

<span data-ttu-id="c5d78-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c5d78-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c5d78-108">属性</span><span class="sxs-lookup"><span data-stu-id="c5d78-108">Attributes</span></span>

<span data-ttu-id="c5d78-109">なし。</span><span class="sxs-lookup"><span data-stu-id="c5d78-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c5d78-110">子要素</span><span class="sxs-lookup"><span data-stu-id="c5d78-110">Child elements</span></span>

|<span data-ttu-id="c5d78-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="c5d78-111">**Element**</span></span>|<span data-ttu-id="c5d78-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="c5d78-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c5d78-113">PhoneCallState</span><span class="sxs-lookup"><span data-stu-id="c5d78-113">PhoneCallState</span></span>](phonecallstate.md) <br/> |<span data-ttu-id="c5d78-114">電話の状態を指定します。</span><span class="sxs-lookup"><span data-stu-id="c5d78-114">Specifies the state for a phone call.</span></span> <span data-ttu-id="c5d78-115">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="c5d78-115">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="c5d78-116">ConnectionFailureCause</span><span class="sxs-lookup"><span data-stu-id="c5d78-116">ConnectionFailureCause</span></span>](connectionfailurecause.md) <br/> |<span data-ttu-id="c5d78-117">接続エラーの原因を指定します。</span><span class="sxs-lookup"><span data-stu-id="c5d78-117">Specifies the cause of a connection failure.</span></span> <span data-ttu-id="c5d78-118">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="c5d78-118">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="c5d78-119">SIPResponseText</span><span class="sxs-lookup"><span data-stu-id="c5d78-119">SIPResponseText</span></span>](sipresponsetext.md) <br/> |<span data-ttu-id="c5d78-120">SIP 応答のテキストを指定します。</span><span class="sxs-lookup"><span data-stu-id="c5d78-120">Specifies the SIP response text.</span></span> <span data-ttu-id="c5d78-121">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="c5d78-121">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="c5d78-122">SIPResponseCode</span><span class="sxs-lookup"><span data-stu-id="c5d78-122">SIPResponseCode</span></span>](sipresponsecode.md) <br/> |<span data-ttu-id="c5d78-123">SIP 応答コードを指定します。</span><span class="sxs-lookup"><span data-stu-id="c5d78-123">Specifies the SIP response code.</span></span> <span data-ttu-id="c5d78-124">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="c5d78-124">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c5d78-125">親要素</span><span class="sxs-lookup"><span data-stu-id="c5d78-125">Parent elements</span></span>

|<span data-ttu-id="c5d78-126">**要素**</span><span class="sxs-lookup"><span data-stu-id="c5d78-126">**Element**</span></span>|<span data-ttu-id="c5d78-127">**説明**</span><span class="sxs-lookup"><span data-stu-id="c5d78-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c5d78-128">GetPhoneCallInformationResponse</span><span class="sxs-lookup"><span data-stu-id="c5d78-128">GetPhoneCallInformationResponse</span></span>](getphonecallinformationresponse.md) <br/> |<span data-ttu-id="c5d78-129">[GetPhoneCallInformation 操作](getphonecallinformation-operation.md)要求に対する応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="c5d78-129">Defines a response to a [GetPhoneCallInformation operation](getphonecallinformation-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c5d78-130">備考</span><span class="sxs-lookup"><span data-stu-id="c5d78-130">Remarks</span></span>

<span data-ttu-id="c5d78-131">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="c5d78-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c5d78-132">要素情報</span><span class="sxs-lookup"><span data-stu-id="c5d78-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c5d78-133">名前空間</span><span class="sxs-lookup"><span data-stu-id="c5d78-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c5d78-134">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c5d78-134">Schema Name</span></span>  <br/> |<span data-ttu-id="c5d78-135">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="c5d78-135">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c5d78-136">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c5d78-136">Validation File</span></span>  <br/> |<span data-ttu-id="c5d78-137">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c5d78-137">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c5d78-138">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="c5d78-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="c5d78-139">False</span><span class="sxs-lookup"><span data-stu-id="c5d78-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c5d78-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="c5d78-140">See also</span></span>



- [<span data-ttu-id="c5d78-141">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="c5d78-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

