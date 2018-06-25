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
description: PlayOnPhone 要素は、携帯電話上のアイテムの読み取り要求を表します。
ms.openlocfilehash: 75493a31940ea609fd6cf454e91ca5881fb7e678
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832816"
---
# <a name="playonphone-exchange-web-services"></a><span data-ttu-id="6cc12-103">PlayOnPhone (Exchange Web サービス)</span><span class="sxs-lookup"><span data-stu-id="6cc12-103">PlayOnPhone (Exchange Web Services)</span></span>

<span data-ttu-id="6cc12-104">**PlayOnPhone**要素は、携帯電話上のアイテムの読み取り要求を表します。</span><span class="sxs-lookup"><span data-stu-id="6cc12-104">The **PlayOnPhone** element represents a request to read an item on a phone.</span></span> 
  
```xml
<PlayOnPhone>   <ItemId/>   <DialString/></PlayOnPhone>
```

 <span data-ttu-id="6cc12-105">**PlayOnPhoneType**</span><span class="sxs-lookup"><span data-stu-id="6cc12-105">**PlayOnPhoneType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6cc12-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="6cc12-106">Attributes and elements</span></span>

<span data-ttu-id="6cc12-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6cc12-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6cc12-108">属性</span><span class="sxs-lookup"><span data-stu-id="6cc12-108">Attributes</span></span>

<span data-ttu-id="6cc12-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6cc12-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6cc12-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6cc12-110">Child elements</span></span>

|<span data-ttu-id="6cc12-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="6cc12-111">**Element**</span></span>|<span data-ttu-id="6cc12-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="6cc12-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6cc12-113">ItemId</span><span class="sxs-lookup"><span data-stu-id="6cc12-113">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="6cc12-114">[電話で再生する項目の識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="6cc12-114">Represents the identifier of an item to play on a phone.</span></span> <span data-ttu-id="6cc12-115">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="6cc12-115">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="6cc12-116">DialString (Exchange Web サービス)</span><span class="sxs-lookup"><span data-stu-id="6cc12-116">DialString (Exchange Web Services)</span></span>](dialstring-exchange-web-services.md) <br/> |<span data-ttu-id="6cc12-117">項目を再生するのには電話で呼び出される電話番号のダイヤル文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="6cc12-117">Represents the dial string of the phone number that is called to play an item by phone.</span></span> <span data-ttu-id="6cc12-118">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="6cc12-118">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6cc12-119">親要素</span><span class="sxs-lookup"><span data-stu-id="6cc12-119">Parent elements</span></span>

<span data-ttu-id="6cc12-120">なし。</span><span class="sxs-lookup"><span data-stu-id="6cc12-120">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6cc12-121">備考</span><span class="sxs-lookup"><span data-stu-id="6cc12-121">Remarks</span></span>

<span data-ttu-id="6cc12-122">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="6cc12-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6cc12-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="6cc12-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6cc12-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="6cc12-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6cc12-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6cc12-125">Schema Name</span></span>  <br/> |<span data-ttu-id="6cc12-126">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="6cc12-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6cc12-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6cc12-127">Validation File</span></span>  <br/> |<span data-ttu-id="6cc12-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6cc12-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6cc12-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="6cc12-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="6cc12-130">False</span><span class="sxs-lookup"><span data-stu-id="6cc12-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6cc12-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="6cc12-131">See also</span></span>



- [<span data-ttu-id="6cc12-132">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="6cc12-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

