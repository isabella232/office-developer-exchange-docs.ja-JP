---
title: ドメイン (メッセージの追跡)
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
description: ドメイン要素を検索するドメインを表します。
ms.openlocfilehash: dc161557b59acc580d918f2e196457714bce4ba9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760142"
---
# <a name="domain-message-tracking"></a><span data-ttu-id="0d1d5-103">ドメイン (メッセージの追跡)</span><span class="sxs-lookup"><span data-stu-id="0d1d5-103">Domain (Message Tracking)</span></span>

<span data-ttu-id="0d1d5-104">**ドメイン**要素を検索するドメインを表します。</span><span class="sxs-lookup"><span data-stu-id="0d1d5-104">The **Domain** element represents the domain to search for.</span></span> 
  
```XML
<Domain/>
```

 <span data-ttu-id="0d1d5-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="0d1d5-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0d1d5-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="0d1d5-106">Attributes and elements</span></span>

<span data-ttu-id="0d1d5-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0d1d5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0d1d5-108">属性</span><span class="sxs-lookup"><span data-stu-id="0d1d5-108">Attributes</span></span>

<span data-ttu-id="0d1d5-109">なし。</span><span class="sxs-lookup"><span data-stu-id="0d1d5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0d1d5-110">子要素</span><span class="sxs-lookup"><span data-stu-id="0d1d5-110">Child elements</span></span>

<span data-ttu-id="0d1d5-111">なし。</span><span class="sxs-lookup"><span data-stu-id="0d1d5-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0d1d5-112">親要素</span><span class="sxs-lookup"><span data-stu-id="0d1d5-112">Parent elements</span></span>

|<span data-ttu-id="0d1d5-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="0d1d5-113">**Element**</span></span>|<span data-ttu-id="0d1d5-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="0d1d5-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0d1d5-115">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="0d1d5-115">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="0d1d5-116">検索するメッセージの種類の条件が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0d1d5-116">Contains criteria for the types of messages to find.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0d1d5-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="0d1d5-117">Text value</span></span>

<span data-ttu-id="0d1d5-118">文字列を表す文字列値は、この要素を使用する場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="0d1d5-118">A text value that represents a string is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0d1d5-119">備考</span><span class="sxs-lookup"><span data-stu-id="0d1d5-119">Remarks</span></span>

<span data-ttu-id="0d1d5-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="0d1d5-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0d1d5-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="0d1d5-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0d1d5-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="0d1d5-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0d1d5-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0d1d5-123">Schema Name</span></span>  <br/> |<span data-ttu-id="0d1d5-124">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="0d1d5-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0d1d5-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0d1d5-125">Validation File</span></span>  <br/> |<span data-ttu-id="0d1d5-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="0d1d5-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0d1d5-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="0d1d5-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="0d1d5-128">False</span><span class="sxs-lookup"><span data-stu-id="0d1d5-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0d1d5-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="0d1d5-129">See also</span></span>

- [<span data-ttu-id="0d1d5-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="0d1d5-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

