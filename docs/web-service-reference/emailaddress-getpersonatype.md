---
title: EmailAddress (GetPersonaType)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 052055b5-4630-40ed-9b24-9e7f4bf7ba1d
description: EmailAddress (GetPersonaType) の要素では、ペルソナに関連付けられている電子メール アドレスを指定します。
ms.openlocfilehash: a28a4a61a9719875fe99e1c950bcd3ec3af9ab13
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760217"
---
# <a name="emailaddress-getpersonatype"></a><span data-ttu-id="49cc9-103">EmailAddress (GetPersonaType)</span><span class="sxs-lookup"><span data-stu-id="49cc9-103">EmailAddress (GetPersonaType)</span></span>

<span data-ttu-id="49cc9-104">**EmailAddress (GetPersonaType)** の要素では、ペルソナに関連付けられている電子メール アドレスを指定します。</span><span class="sxs-lookup"><span data-stu-id="49cc9-104">The **EmailAddress (GetPersonaType)** element specifies the email address associated with the persona.</span></span> 
  
```XML
<EmailAddress>
    <Name></Name>
    <EmailAddress></EmailAddress>
    <RoutingType></RoutingType>
    <MailboxType></MailboxType>
    <ItemId></ItemId>
    <OriginalDisplayName></OriginalDisplayName>
</EmailAddress>>
```

 <span data-ttu-id="49cc9-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="49cc9-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="49cc9-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="49cc9-106">Attributes and elements</span></span>

<span data-ttu-id="49cc9-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="49cc9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="49cc9-108">属性</span><span class="sxs-lookup"><span data-stu-id="49cc9-108">Attributes</span></span>

<span data-ttu-id="49cc9-109">なし。</span><span class="sxs-lookup"><span data-stu-id="49cc9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="49cc9-110">子要素</span><span class="sxs-lookup"><span data-stu-id="49cc9-110">Child elements</span></span>

<span data-ttu-id="49cc9-111">[名 (文字列)](name-string.md) | [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) | [RoutingType (EmailAddressType)](routingtype-emailaddresstype.md) | [MailboxType](mailboxtype.md) | [アイテム Id](itemid.md) | [OriginalDisplayName](originaldisplayname.md)</span><span class="sxs-lookup"><span data-stu-id="49cc9-111">[Name (string)](name-string.md) | [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) | [RoutingType (EmailAddressType)](routingtype-emailaddresstype.md) | [MailboxType](mailboxtype.md) | [ItemId](itemid.md) | [OriginalDisplayName](originaldisplayname.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="49cc9-112">親要素</span><span class="sxs-lookup"><span data-stu-id="49cc9-112">Parent elements</span></span>

[<span data-ttu-id="49cc9-113">GetPersona</span><span class="sxs-lookup"><span data-stu-id="49cc9-113">GetPersona</span></span>](getpersona.md)
  
## <a name="remarks"></a><span data-ttu-id="49cc9-114">備考</span><span class="sxs-lookup"><span data-stu-id="49cc9-114">Remarks</span></span>

<span data-ttu-id="49cc9-115">この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="49cc9-115">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="49cc9-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="49cc9-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="49cc9-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="49cc9-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="49cc9-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="49cc9-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="49cc9-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="49cc9-119">Schema Name</span></span>  <br/> |<span data-ttu-id="49cc9-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="49cc9-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="49cc9-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="49cc9-121">Validation File</span></span>  <br/> |<span data-ttu-id="49cc9-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="49cc9-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="49cc9-123">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="49cc9-123">Can be Empty</span></span>  <br/> |<span data-ttu-id="49cc9-124">True</span><span class="sxs-lookup"><span data-stu-id="49cc9-124">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="49cc9-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="49cc9-125">See also</span></span>

- [<span data-ttu-id="49cc9-126">GetPersona</span><span class="sxs-lookup"><span data-stu-id="49cc9-126">GetPersona</span></span>](getpersona.md)
- [<span data-ttu-id="49cc9-127">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="49cc9-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

