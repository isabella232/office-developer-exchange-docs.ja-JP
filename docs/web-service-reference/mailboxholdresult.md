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
ms.openlocfilehash: 3895c1351587db45881c661809a19dad1929b4a9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466396"
---
# <a name="mailboxholdresult"></a><span data-ttu-id="2ab0f-103">MailboxHoldResult</span><span class="sxs-lookup"><span data-stu-id="2ab0f-103">MailboxHoldResult</span></span>

<span data-ttu-id="2ab0f-104">**MailboxHoldResult**要素には、 **GetHoldOnMailboxes**要求の結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="2ab0f-104">The **MailboxHoldResult** element contains the result of the **GetHoldOnMailboxes** request.</span></span> 
  
```XML
<MailboxHoldResult>
   <HoldId/>
   <Query/>
   <MailboxHoldStatuses/>
</MailboxHoldResult>
```

<span data-ttu-id="2ab0f-105">**MailboxHoldResultType**</span><span class="sxs-lookup"><span data-stu-id="2ab0f-105">**MailboxHoldResultType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="2ab0f-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="2ab0f-106">Attributes and elements</span></span>

<span data-ttu-id="2ab0f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2ab0f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2ab0f-108">属性</span><span class="sxs-lookup"><span data-stu-id="2ab0f-108">Attributes</span></span>

<span data-ttu-id="2ab0f-109">なし。</span><span class="sxs-lookup"><span data-stu-id="2ab0f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2ab0f-110">子要素</span><span class="sxs-lookup"><span data-stu-id="2ab0f-110">Child elements</span></span>

<span data-ttu-id="2ab0f-111">[HoldId](holdid.md)  | [クエリ](query.md)  | [MailboxHoldStatuses](mailboxholdstatuses.md)</span><span class="sxs-lookup"><span data-stu-id="2ab0f-111">[HoldId](holdid.md) | [Query](query.md) | [MailboxHoldStatuses](mailboxholdstatuses.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2ab0f-112">親要素</span><span class="sxs-lookup"><span data-stu-id="2ab0f-112">Parent elements</span></span>

<span data-ttu-id="2ab0f-113">なし。</span><span class="sxs-lookup"><span data-stu-id="2ab0f-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2ab0f-114">注釈</span><span class="sxs-lookup"><span data-stu-id="2ab0f-114">Remarks</span></span>

<span data-ttu-id="2ab0f-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="2ab0f-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="2ab0f-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="2ab0f-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2ab0f-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="2ab0f-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2ab0f-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="2ab0f-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2ab0f-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2ab0f-119">Schema name</span></span>  <br/> |<span data-ttu-id="2ab0f-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="2ab0f-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="2ab0f-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2ab0f-121">Validation file</span></span>  <br/> |<span data-ttu-id="2ab0f-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="2ab0f-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2ab0f-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="2ab0f-123">Can be empty</span></span>  <br/> ||
   

