---
title: 電話
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DisconnectPhoneCall
api_type:
- schema
ms.assetid: f9252536-9852-4dd9-9ebc-91f5cf281171
description: 外さ Phonecall 要素は、呼び出しを切断する要求を表します。
ms.openlocfilehash: 8d64ecb9dce1d8b7efcebc70686db8fcbf867217
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529708"
---
# <a name="disconnectphonecall"></a><span data-ttu-id="a49cd-103">電話</span><span class="sxs-lookup"><span data-stu-id="a49cd-103">DisconnectPhoneCall</span></span>

<span data-ttu-id="a49cd-104">外さ**phonecall**要素は、呼び出しを切断する要求を表します。</span><span class="sxs-lookup"><span data-stu-id="a49cd-104">The **DisconnectPhoneCall** element represents a request to disconnect a call.</span></span> 
  
```xml
<DisconnectPhoneCall>
   <PhoneCallId/>
</DisconnectPhoneCall>
```

 <span data-ttu-id="a49cd-105">**DisconnectPhoneCallType**</span><span class="sxs-lookup"><span data-stu-id="a49cd-105">**DisconnectPhoneCallType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a49cd-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="a49cd-106">Attributes and elements</span></span>

<span data-ttu-id="a49cd-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a49cd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a49cd-108">属性</span><span class="sxs-lookup"><span data-stu-id="a49cd-108">Attributes</span></span>

<span data-ttu-id="a49cd-109">なし。</span><span class="sxs-lookup"><span data-stu-id="a49cd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a49cd-110">子要素</span><span class="sxs-lookup"><span data-stu-id="a49cd-110">Child elements</span></span>

|<span data-ttu-id="a49cd-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="a49cd-111">**Element**</span></span>|<span data-ttu-id="a49cd-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="a49cd-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a49cd-113">PhoneCallId</span><span class="sxs-lookup"><span data-stu-id="a49cd-113">PhoneCallId</span></span>](phonecallid.md) <br/> |<span data-ttu-id="a49cd-114">切断する呼び出しの識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="a49cd-114">Specifies the identifier of the call to disconnect.</span></span> <span data-ttu-id="a49cd-115">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="a49cd-115">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a49cd-116">親要素</span><span class="sxs-lookup"><span data-stu-id="a49cd-116">Parent elements</span></span>

<span data-ttu-id="a49cd-117">なし。</span><span class="sxs-lookup"><span data-stu-id="a49cd-117">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="a49cd-118">テキスト値</span><span class="sxs-lookup"><span data-stu-id="a49cd-118">Text value</span></span>

<span data-ttu-id="a49cd-119">なし。</span><span class="sxs-lookup"><span data-stu-id="a49cd-119">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a49cd-120">注釈</span><span class="sxs-lookup"><span data-stu-id="a49cd-120">Remarks</span></span>

<span data-ttu-id="a49cd-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="a49cd-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a49cd-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="a49cd-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a49cd-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="a49cd-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a49cd-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a49cd-124">Schema Name</span></span>  <br/> |<span data-ttu-id="a49cd-125">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="a49cd-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a49cd-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a49cd-126">Validation File</span></span>  <br/> |<span data-ttu-id="a49cd-127">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="a49cd-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a49cd-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="a49cd-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="a49cd-129">正しくない</span><span class="sxs-lookup"><span data-stu-id="a49cd-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a49cd-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="a49cd-130">See also</span></span>

- [<span data-ttu-id="a49cd-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="a49cd-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

