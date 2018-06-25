---
title: RoutingType (EmailAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RoutingType
api_type:
- schema
ms.assetid: 683216be-9972-4f48-a148-c34bfe7f53e5
description: RoutingType 要素は、メールボックスのアドレスの種類を定義します。
ms.openlocfilehash: a02c3b5711a657311428d67cccabd9c8c231db67
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833256"
---
# <a name="routingtype-emailaddresstype"></a><span data-ttu-id="befa5-103">RoutingType (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="befa5-103">RoutingType (EmailAddressType)</span></span>

<span data-ttu-id="befa5-104">**RoutingType**要素は、メールボックスのアドレスの種類を定義します。</span><span class="sxs-lookup"><span data-stu-id="befa5-104">The **RoutingType** element defines the address type for the mailbox.</span></span> 
  
```XML
<RoutingType/>
```

 <span data-ttu-id="befa5-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="befa5-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="befa5-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="befa5-106">Attributes and elements</span></span>

<span data-ttu-id="befa5-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="befa5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="befa5-108">属性</span><span class="sxs-lookup"><span data-stu-id="befa5-108">Attributes</span></span>

<span data-ttu-id="befa5-109">なし。</span><span class="sxs-lookup"><span data-stu-id="befa5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="befa5-110">子要素</span><span class="sxs-lookup"><span data-stu-id="befa5-110">Child elements</span></span>

<span data-ttu-id="befa5-111">なし。</span><span class="sxs-lookup"><span data-stu-id="befa5-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="befa5-112">親要素</span><span class="sxs-lookup"><span data-stu-id="befa5-112">Parent elements</span></span>

|<span data-ttu-id="befa5-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="befa5-113">**Element**</span></span>|<span data-ttu-id="befa5-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="befa5-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="befa5-115">ActingAs</span><span class="sxs-lookup"><span data-stu-id="befa5-115">ActingAs</span></span>](actingas.md) <br/> |<span data-ttu-id="befa5-116">として送信する呼び出し元を識別します。</span><span class="sxs-lookup"><span data-stu-id="befa5-116">Identifies who the caller is sending as.</span></span>  <br/> |
|[<span data-ttu-id="befa5-117">メールボックス</span><span class="sxs-lookup"><span data-stu-id="befa5-117">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="befa5-118">完全に解決された電子メール アドレスを識別します。</span><span class="sxs-lookup"><span data-stu-id="befa5-118">Identifies a fully resolved e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="befa5-119">RoomList</span><span class="sxs-lookup"><span data-stu-id="befa5-119">RoomList</span></span>](roomlist.md) <br/> |<span data-ttu-id="befa5-120">会議室の一覧を識別します。</span><span class="sxs-lookup"><span data-stu-id="befa5-120">Identifies a list of meeting rooms.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="befa5-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="befa5-121">Text value</span></span>

<span data-ttu-id="befa5-122">テキスト値は、ルーティングの種類を表します。</span><span class="sxs-lookup"><span data-stu-id="befa5-122">The text value represents a routing type.</span></span> <span data-ttu-id="befa5-123">SMTP は、この要素の一般的なテキスト値です。</span><span class="sxs-lookup"><span data-stu-id="befa5-123">SMTP is the typical text value for this element.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="befa5-124">備考</span><span class="sxs-lookup"><span data-stu-id="befa5-124">Remarks</span></span>

<span data-ttu-id="befa5-125">この要素は、[メールボックス](mailbox.md)の要素では省略可能です。</span><span class="sxs-lookup"><span data-stu-id="befa5-125">This element is optional in the [Mailbox](mailbox.md) element.</span></span> <span data-ttu-id="befa5-126">[RoutingType (EmailAddress)](routingtype-emailaddress.md)の別の要素は、可用性の操作に使用されます。</span><span class="sxs-lookup"><span data-stu-id="befa5-126">Another [RoutingType (EmailAddress)](routingtype-emailaddress.md) element is used for Availability operations.</span></span> 
  
<span data-ttu-id="befa5-127">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="befa5-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="befa5-128">要素情報</span><span class="sxs-lookup"><span data-stu-id="befa5-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="befa5-129">名前空間</span><span class="sxs-lookup"><span data-stu-id="befa5-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="befa5-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="befa5-130">Schema Name</span></span>  <br/> |<span data-ttu-id="befa5-131">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="befa5-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="befa5-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="befa5-132">Validation File</span></span>  <br/> |<span data-ttu-id="befa5-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="befa5-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="befa5-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="befa5-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="befa5-135">False</span><span class="sxs-lookup"><span data-stu-id="befa5-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="befa5-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="befa5-136">See also</span></span>



- [<span data-ttu-id="befa5-137">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="befa5-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

