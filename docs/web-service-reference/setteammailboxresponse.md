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
ms.openlocfilehash: 4b1ea132a86197e104b3e8873801f73876fdb289
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833456"
---
# <a name="setteammailboxresponse"></a><span data-ttu-id="da518-103">SetTeamMailboxResponse</span><span class="sxs-lookup"><span data-stu-id="da518-103">SetTeamMailboxResponse</span></span>

<span data-ttu-id="da518-104">**SetTeamMailboxResponse**要素は、 **SetTeamMailbox**要求への応答を表します。</span><span class="sxs-lookup"><span data-stu-id="da518-104">The **SetTeamMailboxResponse** element represents a response to a **SetTeamMailbox** request.</span></span> 
  
```XML
<SetTeamMailboxResponse>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</SetTeamMailboxResponse>
```

 <span data-ttu-id="da518-105">**SetTeamMailboxResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="da518-105">**SetTeamMailboxResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="da518-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="da518-106">Attributes and elements</span></span>

<span data-ttu-id="da518-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="da518-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="da518-108">属性</span><span class="sxs-lookup"><span data-stu-id="da518-108">Attributes</span></span>

<span data-ttu-id="da518-109">なし。</span><span class="sxs-lookup"><span data-stu-id="da518-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="da518-110">子要素</span><span class="sxs-lookup"><span data-stu-id="da518-110">Child elements</span></span>

<span data-ttu-id="da518-111">[メッセージ テキスト](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md)</span><span class="sxs-lookup"><span data-stu-id="da518-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="da518-112">親要素</span><span class="sxs-lookup"><span data-stu-id="da518-112">Parent elements</span></span>

<span data-ttu-id="da518-113">なし。</span><span class="sxs-lookup"><span data-stu-id="da518-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="da518-114">備考</span><span class="sxs-lookup"><span data-stu-id="da518-114">Remarks</span></span>

<span data-ttu-id="da518-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="da518-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="da518-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="da518-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="da518-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="da518-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="da518-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="da518-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="da518-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="da518-119">Schema name</span></span>  <br/> |<span data-ttu-id="da518-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="da518-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="da518-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="da518-121">Validation file</span></span>  <br/> |<span data-ttu-id="da518-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="da518-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="da518-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="da518-123">Can be empty</span></span>  <br/> |<span data-ttu-id="da518-124">false</span><span class="sxs-lookup"><span data-stu-id="da518-124">false</span></span>  <br/> |
   

