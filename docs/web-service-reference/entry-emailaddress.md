---
title: Entry (EmailAddress)
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
description: Entry 要素は、連絡先の1つの電子メールアドレスを表します。
ms.openlocfilehash: 766d67cda10b02c07a7677e541fddfc38a4285cf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459645"
---
# <a name="entry-emailaddress"></a><span data-ttu-id="4d4e3-103">Entry (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="4d4e3-103">Entry (EmailAddress)</span></span>

<span data-ttu-id="4d4e3-104">**Entry**要素は、連絡先の1つの電子メールアドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="4d4e3-104">The **Entry** element represents a single e-mail address for a contact.</span></span> 
  
```XML
<Entry Key="" Name="" RoutingType="" MailboxType="" />
```

<span data-ttu-id="4d4e3-105">**EmailAddressDictionaryEntryType**</span><span class="sxs-lookup"><span data-stu-id="4d4e3-105">**EmailAddressDictionaryEntryType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="4d4e3-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="4d4e3-106">Attributes and elements</span></span>

<span data-ttu-id="4d4e3-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4d4e3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4d4e3-108">属性</span><span class="sxs-lookup"><span data-stu-id="4d4e3-108">Attributes</span></span>

|<span data-ttu-id="4d4e3-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="4d4e3-109">**Attribute**</span></span>|<span data-ttu-id="4d4e3-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="4d4e3-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4d4e3-111">**Key**</span><span class="sxs-lookup"><span data-stu-id="4d4e3-111">**Key**</span></span> <br/> | <span data-ttu-id="4d4e3-112">電子メールアドレスを識別します。</span><span class="sxs-lookup"><span data-stu-id="4d4e3-112">Identifies the e-mail address.</span></span><br/><br/><span data-ttu-id="4d4e3-113">次に、この属性で使用できる値を示します。</span><span class="sxs-lookup"><span data-stu-id="4d4e3-113">The following are the possible values for this attribute:</span></span><br/><br/><span data-ttu-id="4d4e3-114">- EmailAddress1</span><span class="sxs-lookup"><span data-stu-id="4d4e3-114">-  EmailAddress1</span></span>  <br/><span data-ttu-id="4d4e3-115">- EmailAddress2</span><span class="sxs-lookup"><span data-stu-id="4d4e3-115">-  EmailAddress2</span></span>  <br/><span data-ttu-id="4d4e3-116">- EmailAddress3</span><span class="sxs-lookup"><span data-stu-id="4d4e3-116">-  EmailAddress3</span></span> <br/><br/>  <span data-ttu-id="4d4e3-117">この属性は必須です。</span><span class="sxs-lookup"><span data-stu-id="4d4e3-117">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="4d4e3-118">**名前**</span><span class="sxs-lookup"><span data-stu-id="4d4e3-118">**Name**</span></span> <br/> |<span data-ttu-id="4d4e3-119">メールボックスユーザーの名前を定義します。</span><span class="sxs-lookup"><span data-stu-id="4d4e3-119">Defines the name of the mailbox user.</span></span> <span data-ttu-id="4d4e3-120">この属性は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="4d4e3-120">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="4d4e3-121">**RoutingType**</span><span class="sxs-lookup"><span data-stu-id="4d4e3-121">**RoutingType**</span></span> <br/> |<span data-ttu-id="4d4e3-122">メールボックスに使用されるルーティングを定義します。</span><span class="sxs-lookup"><span data-stu-id="4d4e3-122">Defines the routing that is used for the mailbox.</span></span> <span data-ttu-id="4d4e3-123">既定値は SMTP です。</span><span class="sxs-lookup"><span data-stu-id="4d4e3-123">The default is SMTP.</span></span> <span data-ttu-id="4d4e3-124">この属性は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="4d4e3-124">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="4d4e3-125">**MailboxType**</span><span class="sxs-lookup"><span data-stu-id="4d4e3-125">**MailboxType**</span></span> <br/> |<span data-ttu-id="4d4e3-126">メールボックスユーザーのメールボックスの種類を定義します。</span><span class="sxs-lookup"><span data-stu-id="4d4e3-126">Defines the mailbox type of a mailbox user.</span></span> <span data-ttu-id="4d4e3-127">この属性は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="4d4e3-127">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="4d4e3-128">子要素</span><span class="sxs-lookup"><span data-stu-id="4d4e3-128">Child elements</span></span>

<span data-ttu-id="4d4e3-129">なし。</span><span class="sxs-lookup"><span data-stu-id="4d4e3-129">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4d4e3-130">親要素</span><span class="sxs-lookup"><span data-stu-id="4d4e3-130">Parent elements</span></span>

|<span data-ttu-id="4d4e3-131">**要素**</span><span class="sxs-lookup"><span data-stu-id="4d4e3-131">**Element**</span></span>|<span data-ttu-id="4d4e3-132">**説明**</span><span class="sxs-lookup"><span data-stu-id="4d4e3-132">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4d4e3-133">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="4d4e3-133">EmailAddresses</span></span>](emailaddresses.md) <br/> |<span data-ttu-id="4d4e3-134">連絡先の電子メールアドレスのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="4d4e3-134">Represents a collection of e-mail addresses for a contact.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4d4e3-135">注釈</span><span class="sxs-lookup"><span data-stu-id="4d4e3-135">Remarks</span></span>

<span data-ttu-id="4d4e3-136">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="4d4e3-136">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4d4e3-137">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="4d4e3-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4d4e3-138">要素の情報</span><span class="sxs-lookup"><span data-stu-id="4d4e3-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4d4e3-139">Namespace</span><span class="sxs-lookup"><span data-stu-id="4d4e3-139">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4d4e3-140">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4d4e3-140">Schema name</span></span>  <br/> |<span data-ttu-id="4d4e3-141">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="4d4e3-141">Types schema</span></span>  <br/> |
|<span data-ttu-id="4d4e3-142">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4d4e3-142">Validation file</span></span>  <br/> |<span data-ttu-id="4d4e3-143">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="4d4e3-143">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4d4e3-144">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="4d4e3-144">Can be empty</span></span>  <br/> |<span data-ttu-id="4d4e3-145">正しくない</span><span class="sxs-lookup"><span data-stu-id="4d4e3-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4d4e3-146">関連項目</span><span class="sxs-lookup"><span data-stu-id="4d4e3-146">See also</span></span>

- [<span data-ttu-id="4d4e3-147">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="4d4e3-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

