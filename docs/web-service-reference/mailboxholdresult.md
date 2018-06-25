---
title: MailboxHoldResult
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: da03b877-37c6-4ecb-8549-c639f140302e
description: MailboxHoldResult 要素には、GetHoldOnMailboxes 要求の結果が含まれています。
ms.openlocfilehash: 333a2d2d4a30a63a78660d167cefe75653f8ea82
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832289"
---
# <a name="mailboxholdresult"></a><span data-ttu-id="a483d-103">MailboxHoldResult</span><span class="sxs-lookup"><span data-stu-id="a483d-103">MailboxHoldResult</span></span>

<span data-ttu-id="a483d-104">**MailboxHoldResult**要素には、 **GetHoldOnMailboxes**要求の結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a483d-104">The **MailboxHoldResult** element contains the result of the **GetHoldOnMailboxes** request.</span></span> 
  
```XML
<MailboxHoldResult>
   <HoldId/>
   <Query/>
   <MailboxHoldStatuses/>
</MailboxHoldResult>
```

<span data-ttu-id="a483d-105">**MailboxHoldResultType**</span><span class="sxs-lookup"><span data-stu-id="a483d-105">**MailboxHoldResultType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="a483d-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="a483d-106">Attributes and elements</span></span>

<span data-ttu-id="a483d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a483d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a483d-108">属性</span><span class="sxs-lookup"><span data-stu-id="a483d-108">Attributes</span></span>

<span data-ttu-id="a483d-109">なし。</span><span class="sxs-lookup"><span data-stu-id="a483d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a483d-110">子要素</span><span class="sxs-lookup"><span data-stu-id="a483d-110">Child elements</span></span>

<span data-ttu-id="a483d-111">[HoldId](holdid.md) | [クエリ](query.md) | [MailboxHoldStatuses](mailboxholdstatuses.md)</span><span class="sxs-lookup"><span data-stu-id="a483d-111">[HoldId](holdid.md) | [Query](query.md) | [MailboxHoldStatuses](mailboxholdstatuses.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a483d-112">親要素</span><span class="sxs-lookup"><span data-stu-id="a483d-112">Parent elements</span></span>

<span data-ttu-id="a483d-113">なし。</span><span class="sxs-lookup"><span data-stu-id="a483d-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a483d-114">備考</span><span class="sxs-lookup"><span data-stu-id="a483d-114">Remarks</span></span>

<span data-ttu-id="a483d-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="a483d-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="a483d-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="a483d-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a483d-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="a483d-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a483d-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="a483d-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a483d-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a483d-119">Schema name</span></span>  <br/> |<span data-ttu-id="a483d-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="a483d-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a483d-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a483d-121">Validation file</span></span>  <br/> |<span data-ttu-id="a483d-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="a483d-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a483d-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="a483d-123">Can be empty</span></span>  <br/> ||
   

