---
title: 値 (EmailAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 24eaa473-0024-47e2-b7d2-051d5dd4f53c
description: Value 要素は、attributions 配列に関連付けられている EmailAddress の値を指定します。
ms.openlocfilehash: 45af2aaab7d2475ae46ae24ed13b1435f5b352c6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467600"
---
# <a name="value-emailaddresstype"></a><span data-ttu-id="4a963-103">値 (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="4a963-103">Value (EmailAddressType)</span></span>

<span data-ttu-id="4a963-104">**Value**要素は、attributions 配列に関連付けられている**EmailAddress**の値を指定します。</span><span class="sxs-lookup"><span data-stu-id="4a963-104">The **Value** element specifies the value of an **EmailAddress** associated with an attributions array.</span></span> 
  
```XML
<Value>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
   <OriginalDisplayName/>
</Value>
```

<span data-ttu-id="4a963-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="4a963-105">**EmailAddressType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="4a963-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="4a963-106">Attributes and elements</span></span>

<span data-ttu-id="4a963-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4a963-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4a963-108">属性</span><span class="sxs-lookup"><span data-stu-id="4a963-108">Attributes</span></span>

<span data-ttu-id="4a963-109">なし。</span><span class="sxs-lookup"><span data-stu-id="4a963-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4a963-110">子要素</span><span class="sxs-lookup"><span data-stu-id="4a963-110">Child elements</span></span>

<span data-ttu-id="4a963-111">[Name (string)](name-string.md)  | [EmailAddress (非 Emptystringtype)](emailaddress-nonemptystringtype.md)  | [Routingtype (EmailAddressType)](routingtype-emailaddresstype.md)  | [MailboxType](mailboxtype.md)  | [ItemId](itemid.md)  | [Originaldisplayname](originaldisplayname.md)</span><span class="sxs-lookup"><span data-stu-id="4a963-111">[Name (string)](name-string.md) | [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) | [RoutingType (EmailAddressType)](routingtype-emailaddresstype.md) | [MailboxType](mailboxtype.md) | [ItemId](itemid.md) | [OriginalDisplayName](originaldisplayname.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4a963-112">親要素</span><span class="sxs-lookup"><span data-stu-id="4a963-112">Parent elements</span></span>

[<span data-ttu-id="4a963-113">EmailAddressAttributedValue</span><span class="sxs-lookup"><span data-stu-id="4a963-113">EmailAddressAttributedValue</span></span>](emailaddressattributedvalue.md)
  
## <a name="remarks"></a><span data-ttu-id="4a963-114">注釈</span><span class="sxs-lookup"><span data-stu-id="4a963-114">Remarks</span></span>

<span data-ttu-id="4a963-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="4a963-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4a963-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="4a963-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4a963-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="4a963-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4a963-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="4a963-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4a963-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4a963-119">Schema name</span></span>  <br/> |<span data-ttu-id="4a963-120">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="4a963-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="4a963-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4a963-121">Validation file</span></span>  <br/> |<span data-ttu-id="4a963-122">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="4a963-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4a963-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="4a963-123">Can be empty</span></span>  <br/> |<span data-ttu-id="4a963-124">false</span><span class="sxs-lookup"><span data-stu-id="4a963-124">false</span></span>  <br/> |
   

