---
title: IsVoicemail
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
description: IsVoicemail 要素は、適用の条件または例外のためにボイス メール メッセージを受信したメッセージがある必要があるかどうかを示します。
ms.openlocfilehash: 513498301aa65eaf0cac5769c940eeedf5c9e629
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832136"
---
# <a name="isvoicemail"></a><span data-ttu-id="962d3-103">IsVoicemail</span><span class="sxs-lookup"><span data-stu-id="962d3-103">IsVoicemail</span></span>

<span data-ttu-id="962d3-104">**IsVoicemail**要素は、適用の条件または例外のためにボイス メール メッセージを受信したメッセージがある必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="962d3-104">The **IsVoicemail** element indicates whether incoming messages must be voice mail messages in order for the condition or exception to apply.</span></span> 
  
```XML
<IsVoicemail>true | false</IsVoicemail>
```

 <span data-ttu-id="962d3-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="962d3-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="962d3-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="962d3-106">Attributes and elements</span></span>

<span data-ttu-id="962d3-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="962d3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="962d3-108">属性</span><span class="sxs-lookup"><span data-stu-id="962d3-108">Attributes</span></span>

<span data-ttu-id="962d3-109">なし。</span><span class="sxs-lookup"><span data-stu-id="962d3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="962d3-110">子要素</span><span class="sxs-lookup"><span data-stu-id="962d3-110">Child elements</span></span>

<span data-ttu-id="962d3-111">なし。</span><span class="sxs-lookup"><span data-stu-id="962d3-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="962d3-112">親要素</span><span class="sxs-lookup"><span data-stu-id="962d3-112">Parent elements</span></span>

|<span data-ttu-id="962d3-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="962d3-113">**Element**</span></span>|<span data-ttu-id="962d3-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="962d3-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="962d3-115">条件</span><span class="sxs-lookup"><span data-stu-id="962d3-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="962d3-116">条件を表しますが、満たされるとときに、ルールのルールの処理をトリガーします。</span><span class="sxs-lookup"><span data-stu-id="962d3-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="962d3-117">Exceptions</span><span class="sxs-lookup"><span data-stu-id="962d3-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="962d3-118">受信トレイ ルールの使用可能なルールの例外条件をすべてを表す例外を表します。</span><span class="sxs-lookup"><span data-stu-id="962d3-118">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="962d3-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="962d3-119">Text value</span></span>

<span data-ttu-id="962d3-120">**True**の場合、テキスト値は、メッセージは適用の条件または例外のためにボイス メール メッセージである必要があることを示します。</span><span class="sxs-lookup"><span data-stu-id="962d3-120">A text value of **true** indicates that the message must be a voice mail message in order for the condition or exception to apply.</span></span> <span data-ttu-id="962d3-121">**False**の値は、メッセージでは、ボイス メール メッセージに適用する条件または例外の順にならないということを示します。</span><span class="sxs-lookup"><span data-stu-id="962d3-121">A value of **false** indicates that the message must not be a voice mail message in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="962d3-122">備考</span><span class="sxs-lookup"><span data-stu-id="962d3-122">Remarks</span></span>

<span data-ttu-id="962d3-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="962d3-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="962d3-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="962d3-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="962d3-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="962d3-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="962d3-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="962d3-126">Schema Name</span></span>  <br/> |<span data-ttu-id="962d3-127">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="962d3-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="962d3-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="962d3-128">Validation File</span></span>  <br/> |<span data-ttu-id="962d3-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="962d3-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="962d3-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="962d3-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="962d3-131">True</span><span class="sxs-lookup"><span data-stu-id="962d3-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="962d3-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="962d3-132">See also</span></span>



- [<span data-ttu-id="962d3-133">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="962d3-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

