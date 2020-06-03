---
title: Emails3
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4f4dc589-4530-4a35-b2a6-0c83cac23637
description: Emails3 要素は、EmailAddressAttributedValue 値の配列と、関連付けられているペルソナのソース attributions の識別子を指定します。
ms.openlocfilehash: 0505b0ea248a3ab2de7ec18a344fa57651f84cca
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460723"
---
# <a name="emails3"></a><span data-ttu-id="1d03a-103">Emails3</span><span class="sxs-lookup"><span data-stu-id="1d03a-103">Emails3</span></span>

<span data-ttu-id="1d03a-104">**Emails3**要素は、 **EmailAddressAttributedValue**値の配列と、関連付けられているペルソナのソース attributions の識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="1d03a-104">The **Emails3** element specifies an array of **EmailAddressAttributedValue** values and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<Emails3>
    <EmailAddressAttributedValue></EmailAddressAttributedValue>
</Emails3>
```

 <span data-ttu-id="1d03a-105">**ArrayOfEmailAddressAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="1d03a-105">**ArrayOfEmailAddressAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1d03a-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="1d03a-106">Attributes and elements</span></span>

<span data-ttu-id="1d03a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1d03a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1d03a-108">属性</span><span class="sxs-lookup"><span data-stu-id="1d03a-108">Attributes</span></span>

<span data-ttu-id="1d03a-109">なし。</span><span class="sxs-lookup"><span data-stu-id="1d03a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1d03a-110">子要素</span><span class="sxs-lookup"><span data-stu-id="1d03a-110">Child elements</span></span>

|<span data-ttu-id="1d03a-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="1d03a-111">**Element**</span></span>|<span data-ttu-id="1d03a-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="1d03a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1d03a-113">EmailAddressAttributedValue</span><span class="sxs-lookup"><span data-stu-id="1d03a-113">EmailAddressAttributedValue</span></span>](emailaddressattributedvalue.md) <br/> |<span data-ttu-id="1d03a-114">電子メールアドレスの配列のインスタンスと、それに関連付けられている attributions を指定します。</span><span class="sxs-lookup"><span data-stu-id="1d03a-114">Specifies an instance of an array of email addresses and their associated attributions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1d03a-115">親要素</span><span class="sxs-lookup"><span data-stu-id="1d03a-115">Parent elements</span></span>

|<span data-ttu-id="1d03a-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="1d03a-116">**Element**</span></span>|<span data-ttu-id="1d03a-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="1d03a-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1d03a-118">ユーザー</span><span class="sxs-lookup"><span data-stu-id="1d03a-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="1d03a-119">**Getpersona**要求によって返される一連のペルソナデータを指定します。</span><span class="sxs-lookup"><span data-stu-id="1d03a-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1d03a-120">注釈</span><span class="sxs-lookup"><span data-stu-id="1d03a-120">Remarks</span></span>

<span data-ttu-id="1d03a-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="1d03a-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="1d03a-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="1d03a-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1d03a-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="1d03a-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1d03a-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="1d03a-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1d03a-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1d03a-125">Schema Name</span></span>  <br/> |<span data-ttu-id="1d03a-126">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="1d03a-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="1d03a-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1d03a-127">Validation File</span></span>  <br/> |<span data-ttu-id="1d03a-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="1d03a-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="1d03a-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="1d03a-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="1d03a-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="1d03a-130">See also</span></span>



- [<span data-ttu-id="1d03a-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="1d03a-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

