---
title: SearchMailboxesResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 6f1bcbfb-d7f6-4fa0-b6f8-681a0b067007
description: SearchMailboxesResponseMessage 要素は、SearchMailboxes ボックス要求の応答メッセージを指定します。
ms.openlocfilehash: 342223b9a8cc7e91b97d637cb104f7bb160b7d5a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44448423"
---
# <a name="searchmailboxesresponsemessage"></a><span data-ttu-id="80099-103">SearchMailboxesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="80099-103">SearchMailboxesResponseMessage</span></span>

<span data-ttu-id="80099-104">**SearchMailboxesResponseMessage**要素は、 **searchmailboxes ボックス**要求の応答メッセージを指定します。</span><span class="sxs-lookup"><span data-stu-id="80099-104">The **SearchMailboxesResponseMessage** element specifies the response message for a **SearchMailboxes** request.</span></span> 
  
```XML
<SearchMailboxesResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <SearchMailboxesResult/>
</SearchMailboxesResponseMessage>
```

 <span data-ttu-id="80099-105">**SearchMailboxesResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="80099-105">**SearchMailboxesResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="80099-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="80099-106">Attributes and elements</span></span>

<span data-ttu-id="80099-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="80099-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="80099-108">属性</span><span class="sxs-lookup"><span data-stu-id="80099-108">Attributes</span></span>

<span data-ttu-id="80099-109">なし。</span><span class="sxs-lookup"><span data-stu-id="80099-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="80099-110">子要素</span><span class="sxs-lookup"><span data-stu-id="80099-110">Child elements</span></span>

<span data-ttu-id="80099-111">[Messagetext](messagetext.md)  | 応答[Secmode](responsecode.md)  | [DescriptiveLinkKey](descriptivelinkkey.md)  | [MessageXml](messagexml.md)  | [SearchMailboxesResult](searchmailboxesresult.md)</span><span class="sxs-lookup"><span data-stu-id="80099-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [SearchMailboxesResult](searchmailboxesresult.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="80099-112">親要素</span><span class="sxs-lookup"><span data-stu-id="80099-112">Parent elements</span></span>

<span data-ttu-id="80099-113">なし。</span><span class="sxs-lookup"><span data-stu-id="80099-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="80099-114">注釈</span><span class="sxs-lookup"><span data-stu-id="80099-114">Remarks</span></span>

<span data-ttu-id="80099-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="80099-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="80099-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="80099-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="80099-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="80099-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="80099-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="80099-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="80099-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="80099-119">Schema name</span></span>  <br/> |<span data-ttu-id="80099-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="80099-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="80099-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="80099-121">Validation file</span></span>  <br/> |<span data-ttu-id="80099-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="80099-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="80099-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="80099-123">Can be empty</span></span>  <br/> ||
   

