---
title: MailTipsEnabled
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailTipsEnabled
api_type:
- schema
ms.assetid: 737388b3-7b73-42af-94d3-3dbb0659718f
description: MailTipsEnabled 要素は、メール ヒントのサービスが利用可能かどうかを示します。
ms.openlocfilehash: 4fe2cae1087ab667133ec685c3325b14c4f12088
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832330"
---
# <a name="mailtipsenabled"></a><span data-ttu-id="ac981-103">MailTipsEnabled</span><span class="sxs-lookup"><span data-stu-id="ac981-103">MailTipsEnabled</span></span>

<span data-ttu-id="ac981-104">**MailTipsEnabled**要素は、メール ヒントのサービスが利用可能かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac981-104">The **MailTipsEnabled** element indicates whether the mail tips service is available.</span></span> 
  
```xml
<MailTipsEnabled>true | false</MailTipsEnabled>
```

 <span data-ttu-id="ac981-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="ac981-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ac981-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="ac981-106">Attributes and elements</span></span>

<span data-ttu-id="ac981-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ac981-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ac981-108">属性</span><span class="sxs-lookup"><span data-stu-id="ac981-108">Attributes</span></span>

<span data-ttu-id="ac981-109">なし。</span><span class="sxs-lookup"><span data-stu-id="ac981-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ac981-110">子要素</span><span class="sxs-lookup"><span data-stu-id="ac981-110">Child elements</span></span>

<span data-ttu-id="ac981-111">なし。</span><span class="sxs-lookup"><span data-stu-id="ac981-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ac981-112">親要素</span><span class="sxs-lookup"><span data-stu-id="ac981-112">Parent elements</span></span>

|<span data-ttu-id="ac981-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="ac981-113">**Element**</span></span>|<span data-ttu-id="ac981-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="ac981-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ac981-115">MailTipsConfiguration (MailTipsServiceConfiguration)</span><span class="sxs-lookup"><span data-stu-id="ac981-115">MailTipsConfiguration (MailTipsServiceConfiguration)</span></span>](mailtipsconfiguration-mailtipsserviceconfiguration.md) <br/> |<span data-ttu-id="ac981-116">メール ヒント サービスのサービスの構成情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ac981-116">Contains service configuration information for the mail tips service.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ac981-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="ac981-117">Text value</span></span>

<span data-ttu-id="ac981-118">**メール ヒントのサービスがある場合はこの要素のテキスト値は**</span><span class="sxs-lookup"><span data-stu-id="ac981-118">The text value of this element is **true** if the mail tips service is available.</span></span> <span data-ttu-id="ac981-119">値は、メール ヒントのサービスが利用できない場合**は false** 。</span><span class="sxs-lookup"><span data-stu-id="ac981-119">The value is **false** if the mail tips service is not available.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="ac981-120">備考</span><span class="sxs-lookup"><span data-stu-id="ac981-120">Remarks</span></span>

<span data-ttu-id="ac981-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="ac981-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ac981-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="ac981-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ac981-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="ac981-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ac981-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ac981-124">Schema Name</span></span>  <br/> |<span data-ttu-id="ac981-125">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="ac981-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="ac981-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ac981-126">Validation File</span></span>  <br/> |<span data-ttu-id="ac981-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ac981-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ac981-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="ac981-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="ac981-129">False</span><span class="sxs-lookup"><span data-stu-id="ac981-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ac981-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="ac981-130">See also</span></span>



- [<span data-ttu-id="ac981-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="ac981-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

