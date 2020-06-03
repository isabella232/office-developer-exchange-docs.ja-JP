---
title: EmailAddressEntity
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 20049467-c01a-4c7d-8ada-ca1801cc95ed
description: EmailAddressEntity 要素は、1つの電子メールアドレスエンティティを指定します。
ms.openlocfilehash: b76b08f93e60c8492906f3cc94e60f5725c8a9dc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526222"
---
# <a name="emailaddressentity"></a><span data-ttu-id="91cad-103">EmailAddressEntity</span><span class="sxs-lookup"><span data-stu-id="91cad-103">EmailAddressEntity</span></span>

<span data-ttu-id="91cad-104">**Emailaddressentity**要素は、1つの電子メールアドレスエンティティを指定します。</span><span class="sxs-lookup"><span data-stu-id="91cad-104">The **EmailAddressEntity** element specifies a single email address entity.</span></span> 
  
```XML
<EmailAddressEntity>
    <EmailAddress></EmailAddress>
</EmailAddressEntity>
```

 <span data-ttu-id="91cad-105">**EmailAddressEntityType**</span><span class="sxs-lookup"><span data-stu-id="91cad-105">**EmailAddressEntityType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="91cad-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="91cad-106">Attributes and elements</span></span>

<span data-ttu-id="91cad-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="91cad-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="91cad-108">属性</span><span class="sxs-lookup"><span data-stu-id="91cad-108">Attributes</span></span>

<span data-ttu-id="91cad-109">なし。</span><span class="sxs-lookup"><span data-stu-id="91cad-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="91cad-110">子要素</span><span class="sxs-lookup"><span data-stu-id="91cad-110">Child elements</span></span>

|<span data-ttu-id="91cad-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="91cad-111">**Element**</span></span>|<span data-ttu-id="91cad-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="91cad-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="91cad-113">EmailAddress (文字列)</span><span class="sxs-lookup"><span data-stu-id="91cad-113">EmailAddress (string)</span></span>](emailaddress-string.md) <br/> |<span data-ttu-id="91cad-114">1つの電子メールアドレスを指定します。</span><span class="sxs-lookup"><span data-stu-id="91cad-114">Specifies a single email address.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="91cad-115">親要素</span><span class="sxs-lookup"><span data-stu-id="91cad-115">Parent elements</span></span>

|<span data-ttu-id="91cad-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="91cad-116">**Element**</span></span>|<span data-ttu-id="91cad-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="91cad-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="91cad-118">EmailAddresses (ArrayOfEmailAddressEntitiesType)</span><span class="sxs-lookup"><span data-stu-id="91cad-118">EmailAddresses (ArrayOfEmailAddressEntitiesType)</span></span>](emailaddresses-arrayofemailaddressentitiestype.md) <br/> |<span data-ttu-id="91cad-119">電子メールアドレスエンティティの配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="91cad-119">Specifies an array of email address entities.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="91cad-120">注釈</span><span class="sxs-lookup"><span data-stu-id="91cad-120">Remarks</span></span>

<span data-ttu-id="91cad-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="91cad-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="91cad-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="91cad-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="91cad-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="91cad-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="91cad-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="91cad-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="91cad-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="91cad-125">Schema Name</span></span>  <br/> |<span data-ttu-id="91cad-126">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="91cad-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="91cad-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="91cad-127">Validation File</span></span>  <br/> |<span data-ttu-id="91cad-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="91cad-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="91cad-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="91cad-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="91cad-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="91cad-130">See also</span></span>



- [<span data-ttu-id="91cad-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="91cad-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

