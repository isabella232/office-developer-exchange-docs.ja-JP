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
ms.openlocfilehash: d4229f2857a5c99cc9bb7ff9b9b103de099a0055
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465087"
---
# <a name="routingtype-emailaddresstype"></a><span data-ttu-id="e4732-103">RoutingType (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="e4732-103">RoutingType (EmailAddressType)</span></span>

<span data-ttu-id="e4732-104">**Routingtype**要素は、メールボックスのアドレスの種類を定義します。</span><span class="sxs-lookup"><span data-stu-id="e4732-104">The **RoutingType** element defines the address type for the mailbox.</span></span> 
  
```XML
<RoutingType/>
```

 <span data-ttu-id="e4732-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="e4732-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e4732-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="e4732-106">Attributes and elements</span></span>

<span data-ttu-id="e4732-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e4732-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e4732-108">属性</span><span class="sxs-lookup"><span data-stu-id="e4732-108">Attributes</span></span>

<span data-ttu-id="e4732-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e4732-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e4732-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e4732-110">Child elements</span></span>

<span data-ttu-id="e4732-111">なし。</span><span class="sxs-lookup"><span data-stu-id="e4732-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e4732-112">親要素</span><span class="sxs-lookup"><span data-stu-id="e4732-112">Parent elements</span></span>

|<span data-ttu-id="e4732-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="e4732-113">**Element**</span></span>|<span data-ttu-id="e4732-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="e4732-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e4732-115">ActingAs</span><span class="sxs-lookup"><span data-stu-id="e4732-115">ActingAs</span></span>](actingas.md) <br/> |<span data-ttu-id="e4732-116">発信者が送信者として送信しているユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="e4732-116">Identifies who the caller is sending as.</span></span>  <br/> |
|[<span data-ttu-id="e4732-117">メールボックス</span><span class="sxs-lookup"><span data-stu-id="e4732-117">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="e4732-118">完全に解決された電子メールアドレスを識別します。</span><span class="sxs-lookup"><span data-stu-id="e4732-118">Identifies a fully resolved e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="e4732-119">RoomList</span><span class="sxs-lookup"><span data-stu-id="e4732-119">RoomList</span></span>](roomlist.md) <br/> |<span data-ttu-id="e4732-120">会議室のリストを識別します。</span><span class="sxs-lookup"><span data-stu-id="e4732-120">Identifies a list of meeting rooms.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e4732-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="e4732-121">Text value</span></span>

<span data-ttu-id="e4732-122">Text 値は、ルーティングの種類を表します。</span><span class="sxs-lookup"><span data-stu-id="e4732-122">The text value represents a routing type.</span></span> <span data-ttu-id="e4732-123">SMTP は、この要素の通常のテキスト値です。</span><span class="sxs-lookup"><span data-stu-id="e4732-123">SMTP is the typical text value for this element.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e4732-124">注釈</span><span class="sxs-lookup"><span data-stu-id="e4732-124">Remarks</span></span>

<span data-ttu-id="e4732-125">この要素は、 [Mailbox](mailbox.md)要素では省略可能です。</span><span class="sxs-lookup"><span data-stu-id="e4732-125">This element is optional in the [Mailbox](mailbox.md) element.</span></span> <span data-ttu-id="e4732-126">別の[Routingtype (EmailAddress)](routingtype-emailaddress.md)要素は、可用性の操作に使用されます。</span><span class="sxs-lookup"><span data-stu-id="e4732-126">Another [RoutingType (EmailAddress)](routingtype-emailaddress.md) element is used for Availability operations.</span></span> 
  
<span data-ttu-id="e4732-127">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="e4732-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e4732-128">要素の情報</span><span class="sxs-lookup"><span data-stu-id="e4732-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e4732-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="e4732-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e4732-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e4732-130">Schema Name</span></span>  <br/> |<span data-ttu-id="e4732-131">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="e4732-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="e4732-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e4732-132">Validation File</span></span>  <br/> |<span data-ttu-id="e4732-133">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="e4732-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e4732-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="e4732-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="e4732-135">正しくない</span><span class="sxs-lookup"><span data-stu-id="e4732-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e4732-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="e4732-136">See also</span></span>



- [<span data-ttu-id="e4732-137">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="e4732-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

