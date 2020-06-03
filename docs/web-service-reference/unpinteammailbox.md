---
title: 非 Pxcb Ammailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1034b013-ef34-4e72-99b3-38bff475b3e8
description: 非検出応答からサイトメールボックスを削除することにより、クライアントからサイトメールボックスのピン留めを解除する要求が、非 Pxcb Ammailbox 要素に含まれています。
ms.openlocfilehash: a6b01bfa9c5908765ff04ef7f5edbef0b99a9be2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467243"
---
# <a name="unpinteammailbox"></a><span data-ttu-id="63d94-103">非 Pxcb Ammailbox</span><span class="sxs-lookup"><span data-stu-id="63d94-103">UnpinTeamMailbox</span></span>

<span data-ttu-id="63d94-104">非**検出**応答からサイトメールボックスを削除することにより、クライアントからサイトメールボックスのピン留めを解除する要求が、非**Pxcb ammailbox**要素に含まれています。</span><span class="sxs-lookup"><span data-stu-id="63d94-104">The **UnpinTeamMailbox** element contains the request to unpin a site mailbox from the client by removing it from the **Autodiscover** response.</span></span> 
  
```XML
<UnpinTeamMailbox>
   <EmailAddress/>
</UnpinTeamMailbox>
```

 <span data-ttu-id="63d94-105">**UnpinTeamMailboxRequestType**</span><span class="sxs-lookup"><span data-stu-id="63d94-105">**UnpinTeamMailboxRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="63d94-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="63d94-106">Attributes and elements</span></span>

<span data-ttu-id="63d94-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="63d94-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="63d94-108">属性</span><span class="sxs-lookup"><span data-stu-id="63d94-108">Attributes</span></span>

<span data-ttu-id="63d94-109">なし。</span><span class="sxs-lookup"><span data-stu-id="63d94-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="63d94-110">子要素</span><span class="sxs-lookup"><span data-stu-id="63d94-110">Child elements</span></span>

[<span data-ttu-id="63d94-111">EmailAddress (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="63d94-111">EmailAddress (EmailAddressType)</span></span>](emailaddress-emailaddresstype.md)
  
### <a name="parent-elements"></a><span data-ttu-id="63d94-112">親要素</span><span class="sxs-lookup"><span data-stu-id="63d94-112">Parent elements</span></span>

<span data-ttu-id="63d94-113">なし。</span><span class="sxs-lookup"><span data-stu-id="63d94-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="63d94-114">注釈</span><span class="sxs-lookup"><span data-stu-id="63d94-114">Remarks</span></span>

<span data-ttu-id="63d94-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="63d94-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="63d94-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="63d94-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="63d94-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="63d94-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="63d94-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="63d94-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="63d94-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="63d94-119">Schema name</span></span>  <br/> |<span data-ttu-id="63d94-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="63d94-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="63d94-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="63d94-121">Validation file</span></span>  <br/> |<span data-ttu-id="63d94-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="63d94-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="63d94-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="63d94-123">Can be empty</span></span>  <br/> ||
   

