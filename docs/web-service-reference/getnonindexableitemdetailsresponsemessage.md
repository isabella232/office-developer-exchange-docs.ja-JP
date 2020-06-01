---
title: GetNonIndexableItemDetailsResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 00566965-6cbd-4f31-9fa9-85b3e5559c0c
description: GetNonIndexableItemDetailsResponseMessage 要素は、GetNonIndexableItemDetails 要求の応答メッセージを指定します。
ms.openlocfilehash: 4cf6b422cc29b20b09d05ea45628fa7133b437b2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456522"
---
# <a name="getnonindexableitemdetailsresponsemessage"></a><span data-ttu-id="cd5c9-103">GetNonIndexableItemDetailsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="cd5c9-103">GetNonIndexableItemDetailsResponseMessage</span></span>

<span data-ttu-id="cd5c9-104">**GetNonIndexableItemDetailsResponseMessage**要素は、 **Getnonindexableitemdetails**要求の応答メッセージを指定します。</span><span class="sxs-lookup"><span data-stu-id="cd5c9-104">The **GetNonIndexableItemDetailsResponseMessage** element specifies the response message for a **GetNonIndexableItemDetails** request.</span></span> 
  
```XML
<GetNonIndexableItemDetailsResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <NonIndexableItemDetailsResult/>
</GetNonIndexableItemDetailsResponseMessage>
```

 <span data-ttu-id="cd5c9-105">**Getnonindexableitem/[Responsemessagetype]**</span><span class="sxs-lookup"><span data-stu-id="cd5c9-105">**GetNonIndexableItemDetailsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cd5c9-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="cd5c9-106">Attributes and elements</span></span>

<span data-ttu-id="cd5c9-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="cd5c9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cd5c9-108">属性</span><span class="sxs-lookup"><span data-stu-id="cd5c9-108">Attributes</span></span>

<span data-ttu-id="cd5c9-109">なし。</span><span class="sxs-lookup"><span data-stu-id="cd5c9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cd5c9-110">子要素</span><span class="sxs-lookup"><span data-stu-id="cd5c9-110">Child elements</span></span>

<span data-ttu-id="cd5c9-111">[Messagetext](messagetext.md)  | 応答[Secmode](responsecode.md)  | [DescriptiveLinkKey](descriptivelinkkey.md)  | [MessageXml](messagexml.md)  | [Nonindexableitemの取得結果](nonindexableitemdetailsresult.md)</span><span class="sxs-lookup"><span data-stu-id="cd5c9-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [NonIndexableItemDetailsResult](nonindexableitemdetailsresult.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="cd5c9-112">親要素</span><span class="sxs-lookup"><span data-stu-id="cd5c9-112">Parent elements</span></span>

[<span data-ttu-id="cd5c9-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="cd5c9-113">ResponseMessages</span></span>](responsemessages.md)
  
## <a name="remarks"></a><span data-ttu-id="cd5c9-114">注釈</span><span class="sxs-lookup"><span data-stu-id="cd5c9-114">Remarks</span></span>

<span data-ttu-id="cd5c9-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="cd5c9-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="cd5c9-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="cd5c9-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cd5c9-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="cd5c9-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cd5c9-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="cd5c9-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="cd5c9-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="cd5c9-119">Schema name</span></span>  <br/> |<span data-ttu-id="cd5c9-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="cd5c9-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="cd5c9-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="cd5c9-121">Validation file</span></span>  <br/> |<span data-ttu-id="cd5c9-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="cd5c9-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="cd5c9-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="cd5c9-123">Can be empty</span></span>  <br/> |<span data-ttu-id="cd5c9-124">false</span><span class="sxs-lookup"><span data-stu-id="cd5c9-124">false</span></span>  <br/> |
   

