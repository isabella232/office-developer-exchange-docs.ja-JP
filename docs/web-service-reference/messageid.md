---
title: メッセージ Id
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MessageId
api_type:
- schema
ms.assetid: 3b038ad5-7752-4ed8-9769-a9f1d86c8fef
description: メッセージ Id 要素は、検索するメッセージ id を表します。
ms.openlocfilehash: 66a7298db2d0052e5653742f781aa3f423b427d5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832455"
---
# <a name="messageid"></a><span data-ttu-id="45a8f-103">メッセージ Id</span><span class="sxs-lookup"><span data-stu-id="45a8f-103">MessageId</span></span>

<span data-ttu-id="45a8f-104">**メッセージ Id**要素は、検索するメッセージ id を表します。</span><span class="sxs-lookup"><span data-stu-id="45a8f-104">The **MessageId** element represents the message identification to search for.</span></span> 
  
```XML
<MessageId/>
```

 <span data-ttu-id="45a8f-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="45a8f-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="45a8f-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="45a8f-106">Attributes and elements</span></span>

<span data-ttu-id="45a8f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="45a8f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="45a8f-108">属性</span><span class="sxs-lookup"><span data-stu-id="45a8f-108">Attributes</span></span>

<span data-ttu-id="45a8f-109">なし。</span><span class="sxs-lookup"><span data-stu-id="45a8f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="45a8f-110">子要素</span><span class="sxs-lookup"><span data-stu-id="45a8f-110">Child elements</span></span>

<span data-ttu-id="45a8f-111">なし。</span><span class="sxs-lookup"><span data-stu-id="45a8f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="45a8f-112">親要素</span><span class="sxs-lookup"><span data-stu-id="45a8f-112">Parent elements</span></span>

|<span data-ttu-id="45a8f-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="45a8f-113">**Element**</span></span>|<span data-ttu-id="45a8f-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="45a8f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="45a8f-115">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="45a8f-115">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="45a8f-116">検索するメッセージの種類の条件を指定します。</span><span class="sxs-lookup"><span data-stu-id="45a8f-116">Specifies criteria for the types of messages to find.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="45a8f-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="45a8f-117">Text value</span></span>

<span data-ttu-id="45a8f-118">文字列を表す文字列値は、この要素を使用する場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="45a8f-118">A text value that represents a string is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="45a8f-119">備考</span><span class="sxs-lookup"><span data-stu-id="45a8f-119">Remarks</span></span>

<span data-ttu-id="45a8f-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="45a8f-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="45a8f-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="45a8f-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="45a8f-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="45a8f-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="45a8f-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="45a8f-123">Schema Name</span></span>  <br/> |<span data-ttu-id="45a8f-124">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="45a8f-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="45a8f-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="45a8f-125">Validation File</span></span>  <br/> |<span data-ttu-id="45a8f-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="45a8f-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="45a8f-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="45a8f-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="45a8f-128">False</span><span class="sxs-lookup"><span data-stu-id="45a8f-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="45a8f-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="45a8f-129">See also</span></span>



- [<span data-ttu-id="45a8f-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="45a8f-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

