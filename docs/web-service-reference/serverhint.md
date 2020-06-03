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
description: ServerHint 要素は、リモートサイトまたはフォレスト内のメッセージを追跡するための開始点を表します。
ms.openlocfilehash: 76a719901f4e4d1da67ce377ab8b73e4a4592dc4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461990"
---
# <a name="serverhint"></a><span data-ttu-id="d894d-103">ServerHint</span><span class="sxs-lookup"><span data-stu-id="d894d-103">ServerHint</span></span>

<span data-ttu-id="d894d-104">**Serverhint**要素は、リモートサイトまたはフォレスト内のメッセージを追跡するための開始点を表します。</span><span class="sxs-lookup"><span data-stu-id="d894d-104">The **ServerHint** element represents the starting point for tracking a message in a remote site or forest.</span></span> 
  
```xml
<ServerHint/>
```

 <span data-ttu-id="d894d-105">**string**</span><span class="sxs-lookup"><span data-stu-id="d894d-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d894d-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d894d-106">Attributes and elements</span></span>

<span data-ttu-id="d894d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d894d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d894d-108">属性</span><span class="sxs-lookup"><span data-stu-id="d894d-108">Attributes</span></span>

<span data-ttu-id="d894d-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d894d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d894d-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d894d-110">Child elements</span></span>

<span data-ttu-id="d894d-111">なし。</span><span class="sxs-lookup"><span data-stu-id="d894d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d894d-112">親要素</span><span class="sxs-lookup"><span data-stu-id="d894d-112">Parent elements</span></span>

|<span data-ttu-id="d894d-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="d894d-113">**Element**</span></span>|<span data-ttu-id="d894d-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="d894d-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d894d-115">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="d894d-115">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="d894d-116">検索するメッセージの種類の条件を指定します。</span><span class="sxs-lookup"><span data-stu-id="d894d-116">Specifies criteria for the types of messages to find.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d894d-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="d894d-117">Text value</span></span>

<span data-ttu-id="d894d-118">なし。</span><span class="sxs-lookup"><span data-stu-id="d894d-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d894d-119">注釈</span><span class="sxs-lookup"><span data-stu-id="d894d-119">Remarks</span></span>

<span data-ttu-id="d894d-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="d894d-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d894d-121">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d894d-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d894d-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="d894d-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d894d-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d894d-123">Schema Name</span></span>  <br/> |<span data-ttu-id="d894d-124">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="d894d-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d894d-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d894d-125">Validation File</span></span>  <br/> |<span data-ttu-id="d894d-126">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="d894d-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d894d-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d894d-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="d894d-128">正しくない</span><span class="sxs-lookup"><span data-stu-id="d894d-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d894d-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="d894d-129">See also</span></span>



[<span data-ttu-id="d894d-130">FindMessageTrackingReport 操作</span><span class="sxs-lookup"><span data-stu-id="d894d-130">FindMessageTrackingReport operation</span></span>](findmessagetrackingreport-operation.md)


- [<span data-ttu-id="d894d-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="d894d-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

