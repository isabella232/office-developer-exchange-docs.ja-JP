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
ms.openlocfilehash: bb1d64b98f5e1ab4cdbe4a297ded46d00b27b364
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833418"
---
# <a name="setholdonmailboxesresponse"></a><span data-ttu-id="138ae-103">SetHoldOnMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="138ae-103">SetHoldOnMailboxesResponse</span></span>

<span data-ttu-id="138ae-104">**SetHoldOnMailboxesResponse**要素は、 **SetHoldOnMailboxes**要求への応答を表します。</span><span class="sxs-lookup"><span data-stu-id="138ae-104">The **SetHoldOnMailboxesResponse** element represents a response to a **SetHoldOnMailboxes** request.</span></span> 
  
```XML
<SetHoldOnMailboxesResponse>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <MailboxHoldResult/>
</SetHoldOnMailboxesResponse>
```

 <span data-ttu-id="138ae-105">**SetHoldOnMailboxesResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="138ae-105">**SetHoldOnMailboxesResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="138ae-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="138ae-106">Attributes and elements</span></span>

<span data-ttu-id="138ae-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="138ae-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="138ae-108">属性</span><span class="sxs-lookup"><span data-stu-id="138ae-108">Attributes</span></span>

<span data-ttu-id="138ae-109">なし。</span><span class="sxs-lookup"><span data-stu-id="138ae-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="138ae-110">子要素</span><span class="sxs-lookup"><span data-stu-id="138ae-110">Child elements</span></span>

<span data-ttu-id="138ae-111">[メッセージ テキスト](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [MailboxHoldResult](mailboxholdresult.md)</span><span class="sxs-lookup"><span data-stu-id="138ae-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [MailboxHoldResult](mailboxholdresult.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="138ae-112">親要素</span><span class="sxs-lookup"><span data-stu-id="138ae-112">Parent elements</span></span>

<span data-ttu-id="138ae-113">なし。</span><span class="sxs-lookup"><span data-stu-id="138ae-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="138ae-114">備考</span><span class="sxs-lookup"><span data-stu-id="138ae-114">Remarks</span></span>

<span data-ttu-id="138ae-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="138ae-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="138ae-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="138ae-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="138ae-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="138ae-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="138ae-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="138ae-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="138ae-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="138ae-119">Schema name</span></span>  <br/> |<span data-ttu-id="138ae-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="138ae-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="138ae-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="138ae-121">Validation file</span></span>  <br/> |<span data-ttu-id="138ae-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="138ae-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="138ae-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="138ae-123">Can be empty</span></span>  <br/> |<span data-ttu-id="138ae-124">false</span><span class="sxs-lookup"><span data-stu-id="138ae-124">false</span></span>  <br/> |
   

