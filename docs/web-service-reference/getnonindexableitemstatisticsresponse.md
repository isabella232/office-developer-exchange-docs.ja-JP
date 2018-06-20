---
title: GetNonIndexableItemStatisticsResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8f68b73c-d6b0-4bb5-b89a-fd398d09346c
description: GetNonIndexableItemStatisticsResponse 要素は、GetNonIndexableItemStatistics 要求への応答を指定します。
ms.openlocfilehash: 95f59df251517cb76183f6f8bd6c2d4a68bd4cdb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760803"
---
# <a name="getnonindexableitemstatisticsresponse"></a><span data-ttu-id="4835a-103">GetNonIndexableItemStatisticsResponse</span><span class="sxs-lookup"><span data-stu-id="4835a-103">GetNonIndexableItemStatisticsResponse</span></span>

<span data-ttu-id="4835a-104">**GetNonIndexableItemStatisticsResponse**要素は、 **GetNonIndexableItemStatistics**要求への応答を指定します。</span><span class="sxs-lookup"><span data-stu-id="4835a-104">The **GetNonIndexableItemStatisticsResponse** element specifies the response to a **GetNonIndexableItemStatistics** request.</span></span> 
  
```XML
<GetNonIndexableItemStatisticsResponse>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <NonIndexableItemStatistics/>
</GetNonIndexableItemStatisticsResponse>
```

 <span data-ttu-id="4835a-105">**GetNonIndexableItemStatisticsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="4835a-105">**GetNonIndexableItemStatisticsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4835a-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="4835a-106">Attributes and elements</span></span>

<span data-ttu-id="4835a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4835a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4835a-108">属性</span><span class="sxs-lookup"><span data-stu-id="4835a-108">Attributes</span></span>

<span data-ttu-id="4835a-109">なし。</span><span class="sxs-lookup"><span data-stu-id="4835a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4835a-110">子要素</span><span class="sxs-lookup"><span data-stu-id="4835a-110">Child elements</span></span>

<span data-ttu-id="4835a-111">[メッセージ テキスト](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [GetNonIndexableItemStatistics](getnonindexableitemstatistics.md)</span><span class="sxs-lookup"><span data-stu-id="4835a-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [GetNonIndexableItemStatistics](getnonindexableitemstatistics.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4835a-112">親要素</span><span class="sxs-lookup"><span data-stu-id="4835a-112">Parent elements</span></span>

[<span data-ttu-id="4835a-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="4835a-113">ResponseMessages</span></span>](responsemessages.md)
  
## <a name="remarks"></a><span data-ttu-id="4835a-114">備考</span><span class="sxs-lookup"><span data-stu-id="4835a-114">Remarks</span></span>

<span data-ttu-id="4835a-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="4835a-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4835a-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="4835a-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4835a-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="4835a-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4835a-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="4835a-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4835a-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4835a-119">Schema name</span></span>  <br/> |<span data-ttu-id="4835a-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="4835a-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4835a-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4835a-121">Validation file</span></span>  <br/> |<span data-ttu-id="4835a-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="4835a-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4835a-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="4835a-123">Can be empty</span></span>  <br/> |<span data-ttu-id="4835a-124">false</span><span class="sxs-lookup"><span data-stu-id="4835a-124">false</span></span>  <br/> |
   

