---
title: PlayOnPhone (Exchange Web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PlayOnPhone
api_type:
- schema
ms.assetid: 486612be-470c-4f99-929a-f2b283e055c1
description: PlayOnPhone 要素は、電話のアイテムを読み取る要求を表します。
ms.openlocfilehash: e2c09a67255106ad9afddb86fa19b7a4a5762ee5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466249"
---
# <a name="playonphone-exchange-web-services"></a><span data-ttu-id="0b9cc-103">PlayOnPhone (Exchange Web サービス)</span><span class="sxs-lookup"><span data-stu-id="0b9cc-103">PlayOnPhone (Exchange Web Services)</span></span>

<span data-ttu-id="0b9cc-104">**Playonphone**要素は、電話のアイテムを読み取る要求を表します。</span><span class="sxs-lookup"><span data-stu-id="0b9cc-104">The **PlayOnPhone** element represents a request to read an item on a phone.</span></span> 
  
```xml
<PlayOnPhone>   <ItemId/>   <DialString/></PlayOnPhone>
```

 <span data-ttu-id="0b9cc-105">**PlayOnPhoneType**</span><span class="sxs-lookup"><span data-stu-id="0b9cc-105">**PlayOnPhoneType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0b9cc-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="0b9cc-106">Attributes and elements</span></span>

<span data-ttu-id="0b9cc-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0b9cc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0b9cc-108">属性</span><span class="sxs-lookup"><span data-stu-id="0b9cc-108">Attributes</span></span>

<span data-ttu-id="0b9cc-109">なし。</span><span class="sxs-lookup"><span data-stu-id="0b9cc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0b9cc-110">子要素</span><span class="sxs-lookup"><span data-stu-id="0b9cc-110">Child elements</span></span>

|<span data-ttu-id="0b9cc-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="0b9cc-111">**Element**</span></span>|<span data-ttu-id="0b9cc-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="0b9cc-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0b9cc-113">ItemId</span><span class="sxs-lookup"><span data-stu-id="0b9cc-113">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="0b9cc-114">電話で再生するアイテムの id を表します。</span><span class="sxs-lookup"><span data-stu-id="0b9cc-114">Represents the identifier of an item to play on a phone.</span></span> <span data-ttu-id="0b9cc-115">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="0b9cc-115">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="0b9cc-116">の方法 (Exchange Web サービス)</span><span class="sxs-lookup"><span data-stu-id="0b9cc-116">DialString (Exchange Web Services)</span></span>](dialstring-exchange-web-services.md) <br/> |<span data-ttu-id="0b9cc-117">電話でアイテムを再生するために呼び出される電話番号のダイヤル文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="0b9cc-117">Represents the dial string of the phone number that is called to play an item by phone.</span></span> <span data-ttu-id="0b9cc-118">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="0b9cc-118">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0b9cc-119">親要素</span><span class="sxs-lookup"><span data-stu-id="0b9cc-119">Parent elements</span></span>

<span data-ttu-id="0b9cc-120">なし。</span><span class="sxs-lookup"><span data-stu-id="0b9cc-120">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0b9cc-121">注釈</span><span class="sxs-lookup"><span data-stu-id="0b9cc-121">Remarks</span></span>

<span data-ttu-id="0b9cc-122">この要素を記述するスキーマは、Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="0b9cc-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0b9cc-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="0b9cc-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0b9cc-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="0b9cc-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0b9cc-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0b9cc-125">Schema Name</span></span>  <br/> |<span data-ttu-id="0b9cc-126">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="0b9cc-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0b9cc-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0b9cc-127">Validation File</span></span>  <br/> |<span data-ttu-id="0b9cc-128">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="0b9cc-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0b9cc-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="0b9cc-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="0b9cc-130">正しくない</span><span class="sxs-lookup"><span data-stu-id="0b9cc-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0b9cc-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="0b9cc-131">See also</span></span>



- [<span data-ttu-id="0b9cc-132">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="0b9cc-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

