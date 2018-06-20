---
title: InPlaceHoldIdentity
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 54f45774-00a0-4392-af1b-8c5f2208a53f
description: InPlaceHoldIdentity 要素は、メールボックス アイテムを保持する保留リストの id を指定します。
ms.openlocfilehash: 954e6ad6c3e0b7786d6bbb8230dba913a32359bc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831938"
---
# <a name="inplaceholdidentity"></a><span data-ttu-id="e4fd3-103">InPlaceHoldIdentity</span><span class="sxs-lookup"><span data-stu-id="e4fd3-103">InPlaceHoldIdentity</span></span>

<span data-ttu-id="e4fd3-104">**InPlaceHoldIdentity**要素は、メールボックス アイテムを保持する保留リストの id を指定します。</span><span class="sxs-lookup"><span data-stu-id="e4fd3-104">The **InPlaceHoldIdentity** element specifies the identity of a hold that preserves the mailbox items.</span></span> 
  
```XML
<InPlaceHoldIdentity></InPlaceHoldIdentity>
```

 <span data-ttu-id="e4fd3-105">**string**</span><span class="sxs-lookup"><span data-stu-id="e4fd3-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e4fd3-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="e4fd3-106">Attributes and elements</span></span>

<span data-ttu-id="e4fd3-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e4fd3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e4fd3-108">属性</span><span class="sxs-lookup"><span data-stu-id="e4fd3-108">Attributes</span></span>

<span data-ttu-id="e4fd3-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e4fd3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e4fd3-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e4fd3-110">Child elements</span></span>

<span data-ttu-id="e4fd3-111">なし。</span><span class="sxs-lookup"><span data-stu-id="e4fd3-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e4fd3-112">親要素</span><span class="sxs-lookup"><span data-stu-id="e4fd3-112">Parent elements</span></span>

<span data-ttu-id="e4fd3-113">[SetHoldOnMailboxes](setholdonmailboxes.md) | [DiscoverySearchConfiguration](discoverysearchconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e4fd3-113">[SetHoldOnMailboxes](setholdonmailboxes.md) | [DiscoverySearchConfiguration](discoverysearchconfiguration.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="e4fd3-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="e4fd3-114">Text value</span></span>

<span data-ttu-id="e4fd3-115">**InPlaceHoldIdentity**要素のテキスト値は、メールボックスの保留中の識別子です。</span><span class="sxs-lookup"><span data-stu-id="e4fd3-115">The text value of the **InPlaceHoldIdentity** element is the mailbox hold identifier.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="e4fd3-116">備考</span><span class="sxs-lookup"><span data-stu-id="e4fd3-116">Remarks</span></span>

<span data-ttu-id="e4fd3-117">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="e4fd3-117">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e4fd3-118">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="e4fd3-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e4fd3-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="e4fd3-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e4fd3-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="e4fd3-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e4fd3-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e4fd3-121">Schema name</span></span>  <br/> |<span data-ttu-id="e4fd3-122">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="e4fd3-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e4fd3-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e4fd3-123">Validation file</span></span>  <br/> |<span data-ttu-id="e4fd3-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e4fd3-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e4fd3-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="e4fd3-125">Can be empty</span></span>  <br/> |<span data-ttu-id="e4fd3-126">False</span><span class="sxs-lookup"><span data-stu-id="e4fd3-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e4fd3-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="e4fd3-127">See also</span></span>



[<span data-ttu-id="e4fd3-128">SetHoldOnMailboxes 操作</span><span class="sxs-lookup"><span data-stu-id="e4fd3-128">SetHoldOnMailboxes operation</span></span>](setholdonmailboxes-operation.md)


- [<span data-ttu-id="e4fd3-129">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="e4fd3-129">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

