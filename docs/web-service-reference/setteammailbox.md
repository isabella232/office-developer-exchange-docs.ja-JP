---
title: SetTeamMailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5d6ee7cc-8f88-4de2-ae5c-cabf2f2193d0
description: SetTeamMailbox 要素には、サイトのメールボックスを設定するための要求が含まれています。
ms.openlocfilehash: 708863168f4e89775deee8c5d66427df41515089
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833455"
---
# <a name="setteammailbox"></a><span data-ttu-id="e025c-103">SetTeamMailbox</span><span class="sxs-lookup"><span data-stu-id="e025c-103">SetTeamMailbox</span></span>

<span data-ttu-id="e025c-104">**SetTeamMailbox**要素には、サイトのメールボックスを設定するための要求が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e025c-104">The **SetTeamMailbox** element contains a request to set a site mailbox.</span></span> 
  
```XML
<SetTeamMailbox>
   <EmailAddress/>
   <SharePointSiteUrl/>
   <State/>
</SetTeamMailbox>
```

 <span data-ttu-id="e025c-105">**SetTeamMailboxRequestType**</span><span class="sxs-lookup"><span data-stu-id="e025c-105">**SetTeamMailboxRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e025c-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="e025c-106">Attributes and elements</span></span>

<span data-ttu-id="e025c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e025c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e025c-108">属性</span><span class="sxs-lookup"><span data-stu-id="e025c-108">Attributes</span></span>

<span data-ttu-id="e025c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e025c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e025c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e025c-110">Child elements</span></span>

<span data-ttu-id="e025c-111">[EmailAddress (EmailAddressType)](emailaddress-emailaddresstype.md) | [SharePointSiteUrl](sharepointsiteurl.md) | [(TeamMailboxLifecycleStateType) の状態](state-teammailboxlifecyclestatetype.md)</span><span class="sxs-lookup"><span data-stu-id="e025c-111">[EmailAddress (EmailAddressType)](emailaddress-emailaddresstype.md) | [SharePointSiteUrl](sharepointsiteurl.md) | [State (TeamMailboxLifecycleStateType)](state-teammailboxlifecyclestatetype.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e025c-112">親要素</span><span class="sxs-lookup"><span data-stu-id="e025c-112">Parent elements</span></span>

<span data-ttu-id="e025c-113">なし。</span><span class="sxs-lookup"><span data-stu-id="e025c-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e025c-114">備考</span><span class="sxs-lookup"><span data-stu-id="e025c-114">Remarks</span></span>

<span data-ttu-id="e025c-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="e025c-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e025c-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="e025c-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e025c-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="e025c-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e025c-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="e025c-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e025c-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e025c-119">Schema name</span></span>  <br/> |<span data-ttu-id="e025c-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="e025c-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e025c-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e025c-121">Validation file</span></span>  <br/> |<span data-ttu-id="e025c-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e025c-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e025c-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="e025c-123">Can be empty</span></span>  <br/> ||
   

