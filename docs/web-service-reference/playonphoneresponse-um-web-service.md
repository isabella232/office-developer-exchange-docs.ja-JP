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
description: PlayOnPhoneResponse 要素は、PlayOnPhone 操作 (UM web サービス) 要求への応答を定義します。
ms.openlocfilehash: ddb9cc9a8feaeb476e6502339fdc74d024797b9b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459617"
---
# <a name="playonphoneresponse-um-web-service"></a><span data-ttu-id="629f0-103">PlayOnPhoneResponse (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="629f0-103">PlayOnPhoneResponse (UM web service)</span></span>

<span data-ttu-id="629f0-104">**PlayOnPhoneResponse**要素は、 [playonphone 操作 (UM web サービス)](playonphone-operation-um-web-service.md)要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="629f0-104">The **PlayOnPhoneResponse** element defines a response to a [PlayOnPhone operation (UM web service)](playonphone-operation-um-web-service.md) request.</span></span> 
  
[<span data-ttu-id="629f0-105">PlayOnPhoneResponse (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="629f0-105">PlayOnPhoneResponse (UM web service)</span></span>](playonphoneresponse-um-web-service.md)
  
```xml
<PlayOnPhoneResponse />
```

 <span data-ttu-id="629f0-106">**string**</span><span class="sxs-lookup"><span data-stu-id="629f0-106">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="629f0-107">属性と要素</span><span class="sxs-lookup"><span data-stu-id="629f0-107">Attributes and elements</span></span>

<span data-ttu-id="629f0-108">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="629f0-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="629f0-109">属性</span><span class="sxs-lookup"><span data-stu-id="629f0-109">Attributes</span></span>

<span data-ttu-id="629f0-110">なし。</span><span class="sxs-lookup"><span data-stu-id="629f0-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="629f0-111">子要素</span><span class="sxs-lookup"><span data-stu-id="629f0-111">Child elements</span></span>

<span data-ttu-id="629f0-112">なし。</span><span class="sxs-lookup"><span data-stu-id="629f0-112">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="629f0-113">親要素</span><span class="sxs-lookup"><span data-stu-id="629f0-113">Parent elements</span></span>

<span data-ttu-id="629f0-114">なし。</span><span class="sxs-lookup"><span data-stu-id="629f0-114">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="629f0-115">テキスト値</span><span class="sxs-lookup"><span data-stu-id="629f0-115">Text value</span></span>

<span data-ttu-id="629f0-116">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="629f0-116">A text value is required.</span></span> <span data-ttu-id="629f0-117">テキスト値は、 [Getcallinfo 操作 (um web](getcallinfo-operation-um-web-service.md)サービス) 要求または[切断操作 (um web サービス)](disconnect-operation-um-web-service.md)要求の[callid (um web サービス)](callid-um-web-service.md)の値として使用する呼び出し識別子です。</span><span class="sxs-lookup"><span data-stu-id="629f0-117">The text value is the call identifier to use for the value of [CallId (UM web service)](callid-um-web-service.md) in a [GetCallInfo operation (UM web service)](getcallinfo-operation-um-web-service.md) request or a [Disconnect operation (UM web service)](disconnect-operation-um-web-service.md) request.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="629f0-118">要素の情報</span><span class="sxs-lookup"><span data-stu-id="629f0-118">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="629f0-119">Namespace</span><span class="sxs-lookup"><span data-stu-id="629f0-119">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="629f0-120">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="629f0-120">Schema Name</span></span>  <br/> |<span data-ttu-id="629f0-121">メッセージ</span><span class="sxs-lookup"><span data-stu-id="629f0-121">Messages</span></span>  <br/> |
|<span data-ttu-id="629f0-122">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="629f0-122">Validation File</span></span>  <br/> |<span data-ttu-id="629f0-123">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="629f0-123">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="629f0-124">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="629f0-124">Can be Empty</span></span>  <br/> |<span data-ttu-id="629f0-125">正しくない</span><span class="sxs-lookup"><span data-stu-id="629f0-125">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="629f0-126">関連項目</span><span class="sxs-lookup"><span data-stu-id="629f0-126">See also</span></span>



[<span data-ttu-id="629f0-127">PlayOnPhone 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="629f0-127">PlayOnPhone operation (UM web service)</span></span>](playonphone-operation-um-web-service.md)

