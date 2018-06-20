---
title: ServerHint
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ServerHint
api_type:
- schema
ms.assetid: 5ac60472-a565-43d1-a5fb-8be0c9511f82
description: ServerHint 要素は、リモート ・ サイトまたはフォレスト内のメッセージを追跡するための開始点を表します。
ms.openlocfilehash: 96953f70c239254d15b9d8173f951b52ca95a546
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833376"
---
# <a name="serverhint"></a><span data-ttu-id="6a322-103">ServerHint</span><span class="sxs-lookup"><span data-stu-id="6a322-103">ServerHint</span></span>

<span data-ttu-id="6a322-104">**ServerHint**要素は、リモート ・ サイトまたはフォレスト内のメッセージを追跡するための開始点を表します。</span><span class="sxs-lookup"><span data-stu-id="6a322-104">The **ServerHint** element represents the starting point for tracking a message in a remote site or forest.</span></span> 
  
```xml
<ServerHint/>
```

 <span data-ttu-id="6a322-105">**string**</span><span class="sxs-lookup"><span data-stu-id="6a322-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6a322-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="6a322-106">Attributes and elements</span></span>

<span data-ttu-id="6a322-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6a322-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6a322-108">属性</span><span class="sxs-lookup"><span data-stu-id="6a322-108">Attributes</span></span>

<span data-ttu-id="6a322-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6a322-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6a322-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6a322-110">Child elements</span></span>

<span data-ttu-id="6a322-111">なし。</span><span class="sxs-lookup"><span data-stu-id="6a322-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6a322-112">親要素</span><span class="sxs-lookup"><span data-stu-id="6a322-112">Parent elements</span></span>

|<span data-ttu-id="6a322-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="6a322-113">**Element**</span></span>|<span data-ttu-id="6a322-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="6a322-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6a322-115">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="6a322-115">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="6a322-116">検索するメッセージの種類の条件を指定します。</span><span class="sxs-lookup"><span data-stu-id="6a322-116">Specifies criteria for the types of messages to find.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6a322-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="6a322-117">Text value</span></span>

<span data-ttu-id="6a322-118">なし。</span><span class="sxs-lookup"><span data-stu-id="6a322-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6a322-119">備考</span><span class="sxs-lookup"><span data-stu-id="6a322-119">Remarks</span></span>

<span data-ttu-id="6a322-120">この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="6a322-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6a322-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="6a322-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6a322-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="6a322-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6a322-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6a322-123">Schema Name</span></span>  <br/> |<span data-ttu-id="6a322-124">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="6a322-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6a322-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6a322-125">Validation File</span></span>  <br/> |<span data-ttu-id="6a322-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6a322-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6a322-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="6a322-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="6a322-128">False</span><span class="sxs-lookup"><span data-stu-id="6a322-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6a322-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="6a322-129">See also</span></span>



[<span data-ttu-id="6a322-130">FindMessageTrackingReport 操作</span><span class="sxs-lookup"><span data-stu-id="6a322-130">FindMessageTrackingReport operation</span></span>](findmessagetrackingreport-operation.md)


- [<span data-ttu-id="6a322-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="6a322-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

