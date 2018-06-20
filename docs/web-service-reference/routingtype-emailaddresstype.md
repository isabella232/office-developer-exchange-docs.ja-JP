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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833256"
---
# <a name="routingtype-emailaddresstype"></a><span data-ttu-id="5c686-103">RoutingType (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="5c686-103">RoutingType (EmailAddressType)</span></span>

<span data-ttu-id="5c686-104">**RoutingType**要素は、メールボックスのアドレスの種類を定義します。</span><span class="sxs-lookup"><span data-stu-id="5c686-104">The **RoutingType** element defines the address type for the mailbox.</span></span> 
  
```XML
<RoutingType/>
```

 <span data-ttu-id="5c686-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="5c686-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5c686-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="5c686-106">Attributes and elements</span></span>

<span data-ttu-id="5c686-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5c686-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5c686-108">属性</span><span class="sxs-lookup"><span data-stu-id="5c686-108">Attributes</span></span>

<span data-ttu-id="5c686-109">なし。</span><span class="sxs-lookup"><span data-stu-id="5c686-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5c686-110">子要素</span><span class="sxs-lookup"><span data-stu-id="5c686-110">Child elements</span></span>

<span data-ttu-id="5c686-111">なし。</span><span class="sxs-lookup"><span data-stu-id="5c686-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5c686-112">親要素</span><span class="sxs-lookup"><span data-stu-id="5c686-112">Parent elements</span></span>

|<span data-ttu-id="5c686-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="5c686-113">**Element**</span></span>|<span data-ttu-id="5c686-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="5c686-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5c686-115">ActingAs</span><span class="sxs-lookup"><span data-stu-id="5c686-115">ActingAs</span></span>](actingas.md) <br/> |<span data-ttu-id="5c686-116">として送信する呼び出し元を識別します。</span><span class="sxs-lookup"><span data-stu-id="5c686-116">Identifies who the caller is sending as.</span></span>  <br/> |
|[<span data-ttu-id="5c686-117">メールボックス</span><span class="sxs-lookup"><span data-stu-id="5c686-117">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="5c686-118">完全に解決された電子メール アドレスを識別します。</span><span class="sxs-lookup"><span data-stu-id="5c686-118">Identifies a fully resolved e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="5c686-119">RoomList</span><span class="sxs-lookup"><span data-stu-id="5c686-119">RoomList</span></span>](roomlist.md) <br/> |<span data-ttu-id="5c686-120">会議室の一覧を識別します。</span><span class="sxs-lookup"><span data-stu-id="5c686-120">Identifies a list of meeting rooms.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5c686-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="5c686-121">Text value</span></span>

<span data-ttu-id="5c686-122">テキスト値は、ルーティングの種類を表します。</span><span class="sxs-lookup"><span data-stu-id="5c686-122">The text value represents a routing type.</span></span> <span data-ttu-id="5c686-123">SMTP は、この要素の一般的なテキスト値です。</span><span class="sxs-lookup"><span data-stu-id="5c686-123">SMTP is the typical text value for this element.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5c686-124">備考</span><span class="sxs-lookup"><span data-stu-id="5c686-124">Remarks</span></span>

<span data-ttu-id="5c686-125">この要素は、[メールボックス](mailbox.md)の要素では省略可能です。</span><span class="sxs-lookup"><span data-stu-id="5c686-125">This element is optional in the [Mailbox](mailbox.md) element.</span></span> <span data-ttu-id="5c686-126">[RoutingType (EmailAddress)](routingtype-emailaddress.md)の別の要素は、可用性の操作に使用されます。</span><span class="sxs-lookup"><span data-stu-id="5c686-126">Another [RoutingType (EmailAddress)](routingtype-emailaddress.md) element is used for Availability operations.</span></span> 
  
<span data-ttu-id="5c686-127">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="5c686-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5c686-128">要素情報</span><span class="sxs-lookup"><span data-stu-id="5c686-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5c686-129">名前空間</span><span class="sxs-lookup"><span data-stu-id="5c686-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5c686-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5c686-130">Schema Name</span></span>  <br/> |<span data-ttu-id="5c686-131">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="5c686-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="5c686-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5c686-132">Validation File</span></span>  <br/> |<span data-ttu-id="5c686-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5c686-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5c686-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="5c686-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="5c686-135">False</span><span class="sxs-lookup"><span data-stu-id="5c686-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5c686-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="5c686-136">See also</span></span>



- [<span data-ttu-id="5c686-137">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="5c686-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

