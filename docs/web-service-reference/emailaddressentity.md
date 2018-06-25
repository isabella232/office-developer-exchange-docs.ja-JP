---
title: EmailAddressEntity
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 20049467-c01a-4c7d-8ada-ca1801cc95ed
description: EmailAddressEntity 要素は、単一の電子メール アドレスのエンティティを指定します。
ms.openlocfilehash: c149ee69c1ed08c33d0341c8dfdac3bcda040afb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760232"
---
# <a name="emailaddressentity"></a><span data-ttu-id="6b469-103">EmailAddressEntity</span><span class="sxs-lookup"><span data-stu-id="6b469-103">EmailAddressEntity</span></span>

<span data-ttu-id="6b469-104">**EmailAddressEntity**要素は、単一の電子メール アドレスのエンティティを指定します。</span><span class="sxs-lookup"><span data-stu-id="6b469-104">The **EmailAddressEntity** element specifies a single email address entity.</span></span> 
  
```XML
<EmailAddressEntity>
    <EmailAddress></EmailAddress>
</EmailAddressEntity>
```

 <span data-ttu-id="6b469-105">**EmailAddressEntityType**</span><span class="sxs-lookup"><span data-stu-id="6b469-105">**EmailAddressEntityType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6b469-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="6b469-106">Attributes and elements</span></span>

<span data-ttu-id="6b469-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6b469-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6b469-108">属性</span><span class="sxs-lookup"><span data-stu-id="6b469-108">Attributes</span></span>

<span data-ttu-id="6b469-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6b469-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6b469-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6b469-110">Child elements</span></span>

|<span data-ttu-id="6b469-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="6b469-111">**Element**</span></span>|<span data-ttu-id="6b469-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="6b469-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6b469-113">EmailAddress (文字列)</span><span class="sxs-lookup"><span data-stu-id="6b469-113">EmailAddress (string)</span></span>](emailaddress-string.md) <br/> |<span data-ttu-id="6b469-114">1 つの電子メール アドレスを指定します。</span><span class="sxs-lookup"><span data-stu-id="6b469-114">Specifies a single email address.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6b469-115">親要素</span><span class="sxs-lookup"><span data-stu-id="6b469-115">Parent elements</span></span>

|<span data-ttu-id="6b469-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="6b469-116">**Element**</span></span>|<span data-ttu-id="6b469-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="6b469-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6b469-118">EmailAddresses (ArrayOfEmailAddressEntitiesType)</span><span class="sxs-lookup"><span data-stu-id="6b469-118">EmailAddresses (ArrayOfEmailAddressEntitiesType)</span></span>](emailaddresses-arrayofemailaddressentitiestype.md) <br/> |<span data-ttu-id="6b469-119">E メール アドレスのエンティティの配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="6b469-119">Specifies an array of email address entities.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6b469-120">備考</span><span class="sxs-lookup"><span data-stu-id="6b469-120">Remarks</span></span>

<span data-ttu-id="6b469-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="6b469-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="6b469-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="6b469-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6b469-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="6b469-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6b469-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="6b469-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6b469-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6b469-125">Schema Name</span></span>  <br/> |<span data-ttu-id="6b469-126">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="6b469-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="6b469-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6b469-127">Validation File</span></span>  <br/> |<span data-ttu-id="6b469-128">types.xsd</span><span class="sxs-lookup"><span data-stu-id="6b469-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="6b469-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="6b469-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="6b469-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="6b469-130">See also</span></span>



- [<span data-ttu-id="6b469-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="6b469-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

