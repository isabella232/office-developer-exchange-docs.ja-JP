---
title: PlayOnPhoneGreeting (UM web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- PlayOnPhoneGreeting
api_type:
- schema
ms.assetid: 43eda596-3609-4e1b-8502-1db2636535cf
description: PlayOnPhoneGreeting 要素は、ユニファイド メッセージング、電話の案内応答を再生する要求を定義します。
ms.openlocfilehash: c30140fc60b9e902517b4cc18deb9b61efa61e0c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832836"
---
# <a name="playonphonegreeting-um-web-service"></a><span data-ttu-id="5053b-103">PlayOnPhoneGreeting (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="5053b-103">PlayOnPhoneGreeting (UM web service)</span></span>

<span data-ttu-id="5053b-104">**PlayOnPhoneGreeting**要素は、ユニファイド メッセージング、電話の案内応答を再生する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="5053b-104">The **PlayOnPhoneGreeting** element defines a request to play a Unified Messaging greeting on a telephone.</span></span> 
  
[<span data-ttu-id="5053b-105">PlayOnPhoneGreeting (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="5053b-105">PlayOnPhoneGreeting (UM web service)</span></span>](playonphonegreeting-um-web-service.md)
  
```xml
<PlayOnPhoneGreeting>
  <GreetingType/>
  <DialString/>
</PlayOnPhoneGreeting>
```

 <span data-ttu-id="5053b-106">**complexType**</span><span class="sxs-lookup"><span data-stu-id="5053b-106">**complexType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5053b-107">属性および要素</span><span class="sxs-lookup"><span data-stu-id="5053b-107">Attributes and elements</span></span>

<span data-ttu-id="5053b-108">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5053b-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5053b-109">属性</span><span class="sxs-lookup"><span data-stu-id="5053b-109">Attributes</span></span>

<span data-ttu-id="5053b-110">なし。</span><span class="sxs-lookup"><span data-stu-id="5053b-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5053b-111">子要素</span><span class="sxs-lookup"><span data-stu-id="5053b-111">Child elements</span></span>

|<span data-ttu-id="5053b-112">**要素**</span><span class="sxs-lookup"><span data-stu-id="5053b-112">**Element**</span></span>|<span data-ttu-id="5053b-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="5053b-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5053b-114">GreetingType (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="5053b-114">GreetingType (UM web service)</span></span>](greetingtype-um-web-service.md) <br/> |<span data-ttu-id="5053b-115">[PlayOnPhoneGreeting 操作 (UM web サービス)](playonphonegreeting-operation-um-web-service.md)の要求で使用するあいさつ文の種類を定義します。</span><span class="sxs-lookup"><span data-stu-id="5053b-115">Defines the type of greeting to use in a [PlayOnPhoneGreeting operation (UM web service)](playonphonegreeting-operation-um-web-service.md) request.</span></span>  <br/> |
|[<span data-ttu-id="5053b-116">dialString (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="5053b-116">dialString (UM web service)</span></span>](dialstring-um-web-service.md) <br/> |<span data-ttu-id="5053b-117">ダイヤルする電話番号の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5053b-117">Contains the value for the telephone number to dial.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5053b-118">親要素</span><span class="sxs-lookup"><span data-stu-id="5053b-118">Parent elements</span></span>

<span data-ttu-id="5053b-119">なし。</span><span class="sxs-lookup"><span data-stu-id="5053b-119">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="5053b-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="5053b-120">Text value</span></span>

<span data-ttu-id="5053b-121">なし。</span><span class="sxs-lookup"><span data-stu-id="5053b-121">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5053b-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="5053b-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5053b-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="5053b-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5053b-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5053b-124">Schema Name</span></span>  <br/> |<span data-ttu-id="5053b-125">メッセージ</span><span class="sxs-lookup"><span data-stu-id="5053b-125">Messages</span></span>  <br/> |
|<span data-ttu-id="5053b-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5053b-126">Validation File</span></span>  <br/> |<span data-ttu-id="5053b-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="5053b-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5053b-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="5053b-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="5053b-129">False</span><span class="sxs-lookup"><span data-stu-id="5053b-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5053b-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="5053b-130">See also</span></span>



[<span data-ttu-id="5053b-131">PlayOnPhoneGreeting 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="5053b-131">PlayOnPhoneGreeting operation (UM web service)</span></span>](playonphonegreeting-operation-um-web-service.md)

