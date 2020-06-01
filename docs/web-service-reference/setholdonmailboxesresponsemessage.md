---
title: SetHoldOnMailboxesResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d61de0f3-24e0-434a-946a-c53d393b7d04
description: SetHoldOnMailboxesResponseMessage 要素は、SetHoldOnMailboxes 要求の応答メッセージを指定します。
ms.openlocfilehash: a6af4181218391bc9d3c177467295d771cce4c89
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456410"
---
# <a name="setholdonmailboxesresponsemessage"></a><span data-ttu-id="947be-103">SetHoldOnMailboxesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="947be-103">SetHoldOnMailboxesResponseMessage</span></span>

<span data-ttu-id="947be-104">**SetHoldOnMailboxesResponseMessage**要素は、 **SetHoldOnMailboxes**要求の応答メッセージを指定します。</span><span class="sxs-lookup"><span data-stu-id="947be-104">The **SetHoldOnMailboxesResponseMessage** element specifies the response message for a **SetHoldOnMailboxes** request.</span></span> 
  
```XML
<SetHoldOnMailboxesResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <MailboxHoldResult/>
</SetHoldOnMailboxesResponseMessage>
```

 <span data-ttu-id="947be-105">**SetHoldOnMailboxesResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="947be-105">**SetHoldOnMailboxesResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="947be-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="947be-106">Attributes and elements</span></span>

<span data-ttu-id="947be-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="947be-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="947be-108">属性</span><span class="sxs-lookup"><span data-stu-id="947be-108">Attributes</span></span>

<span data-ttu-id="947be-109">なし。</span><span class="sxs-lookup"><span data-stu-id="947be-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="947be-110">子要素</span><span class="sxs-lookup"><span data-stu-id="947be-110">Child elements</span></span>

<span data-ttu-id="947be-111">[Messagetext](messagetext.md)  | 応答[Secmode](responsecode.md)  | [DescriptiveLinkKey](descriptivelinkkey.md)  | [MessageXml](messagexml.md)  | [MailboxHoldResult](mailboxholdresult.md)</span><span class="sxs-lookup"><span data-stu-id="947be-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [MailboxHoldResult](mailboxholdresult.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="947be-112">親要素</span><span class="sxs-lookup"><span data-stu-id="947be-112">Parent elements</span></span>

[<span data-ttu-id="947be-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="947be-113">ResponseMessages</span></span>](responsemessages.md)
  
## <a name="remarks"></a><span data-ttu-id="947be-114">注釈</span><span class="sxs-lookup"><span data-stu-id="947be-114">Remarks</span></span>

<span data-ttu-id="947be-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="947be-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="947be-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="947be-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="947be-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="947be-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="947be-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="947be-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="947be-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="947be-119">Schema name</span></span>  <br/> |<span data-ttu-id="947be-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="947be-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="947be-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="947be-121">Validation file</span></span>  <br/> |<span data-ttu-id="947be-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="947be-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="947be-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="947be-123">Can be empty</span></span>  <br/> ||
   

