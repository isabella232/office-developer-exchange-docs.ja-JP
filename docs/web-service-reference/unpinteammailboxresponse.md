---
title: UnpinTeamMailboxResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 82dfa204-e316-432f-a753-5bd97f576389
description: UnpinTeamMailboxResponse 要素には、サイトのメールボックスの固定を解除するための要求への応答が含まれています。
ms.openlocfilehash: eb936c5f8d61b7005d7e2e9d5dfff7632e702a28
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839811"
---
# <a name="unpinteammailboxresponse"></a><span data-ttu-id="c63ba-103">UnpinTeamMailboxResponse</span><span class="sxs-lookup"><span data-stu-id="c63ba-103">UnpinTeamMailboxResponse</span></span>

<span data-ttu-id="c63ba-104">**UnpinTeamMailboxResponse**要素には、サイトのメールボックスの固定を解除するための要求への応答が含まれています。</span><span class="sxs-lookup"><span data-stu-id="c63ba-104">The **UnpinTeamMailboxResponse** element contains a response to a request to unpin a site mailbox.</span></span> 
  
```XML
<UnpinTeamMailboxResponse>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</UnpinTeamMailboxResponse>
```

 <span data-ttu-id="c63ba-105">**UnpinTeamMailboxResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="c63ba-105">**UnpinTeamMailboxResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c63ba-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="c63ba-106">Attributes and elements</span></span>

<span data-ttu-id="c63ba-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c63ba-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c63ba-108">属性</span><span class="sxs-lookup"><span data-stu-id="c63ba-108">Attributes</span></span>

<span data-ttu-id="c63ba-109">なし。</span><span class="sxs-lookup"><span data-stu-id="c63ba-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c63ba-110">子要素</span><span class="sxs-lookup"><span data-stu-id="c63ba-110">Child elements</span></span>

<span data-ttu-id="c63ba-111">[メッセージ テキスト](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md)</span><span class="sxs-lookup"><span data-stu-id="c63ba-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c63ba-112">親要素</span><span class="sxs-lookup"><span data-stu-id="c63ba-112">Parent elements</span></span>

<span data-ttu-id="c63ba-113">なし。</span><span class="sxs-lookup"><span data-stu-id="c63ba-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c63ba-114">備考</span><span class="sxs-lookup"><span data-stu-id="c63ba-114">Remarks</span></span>

<span data-ttu-id="c63ba-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="c63ba-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="c63ba-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="c63ba-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c63ba-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="c63ba-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c63ba-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="c63ba-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c63ba-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c63ba-119">Schema name</span></span>  <br/> |<span data-ttu-id="c63ba-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="c63ba-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c63ba-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c63ba-121">Validation file</span></span>  <br/> |<span data-ttu-id="c63ba-122">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c63ba-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c63ba-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="c63ba-123">Can be empty</span></span>  <br/> ||
   

