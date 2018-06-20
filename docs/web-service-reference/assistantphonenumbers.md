---
title: AssistantPhoneNumbers
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f9bd9ac1-7db3-44ea-9117-18488dddde15
description: AssistantPhoneNumbers 要素は、アシスタントの電話番号の配列と関連付けられているペルソナにそのソースの帰属の識別子を指定します。
ms.openlocfilehash: 747835102af28d94d60b763fdbc5b2ea0947d47e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759447"
---
# <a name="assistantphonenumbers"></a><span data-ttu-id="53184-103">AssistantPhoneNumbers</span><span class="sxs-lookup"><span data-stu-id="53184-103">AssistantPhoneNumbers</span></span>

<span data-ttu-id="53184-104">**AssistantPhoneNumbers**要素は、アシスタントの電話番号の配列と関連付けられているペルソナにそのソースの帰属の識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="53184-104">The **AssistantPhoneNumbers** element specifies an array of assistant phone numbers and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<AssistantPhoneNumbers>
    <PhoneNumberAttributedValue></PhoneNumberAttributedValue>
</AssistantPhoneNumbers>
```

 <span data-ttu-id="53184-105">**ArrayOfPhoneNumberAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="53184-105">**ArrayOfPhoneNumberAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="53184-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="53184-106">Attributes and elements</span></span>

<span data-ttu-id="53184-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="53184-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="53184-108">属性</span><span class="sxs-lookup"><span data-stu-id="53184-108">Attributes</span></span>

<span data-ttu-id="53184-109">なし。</span><span class="sxs-lookup"><span data-stu-id="53184-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="53184-110">子要素</span><span class="sxs-lookup"><span data-stu-id="53184-110">Child elements</span></span>

|<span data-ttu-id="53184-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="53184-111">**Element**</span></span>|<span data-ttu-id="53184-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="53184-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="53184-113">PhoneNumberAttributedValue</span><span class="sxs-lookup"><span data-stu-id="53184-113">PhoneNumberAttributedValue</span></span>](phonenumberattributedvalue.md) <br/> |<span data-ttu-id="53184-114">電話番号と、関連付けられている帰属の配列のインスタンスを指定します。</span><span class="sxs-lookup"><span data-stu-id="53184-114">Specifies an instance of an array of phone numbers and their associated attributions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="53184-115">親要素</span><span class="sxs-lookup"><span data-stu-id="53184-115">Parent elements</span></span>

|<span data-ttu-id="53184-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="53184-116">**Element**</span></span>|<span data-ttu-id="53184-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="53184-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="53184-118">ペルソナ</span><span class="sxs-lookup"><span data-stu-id="53184-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="53184-119">**GetPersona**の要求によって返されるペルソナ データのセットを指定します。</span><span class="sxs-lookup"><span data-stu-id="53184-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="53184-120">備考</span><span class="sxs-lookup"><span data-stu-id="53184-120">Remarks</span></span>

<span data-ttu-id="53184-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="53184-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="53184-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="53184-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="53184-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="53184-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="53184-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="53184-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="53184-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="53184-125">Schema Name</span></span>  <br/> |<span data-ttu-id="53184-126">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="53184-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="53184-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="53184-127">Validation File</span></span>  <br/> |<span data-ttu-id="53184-128">types.xsd</span><span class="sxs-lookup"><span data-stu-id="53184-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="53184-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="53184-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="53184-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="53184-130">See also</span></span>

- [<span data-ttu-id="53184-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="53184-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

