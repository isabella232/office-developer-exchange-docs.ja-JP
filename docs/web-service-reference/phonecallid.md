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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832757"
---
# <a name="phonecallid"></a><span data-ttu-id="a642a-104">PhoneCallId</span><span class="sxs-lookup"><span data-stu-id="a642a-104">PhoneCallId</span></span>

<span data-ttu-id="a642a-105">**PhoneCallId**要素は、電話の呼び出しの id を指定します。</span><span class="sxs-lookup"><span data-stu-id="a642a-105">The **PhoneCallId** element specifies the identifier of a phone call.</span></span> <span data-ttu-id="a642a-106">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="a642a-106">This element is required.</span></span> 
  
```xml
<PhoneCallId Id="" />
```

 <span data-ttu-id="a642a-107">**PhoneCallIdType**</span><span class="sxs-lookup"><span data-stu-id="a642a-107">**PhoneCallIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a642a-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="a642a-108">Attributes and elements</span></span>

<span data-ttu-id="a642a-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a642a-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a642a-110">属性</span><span class="sxs-lookup"><span data-stu-id="a642a-110">Attributes</span></span>

|<span data-ttu-id="a642a-111">**属性**</span><span class="sxs-lookup"><span data-stu-id="a642a-111">**Attribute**</span></span>|<span data-ttu-id="a642a-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="a642a-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a642a-113">ID</span><span class="sxs-lookup"><span data-stu-id="a642a-113">Id</span></span>  <br/> |<span data-ttu-id="a642a-114">切断するのには電話の呼び出しを識別します。</span><span class="sxs-lookup"><span data-stu-id="a642a-114">Identifies the phone call to disconnect.</span></span> <span data-ttu-id="a642a-115">この属性は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="a642a-115">This attribute is required.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="a642a-116">子要素</span><span class="sxs-lookup"><span data-stu-id="a642a-116">Child elements</span></span>

<span data-ttu-id="a642a-117">なし。</span><span class="sxs-lookup"><span data-stu-id="a642a-117">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a642a-118">親要素</span><span class="sxs-lookup"><span data-stu-id="a642a-118">Parent elements</span></span>

|<span data-ttu-id="a642a-119">**要素**</span><span class="sxs-lookup"><span data-stu-id="a642a-119">**Element**</span></span>|<span data-ttu-id="a642a-120">**説明**</span><span class="sxs-lookup"><span data-stu-id="a642a-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a642a-121">DisconnectPhoneCall</span><span class="sxs-lookup"><span data-stu-id="a642a-121">DisconnectPhoneCall</span></span>](disconnectphonecall.md) <br/> |<span data-ttu-id="a642a-122">呼び出しを切断するのには要求を表します。</span><span class="sxs-lookup"><span data-stu-id="a642a-122">Represents a request to disconnect a call.</span></span>  <br/> |
|[<span data-ttu-id="a642a-123">GetPhoneCallInformation</span><span class="sxs-lookup"><span data-stu-id="a642a-123">GetPhoneCallInformation</span></span>](getphonecallinformation.md) <br/> |<span data-ttu-id="a642a-124">電話の情報を取得する要求を表します。</span><span class="sxs-lookup"><span data-stu-id="a642a-124">Represents a request to get telephone call information.</span></span>  <br/> |
|[<span data-ttu-id="a642a-125">PlayOnPhoneResponse (Exchange Web サービス)</span><span class="sxs-lookup"><span data-stu-id="a642a-125">PlayOnPhoneResponse (Exchange Web Services)</span></span>](playonphoneresponse-exchange-web-services.md) <br/> |<span data-ttu-id="a642a-126">PlayOnPhone 要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="a642a-126">Defines a response to a PlayOnPhone request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a642a-127">備考</span><span class="sxs-lookup"><span data-stu-id="a642a-127">Remarks</span></span>

<span data-ttu-id="a642a-128">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="a642a-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a642a-129">要素情報</span><span class="sxs-lookup"><span data-stu-id="a642a-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a642a-130">名前空間</span><span class="sxs-lookup"><span data-stu-id="a642a-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a642a-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a642a-131">Schema Name</span></span>  <br/> |<span data-ttu-id="a642a-132">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="a642a-132">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a642a-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a642a-133">Validation File</span></span>  <br/> |<span data-ttu-id="a642a-134">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="a642a-134">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a642a-135">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="a642a-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="a642a-136">False</span><span class="sxs-lookup"><span data-stu-id="a642a-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a642a-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="a642a-137">See also</span></span>



- [<span data-ttu-id="a642a-138">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="a642a-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

