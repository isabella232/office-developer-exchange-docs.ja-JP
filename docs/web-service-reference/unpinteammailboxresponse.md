---
title: UnpinTeamMailboxResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 82dfa204-e316-432f-a753-5bd97f576389
description: UnpinTeamMailboxResponse 要素は、サイトメールボックスの固定を解除する要求に対する応答を含みます。
ms.openlocfilehash: ba1f61a7b5b5b4d5af6805c13d84ee15e3559751
ms.sourcegitcommit: eeda51cb037aa25566adb293f25574674fdb2d9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/01/2020
ms.locfileid: "45012581"
---
# <a name="unpinteammailboxresponse"></a><span data-ttu-id="b6801-103">UnpinTeamMailboxResponse</span><span class="sxs-lookup"><span data-stu-id="b6801-103">UnpinTeamMailboxResponse</span></span>

<span data-ttu-id="b6801-104">**UnpinTeamMailboxResponse**要素は、サイトメールボックスの固定を解除する要求に対する応答を含みます。</span><span class="sxs-lookup"><span data-stu-id="b6801-104">The **UnpinTeamMailboxResponse** element contains a response to a request to unpin a site mailbox.</span></span> 
  
```XML
<UnpinTeamMailboxResponse>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</UnpinTeamMailboxResponse>
```

 <span data-ttu-id="b6801-105">**UnpinTeamMailboxResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="b6801-105">**UnpinTeamMailboxResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b6801-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="b6801-106">Attributes and elements</span></span>

<span data-ttu-id="b6801-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b6801-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b6801-108">属性</span><span class="sxs-lookup"><span data-stu-id="b6801-108">Attributes</span></span>

<span data-ttu-id="b6801-109">なし。</span><span class="sxs-lookup"><span data-stu-id="b6801-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b6801-110">子要素</span><span class="sxs-lookup"><span data-stu-id="b6801-110">Child elements</span></span>

<span data-ttu-id="b6801-111">[Messagetext](messagetext.md)  | 応答[Secmode](responsecode.md)  | [DescriptiveLinkKey](descriptivelinkkey.md)  | [MessageXml](messagexml.md)</span><span class="sxs-lookup"><span data-stu-id="b6801-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b6801-112">親要素</span><span class="sxs-lookup"><span data-stu-id="b6801-112">Parent elements</span></span>

<span data-ttu-id="b6801-113">なし。</span><span class="sxs-lookup"><span data-stu-id="b6801-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b6801-114">注釈</span><span class="sxs-lookup"><span data-stu-id="b6801-114">Remarks</span></span>

<span data-ttu-id="b6801-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="b6801-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b6801-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="b6801-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b6801-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="b6801-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b6801-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="b6801-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b6801-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b6801-119">Schema name</span></span>  <br/> |<span data-ttu-id="b6801-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="b6801-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b6801-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b6801-121">Validation file</span></span>  <br/> |<span data-ttu-id="b6801-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="b6801-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b6801-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="b6801-123">Can be empty</span></span>  <br/> ||
   

