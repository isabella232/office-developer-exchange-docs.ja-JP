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
ms.openlocfilehash: fee6cd4781533cb779a971ebba46707527623dcc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462837"
---
# <a name="getholdonmailboxesresponse"></a><span data-ttu-id="faa16-103">GetHoldOnMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="faa16-103">GetHoldOnMailboxesResponse</span></span>

<span data-ttu-id="faa16-104">**GetHoldOnMailboxes**要素には、メールボックスの保留状態を取得する要求が含まれています。</span><span class="sxs-lookup"><span data-stu-id="faa16-104">The **GetHoldOnMailboxes** element contains the request to get the hold status for a mailbox.</span></span> 
  
```XML
<GetHoldOnMailboxes>
   <HoldId/>
</GetHoldOnMailboxes>
```

 <span data-ttu-id="faa16-105">**GetHoldOnMailboxesType**</span><span class="sxs-lookup"><span data-stu-id="faa16-105">**GetHoldOnMailboxesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="faa16-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="faa16-106">Attributes and elements</span></span>

<span data-ttu-id="faa16-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="faa16-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="faa16-108">属性</span><span class="sxs-lookup"><span data-stu-id="faa16-108">Attributes</span></span>

<span data-ttu-id="faa16-109">なし。</span><span class="sxs-lookup"><span data-stu-id="faa16-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="faa16-110">子要素</span><span class="sxs-lookup"><span data-stu-id="faa16-110">Child elements</span></span>

[<span data-ttu-id="faa16-111">HoldId</span><span class="sxs-lookup"><span data-stu-id="faa16-111">HoldId</span></span>](holdid.md)
  
### <a name="parent-elements"></a><span data-ttu-id="faa16-112">親要素</span><span class="sxs-lookup"><span data-stu-id="faa16-112">Parent elements</span></span>

<span data-ttu-id="faa16-113">なし。</span><span class="sxs-lookup"><span data-stu-id="faa16-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="faa16-114">注釈</span><span class="sxs-lookup"><span data-stu-id="faa16-114">Remarks</span></span>

<span data-ttu-id="faa16-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="faa16-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="faa16-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="faa16-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="faa16-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="faa16-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="faa16-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="faa16-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="faa16-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="faa16-119">Schema name</span></span>  <br/> |<span data-ttu-id="faa16-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="faa16-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="faa16-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="faa16-121">Validation file</span></span>  <br/> |<span data-ttu-id="faa16-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="faa16-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="faa16-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="faa16-123">Can be empty</span></span>  <br/> ||
   

