---
title: Playon電話応答メッセージ (UM web サービス)
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
description: Playonphone 案内応答要素は、電話でユニファイドメッセージングの応答メッセージを再生するための要求を定義します。
ms.openlocfilehash: 197e4ba671e1711b73b1e7c239339db589357581
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529925"
---
# <a name="playonphonegreeting-um-web-service"></a><span data-ttu-id="84a66-103">Playon電話応答メッセージ (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="84a66-103">PlayOnPhoneGreeting (UM web service)</span></span>

<span data-ttu-id="84a66-104">**Playonphone 案内応答**要素は、電話でユニファイドメッセージングの応答メッセージを再生するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="84a66-104">The **PlayOnPhoneGreeting** element defines a request to play a Unified Messaging greeting on a telephone.</span></span> 
  
[<span data-ttu-id="84a66-105">Playon電話応答メッセージ (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="84a66-105">PlayOnPhoneGreeting (UM web service)</span></span>](playonphonegreeting-um-web-service.md)
  
```xml
<PlayOnPhoneGreeting>
  <GreetingType/>
  <DialString/>
</PlayOnPhoneGreeting>
```

 <span data-ttu-id="84a66-106">**complexType**</span><span class="sxs-lookup"><span data-stu-id="84a66-106">**complexType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="84a66-107">属性と要素</span><span class="sxs-lookup"><span data-stu-id="84a66-107">Attributes and elements</span></span>

<span data-ttu-id="84a66-108">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="84a66-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="84a66-109">属性</span><span class="sxs-lookup"><span data-stu-id="84a66-109">Attributes</span></span>

<span data-ttu-id="84a66-110">なし。</span><span class="sxs-lookup"><span data-stu-id="84a66-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="84a66-111">子要素</span><span class="sxs-lookup"><span data-stu-id="84a66-111">Child elements</span></span>

|<span data-ttu-id="84a66-112">**Element**</span><span class="sxs-lookup"><span data-stu-id="84a66-112">**Element**</span></span>|<span data-ttu-id="84a66-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="84a66-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="84a66-114">GreetingType (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="84a66-114">GreetingType (UM web service)</span></span>](greetingtype-um-web-service.md) <br/> |<span data-ttu-id="84a66-115">[Playon電話案内応答操作 (UM web サービス)](playonphonegreeting-operation-um-web-service.md)要求で使用する案内応答の種類を定義します。</span><span class="sxs-lookup"><span data-stu-id="84a66-115">Defines the type of greeting to use in a [PlayOnPhoneGreeting operation (UM web service)](playonphonegreeting-operation-um-web-service.md) request.</span></span>  <br/> |
|<span data-ttu-id="84a66-116">[[] (UM web サービス)](dialstring-um-web-service.md)</span><span class="sxs-lookup"><span data-stu-id="84a66-116">[dialString (UM web service)](dialstring-um-web-service.md)</span></span> <br/> |<span data-ttu-id="84a66-117">ダイヤルする電話番号の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="84a66-117">Contains the value for the telephone number to dial.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="84a66-118">親要素</span><span class="sxs-lookup"><span data-stu-id="84a66-118">Parent elements</span></span>

<span data-ttu-id="84a66-119">なし。</span><span class="sxs-lookup"><span data-stu-id="84a66-119">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="84a66-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="84a66-120">Text value</span></span>

<span data-ttu-id="84a66-121">なし。</span><span class="sxs-lookup"><span data-stu-id="84a66-121">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="84a66-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="84a66-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="84a66-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="84a66-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="84a66-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="84a66-124">Schema Name</span></span>  <br/> |<span data-ttu-id="84a66-125">メッセージ</span><span class="sxs-lookup"><span data-stu-id="84a66-125">Messages</span></span>  <br/> |
|<span data-ttu-id="84a66-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="84a66-126">Validation File</span></span>  <br/> |<span data-ttu-id="84a66-127">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="84a66-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="84a66-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="84a66-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="84a66-129">正しくない</span><span class="sxs-lookup"><span data-stu-id="84a66-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="84a66-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="84a66-130">See also</span></span>



[<span data-ttu-id="84a66-131">Playon電話案内応答操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="84a66-131">PlayOnPhoneGreeting operation (UM web service)</span></span>](playonphonegreeting-operation-um-web-service.md)

