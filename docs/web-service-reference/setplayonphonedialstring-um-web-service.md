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
description: SetPlayOnPhoneDialString 要素は、PlayOnPhone 操作 (UM web サービス) の既定のダイヤル文字列を設定するための要求および PlayOnPhoneGreeting (UM web サービス) の操作の要求を定義します。
ms.openlocfilehash: fd82dc6ef0dd90a2318da93191f657005b7a5c87
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833450"
---
# <a name="setplayonphonedialstring-um-web-service"></a><span data-ttu-id="26905-103">SetPlayOnPhoneDialString (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="26905-103">SetPlayOnPhoneDialString (UM web service)</span></span>

<span data-ttu-id="26905-104">**SetPlayOnPhoneDialString**要素は、 [PlayOnPhone 操作 (UM web サービス)](playonphone-operation-um-web-service.md)および[PlayOnPhoneGreeting 操作 (UM web サービス)](playonphonegreeting-operation-um-web-service.md)の要求の既定のダイヤル文字列を設定する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="26905-104">The **SetPlayOnPhoneDialString** element defines a request to set the default dial string for [PlayOnPhone operation (UM web service)](playonphone-operation-um-web-service.md) and [PlayOnPhoneGreeting operation (UM web service)](playonphonegreeting-operation-um-web-service.md) requests.</span></span> 
  
[<span data-ttu-id="26905-105">SetPlayOnPhoneDialString (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="26905-105">SetPlayOnPhoneDialString (UM web service)</span></span>](setplayonphonedialstring-um-web-service.md)
  
```xml
<SetPlayOnPhoneDialString>
  <dialString>   </dialString>
</SetPlayOnPhoneDialString>
```

 <span data-ttu-id="26905-106">**complexType**</span><span class="sxs-lookup"><span data-stu-id="26905-106">**complexType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="26905-107">属性および要素</span><span class="sxs-lookup"><span data-stu-id="26905-107">Attributes and elements</span></span>

<span data-ttu-id="26905-108">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="26905-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="26905-109">属性</span><span class="sxs-lookup"><span data-stu-id="26905-109">Attributes</span></span>

<span data-ttu-id="26905-110">なし。</span><span class="sxs-lookup"><span data-stu-id="26905-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="26905-111">子要素</span><span class="sxs-lookup"><span data-stu-id="26905-111">Child elements</span></span>

|<span data-ttu-id="26905-112">**要素**</span><span class="sxs-lookup"><span data-stu-id="26905-112">**Element**</span></span>|<span data-ttu-id="26905-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="26905-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="26905-114">dialString (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="26905-114">dialString (UM web service)</span></span>](dialstring-um-web-service.md) <br/> |<span data-ttu-id="26905-115">ダイヤルの既定の文字列として設定するのには電話番号です。</span><span class="sxs-lookup"><span data-stu-id="26905-115">The telephone number to set as the default dial string.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="26905-116">親要素</span><span class="sxs-lookup"><span data-stu-id="26905-116">Parent elements</span></span>

<span data-ttu-id="26905-117">なし。</span><span class="sxs-lookup"><span data-stu-id="26905-117">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="26905-118">テキスト値</span><span class="sxs-lookup"><span data-stu-id="26905-118">Text value</span></span>

<span data-ttu-id="26905-119">なし。</span><span class="sxs-lookup"><span data-stu-id="26905-119">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="26905-120">要素情報</span><span class="sxs-lookup"><span data-stu-id="26905-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="26905-121">名前空間</span><span class="sxs-lookup"><span data-stu-id="26905-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="26905-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="26905-122">Schema Name</span></span>  <br/> |<span data-ttu-id="26905-123">メッセージ</span><span class="sxs-lookup"><span data-stu-id="26905-123">Messages</span></span>  <br/> |
|<span data-ttu-id="26905-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="26905-124">Validation File</span></span>  <br/> |<span data-ttu-id="26905-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="26905-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="26905-126">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="26905-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="26905-127">False</span><span class="sxs-lookup"><span data-stu-id="26905-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="26905-128">関連項目</span><span class="sxs-lookup"><span data-stu-id="26905-128">See also</span></span>



[<span data-ttu-id="26905-129">SetPlayOnPhoneDialString 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="26905-129">SetPlayOnPhoneDialString operation (UM web service)</span></span>](setplayonphonedialstring-operation-um-web-service.md)

