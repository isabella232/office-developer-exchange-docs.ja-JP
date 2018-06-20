---
title: PlayOnPhoneResponse (UM web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- PlayOnPhoneResponse
api_type:
- schema
ms.assetid: 42b16880-1271-4690-abd0-0072d95b04b7
description: PlayOnPhoneResponse 要素は、PlayOnPhone の操作 (UM web サービス) 要求に対する応答を定義します。
ms.openlocfilehash: 482739d924bbac1d58624e50596af48cc405a3ef
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832832"
---
# <a name="playonphoneresponse-um-web-service"></a><span data-ttu-id="020e2-103">PlayOnPhoneResponse (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="020e2-103">PlayOnPhoneResponse (UM web service)</span></span>

<span data-ttu-id="020e2-104">**PlayOnPhoneResponse**要素は、 [PlayOnPhone 操作 (UM web サービス)](playonphone-operation-um-web-service.md)要求に対する応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="020e2-104">The **PlayOnPhoneResponse** element defines a response to a [PlayOnPhone operation (UM web service)](playonphone-operation-um-web-service.md) request.</span></span> 
  
[<span data-ttu-id="020e2-105">PlayOnPhoneResponse (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="020e2-105">PlayOnPhoneResponse (UM web service)</span></span>](playonphoneresponse-um-web-service.md)
  
```xml
<PlayOnPhoneResponse />
```

 <span data-ttu-id="020e2-106">**string**</span><span class="sxs-lookup"><span data-stu-id="020e2-106">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="020e2-107">属性および要素</span><span class="sxs-lookup"><span data-stu-id="020e2-107">Attributes and elements</span></span>

<span data-ttu-id="020e2-108">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="020e2-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="020e2-109">属性</span><span class="sxs-lookup"><span data-stu-id="020e2-109">Attributes</span></span>

<span data-ttu-id="020e2-110">なし。</span><span class="sxs-lookup"><span data-stu-id="020e2-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="020e2-111">子要素</span><span class="sxs-lookup"><span data-stu-id="020e2-111">Child elements</span></span>

<span data-ttu-id="020e2-112">なし。</span><span class="sxs-lookup"><span data-stu-id="020e2-112">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="020e2-113">親要素</span><span class="sxs-lookup"><span data-stu-id="020e2-113">Parent elements</span></span>

<span data-ttu-id="020e2-114">なし。</span><span class="sxs-lookup"><span data-stu-id="020e2-114">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="020e2-115">テキスト値</span><span class="sxs-lookup"><span data-stu-id="020e2-115">Text value</span></span>

<span data-ttu-id="020e2-116">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="020e2-116">A text value is required.</span></span> <span data-ttu-id="020e2-117">テキスト値は、 [GetCallInfo 操作 (UM web サービス)](getcallinfo-operation-um-web-service.md)の要求または[切断の操作 (UM web サービス)](disconnect-operation-um-web-service.md)要求の[CallId (UM web サービス)](callid-um-web-service.md)の値を使用する呼び出しの id です。</span><span class="sxs-lookup"><span data-stu-id="020e2-117">The text value is the call identifier to use for the value of [CallId (UM web service)](callid-um-web-service.md) in a [GetCallInfo operation (UM web service)](getcallinfo-operation-um-web-service.md) request or a [Disconnect operation (UM web service)](disconnect-operation-um-web-service.md) request.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="020e2-118">要素情報</span><span class="sxs-lookup"><span data-stu-id="020e2-118">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="020e2-119">名前空間</span><span class="sxs-lookup"><span data-stu-id="020e2-119">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="020e2-120">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="020e2-120">Schema Name</span></span>  <br/> |<span data-ttu-id="020e2-121">メッセージ</span><span class="sxs-lookup"><span data-stu-id="020e2-121">Messages</span></span>  <br/> |
|<span data-ttu-id="020e2-122">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="020e2-122">Validation File</span></span>  <br/> |<span data-ttu-id="020e2-123">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="020e2-123">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="020e2-124">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="020e2-124">Can be Empty</span></span>  <br/> |<span data-ttu-id="020e2-125">False</span><span class="sxs-lookup"><span data-stu-id="020e2-125">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="020e2-126">関連項目</span><span class="sxs-lookup"><span data-stu-id="020e2-126">See also</span></span>



[<span data-ttu-id="020e2-127">PlayOnPhone 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="020e2-127">PlayOnPhone operation (UM web service)</span></span>](playonphone-operation-um-web-service.md)

