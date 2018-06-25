---
title: UnpinTeamMailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1034b013-ef34-4e72-99b3-38bff475b3e8
description: UnpinTeamMailbox 要素には、自動検出応答から削除することによって、クライアントからサイトのメールボックスの固定を解除する要求が含まれています。
ms.openlocfilehash: d303b47f0796f9bec7e9f198afa81d2ecd9fd5cd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839807"
---
# <a name="unpinteammailbox"></a><span data-ttu-id="57e1b-103">UnpinTeamMailbox</span><span class="sxs-lookup"><span data-stu-id="57e1b-103">UnpinTeamMailbox</span></span>

<span data-ttu-id="57e1b-104">**UnpinTeamMailbox**要素には、**自動検出**応答から削除することによって、クライアントからサイトのメールボックスの固定を解除する要求が含まれています。</span><span class="sxs-lookup"><span data-stu-id="57e1b-104">The **UnpinTeamMailbox** element contains the request to unpin a site mailbox from the client by removing it from the **Autodiscover** response.</span></span> 
  
```XML
<UnpinTeamMailbox>
   <EmailAddress/>
</UnpinTeamMailbox>
```

 <span data-ttu-id="57e1b-105">**UnpinTeamMailboxRequestType**</span><span class="sxs-lookup"><span data-stu-id="57e1b-105">**UnpinTeamMailboxRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="57e1b-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="57e1b-106">Attributes and elements</span></span>

<span data-ttu-id="57e1b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="57e1b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="57e1b-108">属性</span><span class="sxs-lookup"><span data-stu-id="57e1b-108">Attributes</span></span>

<span data-ttu-id="57e1b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="57e1b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="57e1b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="57e1b-110">Child elements</span></span>

[<span data-ttu-id="57e1b-111">EmailAddress (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="57e1b-111">EmailAddress (EmailAddressType)</span></span>](emailaddress-emailaddresstype.md)
  
### <a name="parent-elements"></a><span data-ttu-id="57e1b-112">親要素</span><span class="sxs-lookup"><span data-stu-id="57e1b-112">Parent elements</span></span>

<span data-ttu-id="57e1b-113">なし。</span><span class="sxs-lookup"><span data-stu-id="57e1b-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="57e1b-114">備考</span><span class="sxs-lookup"><span data-stu-id="57e1b-114">Remarks</span></span>

<span data-ttu-id="57e1b-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="57e1b-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="57e1b-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="57e1b-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="57e1b-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="57e1b-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="57e1b-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="57e1b-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="57e1b-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="57e1b-119">Schema name</span></span>  <br/> |<span data-ttu-id="57e1b-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="57e1b-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="57e1b-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="57e1b-121">Validation file</span></span>  <br/> |<span data-ttu-id="57e1b-122">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="57e1b-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="57e1b-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="57e1b-123">Can be empty</span></span>  <br/> ||
   

