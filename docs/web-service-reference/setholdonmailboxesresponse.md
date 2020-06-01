---
title: SetHoldOnMailboxesResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 909194d6-e2b1-4774-bf29-04ed4318df1d
description: SetHoldOnMailboxesResponse 要素は、SetHoldOnMailboxes 要求への応答を表します。
ms.openlocfilehash: 37ad5c6e8f880831a98ff2e649a92cee99930889
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44438083"
---
# <a name="setholdonmailboxesresponse"></a><span data-ttu-id="c933a-103">SetHoldOnMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="c933a-103">SetHoldOnMailboxesResponse</span></span>

<span data-ttu-id="c933a-104">**SetHoldOnMailboxesResponse**要素は、 **SetHoldOnMailboxes**要求への応答を表します。</span><span class="sxs-lookup"><span data-stu-id="c933a-104">The **SetHoldOnMailboxesResponse** element represents a response to a **SetHoldOnMailboxes** request.</span></span> 
  
```XML
<SetHoldOnMailboxesResponse>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <MailboxHoldResult/>
</SetHoldOnMailboxesResponse>
```

 <span data-ttu-id="c933a-105">**SetHoldOnMailboxesResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="c933a-105">**SetHoldOnMailboxesResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c933a-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="c933a-106">Attributes and elements</span></span>

<span data-ttu-id="c933a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c933a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c933a-108">属性</span><span class="sxs-lookup"><span data-stu-id="c933a-108">Attributes</span></span>

<span data-ttu-id="c933a-109">なし。</span><span class="sxs-lookup"><span data-stu-id="c933a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c933a-110">子要素</span><span class="sxs-lookup"><span data-stu-id="c933a-110">Child elements</span></span>

<span data-ttu-id="c933a-111">[Messagetext](messagetext.md)  | 応答[Secmode](responsecode.md)  | [DescriptiveLinkKey](descriptivelinkkey.md)  | [MessageXml](messagexml.md)  | [MailboxHoldResult](mailboxholdresult.md)</span><span class="sxs-lookup"><span data-stu-id="c933a-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [MailboxHoldResult](mailboxholdresult.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c933a-112">親要素</span><span class="sxs-lookup"><span data-stu-id="c933a-112">Parent elements</span></span>

<span data-ttu-id="c933a-113">なし。</span><span class="sxs-lookup"><span data-stu-id="c933a-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c933a-114">注釈</span><span class="sxs-lookup"><span data-stu-id="c933a-114">Remarks</span></span>

<span data-ttu-id="c933a-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="c933a-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="c933a-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="c933a-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c933a-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="c933a-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c933a-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="c933a-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c933a-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c933a-119">Schema name</span></span>  <br/> |<span data-ttu-id="c933a-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="c933a-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c933a-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c933a-121">Validation file</span></span>  <br/> |<span data-ttu-id="c933a-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="c933a-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c933a-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="c933a-123">Can be empty</span></span>  <br/> |<span data-ttu-id="c933a-124">false</span><span class="sxs-lookup"><span data-stu-id="c933a-124">false</span></span>  <br/> |
   

