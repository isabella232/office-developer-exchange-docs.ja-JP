---
title: AssistantPhoneNumbers
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f9bd9ac1-7db3-44ea-9117-18488dddde15
description: AssistantPhoneNumbers 要素は、補佐電話番号の配列と、関連付けられているペルソナのソース attributions の識別子を指定します。
ms.openlocfilehash: a72c8d646750b5d7cf9ebca13a51f4df84bf7bdb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464484"
---
# <a name="assistantphonenumbers"></a><span data-ttu-id="c2c81-103">AssistantPhoneNumbers</span><span class="sxs-lookup"><span data-stu-id="c2c81-103">AssistantPhoneNumbers</span></span>

<span data-ttu-id="c2c81-104">**AssistantPhoneNumbers**要素は、補佐電話番号の配列と、関連付けられているペルソナのソース attributions の識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="c2c81-104">The **AssistantPhoneNumbers** element specifies an array of assistant phone numbers and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<AssistantPhoneNumbers>
    <PhoneNumberAttributedValue></PhoneNumberAttributedValue>
</AssistantPhoneNumbers>
```

 <span data-ttu-id="c2c81-105">**ArrayOfPhoneNumberAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="c2c81-105">**ArrayOfPhoneNumberAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c2c81-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="c2c81-106">Attributes and elements</span></span>

<span data-ttu-id="c2c81-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c2c81-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c2c81-108">属性</span><span class="sxs-lookup"><span data-stu-id="c2c81-108">Attributes</span></span>

<span data-ttu-id="c2c81-109">なし。</span><span class="sxs-lookup"><span data-stu-id="c2c81-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c2c81-110">子要素</span><span class="sxs-lookup"><span data-stu-id="c2c81-110">Child elements</span></span>

|<span data-ttu-id="c2c81-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="c2c81-111">**Element**</span></span>|<span data-ttu-id="c2c81-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="c2c81-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c2c81-113">PhoneNumberAttributedValue</span><span class="sxs-lookup"><span data-stu-id="c2c81-113">PhoneNumberAttributedValue</span></span>](phonenumberattributedvalue.md) <br/> |<span data-ttu-id="c2c81-114">電話番号の配列のインスタンスと、それに関連付けられている attributions を指定します。</span><span class="sxs-lookup"><span data-stu-id="c2c81-114">Specifies an instance of an array of phone numbers and their associated attributions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c2c81-115">親要素</span><span class="sxs-lookup"><span data-stu-id="c2c81-115">Parent elements</span></span>

|<span data-ttu-id="c2c81-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="c2c81-116">**Element**</span></span>|<span data-ttu-id="c2c81-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="c2c81-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c2c81-118">ユーザー</span><span class="sxs-lookup"><span data-stu-id="c2c81-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="c2c81-119">**Getpersona**要求によって返される一連のペルソナデータを指定します。</span><span class="sxs-lookup"><span data-stu-id="c2c81-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c2c81-120">注釈</span><span class="sxs-lookup"><span data-stu-id="c2c81-120">Remarks</span></span>

<span data-ttu-id="c2c81-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="c2c81-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="c2c81-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="c2c81-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c2c81-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="c2c81-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c2c81-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="c2c81-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c2c81-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c2c81-125">Schema Name</span></span>  <br/> |<span data-ttu-id="c2c81-126">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="c2c81-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="c2c81-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c2c81-127">Validation File</span></span>  <br/> |<span data-ttu-id="c2c81-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="c2c81-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="c2c81-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="c2c81-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="c2c81-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="c2c81-130">See also</span></span>

- [<span data-ttu-id="c2c81-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="c2c81-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

