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
ms.openlocfilehash: b7cb890a71d27340e328e39c1c463fefa080b8cb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833420"
---
# <a name="setholdonmailboxesresponsemessage"></a><span data-ttu-id="f7f61-103">SetHoldOnMailboxesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="f7f61-103">SetHoldOnMailboxesResponseMessage</span></span>

<span data-ttu-id="f7f61-104">**SetHoldOnMailboxesResponseMessage**要素は、 **SetHoldOnMailboxes**要求の応答メッセージを指定します。</span><span class="sxs-lookup"><span data-stu-id="f7f61-104">The **SetHoldOnMailboxesResponseMessage** element specifies the response message for a **SetHoldOnMailboxes** request.</span></span> 
  
```XML
<SetHoldOnMailboxesResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <MailboxHoldResult/>
</SetHoldOnMailboxesResponseMessage>
```

 <span data-ttu-id="f7f61-105">**SetHoldOnMailboxesResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="f7f61-105">**SetHoldOnMailboxesResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f7f61-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="f7f61-106">Attributes and elements</span></span>

<span data-ttu-id="f7f61-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f7f61-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f7f61-108">属性</span><span class="sxs-lookup"><span data-stu-id="f7f61-108">Attributes</span></span>

<span data-ttu-id="f7f61-109">なし。</span><span class="sxs-lookup"><span data-stu-id="f7f61-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f7f61-110">子要素</span><span class="sxs-lookup"><span data-stu-id="f7f61-110">Child elements</span></span>

<span data-ttu-id="f7f61-111">[メッセージ テキスト](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [MailboxHoldResult](mailboxholdresult.md)</span><span class="sxs-lookup"><span data-stu-id="f7f61-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [MailboxHoldResult](mailboxholdresult.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f7f61-112">親要素</span><span class="sxs-lookup"><span data-stu-id="f7f61-112">Parent elements</span></span>

[<span data-ttu-id="f7f61-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="f7f61-113">ResponseMessages</span></span>](responsemessages.md)
  
## <a name="remarks"></a><span data-ttu-id="f7f61-114">備考</span><span class="sxs-lookup"><span data-stu-id="f7f61-114">Remarks</span></span>

<span data-ttu-id="f7f61-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="f7f61-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f7f61-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="f7f61-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f7f61-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="f7f61-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f7f61-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="f7f61-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f7f61-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f7f61-119">Schema name</span></span>  <br/> |<span data-ttu-id="f7f61-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="f7f61-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f7f61-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f7f61-121">Validation file</span></span>  <br/> |<span data-ttu-id="f7f61-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f7f61-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f7f61-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="f7f61-123">Can be empty</span></span>  <br/> ||
   

