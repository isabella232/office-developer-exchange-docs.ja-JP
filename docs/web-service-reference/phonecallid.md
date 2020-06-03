---
title: PhoneCallId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PhoneCallId
api_type:
- schema
ms.assetid: 79e31a4c-fc84-4802-8761-470df8d63694
description: PhoneCallId 要素は、電話呼び出しの識別子を指定します。 この要素は必須です。
ms.openlocfilehash: 3e4b9dba5e8be6e45a0c16508531fbc6cf91c170
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459701"
---
# <a name="phonecallid"></a><span data-ttu-id="7efad-104">PhoneCallId</span><span class="sxs-lookup"><span data-stu-id="7efad-104">PhoneCallId</span></span>

<span data-ttu-id="7efad-105">**PhoneCallId**要素は、電話呼び出しの識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="7efad-105">The **PhoneCallId** element specifies the identifier of a phone call.</span></span> <span data-ttu-id="7efad-106">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="7efad-106">This element is required.</span></span> 
  
```xml
<PhoneCallId Id="" />
```

 <span data-ttu-id="7efad-107">**PhoneCallIdType**</span><span class="sxs-lookup"><span data-stu-id="7efad-107">**PhoneCallIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7efad-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="7efad-108">Attributes and elements</span></span>

<span data-ttu-id="7efad-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7efad-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7efad-110">属性</span><span class="sxs-lookup"><span data-stu-id="7efad-110">Attributes</span></span>

|<span data-ttu-id="7efad-111">**属性**</span><span class="sxs-lookup"><span data-stu-id="7efad-111">**Attribute**</span></span>|<span data-ttu-id="7efad-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="7efad-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7efad-113">ID</span><span class="sxs-lookup"><span data-stu-id="7efad-113">Id</span></span>  <br/> |<span data-ttu-id="7efad-114">切断する電話通話を識別します。</span><span class="sxs-lookup"><span data-stu-id="7efad-114">Identifies the phone call to disconnect.</span></span> <span data-ttu-id="7efad-115">この属性は必須です。</span><span class="sxs-lookup"><span data-stu-id="7efad-115">This attribute is required.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="7efad-116">子要素</span><span class="sxs-lookup"><span data-stu-id="7efad-116">Child elements</span></span>

<span data-ttu-id="7efad-117">なし。</span><span class="sxs-lookup"><span data-stu-id="7efad-117">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7efad-118">親要素</span><span class="sxs-lookup"><span data-stu-id="7efad-118">Parent elements</span></span>

|<span data-ttu-id="7efad-119">**要素**</span><span class="sxs-lookup"><span data-stu-id="7efad-119">**Element**</span></span>|<span data-ttu-id="7efad-120">**説明**</span><span class="sxs-lookup"><span data-stu-id="7efad-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7efad-121">電話</span><span class="sxs-lookup"><span data-stu-id="7efad-121">DisconnectPhoneCall</span></span>](disconnectphonecall.md) <br/> |<span data-ttu-id="7efad-122">呼び出しを切断する要求を表します。</span><span class="sxs-lookup"><span data-stu-id="7efad-122">Represents a request to disconnect a call.</span></span>  <br/> |
|[<span data-ttu-id="7efad-123">GetPhoneCallInformation</span><span class="sxs-lookup"><span data-stu-id="7efad-123">GetPhoneCallInformation</span></span>](getphonecallinformation.md) <br/> |<span data-ttu-id="7efad-124">電話呼び出し情報を取得するための要求を表します。</span><span class="sxs-lookup"><span data-stu-id="7efad-124">Represents a request to get telephone call information.</span></span>  <br/> |
|[<span data-ttu-id="7efad-125">PlayOnPhoneResponse (Exchange Web サービス)</span><span class="sxs-lookup"><span data-stu-id="7efad-125">PlayOnPhoneResponse (Exchange Web Services)</span></span>](playonphoneresponse-exchange-web-services.md) <br/> |<span data-ttu-id="7efad-126">PlayOnPhone 要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="7efad-126">Defines a response to a PlayOnPhone request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7efad-127">注釈</span><span class="sxs-lookup"><span data-stu-id="7efad-127">Remarks</span></span>

<span data-ttu-id="7efad-128">この要素を記述するスキーマは、Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="7efad-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7efad-129">要素の情報</span><span class="sxs-lookup"><span data-stu-id="7efad-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7efad-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="7efad-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7efad-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7efad-131">Schema Name</span></span>  <br/> |<span data-ttu-id="7efad-132">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="7efad-132">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7efad-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7efad-133">Validation File</span></span>  <br/> |<span data-ttu-id="7efad-134">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="7efad-134">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7efad-135">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="7efad-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="7efad-136">正しくない</span><span class="sxs-lookup"><span data-stu-id="7efad-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7efad-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="7efad-137">See also</span></span>



- [<span data-ttu-id="7efad-138">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="7efad-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

