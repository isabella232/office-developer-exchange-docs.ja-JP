---
title: SetTeamMailboxResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 78e0784b-8fe8-42f1-aa6f-4f4a0bc2505e
description: SetTeamMailboxResponse 要素は、SetTeamMailbox 要求への応答を表します。
ms.openlocfilehash: 38754cd03ab82e83b28192f6b0a3fd9e7fe87333
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467341"
---
# <a name="setteammailboxresponse"></a><span data-ttu-id="92475-103">SetTeamMailboxResponse</span><span class="sxs-lookup"><span data-stu-id="92475-103">SetTeamMailboxResponse</span></span>

<span data-ttu-id="92475-104">**SetTeamMailboxResponse**要素は、 **setteammailbox**要求への応答を表します。</span><span class="sxs-lookup"><span data-stu-id="92475-104">The **SetTeamMailboxResponse** element represents a response to a **SetTeamMailbox** request.</span></span> 
  
```XML
<SetTeamMailboxResponse>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</SetTeamMailboxResponse>
```

 <span data-ttu-id="92475-105">**SetTeamMailboxResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="92475-105">**SetTeamMailboxResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="92475-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="92475-106">Attributes and elements</span></span>

<span data-ttu-id="92475-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="92475-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="92475-108">属性</span><span class="sxs-lookup"><span data-stu-id="92475-108">Attributes</span></span>

<span data-ttu-id="92475-109">なし。</span><span class="sxs-lookup"><span data-stu-id="92475-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="92475-110">子要素</span><span class="sxs-lookup"><span data-stu-id="92475-110">Child elements</span></span>

<span data-ttu-id="92475-111">[Messagetext](messagetext.md)  | 応答[Secmode](responsecode.md)  | [DescriptiveLinkKey](descriptivelinkkey.md)  | [MessageXml](messagexml.md)</span><span class="sxs-lookup"><span data-stu-id="92475-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="92475-112">親要素</span><span class="sxs-lookup"><span data-stu-id="92475-112">Parent elements</span></span>

<span data-ttu-id="92475-113">なし。</span><span class="sxs-lookup"><span data-stu-id="92475-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="92475-114">注釈</span><span class="sxs-lookup"><span data-stu-id="92475-114">Remarks</span></span>

<span data-ttu-id="92475-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="92475-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="92475-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="92475-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="92475-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="92475-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="92475-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="92475-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="92475-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="92475-119">Schema name</span></span>  <br/> |<span data-ttu-id="92475-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="92475-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="92475-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="92475-121">Validation file</span></span>  <br/> |<span data-ttu-id="92475-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="92475-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="92475-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="92475-123">Can be empty</span></span>  <br/> |<span data-ttu-id="92475-124">false</span><span class="sxs-lookup"><span data-stu-id="92475-124">false</span></span>  <br/> |
   

