---
title: DisconnectPhoneCall
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DisconnectPhoneCall
api_type:
- schema
ms.assetid: f9252536-9852-4dd9-9ebc-91f5cf281171
description: DisconnectPhoneCall 要素は、呼び出しを切断するのには要求を表します。
ms.openlocfilehash: 56947ea9ba56c76bb02d6a425ff43b3b846a2f60
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760079"
---
# <a name="disconnectphonecall"></a><span data-ttu-id="9d9be-103">DisconnectPhoneCall</span><span class="sxs-lookup"><span data-stu-id="9d9be-103">DisconnectPhoneCall</span></span>

<span data-ttu-id="9d9be-104">**DisconnectPhoneCall**要素は、呼び出しを切断するのには要求を表します。</span><span class="sxs-lookup"><span data-stu-id="9d9be-104">The **DisconnectPhoneCall** element represents a request to disconnect a call.</span></span> 
  
```xml
<DisconnectPhoneCall>
   <PhoneCallId/>
</DisconnectPhoneCall>
```

 <span data-ttu-id="9d9be-105">**DisconnectPhoneCallType**</span><span class="sxs-lookup"><span data-stu-id="9d9be-105">**DisconnectPhoneCallType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9d9be-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="9d9be-106">Attributes and elements</span></span>

<span data-ttu-id="9d9be-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9d9be-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9d9be-108">属性</span><span class="sxs-lookup"><span data-stu-id="9d9be-108">Attributes</span></span>

<span data-ttu-id="9d9be-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9d9be-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9d9be-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9d9be-110">Child elements</span></span>

|<span data-ttu-id="9d9be-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="9d9be-111">**Element**</span></span>|<span data-ttu-id="9d9be-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="9d9be-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9d9be-113">PhoneCallId</span><span class="sxs-lookup"><span data-stu-id="9d9be-113">PhoneCallId</span></span>](phonecallid.md) <br/> |<span data-ttu-id="9d9be-114">切断するのには、呼び出しの id を指定します。</span><span class="sxs-lookup"><span data-stu-id="9d9be-114">Specifies the identifier of the call to disconnect.</span></span> <span data-ttu-id="9d9be-115">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="9d9be-115">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9d9be-116">親要素</span><span class="sxs-lookup"><span data-stu-id="9d9be-116">Parent elements</span></span>

<span data-ttu-id="9d9be-117">なし。</span><span class="sxs-lookup"><span data-stu-id="9d9be-117">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="9d9be-118">テキスト値</span><span class="sxs-lookup"><span data-stu-id="9d9be-118">Text value</span></span>

<span data-ttu-id="9d9be-119">なし。</span><span class="sxs-lookup"><span data-stu-id="9d9be-119">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9d9be-120">備考</span><span class="sxs-lookup"><span data-stu-id="9d9be-120">Remarks</span></span>

<span data-ttu-id="9d9be-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="9d9be-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9d9be-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="9d9be-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9d9be-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="9d9be-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9d9be-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9d9be-124">Schema Name</span></span>  <br/> |<span data-ttu-id="9d9be-125">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="9d9be-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9d9be-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9d9be-126">Validation File</span></span>  <br/> |<span data-ttu-id="9d9be-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9d9be-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9d9be-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="9d9be-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="9d9be-129">False</span><span class="sxs-lookup"><span data-stu-id="9d9be-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9d9be-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="9d9be-130">See also</span></span>

- [<span data-ttu-id="9d9be-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="9d9be-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

