---
title: MaxRecipientsPerGetMailTipsRequest
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MaxRecipientsPerGetMailTipsRequest
api_type:
- schema
ms.assetid: 8ff5df18-1989-4217-b4c0-599232911d0c
description: MaxRecipientsPerGetMailTipsRequest 要素は、GetMailTips 操作に渡すことができる受信者の最大数を示します。
ms.openlocfilehash: 4c873fe534582e582bf5b1c1d5fd2789616e056a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832386"
---
# <a name="maxrecipientspergetmailtipsrequest"></a><span data-ttu-id="fca49-103">MaxRecipientsPerGetMailTipsRequest</span><span class="sxs-lookup"><span data-stu-id="fca49-103">MaxRecipientsPerGetMailTipsRequest</span></span>

<span data-ttu-id="fca49-104">**MaxRecipientsPerGetMailTipsRequest**要素は、 [GetMailTips 操作](getmailtips-operation.md)に渡すことができる受信者の最大数を示します。</span><span class="sxs-lookup"><span data-stu-id="fca49-104">The **MaxRecipientsPerGetMailTipsRequest** element indicates the maximum number of recipients that can be passed to the [GetMailTips operation](getmailtips-operation.md).</span></span>
  
```XML
<MaxRecipientsPerGetMailTipsRequest/>
```

 <span data-ttu-id="fca49-105">**int**</span><span class="sxs-lookup"><span data-stu-id="fca49-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fca49-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="fca49-106">Attributes and elements</span></span>

<span data-ttu-id="fca49-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="fca49-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fca49-108">属性</span><span class="sxs-lookup"><span data-stu-id="fca49-108">Attributes</span></span>

<span data-ttu-id="fca49-109">なし。</span><span class="sxs-lookup"><span data-stu-id="fca49-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fca49-110">子要素</span><span class="sxs-lookup"><span data-stu-id="fca49-110">Child elements</span></span>

<span data-ttu-id="fca49-111">なし。</span><span class="sxs-lookup"><span data-stu-id="fca49-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fca49-112">親要素</span><span class="sxs-lookup"><span data-stu-id="fca49-112">Parent elements</span></span>

|<span data-ttu-id="fca49-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="fca49-113">**Element**</span></span>|<span data-ttu-id="fca49-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="fca49-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fca49-115">MailTipsConfiguration (MailTipsServiceConfiguration)</span><span class="sxs-lookup"><span data-stu-id="fca49-115">MailTipsConfiguration (MailTipsServiceConfiguration)</span></span>](mailtipsconfiguration-mailtipsserviceconfiguration.md) <br/> |<span data-ttu-id="fca49-116">メール ヒント サービスのサービスの構成情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="fca49-116">Contains service configuration information for the mail tips service.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fca49-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="fca49-117">Text value</span></span>

<span data-ttu-id="fca49-118">テキスト値は、 [GetMailTips 操作](getmailtips-operation.md)に渡すことができる受信者の最大数を表す整数です。</span><span class="sxs-lookup"><span data-stu-id="fca49-118">The text value is an integer that represents the maximum number of recipients that can be passed to the [GetMailTips operation](getmailtips-operation.md).</span></span>
  
## <a name="remarks"></a><span data-ttu-id="fca49-119">備考</span><span class="sxs-lookup"><span data-stu-id="fca49-119">Remarks</span></span>

<span data-ttu-id="fca49-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="fca49-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fca49-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="fca49-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fca49-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="fca49-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fca49-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="fca49-123">Schema Name</span></span>  <br/> |<span data-ttu-id="fca49-124">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="fca49-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="fca49-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="fca49-125">Validation File</span></span>  <br/> |<span data-ttu-id="fca49-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="fca49-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fca49-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="fca49-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="fca49-128">False</span><span class="sxs-lookup"><span data-stu-id="fca49-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fca49-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="fca49-129">See also</span></span>



[<span data-ttu-id="fca49-130">GetMailTips 操作</span><span class="sxs-lookup"><span data-stu-id="fca49-130">GetMailTips operation</span></span>](getmailtips-operation.md)


- [<span data-ttu-id="fca49-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="fca49-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

