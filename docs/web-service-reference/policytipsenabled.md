---
title: Policyヒント Enabled
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 16409652-21e4-4bd3-9373-67e1882236b4
description: Policyヒント Enabled 要素は、ポリシーヒントが有効になっているかどうかを示します。
ms.openlocfilehash: 26a527022d60dd4b98f70c2b3bf020b649066057
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468517"
---
# <a name="policytipsenabled"></a><span data-ttu-id="b09e4-103">Policyヒント Enabled</span><span class="sxs-lookup"><span data-stu-id="b09e4-103">PolicyTipsEnabled</span></span>

<span data-ttu-id="b09e4-104">**Policyヒント enabled**要素は、ポリシーヒントが有効になっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b09e4-104">The **PolicyTipsEnabled** element indicates whether policy tips are enabled.</span></span> 
  
```XML
<PolicyTipsEnabled> true | false </PolicyTipsEnabled>
```

 <span data-ttu-id="b09e4-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="b09e4-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b09e4-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="b09e4-106">Attributes and elements</span></span>

<span data-ttu-id="b09e4-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b09e4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b09e4-108">属性</span><span class="sxs-lookup"><span data-stu-id="b09e4-108">Attributes</span></span>

<span data-ttu-id="b09e4-109">なし。</span><span class="sxs-lookup"><span data-stu-id="b09e4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b09e4-110">子要素</span><span class="sxs-lookup"><span data-stu-id="b09e4-110">Child elements</span></span>

<span data-ttu-id="b09e4-111">なし。</span><span class="sxs-lookup"><span data-stu-id="b09e4-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b09e4-112">親要素</span><span class="sxs-lookup"><span data-stu-id="b09e4-112">Parent elements</span></span>

[<span data-ttu-id="b09e4-113">Mailヒント構成 (MailTipsServiceConfiguration)</span><span class="sxs-lookup"><span data-stu-id="b09e4-113">MailTipsConfiguration (MailTipsServiceConfiguration)</span></span>](mailtipsconfiguration-mailtipsserviceconfiguration.md)
  
## <a name="text-value"></a><span data-ttu-id="b09e4-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="b09e4-114">Text value</span></span>

<span data-ttu-id="b09e4-115">**Policyヒント enabled**要素のテキスト値が**true**の場合は、メールボックスに対してポリシーヒントが有効になっていることを示します。</span><span class="sxs-lookup"><span data-stu-id="b09e4-115">A text value of **true** for the **PolicyTipsEnabled** element indicates that policy tips are enabled for a mailbox.</span></span> <span data-ttu-id="b09e4-116">値が**false**の場合、メールボックスに対してポリシーヒントが有効になっていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="b09e4-116">A value of **false** indicates that policy tips are not enabled for a mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="b09e4-117">注釈</span><span class="sxs-lookup"><span data-stu-id="b09e4-117">Remarks</span></span>

<span data-ttu-id="b09e4-118">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="b09e4-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b09e4-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="b09e4-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b09e4-120">要素の情報</span><span class="sxs-lookup"><span data-stu-id="b09e4-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b09e4-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="b09e4-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b09e4-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b09e4-122">Schema name</span></span>  <br/> |<span data-ttu-id="b09e4-123">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="b09e4-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="b09e4-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b09e4-124">Validation file</span></span>  <br/> |<span data-ttu-id="b09e4-125">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="b09e4-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b09e4-126">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="b09e4-126">Can be empty</span></span>  <br/> ||
   

