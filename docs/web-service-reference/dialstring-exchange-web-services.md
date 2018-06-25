---
title: DialString (Exchange Web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DialString
api_type:
- schema
ms.assetid: 077501f6-b3a8-4799-8c37-09e77af49ddb
description: DialString 要素は、項目を再生するのには電話で呼び出される電話番号のダイヤル文字列を表します。 この要素は必須です。
ms.openlocfilehash: a2b9a12e714d29923402e4d5563c26b6b2d5f632
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760032"
---
# <a name="dialstring-exchange-web-services"></a><span data-ttu-id="fb6c4-104">DialString (Exchange Web サービス)</span><span class="sxs-lookup"><span data-stu-id="fb6c4-104">DialString (Exchange Web Services)</span></span>

<span data-ttu-id="fb6c4-105">**DialString**要素は、項目を再生するのには電話で呼び出される電話番号のダイヤル文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="fb6c4-105">The **DialString** element represents the dial string of the telephone number that is called to play an item by telephone.</span></span> <span data-ttu-id="fb6c4-106">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="fb6c4-106">This element is required.</span></span> 
  
```xml
<DialString/>
```

 <span data-ttu-id="fb6c4-107">**string**</span><span class="sxs-lookup"><span data-stu-id="fb6c4-107">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fb6c4-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="fb6c4-108">Attributes and elements</span></span>

<span data-ttu-id="fb6c4-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="fb6c4-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fb6c4-110">属性</span><span class="sxs-lookup"><span data-stu-id="fb6c4-110">Attributes</span></span>

<span data-ttu-id="fb6c4-111">なし。</span><span class="sxs-lookup"><span data-stu-id="fb6c4-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fb6c4-112">子要素</span><span class="sxs-lookup"><span data-stu-id="fb6c4-112">Child elements</span></span>

<span data-ttu-id="fb6c4-113">なし。</span><span class="sxs-lookup"><span data-stu-id="fb6c4-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fb6c4-114">親要素</span><span class="sxs-lookup"><span data-stu-id="fb6c4-114">Parent elements</span></span>

|<span data-ttu-id="fb6c4-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="fb6c4-115">**Element**</span></span>|<span data-ttu-id="fb6c4-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="fb6c4-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fb6c4-117">PlayOnPhone (Exchange Web サービス)</span><span class="sxs-lookup"><span data-stu-id="fb6c4-117">PlayOnPhone (Exchange Web Services)</span></span>](playonphone-exchange-web-services.md) <br/> |<span data-ttu-id="fb6c4-118">電話上のアイテムの読み取り要求を表します。</span><span class="sxs-lookup"><span data-stu-id="fb6c4-118">Represents a request to read an item on a telephone.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="fb6c4-119">備考</span><span class="sxs-lookup"><span data-stu-id="fb6c4-119">Remarks</span></span>

<span data-ttu-id="fb6c4-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="fb6c4-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fb6c4-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="fb6c4-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fb6c4-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="fb6c4-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="fb6c4-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="fb6c4-123">Schema Name</span></span>  <br/> |<span data-ttu-id="fb6c4-124">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="fb6c4-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="fb6c4-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="fb6c4-125">Validation File</span></span>  <br/> |<span data-ttu-id="fb6c4-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="fb6c4-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fb6c4-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="fb6c4-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="fb6c4-128">False</span><span class="sxs-lookup"><span data-stu-id="fb6c4-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fb6c4-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="fb6c4-129">See also</span></span>

- [<span data-ttu-id="fb6c4-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="fb6c4-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

