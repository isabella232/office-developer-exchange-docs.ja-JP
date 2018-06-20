---
title: 連絡先 (ContactType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7f7119b7-f5b4-484d-a7de-fa74836d9aee
description: 連絡先の要素は、統合連絡先ストアに取引先担当者を指定します。
ms.openlocfilehash: f1593da78a46851c7db43abc567eb66c0c74e0f2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759668"
---
# <a name="contact-contacttype"></a><span data-ttu-id="50821-103">連絡先 (ContactType)</span><span class="sxs-lookup"><span data-stu-id="50821-103">Contact (ContactType)</span></span>

<span data-ttu-id="50821-104">**連絡**の要素は、統合連絡先ストアに取引先担当者を指定します。</span><span class="sxs-lookup"><span data-stu-id="50821-104">The **Contact** element specifies a contact in the Unified Contact Store.</span></span> 
  
```XML
<Contact>
    <PersonName></PersonName>
    <BusinessName></BusinessName>
    <PhoneNumbers></PhoneNumbers>
    <Urls></Urls>
    <EmailAddresses></EmailAddresses>
    <Addresses></Addesses>    <ContactString></ContactString
</Contact>
```

 <span data-ttu-id="50821-105">**ContactType**</span><span class="sxs-lookup"><span data-stu-id="50821-105">**ContactType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="50821-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="50821-106">Attributes and elements</span></span>

<span data-ttu-id="50821-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="50821-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="50821-108">属性</span><span class="sxs-lookup"><span data-stu-id="50821-108">Attributes</span></span>

<span data-ttu-id="50821-109">なし。</span><span class="sxs-lookup"><span data-stu-id="50821-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="50821-110">子要素</span><span class="sxs-lookup"><span data-stu-id="50821-110">Child elements</span></span>

|<span data-ttu-id="50821-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="50821-111">**Element**</span></span>|<span data-ttu-id="50821-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="50821-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="50821-113">PersonName</span><span class="sxs-lookup"><span data-stu-id="50821-113">PersonName</span></span>](personname.md) <br/> |<span data-ttu-id="50821-114">個人の名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="50821-114">Specifies the name of an individual.</span></span>  <br/> |
|[<span data-ttu-id="50821-115">BusinessName</span><span class="sxs-lookup"><span data-stu-id="50821-115">BusinessName</span></span>](businessname.md) <br/> |<span data-ttu-id="50821-116">ビジネスの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="50821-116">Specifies the name of a business.</span></span>  <br/> |
|[<span data-ttu-id="50821-117">PhoneNumbers</span><span class="sxs-lookup"><span data-stu-id="50821-117">PhoneNumbers</span></span>](phonenumbers.md) <br/> |<span data-ttu-id="50821-118">連絡先の電話番号のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="50821-118">Represents a collection of telephone numbers for a contact.</span></span>  <br/> |
|[<span data-ttu-id="50821-119">Url</span><span class="sxs-lookup"><span data-stu-id="50821-119">Urls</span></span>](urls.md) <br/> |<span data-ttu-id="50821-120">ペルソナの Url の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="50821-120">Specifies an array of URLs for a persona.</span></span>  <br/> |
|[<span data-ttu-id="50821-121">EmailAddresses (ArrayOfExtractedEmailAddresses)</span><span class="sxs-lookup"><span data-stu-id="50821-121">EmailAddresses (ArrayOfExtractedEmailAddresses)</span></span>](emailaddresses-arrayofextractedemailaddresses.md) <br/> |<span data-ttu-id="50821-122">抽出された電子メール アドレスの配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="50821-122">Specifies an array of extracted email addresses.</span></span>  <br/> |
|[<span data-ttu-id="50821-123">アドレス (ArrayOfAddressesType)</span><span class="sxs-lookup"><span data-stu-id="50821-123">Addresses (ArrayOfAddressesType)</span></span>](addresses-arrayofaddressestype.md) <br/> |<span data-ttu-id="50821-124">**アドレス**要素の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="50821-124">Specifies an array of **Address** elements.</span></span>  <br/> |
|[<span data-ttu-id="50821-125">ContactString</span><span class="sxs-lookup"><span data-stu-id="50821-125">ContactString</span></span>](contactstring.md) <br/> |<span data-ttu-id="50821-126">連絡先の表示名を指定します。</span><span class="sxs-lookup"><span data-stu-id="50821-126">Specifies the display name of a contact.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="50821-127">親要素</span><span class="sxs-lookup"><span data-stu-id="50821-127">Parent elements</span></span>

|<span data-ttu-id="50821-128">**要素**</span><span class="sxs-lookup"><span data-stu-id="50821-128">**Element**</span></span>|<span data-ttu-id="50821-129">**説明**</span><span class="sxs-lookup"><span data-stu-id="50821-129">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="50821-130">連絡先 (ArrayOfContactsType)</span><span class="sxs-lookup"><span data-stu-id="50821-130">Contacts (ArrayOfContactsType)</span></span>](contacts-arrayofcontactstype.md) <br/> |<span data-ttu-id="50821-131">メンバーの配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="50821-131">Specifies an array of contacts.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="50821-132">備考</span><span class="sxs-lookup"><span data-stu-id="50821-132">Remarks</span></span>

<span data-ttu-id="50821-133">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="50821-133">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="50821-134">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="50821-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="50821-135">要素情報</span><span class="sxs-lookup"><span data-stu-id="50821-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="50821-136">名前空間</span><span class="sxs-lookup"><span data-stu-id="50821-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="50821-137">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="50821-137">Schema Name</span></span>  <br/> |<span data-ttu-id="50821-138">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="50821-138">Type schema</span></span>  <br/> |
|<span data-ttu-id="50821-139">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="50821-139">Validation File</span></span>  <br/> |<span data-ttu-id="50821-140">types.xsd</span><span class="sxs-lookup"><span data-stu-id="50821-140">types.xsd</span></span>  <br/> |
|<span data-ttu-id="50821-141">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="50821-141">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="50821-142">関連項目</span><span class="sxs-lookup"><span data-stu-id="50821-142">See also</span></span>



- [<span data-ttu-id="50821-143">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="50821-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

