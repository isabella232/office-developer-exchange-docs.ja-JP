---
title: EmailAddresses (ArrayOfEmailAddressesType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 95084659-aa5a-4bac-8977-00db3b87883e
description: EmailAddresses 要素は、関連付けられているペルソナのすべての電子メール アドレスの配列を指定します。
ms.openlocfilehash: 292d4c3f12b01f25fd094b2ab6d9c2d484d37694
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760234"
---
# <a name="emailaddresses-arrayofemailaddressestype"></a><span data-ttu-id="18e98-103">EmailAddresses (ArrayOfEmailAddressesType)</span><span class="sxs-lookup"><span data-stu-id="18e98-103">EmailAddresses (ArrayOfEmailAddressesType)</span></span>

<span data-ttu-id="18e98-104">**EmailAddresses**要素は、関連付けられているペルソナのすべての電子メール アドレスの配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="18e98-104">The **EmailAddresses** element specifies an array of all email addresses of the associated persona.</span></span> 
  
```XML
<EmailAddresses>
    <Address></Address>
</EmailAddresses>
```

 <span data-ttu-id="18e98-105">**ArrayOfEmailAddressesType**</span><span class="sxs-lookup"><span data-stu-id="18e98-105">**ArrayOfEmailAddressesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="18e98-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="18e98-106">Attributes and elements</span></span>

<span data-ttu-id="18e98-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="18e98-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="18e98-108">属性</span><span class="sxs-lookup"><span data-stu-id="18e98-108">Attributes</span></span>

<span data-ttu-id="18e98-109">なし。</span><span class="sxs-lookup"><span data-stu-id="18e98-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="18e98-110">子要素</span><span class="sxs-lookup"><span data-stu-id="18e98-110">Child elements</span></span>

|<span data-ttu-id="18e98-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="18e98-111">**Element**</span></span>|<span data-ttu-id="18e98-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="18e98-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="18e98-113">アドレス (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="18e98-113">Address (EmailAddressType)</span></span>](address-emailaddresstype.md) <br/> |<span data-ttu-id="18e98-114">完全に解決された電子メール アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="18e98-114">Represents a fully resolved e-mail address.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="18e98-115">親要素</span><span class="sxs-lookup"><span data-stu-id="18e98-115">Parent elements</span></span>

|<span data-ttu-id="18e98-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="18e98-116">**Element**</span></span>|<span data-ttu-id="18e98-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="18e98-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="18e98-118">ペルソナ</span><span class="sxs-lookup"><span data-stu-id="18e98-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="18e98-119">**GetPersona**の要求によって返されるペルソナ データのセットを指定します。</span><span class="sxs-lookup"><span data-stu-id="18e98-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="18e98-120">備考</span><span class="sxs-lookup"><span data-stu-id="18e98-120">Remarks</span></span>

<span data-ttu-id="18e98-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="18e98-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="18e98-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="18e98-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="18e98-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="18e98-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="18e98-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="18e98-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="18e98-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="18e98-125">Schema Name</span></span>  <br/> |<span data-ttu-id="18e98-126">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="18e98-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="18e98-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="18e98-127">Validation File</span></span>  <br/> |<span data-ttu-id="18e98-128">types.xsd</span><span class="sxs-lookup"><span data-stu-id="18e98-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="18e98-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="18e98-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="18e98-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="18e98-130">See also</span></span>



- [<span data-ttu-id="18e98-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="18e98-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

