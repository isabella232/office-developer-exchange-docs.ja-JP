---
title: InPlaceHoldIdentity
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 54f45774-00a0-4392-af1b-8c5f2208a53f
description: InPlaceHoldIdentity 要素は、メールボックスアイテムを保持するホールドの id を指定します。
ms.openlocfilehash: a06f72e478e7dc5bd1a499dceefeb352b14d7362
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466095"
---
# <a name="inplaceholdidentity"></a><span data-ttu-id="79f7c-103">InPlaceHoldIdentity</span><span class="sxs-lookup"><span data-stu-id="79f7c-103">InPlaceHoldIdentity</span></span>

<span data-ttu-id="79f7c-104">**InPlaceHoldIdentity**要素は、メールボックスアイテムを保持するホールドの id を指定します。</span><span class="sxs-lookup"><span data-stu-id="79f7c-104">The **InPlaceHoldIdentity** element specifies the identity of a hold that preserves the mailbox items.</span></span> 
  
```XML
<InPlaceHoldIdentity></InPlaceHoldIdentity>
```

 <span data-ttu-id="79f7c-105">**string**</span><span class="sxs-lookup"><span data-stu-id="79f7c-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="79f7c-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="79f7c-106">Attributes and elements</span></span>

<span data-ttu-id="79f7c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="79f7c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="79f7c-108">属性</span><span class="sxs-lookup"><span data-stu-id="79f7c-108">Attributes</span></span>

<span data-ttu-id="79f7c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="79f7c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="79f7c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="79f7c-110">Child elements</span></span>

<span data-ttu-id="79f7c-111">なし。</span><span class="sxs-lookup"><span data-stu-id="79f7c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="79f7c-112">親要素</span><span class="sxs-lookup"><span data-stu-id="79f7c-112">Parent elements</span></span>

<span data-ttu-id="79f7c-113">[SetHoldOnMailboxes](setholdonmailboxes.md)  | [Discoverysearchconfiguration](discoverysearchconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="79f7c-113">[SetHoldOnMailboxes](setholdonmailboxes.md) | [DiscoverySearchConfiguration](discoverysearchconfiguration.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="79f7c-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="79f7c-114">Text value</span></span>

<span data-ttu-id="79f7c-115">**InPlaceHoldIdentity**要素のテキスト値は、メールボックスのホールド識別子です。</span><span class="sxs-lookup"><span data-stu-id="79f7c-115">The text value of the **InPlaceHoldIdentity** element is the mailbox hold identifier.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="79f7c-116">注釈</span><span class="sxs-lookup"><span data-stu-id="79f7c-116">Remarks</span></span>

<span data-ttu-id="79f7c-117">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="79f7c-117">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="79f7c-118">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="79f7c-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="79f7c-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="79f7c-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="79f7c-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="79f7c-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="79f7c-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="79f7c-121">Schema name</span></span>  <br/> |<span data-ttu-id="79f7c-122">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="79f7c-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="79f7c-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="79f7c-123">Validation file</span></span>  <br/> |<span data-ttu-id="79f7c-124">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="79f7c-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="79f7c-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="79f7c-125">Can be empty</span></span>  <br/> |<span data-ttu-id="79f7c-126">正しくない</span><span class="sxs-lookup"><span data-stu-id="79f7c-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="79f7c-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="79f7c-127">See also</span></span>



[<span data-ttu-id="79f7c-128">SetHoldOnMailboxes 操作</span><span class="sxs-lookup"><span data-stu-id="79f7c-128">SetHoldOnMailboxes operation</span></span>](setholdonmailboxes-operation.md)


- [<span data-ttu-id="79f7c-129">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="79f7c-129">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

