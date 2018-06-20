---
title: 値 (EmailAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 24eaa473-0024-47e2-b7d2-051d5dd4f53c
description: 値要素は、帰属配列に関連付けられている、EmailAddress の値を指定します。
ms.openlocfilehash: 097444d90e98e73b9e83912274ecf87249008116
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839973"
---
# <a name="value-emailaddresstype"></a><span data-ttu-id="6a037-103">値 (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="6a037-103">Value (EmailAddressType)</span></span>

<span data-ttu-id="6a037-104">帰属配列に、 **EmailAddress**の値が関連付けられている**値**の要素を指定します。</span><span class="sxs-lookup"><span data-stu-id="6a037-104">The **Value** element specifies the value of an **EmailAddress** associated with an attributions array.</span></span> 
  
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

<span data-ttu-id="6a037-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="6a037-105">**EmailAddressType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="6a037-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="6a037-106">Attributes and elements</span></span>

<span data-ttu-id="6a037-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6a037-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6a037-108">属性</span><span class="sxs-lookup"><span data-stu-id="6a037-108">Attributes</span></span>

<span data-ttu-id="6a037-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6a037-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6a037-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6a037-110">Child elements</span></span>

<span data-ttu-id="6a037-111">[名 (文字列)](name-string.md) | [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) | [RoutingType (EmailAddressType)](routingtype-emailaddresstype.md) | [MailboxType](mailboxtype.md) | [アイテム Id](itemid.md) | [OriginalDisplayName](originaldisplayname.md)</span><span class="sxs-lookup"><span data-stu-id="6a037-111">[Name (string)](name-string.md) | [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) | [RoutingType (EmailAddressType)](routingtype-emailaddresstype.md) | [MailboxType](mailboxtype.md) | [ItemId](itemid.md) | [OriginalDisplayName](originaldisplayname.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6a037-112">親要素</span><span class="sxs-lookup"><span data-stu-id="6a037-112">Parent elements</span></span>

[<span data-ttu-id="6a037-113">EmailAddressAttributedValue</span><span class="sxs-lookup"><span data-stu-id="6a037-113">EmailAddressAttributedValue</span></span>](emailaddressattributedvalue.md)
  
## <a name="remarks"></a><span data-ttu-id="6a037-114">備考</span><span class="sxs-lookup"><span data-stu-id="6a037-114">Remarks</span></span>

<span data-ttu-id="6a037-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="6a037-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="6a037-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="6a037-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6a037-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="6a037-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6a037-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="6a037-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6a037-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6a037-119">Schema name</span></span>  <br/> |<span data-ttu-id="6a037-120">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="6a037-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="6a037-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6a037-121">Validation file</span></span>  <br/> |<span data-ttu-id="6a037-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6a037-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6a037-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="6a037-123">Can be empty</span></span>  <br/> |<span data-ttu-id="6a037-124">false</span><span class="sxs-lookup"><span data-stu-id="6a037-124">false</span></span>  <br/> |
   

