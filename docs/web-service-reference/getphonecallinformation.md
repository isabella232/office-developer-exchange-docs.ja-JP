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
description: GetPhoneCallInformation 要素は、電話呼び出し情報を取得するための要求を指定します。
ms.openlocfilehash: b835cd301b1c243e88034d1057026ef1305b9038
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530198"
---
# <a name="getphonecallinformation"></a><span data-ttu-id="a1923-103">GetPhoneCallInformation</span><span class="sxs-lookup"><span data-stu-id="a1923-103">GetPhoneCallInformation</span></span>

<span data-ttu-id="a1923-104">**GetPhoneCallInformation**要素は、電話呼び出し情報を取得するための要求を指定します。</span><span class="sxs-lookup"><span data-stu-id="a1923-104">The **GetPhoneCallInformation** element specifies a request to get telephone call information.</span></span> 
  
```xml
<GetPhoneCallInformation>
   <PhoneCallId/>
</GetPhoneCallInformation>
```

 <span data-ttu-id="a1923-105">**GetPhoneCallInformationType**</span><span class="sxs-lookup"><span data-stu-id="a1923-105">**GetPhoneCallInformationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a1923-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="a1923-106">Attributes and elements</span></span>

<span data-ttu-id="a1923-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a1923-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a1923-108">属性</span><span class="sxs-lookup"><span data-stu-id="a1923-108">Attributes</span></span>

<span data-ttu-id="a1923-109">なし。</span><span class="sxs-lookup"><span data-stu-id="a1923-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a1923-110">子要素</span><span class="sxs-lookup"><span data-stu-id="a1923-110">Child elements</span></span>

|<span data-ttu-id="a1923-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="a1923-111">**Element**</span></span>|<span data-ttu-id="a1923-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="a1923-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a1923-113">PhoneCallId</span><span class="sxs-lookup"><span data-stu-id="a1923-113">PhoneCallId</span></span>](phonecallid.md) <br/> |<span data-ttu-id="a1923-114">電話呼び出しの id を指定します。</span><span class="sxs-lookup"><span data-stu-id="a1923-114">Specifies the identifier of a phone call.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a1923-115">親要素</span><span class="sxs-lookup"><span data-stu-id="a1923-115">Parent elements</span></span>

<span data-ttu-id="a1923-116">なし。</span><span class="sxs-lookup"><span data-stu-id="a1923-116">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="a1923-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="a1923-117">Text value</span></span>

<span data-ttu-id="a1923-118">なし。</span><span class="sxs-lookup"><span data-stu-id="a1923-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a1923-119">注釈</span><span class="sxs-lookup"><span data-stu-id="a1923-119">Remarks</span></span>

<span data-ttu-id="a1923-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="a1923-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a1923-121">要素の情報</span><span class="sxs-lookup"><span data-stu-id="a1923-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a1923-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="a1923-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a1923-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a1923-123">Schema Name</span></span>  <br/> |<span data-ttu-id="a1923-124">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="a1923-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a1923-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a1923-125">Validation File</span></span>  <br/> |<span data-ttu-id="a1923-126">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="a1923-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a1923-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="a1923-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="a1923-128">正しくない</span><span class="sxs-lookup"><span data-stu-id="a1923-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a1923-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="a1923-129">See also</span></span>



- [<span data-ttu-id="a1923-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="a1923-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

