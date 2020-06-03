---
title: IsVoicemail メール
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsVoicemail
api_type:
- schema
ms.assetid: 96d81d6e-4b75-43ad-b151-2dd4fd57db94
description: IsVoicemail メール要素は、条件または例外を適用するために、受信メッセージがボイスメールメッセージである必要があるかどうかを示します。
ms.openlocfilehash: 8c60513a54cbf2398fde4b71ab1fbcf8a5efb608
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458139"
---
# <a name="isvoicemail"></a><span data-ttu-id="d3cb8-103">IsVoicemail メール</span><span class="sxs-lookup"><span data-stu-id="d3cb8-103">IsVoicemail</span></span>

<span data-ttu-id="d3cb8-104">**Isvoicemail**メール要素は、条件または例外を適用するために、受信メッセージがボイスメールメッセージである必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d3cb8-104">The **IsVoicemail** element indicates whether incoming messages must be voice mail messages in order for the condition or exception to apply.</span></span> 
  
```XML
<IsVoicemail>true | false</IsVoicemail>
```

 <span data-ttu-id="d3cb8-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="d3cb8-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d3cb8-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d3cb8-106">Attributes and elements</span></span>

<span data-ttu-id="d3cb8-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d3cb8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d3cb8-108">属性</span><span class="sxs-lookup"><span data-stu-id="d3cb8-108">Attributes</span></span>

<span data-ttu-id="d3cb8-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d3cb8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d3cb8-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d3cb8-110">Child elements</span></span>

<span data-ttu-id="d3cb8-111">なし。</span><span class="sxs-lookup"><span data-stu-id="d3cb8-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d3cb8-112">親要素</span><span class="sxs-lookup"><span data-stu-id="d3cb8-112">Parent elements</span></span>

|<span data-ttu-id="d3cb8-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="d3cb8-113">**Element**</span></span>|<span data-ttu-id="d3cb8-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="d3cb8-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d3cb8-115">条件</span><span class="sxs-lookup"><span data-stu-id="d3cb8-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="d3cb8-116">ルールのルールの処理を開始するときに実行される条件を表します。</span><span class="sxs-lookup"><span data-stu-id="d3cb8-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="d3cb8-117">例外</span><span class="sxs-lookup"><span data-stu-id="d3cb8-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="d3cb8-118">受信トレイルールに対して使用可能なルールの例外条件をすべて表す例外を表します。</span><span class="sxs-lookup"><span data-stu-id="d3cb8-118">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d3cb8-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="d3cb8-119">Text value</span></span>

<span data-ttu-id="d3cb8-120">**True**のテキスト値は、条件または例外を適用するために、メッセージがボイスメールメッセージである必要があることを示します。</span><span class="sxs-lookup"><span data-stu-id="d3cb8-120">A text value of **true** indicates that the message must be a voice mail message in order for the condition or exception to apply.</span></span> <span data-ttu-id="d3cb8-121">値が**false**の場合、条件または例外を適用するために、メッセージがボイスメールメッセージではない必要があることを示します。</span><span class="sxs-lookup"><span data-stu-id="d3cb8-121">A value of **false** indicates that the message must not be a voice mail message in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="d3cb8-122">注釈</span><span class="sxs-lookup"><span data-stu-id="d3cb8-122">Remarks</span></span>

<span data-ttu-id="d3cb8-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="d3cb8-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d3cb8-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d3cb8-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d3cb8-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="d3cb8-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d3cb8-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d3cb8-126">Schema Name</span></span>  <br/> |<span data-ttu-id="d3cb8-127">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="d3cb8-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d3cb8-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d3cb8-128">Validation File</span></span>  <br/> |<span data-ttu-id="d3cb8-129">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="d3cb8-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d3cb8-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d3cb8-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="d3cb8-131">正しい</span><span class="sxs-lookup"><span data-stu-id="d3cb8-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d3cb8-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="d3cb8-132">See also</span></span>



- [<span data-ttu-id="d3cb8-133">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="d3cb8-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

