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
ms.openlocfilehash: 2535ef43228c8ecca958da88178cfb2cb6584ad3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44452784"
---
# <a name="getnonindexableitemstatisticsresponse"></a><span data-ttu-id="d338f-103">GetNonIndexableItemStatisticsResponse</span><span class="sxs-lookup"><span data-stu-id="d338f-103">GetNonIndexableItemStatisticsResponse</span></span>

<span data-ttu-id="d338f-104">**GetNonIndexableItemStatisticsResponse**要素は、 **Getnonindexableitemstatistics**要求への応答を指定します。</span><span class="sxs-lookup"><span data-stu-id="d338f-104">The **GetNonIndexableItemStatisticsResponse** element specifies the response to a **GetNonIndexableItemStatistics** request.</span></span> 
  
```XML
<GetNonIndexableItemStatisticsResponse>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <NonIndexableItemStatistics/>
</GetNonIndexableItemStatisticsResponse>
```

 <span data-ttu-id="d338f-105">**GetNonIndexableItemStatisticsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="d338f-105">**GetNonIndexableItemStatisticsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d338f-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d338f-106">Attributes and elements</span></span>

<span data-ttu-id="d338f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d338f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d338f-108">属性</span><span class="sxs-lookup"><span data-stu-id="d338f-108">Attributes</span></span>

<span data-ttu-id="d338f-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d338f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d338f-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d338f-110">Child elements</span></span>

<span data-ttu-id="d338f-111">[Messagetext](messagetext.md)  | 応答[Secmode](responsecode.md)  | [DescriptiveLinkKey](descriptivelinkkey.md)  | [MessageXml](messagexml.md)  | [Getnonindexableitemstatistics](getnonindexableitemstatistics.md)</span><span class="sxs-lookup"><span data-stu-id="d338f-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [GetNonIndexableItemStatistics](getnonindexableitemstatistics.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d338f-112">親要素</span><span class="sxs-lookup"><span data-stu-id="d338f-112">Parent elements</span></span>

[<span data-ttu-id="d338f-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="d338f-113">ResponseMessages</span></span>](responsemessages.md)
  
## <a name="remarks"></a><span data-ttu-id="d338f-114">注釈</span><span class="sxs-lookup"><span data-stu-id="d338f-114">Remarks</span></span>

<span data-ttu-id="d338f-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="d338f-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d338f-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="d338f-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d338f-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d338f-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d338f-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="d338f-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d338f-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d338f-119">Schema name</span></span>  <br/> |<span data-ttu-id="d338f-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="d338f-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d338f-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d338f-121">Validation file</span></span>  <br/> |<span data-ttu-id="d338f-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="d338f-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d338f-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="d338f-123">Can be empty</span></span>  <br/> |<span data-ttu-id="d338f-124">false</span><span class="sxs-lookup"><span data-stu-id="d338f-124">false</span></span>  <br/> |
   

