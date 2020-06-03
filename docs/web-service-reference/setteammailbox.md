---
title: SetTeamMailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5d6ee7cc-8f88-4de2-ae5c-cabf2f2193d0
description: SetTeamMailbox 要素には、サイトメールボックスを設定するための要求が含まれています。
ms.openlocfilehash: e4b7ebd308f4b58b6b6491289f24b9176c5dcf15
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465262"
---
# <a name="setteammailbox"></a><span data-ttu-id="28ff9-103">SetTeamMailbox</span><span class="sxs-lookup"><span data-stu-id="28ff9-103">SetTeamMailbox</span></span>

<span data-ttu-id="28ff9-104">**Setteammailbox**要素には、サイトメールボックスを設定するための要求が含まれています。</span><span class="sxs-lookup"><span data-stu-id="28ff9-104">The **SetTeamMailbox** element contains a request to set a site mailbox.</span></span> 
  
```XML
<SetTeamMailbox>
   <EmailAddress/>
   <SharePointSiteUrl/>
   <State/>
</SetTeamMailbox>
```

 <span data-ttu-id="28ff9-105">**SetTeamMailboxRequestType**</span><span class="sxs-lookup"><span data-stu-id="28ff9-105">**SetTeamMailboxRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="28ff9-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="28ff9-106">Attributes and elements</span></span>

<span data-ttu-id="28ff9-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="28ff9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="28ff9-108">属性</span><span class="sxs-lookup"><span data-stu-id="28ff9-108">Attributes</span></span>

<span data-ttu-id="28ff9-109">なし。</span><span class="sxs-lookup"><span data-stu-id="28ff9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="28ff9-110">子要素</span><span class="sxs-lookup"><span data-stu-id="28ff9-110">Child elements</span></span>

<span data-ttu-id="28ff9-111">[EmailAddress (EmailAddressType)](emailaddress-emailaddresstype.md)  | [Sharepointsiteurl](sharepointsiteurl.md)  | [State (TeamMailboxLifecycleStateType)](state-teammailboxlifecyclestatetype.md)</span><span class="sxs-lookup"><span data-stu-id="28ff9-111">[EmailAddress (EmailAddressType)](emailaddress-emailaddresstype.md) | [SharePointSiteUrl](sharepointsiteurl.md) | [State (TeamMailboxLifecycleStateType)](state-teammailboxlifecyclestatetype.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="28ff9-112">親要素</span><span class="sxs-lookup"><span data-stu-id="28ff9-112">Parent elements</span></span>

<span data-ttu-id="28ff9-113">なし。</span><span class="sxs-lookup"><span data-stu-id="28ff9-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="28ff9-114">注釈</span><span class="sxs-lookup"><span data-stu-id="28ff9-114">Remarks</span></span>

<span data-ttu-id="28ff9-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="28ff9-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="28ff9-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="28ff9-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="28ff9-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="28ff9-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="28ff9-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="28ff9-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="28ff9-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="28ff9-119">Schema name</span></span>  <br/> |<span data-ttu-id="28ff9-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="28ff9-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="28ff9-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="28ff9-121">Validation file</span></span>  <br/> |<span data-ttu-id="28ff9-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="28ff9-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="28ff9-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="28ff9-123">Can be empty</span></span>  <br/> ||
   

