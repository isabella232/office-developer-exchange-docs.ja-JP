---
title: Disconnect (UM web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- Disconnect
api_type:
- schema
ms.assetid: 2f8c1e8c-3bd4-4988-96b9-735c347b29f7
description: Disconnect 要素は、呼び出しを切断する要求を定義します。
ms.openlocfilehash: a00d957927a7a97d12c0d8c0c662956a18529cde
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458454"
---
# <a name="disconnect-um-web-service"></a><span data-ttu-id="93c68-103">Disconnect (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="93c68-103">Disconnect (UM web service)</span></span>

<span data-ttu-id="93c68-104">**Disconnect**要素は、呼び出しを切断する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="93c68-104">The **Disconnect** element defines a request to disconnect a call.</span></span> 
  
- [<span data-ttu-id="93c68-105">Disconnect (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="93c68-105">Disconnect (UM web service)</span></span>](disconnect-um-web-service.md)
  
```xml
<Disconnect>
  <CallId>   </CallId>
</Disconnect>
```

 <span data-ttu-id="93c68-106">**complexType**</span><span class="sxs-lookup"><span data-stu-id="93c68-106">**complexType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="93c68-107">属性と要素</span><span class="sxs-lookup"><span data-stu-id="93c68-107">Attributes and elements</span></span>

<span data-ttu-id="93c68-108">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="93c68-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="93c68-109">属性</span><span class="sxs-lookup"><span data-stu-id="93c68-109">Attributes</span></span>

<span data-ttu-id="93c68-110">なし。</span><span class="sxs-lookup"><span data-stu-id="93c68-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="93c68-111">子要素</span><span class="sxs-lookup"><span data-stu-id="93c68-111">Child elements</span></span>

|<span data-ttu-id="93c68-112">**Element**</span><span class="sxs-lookup"><span data-stu-id="93c68-112">**Element**</span></span>|<span data-ttu-id="93c68-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="93c68-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="93c68-114">CallId (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="93c68-114">CallId (UM web service)</span></span>](callid-um-web-service.md) <br/> |<span data-ttu-id="93c68-115">切断する呼び出しの識別子。</span><span class="sxs-lookup"><span data-stu-id="93c68-115">The identifier of the call to disconnect.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="93c68-116">親要素</span><span class="sxs-lookup"><span data-stu-id="93c68-116">Parent elements</span></span>

<span data-ttu-id="93c68-117">なし。</span><span class="sxs-lookup"><span data-stu-id="93c68-117">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="93c68-118">テキスト値</span><span class="sxs-lookup"><span data-stu-id="93c68-118">Text value</span></span>

<span data-ttu-id="93c68-119">なし。</span><span class="sxs-lookup"><span data-stu-id="93c68-119">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="93c68-120">要素の情報</span><span class="sxs-lookup"><span data-stu-id="93c68-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="93c68-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="93c68-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="93c68-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="93c68-122">Schema Name</span></span>  <br/> |<span data-ttu-id="93c68-123">メッセージ</span><span class="sxs-lookup"><span data-stu-id="93c68-123">Messages</span></span>  <br/> |
|<span data-ttu-id="93c68-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="93c68-124">Validation File</span></span>  <br/> |<span data-ttu-id="93c68-125">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="93c68-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="93c68-126">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="93c68-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="93c68-127">正しくない</span><span class="sxs-lookup"><span data-stu-id="93c68-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="93c68-128">関連項目</span><span class="sxs-lookup"><span data-stu-id="93c68-128">See also</span></span>

- [<span data-ttu-id="93c68-129">Disconnect 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="93c68-129">Disconnect operation (UM web service)</span></span>](disconnect-operation-um-web-service.md)  
- [<span data-ttu-id="93c68-130">PlayOnPhone 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="93c68-130">PlayOnPhone operation (UM web service)</span></span>](playonphone-operation-um-web-service.md) 
- [<span data-ttu-id="93c68-131">Playon電話案内応答操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="93c68-131">PlayOnPhoneGreeting operation (UM web service)</span></span>](playonphonegreeting-operation-um-web-service.md)  
- [<span data-ttu-id="93c68-132">CallId (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="93c68-132">CallId (UM web service)</span></span>](callid-um-web-service.md)

