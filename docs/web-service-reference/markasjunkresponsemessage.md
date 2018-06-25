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
ms.openlocfilehash: 146ece430436c60fced53d4dfbfd7d92c0e42e98
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832352"
---
# <a name="markasjunkresponsemessage"></a><span data-ttu-id="d1d02-103">MarkAsJunkResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d1d02-103">MarkAsJunkResponseMessage</span></span>

<span data-ttu-id="d1d02-104">**MarkAsJunkResponseMessage**要素は、 **MarkAsJunk**要求の応答メッセージを指定します。</span><span class="sxs-lookup"><span data-stu-id="d1d02-104">The **MarkAsJunkResponseMessage** element specifies the response message for a **MarkAsJunk** request.</span></span> 
  
```XML
<MarkAsJunkResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <MovedItemId/>
</MarkAsJunkResponseMessage>
```

 <span data-ttu-id="d1d02-105">**MarkAsJunkResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="d1d02-105">**MarkAsJunkResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d1d02-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="d1d02-106">Attributes and elements</span></span>

<span data-ttu-id="d1d02-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d1d02-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d1d02-108">属性</span><span class="sxs-lookup"><span data-stu-id="d1d02-108">Attributes</span></span>

<span data-ttu-id="d1d02-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d1d02-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d1d02-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d1d02-110">Child elements</span></span>

<span data-ttu-id="d1d02-111">[メッセージ テキスト](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [MovedItemId](moveditemid.md)</span><span class="sxs-lookup"><span data-stu-id="d1d02-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [MovedItemId](moveditemid.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d1d02-112">親要素</span><span class="sxs-lookup"><span data-stu-id="d1d02-112">Parent elements</span></span>

[<span data-ttu-id="d1d02-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="d1d02-113">ResponseMessages</span></span>](responsemessages.md)
  
## <a name="remarks"></a><span data-ttu-id="d1d02-114">備考</span><span class="sxs-lookup"><span data-stu-id="d1d02-114">Remarks</span></span>

<span data-ttu-id="d1d02-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="d1d02-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d1d02-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="d1d02-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d1d02-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="d1d02-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d1d02-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="d1d02-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d1d02-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d1d02-119">Schema name</span></span>  <br/> |<span data-ttu-id="d1d02-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="d1d02-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d1d02-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d1d02-121">Validation file</span></span>  <br/> |<span data-ttu-id="d1d02-122">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d1d02-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d1d02-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="d1d02-123">Can be empty</span></span>  <br/> ||
   

