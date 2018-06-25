---
title: OriginalRecipients
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OriginalRecipients
api_type:
- schema
ms.assetid: e4af86a5-85af-4239-8055-e29f0acf77c1
description: OriginalRecipients 要素は、最初のメッセージの受信者の電子メール アドレスのリストを表します。
ms.openlocfilehash: 8f99368409dbfb5ac798b691be65c7fd64f32660
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832665"
---
# <a name="originalrecipients"></a><span data-ttu-id="78986-103">OriginalRecipients</span><span class="sxs-lookup"><span data-stu-id="78986-103">OriginalRecipients</span></span>

<span data-ttu-id="78986-104">**OriginalRecipients**要素は、最初のメッセージの受信者の電子メール アドレスのリストを表します。</span><span class="sxs-lookup"><span data-stu-id="78986-104">The **OriginalRecipients** element represents a list of e-mail addresses of the first message recipients.</span></span> 
  
```XML
<OriginalRecipients>
   <Address/>
</OriginalRecipients>
```

 <span data-ttu-id="78986-105">**ArrayOfEmailAddressesType**</span><span class="sxs-lookup"><span data-stu-id="78986-105">**ArrayOfEmailAddressesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="78986-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="78986-106">Attributes and elements</span></span>

<span data-ttu-id="78986-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="78986-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="78986-108">属性</span><span class="sxs-lookup"><span data-stu-id="78986-108">Attributes</span></span>

<span data-ttu-id="78986-109">なし。</span><span class="sxs-lookup"><span data-stu-id="78986-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="78986-110">子要素</span><span class="sxs-lookup"><span data-stu-id="78986-110">Child elements</span></span>

|<span data-ttu-id="78986-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="78986-111">**Element**</span></span>|<span data-ttu-id="78986-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="78986-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="78986-113">アドレス (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="78986-113">Address (EmailAddressType)</span></span>](address-emailaddresstype.md) <br/> |<span data-ttu-id="78986-114">完全に解決された電子メール アドレスが含まれています。</span><span class="sxs-lookup"><span data-stu-id="78986-114">Contains a fully resolved e-mail address.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="78986-115">親要素</span><span class="sxs-lookup"><span data-stu-id="78986-115">Parent elements</span></span>

|<span data-ttu-id="78986-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="78986-116">**Element**</span></span>|<span data-ttu-id="78986-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="78986-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="78986-118">MessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="78986-118">MessageTrackingReport</span></span>](messagetrackingreport.md) <br/> |<span data-ttu-id="78986-119">[GetMessageTrackingReport 操作](getmessagetrackingreport-operation.md)で返される 1 つのメッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="78986-119">Contains a single message that is returned in a [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="78986-120">備考</span><span class="sxs-lookup"><span data-stu-id="78986-120">Remarks</span></span>

<span data-ttu-id="78986-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="78986-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="78986-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="78986-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="78986-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="78986-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="78986-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="78986-124">Schema Name</span></span>  <br/> |<span data-ttu-id="78986-125">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="78986-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="78986-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="78986-126">Validation File</span></span>  <br/> |<span data-ttu-id="78986-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="78986-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="78986-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="78986-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="78986-129">False</span><span class="sxs-lookup"><span data-stu-id="78986-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="78986-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="78986-130">See also</span></span>



[<span data-ttu-id="78986-131">GetMessageTrackingReport 操作</span><span class="sxs-lookup"><span data-stu-id="78986-131">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="78986-132">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="78986-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

