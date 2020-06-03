---
title: EmailAddress (Get個人 Atype)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 052055b5-4630-40ed-9b24-9e7f4bf7ba1d
description: EmailAddress (Get個人 Atype) 要素は、ペルソナに関連付けられている電子メールアドレスを指定します。
ms.openlocfilehash: b58f61202cd94ff282b21138b47b40887b38752a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463455"
---
# <a name="emailaddress-getpersonatype"></a><span data-ttu-id="489f3-103">EmailAddress (Get個人 Atype)</span><span class="sxs-lookup"><span data-stu-id="489f3-103">EmailAddress (GetPersonaType)</span></span>

<span data-ttu-id="489f3-104">**EmailAddress (Get個人 atype)** 要素は、ペルソナに関連付けられている電子メールアドレスを指定します。</span><span class="sxs-lookup"><span data-stu-id="489f3-104">The **EmailAddress (GetPersonaType)** element specifies the email address associated with the persona.</span></span> 
  
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

 <span data-ttu-id="489f3-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="489f3-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="489f3-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="489f3-106">Attributes and elements</span></span>

<span data-ttu-id="489f3-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="489f3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="489f3-108">属性</span><span class="sxs-lookup"><span data-stu-id="489f3-108">Attributes</span></span>

<span data-ttu-id="489f3-109">なし。</span><span class="sxs-lookup"><span data-stu-id="489f3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="489f3-110">子要素</span><span class="sxs-lookup"><span data-stu-id="489f3-110">Child elements</span></span>

<span data-ttu-id="489f3-111">[Name (string)](name-string.md)  | [EmailAddress (非 Emptystringtype)](emailaddress-nonemptystringtype.md)  | [Routingtype (EmailAddressType)](routingtype-emailaddresstype.md)  | [MailboxType](mailboxtype.md)  | [ItemId](itemid.md)  | [Originaldisplayname](originaldisplayname.md)</span><span class="sxs-lookup"><span data-stu-id="489f3-111">[Name (string)](name-string.md) | [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) | [RoutingType (EmailAddressType)](routingtype-emailaddresstype.md) | [MailboxType](mailboxtype.md) | [ItemId](itemid.md) | [OriginalDisplayName](originaldisplayname.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="489f3-112">親要素</span><span class="sxs-lookup"><span data-stu-id="489f3-112">Parent elements</span></span>

[<span data-ttu-id="489f3-113">GetPersona</span><span class="sxs-lookup"><span data-stu-id="489f3-113">GetPersona</span></span>](getpersona.md)
  
## <a name="remarks"></a><span data-ttu-id="489f3-114">注釈</span><span class="sxs-lookup"><span data-stu-id="489f3-114">Remarks</span></span>

<span data-ttu-id="489f3-115">この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="489f3-115">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="489f3-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="489f3-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="489f3-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="489f3-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="489f3-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="489f3-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="489f3-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="489f3-119">Schema Name</span></span>  <br/> |<span data-ttu-id="489f3-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="489f3-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="489f3-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="489f3-121">Validation File</span></span>  <br/> |<span data-ttu-id="489f3-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="489f3-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="489f3-123">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="489f3-123">Can be Empty</span></span>  <br/> |<span data-ttu-id="489f3-124">正しい</span><span class="sxs-lookup"><span data-stu-id="489f3-124">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="489f3-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="489f3-125">See also</span></span>

- [<span data-ttu-id="489f3-126">GetPersona</span><span class="sxs-lookup"><span data-stu-id="489f3-126">GetPersona</span></span>](getpersona.md)
- [<span data-ttu-id="489f3-127">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="489f3-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

