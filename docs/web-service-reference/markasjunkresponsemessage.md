---
title: MarkAsJunkResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3e2b7b53-ef3c-438e-93df-b08409dbab46
description: MarkAsJunkResponseMessage 要素は、MarkAsJunk 要求の応答メッセージを指定します。
ms.openlocfilehash: be03fc964b56c463320f09e68d143a0377300f5c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460100"
---
# <a name="markasjunkresponsemessage"></a><span data-ttu-id="fd8df-103">MarkAsJunkResponseMessage</span><span class="sxs-lookup"><span data-stu-id="fd8df-103">MarkAsJunkResponseMessage</span></span>

<span data-ttu-id="fd8df-104">**MarkAsJunkResponseMessage**要素は、 **markasjunk**要求の応答メッセージを指定します。</span><span class="sxs-lookup"><span data-stu-id="fd8df-104">The **MarkAsJunkResponseMessage** element specifies the response message for a **MarkAsJunk** request.</span></span> 
  
```XML
<MarkAsJunkResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <MovedItemId/>
</MarkAsJunkResponseMessage>
```

 <span data-ttu-id="fd8df-105">**MarkAsJunkResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="fd8df-105">**MarkAsJunkResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fd8df-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="fd8df-106">Attributes and elements</span></span>

<span data-ttu-id="fd8df-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="fd8df-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fd8df-108">属性</span><span class="sxs-lookup"><span data-stu-id="fd8df-108">Attributes</span></span>

<span data-ttu-id="fd8df-109">なし。</span><span class="sxs-lookup"><span data-stu-id="fd8df-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fd8df-110">子要素</span><span class="sxs-lookup"><span data-stu-id="fd8df-110">Child elements</span></span>

<span data-ttu-id="fd8df-111">[Messagetext](messagetext.md)  | 応答[Secmode](responsecode.md)  | [DescriptiveLinkKey](descriptivelinkkey.md)  | [MessageXml](messagexml.md)  | [Moveditemid](moveditemid.md)</span><span class="sxs-lookup"><span data-stu-id="fd8df-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [MovedItemId](moveditemid.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fd8df-112">親要素</span><span class="sxs-lookup"><span data-stu-id="fd8df-112">Parent elements</span></span>

[<span data-ttu-id="fd8df-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="fd8df-113">ResponseMessages</span></span>](responsemessages.md)
  
## <a name="remarks"></a><span data-ttu-id="fd8df-114">注釈</span><span class="sxs-lookup"><span data-stu-id="fd8df-114">Remarks</span></span>

<span data-ttu-id="fd8df-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="fd8df-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="fd8df-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="fd8df-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fd8df-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="fd8df-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fd8df-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="fd8df-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="fd8df-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="fd8df-119">Schema name</span></span>  <br/> |<span data-ttu-id="fd8df-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="fd8df-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="fd8df-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="fd8df-121">Validation file</span></span>  <br/> |<span data-ttu-id="fd8df-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="fd8df-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fd8df-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="fd8df-123">Can be empty</span></span>  <br/> ||
   

