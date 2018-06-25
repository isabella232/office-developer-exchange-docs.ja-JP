---
title: GetNonIndexableItemDetailsResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 6cf2aea3-c6f7-4cad-a45d-2daffeece4b6
description: GetNonIndexableItemDetailsResponse 要素は、GetNonIndexableItemDetails 要求への応答を指定します。
ms.openlocfilehash: c4b8cf4c5c20889a74cab990bc7f26c0072cdc47
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760793"
---
# <a name="getnonindexableitemdetailsresponse"></a><span data-ttu-id="a4b86-103">GetNonIndexableItemDetailsResponse</span><span class="sxs-lookup"><span data-stu-id="a4b86-103">GetNonIndexableItemDetailsResponse</span></span>

<span data-ttu-id="a4b86-104">**GetNonIndexableItemDetailsResponse**要素は、 **GetNonIndexableItemDetails**要求への応答を指定します。</span><span class="sxs-lookup"><span data-stu-id="a4b86-104">The **GetNonIndexableItemDetailsResponse** element specifies the response to a **GetNonIndexableItemDetails** request.</span></span> 
  
```XML
<GetNonIndexableItemDetailsResponse>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <NonIndexableItemDetailsResult/>
</GetNonIndexableItemDetailsResponse>
```

 <span data-ttu-id="a4b86-105">**GetNonIndexableItemDetailsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="a4b86-105">**GetNonIndexableItemDetailsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a4b86-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="a4b86-106">Attributes and elements</span></span>

<span data-ttu-id="a4b86-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a4b86-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a4b86-108">属性</span><span class="sxs-lookup"><span data-stu-id="a4b86-108">Attributes</span></span>

<span data-ttu-id="a4b86-109">なし。</span><span class="sxs-lookup"><span data-stu-id="a4b86-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a4b86-110">子要素</span><span class="sxs-lookup"><span data-stu-id="a4b86-110">Child elements</span></span>

<span data-ttu-id="a4b86-111">[メッセージ テキスト](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [NonIndexableItemDetailsResult](nonindexableitemdetailsresult.md)</span><span class="sxs-lookup"><span data-stu-id="a4b86-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [NonIndexableItemDetailsResult](nonindexableitemdetailsresult.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a4b86-112">親要素</span><span class="sxs-lookup"><span data-stu-id="a4b86-112">Parent elements</span></span>

[<span data-ttu-id="a4b86-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="a4b86-113">ResponseMessages</span></span>](responsemessages.md)
  
## <a name="remarks"></a><span data-ttu-id="a4b86-114">備考</span><span class="sxs-lookup"><span data-stu-id="a4b86-114">Remarks</span></span>

<span data-ttu-id="a4b86-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="a4b86-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="a4b86-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="a4b86-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a4b86-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="a4b86-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a4b86-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="a4b86-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a4b86-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a4b86-119">Schema name</span></span>  <br/> |<span data-ttu-id="a4b86-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="a4b86-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a4b86-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a4b86-121">Validation file</span></span>  <br/> |<span data-ttu-id="a4b86-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="a4b86-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a4b86-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="a4b86-123">Can be empty</span></span>  <br/> |<span data-ttu-id="a4b86-124">false</span><span class="sxs-lookup"><span data-stu-id="a4b86-124">false</span></span>  <br/> |
   

