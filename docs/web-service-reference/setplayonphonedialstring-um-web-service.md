---
title: SetPlayOnPhoneDialString (UM web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- SetPlayOnPhoneDialString
api_type:
- schema
ms.assetid: 513a5072-c3ac-405f-98c2-0ab982d0a360
description: SetPlayOnPhoneDialString 要素は、PlayOnPhone 操作 (UM web サービス) および Playonphone 案内応答操作 (UM web サービス) 要求の既定のダイヤル文字列を設定するための要求を定義します。
ms.openlocfilehash: 40021e9dedafb5fafda91bf3612d8a6485dae8e7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458629"
---
# <a name="setplayonphonedialstring-um-web-service"></a><span data-ttu-id="17a81-103">SetPlayOnPhoneDialString (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="17a81-103">SetPlayOnPhoneDialString (UM web service)</span></span>

<span data-ttu-id="17a81-104">**SetPlayOnPhoneDialString**要素は、 [playonphone 操作 (um web サービス)](playonphone-operation-um-web-service.md)および[playonphone 案内応答操作 (um web サービス)](playonphonegreeting-operation-um-web-service.md)要求の既定のダイヤル文字列を設定するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="17a81-104">The **SetPlayOnPhoneDialString** element defines a request to set the default dial string for [PlayOnPhone operation (UM web service)](playonphone-operation-um-web-service.md) and [PlayOnPhoneGreeting operation (UM web service)](playonphonegreeting-operation-um-web-service.md) requests.</span></span> 
  
[<span data-ttu-id="17a81-105">SetPlayOnPhoneDialString (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="17a81-105">SetPlayOnPhoneDialString (UM web service)</span></span>](setplayonphonedialstring-um-web-service.md)
  
```xml
<SetPlayOnPhoneDialString>
  <dialString>   </dialString>
</SetPlayOnPhoneDialString>
```

 <span data-ttu-id="17a81-106">**complexType**</span><span class="sxs-lookup"><span data-stu-id="17a81-106">**complexType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="17a81-107">属性と要素</span><span class="sxs-lookup"><span data-stu-id="17a81-107">Attributes and elements</span></span>

<span data-ttu-id="17a81-108">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="17a81-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="17a81-109">属性</span><span class="sxs-lookup"><span data-stu-id="17a81-109">Attributes</span></span>

<span data-ttu-id="17a81-110">なし。</span><span class="sxs-lookup"><span data-stu-id="17a81-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="17a81-111">子要素</span><span class="sxs-lookup"><span data-stu-id="17a81-111">Child elements</span></span>

|<span data-ttu-id="17a81-112">**Element**</span><span class="sxs-lookup"><span data-stu-id="17a81-112">**Element**</span></span>|<span data-ttu-id="17a81-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="17a81-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="17a81-114">[[] (UM web サービス)](dialstring-um-web-service.md)</span><span class="sxs-lookup"><span data-stu-id="17a81-114">[dialString (UM web service)](dialstring-um-web-service.md)</span></span> <br/> |<span data-ttu-id="17a81-115">既定のダイヤル文字列として設定する電話番号です。</span><span class="sxs-lookup"><span data-stu-id="17a81-115">The telephone number to set as the default dial string.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="17a81-116">親要素</span><span class="sxs-lookup"><span data-stu-id="17a81-116">Parent elements</span></span>

<span data-ttu-id="17a81-117">なし。</span><span class="sxs-lookup"><span data-stu-id="17a81-117">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="17a81-118">テキスト値</span><span class="sxs-lookup"><span data-stu-id="17a81-118">Text value</span></span>

<span data-ttu-id="17a81-119">なし。</span><span class="sxs-lookup"><span data-stu-id="17a81-119">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="17a81-120">要素の情報</span><span class="sxs-lookup"><span data-stu-id="17a81-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="17a81-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="17a81-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="17a81-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="17a81-122">Schema Name</span></span>  <br/> |<span data-ttu-id="17a81-123">メッセージ</span><span class="sxs-lookup"><span data-stu-id="17a81-123">Messages</span></span>  <br/> |
|<span data-ttu-id="17a81-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="17a81-124">Validation File</span></span>  <br/> |<span data-ttu-id="17a81-125">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="17a81-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="17a81-126">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="17a81-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="17a81-127">正しくない</span><span class="sxs-lookup"><span data-stu-id="17a81-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="17a81-128">関連項目</span><span class="sxs-lookup"><span data-stu-id="17a81-128">See also</span></span>



[<span data-ttu-id="17a81-129">SetPlayOnPhoneDialString 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="17a81-129">SetPlayOnPhoneDialString operation (UM web service)</span></span>](setplayonphonedialstring-operation-um-web-service.md)

