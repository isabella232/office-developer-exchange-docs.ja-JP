---
title: Emails3
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4f4dc589-4530-4a35-b2a6-0c83cac23637
description: Emails3 要素は、EmailAddressAttributedValue の値の配列と関連付けられているペルソナにそのソースの帰属の識別子を指定します。
ms.openlocfilehash: 1d174000d59883446bb7f61af90278d197ef5ed9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760242"
---
# <a name="emails3"></a><span data-ttu-id="27283-103">Emails3</span><span class="sxs-lookup"><span data-stu-id="27283-103">Emails3</span></span>

<span data-ttu-id="27283-104">**Emails3**要素は、 **EmailAddressAttributedValue**の値の配列と関連付けられているペルソナにそのソースの帰属の識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="27283-104">The **Emails3** element specifies an array of **EmailAddressAttributedValue** values and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<Emails3>
    <EmailAddressAttributedValue></EmailAddressAttributedValue>
</Emails3>
```

 <span data-ttu-id="27283-105">**ArrayOfEmailAddressAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="27283-105">**ArrayOfEmailAddressAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="27283-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="27283-106">Attributes and elements</span></span>

<span data-ttu-id="27283-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="27283-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="27283-108">属性</span><span class="sxs-lookup"><span data-stu-id="27283-108">Attributes</span></span>

<span data-ttu-id="27283-109">なし。</span><span class="sxs-lookup"><span data-stu-id="27283-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="27283-110">子要素</span><span class="sxs-lookup"><span data-stu-id="27283-110">Child elements</span></span>

|<span data-ttu-id="27283-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="27283-111">**Element**</span></span>|<span data-ttu-id="27283-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="27283-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="27283-113">EmailAddressAttributedValue</span><span class="sxs-lookup"><span data-stu-id="27283-113">EmailAddressAttributedValue</span></span>](emailaddressattributedvalue.md) <br/> |<span data-ttu-id="27283-114">電子メール アドレスと関連付けられている、帰属の配列のインスタンスを指定します。</span><span class="sxs-lookup"><span data-stu-id="27283-114">Specifies an instance of an array of email addresses and their associated attributions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="27283-115">親要素</span><span class="sxs-lookup"><span data-stu-id="27283-115">Parent elements</span></span>

|<span data-ttu-id="27283-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="27283-116">**Element**</span></span>|<span data-ttu-id="27283-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="27283-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="27283-118">ペルソナ</span><span class="sxs-lookup"><span data-stu-id="27283-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="27283-119">**GetPersona**の要求によって返されるペルソナ データのセットを指定します。</span><span class="sxs-lookup"><span data-stu-id="27283-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="27283-120">備考</span><span class="sxs-lookup"><span data-stu-id="27283-120">Remarks</span></span>

<span data-ttu-id="27283-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="27283-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="27283-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="27283-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="27283-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="27283-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="27283-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="27283-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="27283-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="27283-125">Schema Name</span></span>  <br/> |<span data-ttu-id="27283-126">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="27283-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="27283-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="27283-127">Validation File</span></span>  <br/> |<span data-ttu-id="27283-128">types.xsd</span><span class="sxs-lookup"><span data-stu-id="27283-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="27283-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="27283-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="27283-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="27283-130">See also</span></span>



- [<span data-ttu-id="27283-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="27283-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

