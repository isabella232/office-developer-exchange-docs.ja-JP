---
title: エントリ (EmailAddress)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Entry
api_type:
- schema
ms.assetid: b028c5c7-3494-4ecd-96d1-78783daa660f
description: エントリ要素は、連絡先の単一の電子メール アドレスを表します。
ms.openlocfilehash: 1852584e507c38da030815c37f85f7c4af4e2ba4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760308"
---
# <a name="entry-emailaddress"></a><span data-ttu-id="6e3f2-103">エントリ (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="6e3f2-103">Entry (EmailAddress)</span></span>

<span data-ttu-id="6e3f2-104">**エントリ**要素は、連絡先の単一の電子メール アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="6e3f2-104">The **Entry** element represents a single e-mail address for a contact.</span></span> 
  
```XML
<Entry Key="" Name="" RoutingType="" MailboxType="" />
```

<span data-ttu-id="6e3f2-105">**EmailAddressDictionaryEntryType**</span><span class="sxs-lookup"><span data-stu-id="6e3f2-105">**EmailAddressDictionaryEntryType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="6e3f2-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="6e3f2-106">Attributes and elements</span></span>

<span data-ttu-id="6e3f2-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6e3f2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6e3f2-108">属性</span><span class="sxs-lookup"><span data-stu-id="6e3f2-108">Attributes</span></span>

|<span data-ttu-id="6e3f2-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="6e3f2-109">**Attribute**</span></span>|<span data-ttu-id="6e3f2-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="6e3f2-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6e3f2-111">**Key**</span><span class="sxs-lookup"><span data-stu-id="6e3f2-111">**Key**</span></span> <br/> | <span data-ttu-id="6e3f2-112">電子メール アドレスを識別します。</span><span class="sxs-lookup"><span data-stu-id="6e3f2-112">Identifies the e-mail address.</span></span><br/><br/><span data-ttu-id="6e3f2-113">次に、この属性で使用できる値を示します。</span><span class="sxs-lookup"><span data-stu-id="6e3f2-113">The following are the possible values for this attribute:</span></span><br/><br/><span data-ttu-id="6e3f2-114">-EmailAddress1</span><span class="sxs-lookup"><span data-stu-id="6e3f2-114">-  EmailAddress1</span></span>  <br/><span data-ttu-id="6e3f2-115">-EmailAddress2</span><span class="sxs-lookup"><span data-stu-id="6e3f2-115">-  EmailAddress2</span></span>  <br/><span data-ttu-id="6e3f2-116">-EmailAddress3</span><span class="sxs-lookup"><span data-stu-id="6e3f2-116">-  EmailAddress3</span></span> <br/><br/>  <span data-ttu-id="6e3f2-117">この属性は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="6e3f2-117">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="6e3f2-118">**名前**</span><span class="sxs-lookup"><span data-stu-id="6e3f2-118">**Name**</span></span> <br/> |<span data-ttu-id="6e3f2-119">メールボックス ユーザーの名前を定義します。</span><span class="sxs-lookup"><span data-stu-id="6e3f2-119">Defines the name of the mailbox user.</span></span> <span data-ttu-id="6e3f2-120">この属性は、省略可能です。</span><span class="sxs-lookup"><span data-stu-id="6e3f2-120">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="6e3f2-121">**RoutingType**</span><span class="sxs-lookup"><span data-stu-id="6e3f2-121">**RoutingType**</span></span> <br/> |<span data-ttu-id="6e3f2-122">メールボックスに使用されるルーティングを定義します。</span><span class="sxs-lookup"><span data-stu-id="6e3f2-122">Defines the routing that is used for the mailbox.</span></span> <span data-ttu-id="6e3f2-123">既定値は、SMTP です。</span><span class="sxs-lookup"><span data-stu-id="6e3f2-123">The default is SMTP.</span></span> <span data-ttu-id="6e3f2-124">この属性は、省略可能です。</span><span class="sxs-lookup"><span data-stu-id="6e3f2-124">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="6e3f2-125">**MailboxType**</span><span class="sxs-lookup"><span data-stu-id="6e3f2-125">**MailboxType**</span></span> <br/> |<span data-ttu-id="6e3f2-126">メールボックスのユーザーのメールボックスの種類を定義します。</span><span class="sxs-lookup"><span data-stu-id="6e3f2-126">Defines the mailbox type of a mailbox user.</span></span> <span data-ttu-id="6e3f2-127">この属性は、省略可能です。</span><span class="sxs-lookup"><span data-stu-id="6e3f2-127">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="6e3f2-128">子要素</span><span class="sxs-lookup"><span data-stu-id="6e3f2-128">Child elements</span></span>

<span data-ttu-id="6e3f2-129">なし。</span><span class="sxs-lookup"><span data-stu-id="6e3f2-129">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6e3f2-130">親要素</span><span class="sxs-lookup"><span data-stu-id="6e3f2-130">Parent elements</span></span>

|<span data-ttu-id="6e3f2-131">**要素**</span><span class="sxs-lookup"><span data-stu-id="6e3f2-131">**Element**</span></span>|<span data-ttu-id="6e3f2-132">**説明**</span><span class="sxs-lookup"><span data-stu-id="6e3f2-132">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6e3f2-133">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="6e3f2-133">EmailAddresses</span></span>](emailaddresses.md) <br/> |<span data-ttu-id="6e3f2-134">連絡先の電子メール アドレスのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="6e3f2-134">Represents a collection of e-mail addresses for a contact.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6e3f2-135">備考</span><span class="sxs-lookup"><span data-stu-id="6e3f2-135">Remarks</span></span>

<span data-ttu-id="6e3f2-136">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="6e3f2-136">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="6e3f2-137">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="6e3f2-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6e3f2-138">要素情報</span><span class="sxs-lookup"><span data-stu-id="6e3f2-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6e3f2-139">名前空間</span><span class="sxs-lookup"><span data-stu-id="6e3f2-139">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6e3f2-140">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6e3f2-140">Schema name</span></span>  <br/> |<span data-ttu-id="6e3f2-141">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="6e3f2-141">Types schema</span></span>  <br/> |
|<span data-ttu-id="6e3f2-142">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6e3f2-142">Validation file</span></span>  <br/> |<span data-ttu-id="6e3f2-143">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6e3f2-143">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6e3f2-144">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="6e3f2-144">Can be empty</span></span>  <br/> |<span data-ttu-id="6e3f2-145">False</span><span class="sxs-lookup"><span data-stu-id="6e3f2-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6e3f2-146">関連項目</span><span class="sxs-lookup"><span data-stu-id="6e3f2-146">See also</span></span>

- [<span data-ttu-id="6e3f2-147">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="6e3f2-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

