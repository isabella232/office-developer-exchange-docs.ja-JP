---
title: GetPhoneCallInformation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetPhoneCallInformation
api_type:
- schema
ms.assetid: 5f4ee71c-bde0-4b0d-b426-0c24dfe67585
description: GetPhoneCallInformation 要素は、電話の情報を取得する要求を指定します。
ms.openlocfilehash: 2084a8b5e13b3fa03e0bf62439978bbe81d86ce9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760835"
---
# <a name="getphonecallinformation"></a><span data-ttu-id="1d460-103">GetPhoneCallInformation</span><span class="sxs-lookup"><span data-stu-id="1d460-103">GetPhoneCallInformation</span></span>

<span data-ttu-id="1d460-104">**GetPhoneCallInformation**要素は、電話の情報を取得する要求を指定します。</span><span class="sxs-lookup"><span data-stu-id="1d460-104">The **GetPhoneCallInformation** element specifies a request to get telephone call information.</span></span> 
  
```xml
<GetPhoneCallInformation>
   <PhoneCallId/>
</GetPhoneCallInformation>
```

 <span data-ttu-id="1d460-105">**GetPhoneCallInformationType**</span><span class="sxs-lookup"><span data-stu-id="1d460-105">**GetPhoneCallInformationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1d460-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="1d460-106">Attributes and elements</span></span>

<span data-ttu-id="1d460-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1d460-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1d460-108">属性</span><span class="sxs-lookup"><span data-stu-id="1d460-108">Attributes</span></span>

<span data-ttu-id="1d460-109">なし。</span><span class="sxs-lookup"><span data-stu-id="1d460-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1d460-110">子要素</span><span class="sxs-lookup"><span data-stu-id="1d460-110">Child elements</span></span>

|<span data-ttu-id="1d460-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="1d460-111">**Element**</span></span>|<span data-ttu-id="1d460-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="1d460-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1d460-113">PhoneCallId</span><span class="sxs-lookup"><span data-stu-id="1d460-113">PhoneCallId</span></span>](phonecallid.md) <br/> |<span data-ttu-id="1d460-114">電話の識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="1d460-114">Specifies the identifier of a phone call.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1d460-115">親要素</span><span class="sxs-lookup"><span data-stu-id="1d460-115">Parent elements</span></span>

<span data-ttu-id="1d460-116">なし。</span><span class="sxs-lookup"><span data-stu-id="1d460-116">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="1d460-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="1d460-117">Text value</span></span>

<span data-ttu-id="1d460-118">なし。</span><span class="sxs-lookup"><span data-stu-id="1d460-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1d460-119">備考</span><span class="sxs-lookup"><span data-stu-id="1d460-119">Remarks</span></span>

<span data-ttu-id="1d460-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="1d460-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1d460-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="1d460-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1d460-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="1d460-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1d460-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1d460-123">Schema Name</span></span>  <br/> |<span data-ttu-id="1d460-124">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="1d460-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1d460-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1d460-125">Validation File</span></span>  <br/> |<span data-ttu-id="1d460-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="1d460-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1d460-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="1d460-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="1d460-128">False</span><span class="sxs-lookup"><span data-stu-id="1d460-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1d460-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="1d460-129">See also</span></span>



- [<span data-ttu-id="1d460-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="1d460-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

