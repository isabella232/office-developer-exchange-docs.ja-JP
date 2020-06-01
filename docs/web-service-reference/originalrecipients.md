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
description: OriginalRecipients 要素は、最初のメッセージ受信者の電子メールアドレスのリストを表します。
ms.openlocfilehash: 7385b1fd62313ee09c94cd04f3f669215e6cd497
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467180"
---
# <a name="originalrecipients"></a><span data-ttu-id="defb2-103">OriginalRecipients</span><span class="sxs-lookup"><span data-stu-id="defb2-103">OriginalRecipients</span></span>

<span data-ttu-id="defb2-104">**Originalrecipients**要素は、最初のメッセージ受信者の電子メールアドレスのリストを表します。</span><span class="sxs-lookup"><span data-stu-id="defb2-104">The **OriginalRecipients** element represents a list of e-mail addresses of the first message recipients.</span></span> 
  
```XML
<OriginalRecipients>
   <Address/>
</OriginalRecipients>
```

 <span data-ttu-id="defb2-105">**ArrayOfEmailAddressesType**</span><span class="sxs-lookup"><span data-stu-id="defb2-105">**ArrayOfEmailAddressesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="defb2-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="defb2-106">Attributes and elements</span></span>

<span data-ttu-id="defb2-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="defb2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="defb2-108">属性</span><span class="sxs-lookup"><span data-stu-id="defb2-108">Attributes</span></span>

<span data-ttu-id="defb2-109">なし。</span><span class="sxs-lookup"><span data-stu-id="defb2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="defb2-110">子要素</span><span class="sxs-lookup"><span data-stu-id="defb2-110">Child elements</span></span>

|<span data-ttu-id="defb2-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="defb2-111">**Element**</span></span>|<span data-ttu-id="defb2-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="defb2-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="defb2-113">Address (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="defb2-113">Address (EmailAddressType)</span></span>](address-emailaddresstype.md) <br/> |<span data-ttu-id="defb2-114">完全に解決された電子メールアドレスが含まれています。</span><span class="sxs-lookup"><span data-stu-id="defb2-114">Contains a fully resolved e-mail address.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="defb2-115">親要素</span><span class="sxs-lookup"><span data-stu-id="defb2-115">Parent elements</span></span>

|<span data-ttu-id="defb2-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="defb2-116">**Element**</span></span>|<span data-ttu-id="defb2-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="defb2-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="defb2-118">および search-messagetrackingreport</span><span class="sxs-lookup"><span data-stu-id="defb2-118">MessageTrackingReport</span></span>](messagetrackingreport.md) <br/> |<span data-ttu-id="defb2-119">[Getmessagetrackingreport 操作](getmessagetrackingreport-operation.md)で返される1つのメッセージを格納します。</span><span class="sxs-lookup"><span data-stu-id="defb2-119">Contains a single message that is returned in a [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="defb2-120">注釈</span><span class="sxs-lookup"><span data-stu-id="defb2-120">Remarks</span></span>

<span data-ttu-id="defb2-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="defb2-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="defb2-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="defb2-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="defb2-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="defb2-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="defb2-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="defb2-124">Schema Name</span></span>  <br/> |<span data-ttu-id="defb2-125">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="defb2-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="defb2-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="defb2-126">Validation File</span></span>  <br/> |<span data-ttu-id="defb2-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="defb2-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="defb2-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="defb2-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="defb2-129">正しくない</span><span class="sxs-lookup"><span data-stu-id="defb2-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="defb2-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="defb2-130">See also</span></span>



[<span data-ttu-id="defb2-131">GetMessageTrackingReport 操作</span><span class="sxs-lookup"><span data-stu-id="defb2-131">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="defb2-132">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="defb2-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

