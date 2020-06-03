---
title: Emails2
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 6ad95936-f61b-431a-9d86-df160b5d4b2d
description: Emails2 要素には、EmailAddressAttributedValue 値の配列と、関連付けられているペルソナのソース attributions の識別子が含まれます。
ms.openlocfilehash: b9445dfdc556ade1ad96d6e56c35ec1e56627e8c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463413"
---
# <a name="emails2"></a><span data-ttu-id="aff77-103">Emails2</span><span class="sxs-lookup"><span data-stu-id="aff77-103">Emails2</span></span>

<span data-ttu-id="aff77-104">**Emails2**要素には、 **EmailAddressAttributedValue**値の配列と、関連付けられているペルソナのソース attributions の識別子が含まれます。</span><span class="sxs-lookup"><span data-stu-id="aff77-104">The **Emails2** element contains an array of **EmailAddressAttributedValue** values and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<Emails2>
    <EmailAddressAttributedValue></EmailAddressAttributedValue>
</Emails2>
```

 <span data-ttu-id="aff77-105">**ArrayOfEmailAddressAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="aff77-105">**ArrayOfEmailAddressAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="aff77-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="aff77-106">Attributes and elements</span></span>

<span data-ttu-id="aff77-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="aff77-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="aff77-108">属性</span><span class="sxs-lookup"><span data-stu-id="aff77-108">Attributes</span></span>

<span data-ttu-id="aff77-109">なし。</span><span class="sxs-lookup"><span data-stu-id="aff77-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="aff77-110">子要素</span><span class="sxs-lookup"><span data-stu-id="aff77-110">Child elements</span></span>

|<span data-ttu-id="aff77-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="aff77-111">**Element**</span></span>|<span data-ttu-id="aff77-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="aff77-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aff77-113">EmailAddressAttributedValue</span><span class="sxs-lookup"><span data-stu-id="aff77-113">EmailAddressAttributedValue</span></span>](emailaddressattributedvalue.md) <br/> |<span data-ttu-id="aff77-114">電子メールアドレスの配列のインスタンスと、それに関連付けられている attributions を指定します。</span><span class="sxs-lookup"><span data-stu-id="aff77-114">Specifies an instance of an array of email addresses and their associated attributions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="aff77-115">親要素</span><span class="sxs-lookup"><span data-stu-id="aff77-115">Parent elements</span></span>

|<span data-ttu-id="aff77-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="aff77-116">**Element**</span></span>|<span data-ttu-id="aff77-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="aff77-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aff77-118">ユーザー</span><span class="sxs-lookup"><span data-stu-id="aff77-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="aff77-119">**Getpersona**要求によって返される一連のペルソナデータを指定します。</span><span class="sxs-lookup"><span data-stu-id="aff77-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="aff77-120">注釈</span><span class="sxs-lookup"><span data-stu-id="aff77-120">Remarks</span></span>

<span data-ttu-id="aff77-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="aff77-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="aff77-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="aff77-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="aff77-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="aff77-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="aff77-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="aff77-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="aff77-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="aff77-125">Schema Name</span></span>  <br/> |<span data-ttu-id="aff77-126">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="aff77-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="aff77-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="aff77-127">Validation File</span></span>  <br/> |<span data-ttu-id="aff77-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="aff77-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="aff77-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="aff77-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="aff77-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="aff77-130">See also</span></span>



- [<span data-ttu-id="aff77-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="aff77-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

