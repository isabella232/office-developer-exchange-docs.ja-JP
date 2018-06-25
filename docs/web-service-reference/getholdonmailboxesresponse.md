---
title: GetHoldOnMailboxesResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8af93c14-c4f0-4ec3-a1e6-4742a0a14eee
description: GetHoldOnMailboxes 要素には、メールボックスの保留状態を取得する要求が含まれています。
ms.openlocfilehash: aa8f02f8bee80060c86a55c27e138be81b59706e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760744"
---
# <a name="getholdonmailboxesresponse"></a><span data-ttu-id="07f88-103">GetHoldOnMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="07f88-103">GetHoldOnMailboxesResponse</span></span>

<span data-ttu-id="07f88-104">**GetHoldOnMailboxes**要素には、メールボックスの保留状態を取得する要求が含まれています。</span><span class="sxs-lookup"><span data-stu-id="07f88-104">The **GetHoldOnMailboxes** element contains the request to get the hold status for a mailbox.</span></span> 
  
```XML
<GetHoldOnMailboxes>
   <HoldId/>
</GetHoldOnMailboxes>
```

 <span data-ttu-id="07f88-105">**GetHoldOnMailboxesType**</span><span class="sxs-lookup"><span data-stu-id="07f88-105">**GetHoldOnMailboxesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="07f88-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="07f88-106">Attributes and elements</span></span>

<span data-ttu-id="07f88-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="07f88-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="07f88-108">属性</span><span class="sxs-lookup"><span data-stu-id="07f88-108">Attributes</span></span>

<span data-ttu-id="07f88-109">なし。</span><span class="sxs-lookup"><span data-stu-id="07f88-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="07f88-110">子要素</span><span class="sxs-lookup"><span data-stu-id="07f88-110">Child elements</span></span>

[<span data-ttu-id="07f88-111">HoldId</span><span class="sxs-lookup"><span data-stu-id="07f88-111">HoldId</span></span>](holdid.md)
  
### <a name="parent-elements"></a><span data-ttu-id="07f88-112">親要素</span><span class="sxs-lookup"><span data-stu-id="07f88-112">Parent elements</span></span>

<span data-ttu-id="07f88-113">なし。</span><span class="sxs-lookup"><span data-stu-id="07f88-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="07f88-114">備考</span><span class="sxs-lookup"><span data-stu-id="07f88-114">Remarks</span></span>

<span data-ttu-id="07f88-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="07f88-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="07f88-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="07f88-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="07f88-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="07f88-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="07f88-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="07f88-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="07f88-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="07f88-119">Schema name</span></span>  <br/> |<span data-ttu-id="07f88-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="07f88-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="07f88-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="07f88-121">Validation file</span></span>  <br/> |<span data-ttu-id="07f88-122">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="07f88-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="07f88-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="07f88-123">Can be empty</span></span>  <br/> ||
   

