---
title: の方法 (Exchange Web サービス)
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
description: Dial String 要素は、電話でアイテムを再生するために呼び出される電話番号のダイヤル文字列を表します。 この要素は必須です。
ms.openlocfilehash: c944c9f6b99f7f8d45f7e08442a7dfb55a5fe9f3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458748"
---
# <a name="dialstring-exchange-web-services"></a><span data-ttu-id="83492-104">の方法 (Exchange Web サービス)</span><span class="sxs-lookup"><span data-stu-id="83492-104">DialString (Exchange Web Services)</span></span>

<span data-ttu-id="83492-105">Dial **string**要素は、電話でアイテムを再生するために呼び出される電話番号のダイヤル文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="83492-105">The **DialString** element represents the dial string of the telephone number that is called to play an item by telephone.</span></span> <span data-ttu-id="83492-106">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="83492-106">This element is required.</span></span> 
  
```xml
<DialString/>
```

 <span data-ttu-id="83492-107">**string**</span><span class="sxs-lookup"><span data-stu-id="83492-107">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="83492-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="83492-108">Attributes and elements</span></span>

<span data-ttu-id="83492-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="83492-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="83492-110">属性</span><span class="sxs-lookup"><span data-stu-id="83492-110">Attributes</span></span>

<span data-ttu-id="83492-111">なし。</span><span class="sxs-lookup"><span data-stu-id="83492-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="83492-112">子要素</span><span class="sxs-lookup"><span data-stu-id="83492-112">Child elements</span></span>

<span data-ttu-id="83492-113">なし。</span><span class="sxs-lookup"><span data-stu-id="83492-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="83492-114">親要素</span><span class="sxs-lookup"><span data-stu-id="83492-114">Parent elements</span></span>

|<span data-ttu-id="83492-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="83492-115">**Element**</span></span>|<span data-ttu-id="83492-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="83492-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="83492-117">PlayOnPhone (Exchange Web サービス)</span><span class="sxs-lookup"><span data-stu-id="83492-117">PlayOnPhone (Exchange Web Services)</span></span>](playonphone-exchange-web-services.md) <br/> |<span data-ttu-id="83492-118">電話のアイテムを読み取るための要求を表します。</span><span class="sxs-lookup"><span data-stu-id="83492-118">Represents a request to read an item on a telephone.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="83492-119">注釈</span><span class="sxs-lookup"><span data-stu-id="83492-119">Remarks</span></span>

<span data-ttu-id="83492-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="83492-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="83492-121">要素の情報</span><span class="sxs-lookup"><span data-stu-id="83492-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="83492-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="83492-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="83492-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="83492-123">Schema Name</span></span>  <br/> |<span data-ttu-id="83492-124">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="83492-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="83492-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="83492-125">Validation File</span></span>  <br/> |<span data-ttu-id="83492-126">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="83492-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="83492-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="83492-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="83492-128">正しくない</span><span class="sxs-lookup"><span data-stu-id="83492-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="83492-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="83492-129">See also</span></span>

- [<span data-ttu-id="83492-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="83492-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

