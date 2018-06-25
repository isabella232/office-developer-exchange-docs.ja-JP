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
description: PhoneCallId 要素は、電話の呼び出しの id を指定します。 この要素は必須です。
ms.openlocfilehash: 1886d9510fe254c016779166efccc9882fd77d2c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832757"
---
# <a name="phonecallid"></a><span data-ttu-id="0b93c-104">PhoneCallId</span><span class="sxs-lookup"><span data-stu-id="0b93c-104">PhoneCallId</span></span>

<span data-ttu-id="0b93c-105">**PhoneCallId**要素は、電話の呼び出しの id を指定します。</span><span class="sxs-lookup"><span data-stu-id="0b93c-105">The **PhoneCallId** element specifies the identifier of a phone call.</span></span> <span data-ttu-id="0b93c-106">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="0b93c-106">This element is required.</span></span> 
  
```xml
<PhoneCallId Id="" />
```

 <span data-ttu-id="0b93c-107">**PhoneCallIdType**</span><span class="sxs-lookup"><span data-stu-id="0b93c-107">**PhoneCallIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0b93c-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="0b93c-108">Attributes and elements</span></span>

<span data-ttu-id="0b93c-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0b93c-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0b93c-110">属性</span><span class="sxs-lookup"><span data-stu-id="0b93c-110">Attributes</span></span>

|<span data-ttu-id="0b93c-111">**属性**</span><span class="sxs-lookup"><span data-stu-id="0b93c-111">**Attribute**</span></span>|<span data-ttu-id="0b93c-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="0b93c-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0b93c-113">ID</span><span class="sxs-lookup"><span data-stu-id="0b93c-113">Id</span></span>  <br/> |<span data-ttu-id="0b93c-114">切断するのには電話の呼び出しを識別します。</span><span class="sxs-lookup"><span data-stu-id="0b93c-114">Identifies the phone call to disconnect.</span></span> <span data-ttu-id="0b93c-115">この属性は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="0b93c-115">This attribute is required.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="0b93c-116">子要素</span><span class="sxs-lookup"><span data-stu-id="0b93c-116">Child elements</span></span>

<span data-ttu-id="0b93c-117">なし。</span><span class="sxs-lookup"><span data-stu-id="0b93c-117">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0b93c-118">親要素</span><span class="sxs-lookup"><span data-stu-id="0b93c-118">Parent elements</span></span>

|<span data-ttu-id="0b93c-119">**要素**</span><span class="sxs-lookup"><span data-stu-id="0b93c-119">**Element**</span></span>|<span data-ttu-id="0b93c-120">**説明**</span><span class="sxs-lookup"><span data-stu-id="0b93c-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0b93c-121">DisconnectPhoneCall</span><span class="sxs-lookup"><span data-stu-id="0b93c-121">DisconnectPhoneCall</span></span>](disconnectphonecall.md) <br/> |<span data-ttu-id="0b93c-122">呼び出しを切断するのには要求を表します。</span><span class="sxs-lookup"><span data-stu-id="0b93c-122">Represents a request to disconnect a call.</span></span>  <br/> |
|[<span data-ttu-id="0b93c-123">GetPhoneCallInformation</span><span class="sxs-lookup"><span data-stu-id="0b93c-123">GetPhoneCallInformation</span></span>](getphonecallinformation.md) <br/> |<span data-ttu-id="0b93c-124">電話の情報を取得する要求を表します。</span><span class="sxs-lookup"><span data-stu-id="0b93c-124">Represents a request to get telephone call information.</span></span>  <br/> |
|[<span data-ttu-id="0b93c-125">PlayOnPhoneResponse (Exchange Web サービス)</span><span class="sxs-lookup"><span data-stu-id="0b93c-125">PlayOnPhoneResponse (Exchange Web Services)</span></span>](playonphoneresponse-exchange-web-services.md) <br/> |<span data-ttu-id="0b93c-126">PlayOnPhone 要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="0b93c-126">Defines a response to a PlayOnPhone request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0b93c-127">備考</span><span class="sxs-lookup"><span data-stu-id="0b93c-127">Remarks</span></span>

<span data-ttu-id="0b93c-128">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="0b93c-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0b93c-129">要素情報</span><span class="sxs-lookup"><span data-stu-id="0b93c-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0b93c-130">名前空間</span><span class="sxs-lookup"><span data-stu-id="0b93c-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0b93c-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0b93c-131">Schema Name</span></span>  <br/> |<span data-ttu-id="0b93c-132">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="0b93c-132">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0b93c-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0b93c-133">Validation File</span></span>  <br/> |<span data-ttu-id="0b93c-134">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="0b93c-134">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0b93c-135">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="0b93c-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="0b93c-136">False</span><span class="sxs-lookup"><span data-stu-id="0b93c-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0b93c-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="0b93c-137">See also</span></span>



- [<span data-ttu-id="0b93c-138">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="0b93c-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

