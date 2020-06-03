---
title: ドメイン (メッセージ追跡)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Domain
api_type:
- schema
ms.assetid: 4e8e9efa-8885-4ca5-bf90-424e63768dc3
description: Domain 要素は、検索対象のドメインを表します。
ms.openlocfilehash: 77da9028766881b9bc633e1b3318cd4d70c6b72f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457026"
---
# <a name="domain-message-tracking"></a><span data-ttu-id="2c1b2-103">ドメイン (メッセージ追跡)</span><span class="sxs-lookup"><span data-stu-id="2c1b2-103">Domain (Message Tracking)</span></span>

<span data-ttu-id="2c1b2-104">**Domain**要素は、検索対象のドメインを表します。</span><span class="sxs-lookup"><span data-stu-id="2c1b2-104">The **Domain** element represents the domain to search for.</span></span> 
  
```XML
<Domain/>
```

 <span data-ttu-id="2c1b2-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="2c1b2-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2c1b2-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="2c1b2-106">Attributes and elements</span></span>

<span data-ttu-id="2c1b2-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2c1b2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2c1b2-108">属性</span><span class="sxs-lookup"><span data-stu-id="2c1b2-108">Attributes</span></span>

<span data-ttu-id="2c1b2-109">なし。</span><span class="sxs-lookup"><span data-stu-id="2c1b2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2c1b2-110">子要素</span><span class="sxs-lookup"><span data-stu-id="2c1b2-110">Child elements</span></span>

<span data-ttu-id="2c1b2-111">なし。</span><span class="sxs-lookup"><span data-stu-id="2c1b2-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2c1b2-112">親要素</span><span class="sxs-lookup"><span data-stu-id="2c1b2-112">Parent elements</span></span>

|<span data-ttu-id="2c1b2-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="2c1b2-113">**Element**</span></span>|<span data-ttu-id="2c1b2-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="2c1b2-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2c1b2-115">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="2c1b2-115">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="2c1b2-116">検索するメッセージの種類に関する条件を含みます。</span><span class="sxs-lookup"><span data-stu-id="2c1b2-116">Contains criteria for the types of messages to find.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2c1b2-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="2c1b2-117">Text value</span></span>

<span data-ttu-id="2c1b2-118">この要素を使用する場合は、文字列を表すテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="2c1b2-118">A text value that represents a string is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2c1b2-119">注釈</span><span class="sxs-lookup"><span data-stu-id="2c1b2-119">Remarks</span></span>

<span data-ttu-id="2c1b2-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="2c1b2-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2c1b2-121">要素の情報</span><span class="sxs-lookup"><span data-stu-id="2c1b2-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2c1b2-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="2c1b2-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2c1b2-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2c1b2-123">Schema Name</span></span>  <br/> |<span data-ttu-id="2c1b2-124">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="2c1b2-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="2c1b2-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2c1b2-125">Validation File</span></span>  <br/> |<span data-ttu-id="2c1b2-126">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="2c1b2-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2c1b2-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="2c1b2-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="2c1b2-128">正しくない</span><span class="sxs-lookup"><span data-stu-id="2c1b2-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2c1b2-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="2c1b2-129">See also</span></span>

- [<span data-ttu-id="2c1b2-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="2c1b2-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

