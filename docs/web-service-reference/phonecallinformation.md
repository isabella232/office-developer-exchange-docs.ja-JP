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
description: PhoneCallInformation 要素は、電話呼び出しの状態情報を指定します。
ms.openlocfilehash: 75370bccb841818a8302bdd055ad96fd16b2e8df
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468846"
---
# <a name="phonecallinformation"></a><span data-ttu-id="1ef7b-103">PhoneCallInformation</span><span class="sxs-lookup"><span data-stu-id="1ef7b-103">PhoneCallInformation</span></span>

<span data-ttu-id="1ef7b-104">**PhoneCallInformation**要素は、電話呼び出しの状態情報を指定します。</span><span class="sxs-lookup"><span data-stu-id="1ef7b-104">The **PhoneCallInformation** element specifies the state information for a phone call.</span></span> 
  
```XML
<PhoneCallInformation>
   <PhoneCallState/>
   <ConnectionFailureCause/>
   <SIPResponseText/>
   <SIPResponseCode/>
</PhoneCallInformation>
```

 <span data-ttu-id="1ef7b-105">**PhoneCallInformationType**</span><span class="sxs-lookup"><span data-stu-id="1ef7b-105">**PhoneCallInformationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1ef7b-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="1ef7b-106">Attributes and elements</span></span>

<span data-ttu-id="1ef7b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1ef7b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1ef7b-108">属性</span><span class="sxs-lookup"><span data-stu-id="1ef7b-108">Attributes</span></span>

<span data-ttu-id="1ef7b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="1ef7b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1ef7b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="1ef7b-110">Child elements</span></span>

|<span data-ttu-id="1ef7b-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="1ef7b-111">**Element**</span></span>|<span data-ttu-id="1ef7b-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="1ef7b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1ef7b-113">PhoneCallState</span><span class="sxs-lookup"><span data-stu-id="1ef7b-113">PhoneCallState</span></span>](phonecallstate.md) <br/> |<span data-ttu-id="1ef7b-114">通話の状態を指定します。</span><span class="sxs-lookup"><span data-stu-id="1ef7b-114">Specifies the state for a phone call.</span></span> <span data-ttu-id="1ef7b-115">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="1ef7b-115">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="1ef7b-116">ConnectionFailureCause</span><span class="sxs-lookup"><span data-stu-id="1ef7b-116">ConnectionFailureCause</span></span>](connectionfailurecause.md) <br/> |<span data-ttu-id="1ef7b-117">接続エラーの原因を指定します。</span><span class="sxs-lookup"><span data-stu-id="1ef7b-117">Specifies the cause of a connection failure.</span></span> <span data-ttu-id="1ef7b-118">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="1ef7b-118">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="1ef7b-119">SIPResponseText</span><span class="sxs-lookup"><span data-stu-id="1ef7b-119">SIPResponseText</span></span>](sipresponsetext.md) <br/> |<span data-ttu-id="1ef7b-120">SIP 応答テキストを指定します。</span><span class="sxs-lookup"><span data-stu-id="1ef7b-120">Specifies the SIP response text.</span></span> <span data-ttu-id="1ef7b-121">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="1ef7b-121">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="1ef7b-122">SIPResponseCode</span><span class="sxs-lookup"><span data-stu-id="1ef7b-122">SIPResponseCode</span></span>](sipresponsecode.md) <br/> |<span data-ttu-id="1ef7b-123">SIP 応答コードを指定します。</span><span class="sxs-lookup"><span data-stu-id="1ef7b-123">Specifies the SIP response code.</span></span> <span data-ttu-id="1ef7b-124">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="1ef7b-124">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1ef7b-125">親要素</span><span class="sxs-lookup"><span data-stu-id="1ef7b-125">Parent elements</span></span>

|<span data-ttu-id="1ef7b-126">**要素**</span><span class="sxs-lookup"><span data-stu-id="1ef7b-126">**Element**</span></span>|<span data-ttu-id="1ef7b-127">**説明**</span><span class="sxs-lookup"><span data-stu-id="1ef7b-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1ef7b-128">GetPhoneCallInformationResponse</span><span class="sxs-lookup"><span data-stu-id="1ef7b-128">GetPhoneCallInformationResponse</span></span>](getphonecallinformationresponse.md) <br/> |<span data-ttu-id="1ef7b-129">[GetPhoneCallInformation 操作](getphonecallinformation-operation.md)要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="1ef7b-129">Defines a response to a [GetPhoneCallInformation operation](getphonecallinformation-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1ef7b-130">注釈</span><span class="sxs-lookup"><span data-stu-id="1ef7b-130">Remarks</span></span>

<span data-ttu-id="1ef7b-131">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="1ef7b-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1ef7b-132">要素の情報</span><span class="sxs-lookup"><span data-stu-id="1ef7b-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1ef7b-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="1ef7b-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1ef7b-134">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1ef7b-134">Schema Name</span></span>  <br/> |<span data-ttu-id="1ef7b-135">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="1ef7b-135">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1ef7b-136">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1ef7b-136">Validation File</span></span>  <br/> |<span data-ttu-id="1ef7b-137">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="1ef7b-137">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1ef7b-138">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="1ef7b-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="1ef7b-139">正しくない</span><span class="sxs-lookup"><span data-stu-id="1ef7b-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1ef7b-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="1ef7b-140">See also</span></span>



- [<span data-ttu-id="1ef7b-141">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="1ef7b-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

