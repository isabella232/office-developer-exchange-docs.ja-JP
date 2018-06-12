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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760079"
---
# <a name="disconnectphonecall"></a><span data-ttu-id="3fde6-103">DisconnectPhoneCall</span><span class="sxs-lookup"><span data-stu-id="3fde6-103">DisconnectPhoneCall</span></span>

<span data-ttu-id="3fde6-104">**DisconnectPhoneCall**要素は、呼び出しを切断するのには要求を表します。</span><span class="sxs-lookup"><span data-stu-id="3fde6-104">The **DisconnectPhoneCall** element represents a request to disconnect a call.</span></span> 
  
```xml
<DisconnectPhoneCall>
   <PhoneCallId/>
</DisconnectPhoneCall>
```

 <span data-ttu-id="3fde6-105">**DisconnectPhoneCallType**</span><span class="sxs-lookup"><span data-stu-id="3fde6-105">**DisconnectPhoneCallType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3fde6-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="3fde6-106">Attributes and elements</span></span>

<span data-ttu-id="3fde6-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3fde6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3fde6-108">属性</span><span class="sxs-lookup"><span data-stu-id="3fde6-108">Attributes</span></span>

<span data-ttu-id="3fde6-109">なし。</span><span class="sxs-lookup"><span data-stu-id="3fde6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3fde6-110">子要素</span><span class="sxs-lookup"><span data-stu-id="3fde6-110">Child elements</span></span>

|<span data-ttu-id="3fde6-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="3fde6-111">**Element**</span></span>|<span data-ttu-id="3fde6-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="3fde6-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3fde6-113">PhoneCallId</span><span class="sxs-lookup"><span data-stu-id="3fde6-113">PhoneCallId</span></span>](phonecallid.md) <br/> |<span data-ttu-id="3fde6-114">切断するのには、呼び出しの id を指定します。</span><span class="sxs-lookup"><span data-stu-id="3fde6-114">Specifies the identifier of the call to disconnect.</span></span> <span data-ttu-id="3fde6-115">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="3fde6-115">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3fde6-116">親要素</span><span class="sxs-lookup"><span data-stu-id="3fde6-116">Parent elements</span></span>

<span data-ttu-id="3fde6-117">なし。</span><span class="sxs-lookup"><span data-stu-id="3fde6-117">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="3fde6-118">テキスト値</span><span class="sxs-lookup"><span data-stu-id="3fde6-118">Text value</span></span>

<span data-ttu-id="3fde6-119">なし。</span><span class="sxs-lookup"><span data-stu-id="3fde6-119">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3fde6-120">解説</span><span class="sxs-lookup"><span data-stu-id="3fde6-120">Remarks</span></span>

<span data-ttu-id="3fde6-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="3fde6-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3fde6-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="3fde6-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3fde6-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="3fde6-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3fde6-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3fde6-124">Schema Name</span></span>  <br/> |<span data-ttu-id="3fde6-125">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="3fde6-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3fde6-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3fde6-126">Validation File</span></span>  <br/> |<span data-ttu-id="3fde6-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="3fde6-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3fde6-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="3fde6-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="3fde6-129">False</span><span class="sxs-lookup"><span data-stu-id="3fde6-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3fde6-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="3fde6-130">See also</span></span>

- [<span data-ttu-id="3fde6-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="3fde6-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

