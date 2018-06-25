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
ms.openlocfilehash: 8df67294c17f9c9b786e73647878ad5b3586d788
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760797"
---
# <a name="getnonindexableitemdetailsresponsemessage"></a><span data-ttu-id="20b61-103">GetNonIndexableItemDetailsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="20b61-103">GetNonIndexableItemDetailsResponseMessage</span></span>

<span data-ttu-id="20b61-104">**GetNonIndexableItemDetailsResponseMessage**要素は、 **GetNonIndexableItemDetails**要求の応答メッセージを指定します。</span><span class="sxs-lookup"><span data-stu-id="20b61-104">The **GetNonIndexableItemDetailsResponseMessage** element specifies the response message for a **GetNonIndexableItemDetails** request.</span></span> 
  
```XML
<GetNonIndexableItemDetailsResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <NonIndexableItemDetailsResult/>
</GetNonIndexableItemDetailsResponseMessage>
```

 <span data-ttu-id="20b61-105">**GetNonIndexableItemDetailsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="20b61-105">**GetNonIndexableItemDetailsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="20b61-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="20b61-106">Attributes and elements</span></span>

<span data-ttu-id="20b61-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="20b61-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="20b61-108">属性</span><span class="sxs-lookup"><span data-stu-id="20b61-108">Attributes</span></span>

<span data-ttu-id="20b61-109">なし。</span><span class="sxs-lookup"><span data-stu-id="20b61-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="20b61-110">子要素</span><span class="sxs-lookup"><span data-stu-id="20b61-110">Child elements</span></span>

<span data-ttu-id="20b61-111">[メッセージ テキスト](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [NonIndexableItemDetailsResult](nonindexableitemdetailsresult.md)</span><span class="sxs-lookup"><span data-stu-id="20b61-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [NonIndexableItemDetailsResult](nonindexableitemdetailsresult.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="20b61-112">親要素</span><span class="sxs-lookup"><span data-stu-id="20b61-112">Parent elements</span></span>

[<span data-ttu-id="20b61-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="20b61-113">ResponseMessages</span></span>](responsemessages.md)
  
## <a name="remarks"></a><span data-ttu-id="20b61-114">備考</span><span class="sxs-lookup"><span data-stu-id="20b61-114">Remarks</span></span>

<span data-ttu-id="20b61-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="20b61-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="20b61-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="20b61-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="20b61-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="20b61-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="20b61-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="20b61-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="20b61-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="20b61-119">Schema name</span></span>  <br/> |<span data-ttu-id="20b61-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="20b61-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="20b61-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="20b61-121">Validation file</span></span>  <br/> |<span data-ttu-id="20b61-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="20b61-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="20b61-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="20b61-123">Can be empty</span></span>  <br/> |<span data-ttu-id="20b61-124">false</span><span class="sxs-lookup"><span data-stu-id="20b61-124">false</span></span>  <br/> |
   

