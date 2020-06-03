---
title: EmailAddresses (ArrayOfEmailAddressesType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 95084659-aa5a-4bac-8977-00db3b87883e
description: EmailAddresses 要素は、関連付けられたペルソナのすべての電子メールアドレスの配列を指定します。
ms.openlocfilehash: e6132e9ef4ed13ea2546783f65d184fafeed5530
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463420"
---
# <a name="emailaddresses-arrayofemailaddressestype"></a><span data-ttu-id="ae4bc-103">EmailAddresses (ArrayOfEmailAddressesType)</span><span class="sxs-lookup"><span data-stu-id="ae4bc-103">EmailAddresses (ArrayOfEmailAddressesType)</span></span>

<span data-ttu-id="ae4bc-104">**Emailaddresses**要素は、関連付けられたペルソナのすべての電子メールアドレスの配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="ae4bc-104">The **EmailAddresses** element specifies an array of all email addresses of the associated persona.</span></span> 
  
```XML
<EmailAddresses>
    <Address></Address>
</EmailAddresses>
```

 <span data-ttu-id="ae4bc-105">**ArrayOfEmailAddressesType**</span><span class="sxs-lookup"><span data-stu-id="ae4bc-105">**ArrayOfEmailAddressesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ae4bc-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="ae4bc-106">Attributes and elements</span></span>

<span data-ttu-id="ae4bc-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ae4bc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ae4bc-108">属性</span><span class="sxs-lookup"><span data-stu-id="ae4bc-108">Attributes</span></span>

<span data-ttu-id="ae4bc-109">なし。</span><span class="sxs-lookup"><span data-stu-id="ae4bc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ae4bc-110">子要素</span><span class="sxs-lookup"><span data-stu-id="ae4bc-110">Child elements</span></span>

|<span data-ttu-id="ae4bc-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="ae4bc-111">**Element**</span></span>|<span data-ttu-id="ae4bc-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="ae4bc-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ae4bc-113">Address (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="ae4bc-113">Address (EmailAddressType)</span></span>](address-emailaddresstype.md) <br/> |<span data-ttu-id="ae4bc-114">完全に解決された電子メールアドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="ae4bc-114">Represents a fully resolved e-mail address.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ae4bc-115">親要素</span><span class="sxs-lookup"><span data-stu-id="ae4bc-115">Parent elements</span></span>

|<span data-ttu-id="ae4bc-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="ae4bc-116">**Element**</span></span>|<span data-ttu-id="ae4bc-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="ae4bc-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ae4bc-118">ユーザー</span><span class="sxs-lookup"><span data-stu-id="ae4bc-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="ae4bc-119">**Getpersona**要求によって返される一連のペルソナデータを指定します。</span><span class="sxs-lookup"><span data-stu-id="ae4bc-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ae4bc-120">注釈</span><span class="sxs-lookup"><span data-stu-id="ae4bc-120">Remarks</span></span>

<span data-ttu-id="ae4bc-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="ae4bc-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="ae4bc-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="ae4bc-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ae4bc-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="ae4bc-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ae4bc-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="ae4bc-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ae4bc-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ae4bc-125">Schema Name</span></span>  <br/> |<span data-ttu-id="ae4bc-126">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="ae4bc-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="ae4bc-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ae4bc-127">Validation File</span></span>  <br/> |<span data-ttu-id="ae4bc-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="ae4bc-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="ae4bc-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="ae4bc-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="ae4bc-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="ae4bc-130">See also</span></span>



- [<span data-ttu-id="ae4bc-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="ae4bc-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

