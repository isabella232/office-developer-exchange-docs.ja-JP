---
title: Contact (ContactType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7f7119b7-f5b4-484d-a7de-fa74836d9aee
description: 連絡先要素は、統合連絡先ストアの連絡先を指定します。
ms.openlocfilehash: e8ebc28456f8bfc26f5d790ac9ff278930041ea0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461521"
---
# <a name="contact-contacttype"></a><span data-ttu-id="26f8a-103">Contact (ContactType)</span><span class="sxs-lookup"><span data-stu-id="26f8a-103">Contact (ContactType)</span></span>

<span data-ttu-id="26f8a-104">**連絡先**要素は、統合連絡先ストアの連絡先を指定します。</span><span class="sxs-lookup"><span data-stu-id="26f8a-104">The **Contact** element specifies a contact in the Unified Contact Store.</span></span> 
  
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

 <span data-ttu-id="26f8a-105">**ContactType**</span><span class="sxs-lookup"><span data-stu-id="26f8a-105">**ContactType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="26f8a-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="26f8a-106">Attributes and elements</span></span>

<span data-ttu-id="26f8a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="26f8a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="26f8a-108">属性</span><span class="sxs-lookup"><span data-stu-id="26f8a-108">Attributes</span></span>

<span data-ttu-id="26f8a-109">なし。</span><span class="sxs-lookup"><span data-stu-id="26f8a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="26f8a-110">子要素</span><span class="sxs-lookup"><span data-stu-id="26f8a-110">Child elements</span></span>

|<span data-ttu-id="26f8a-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="26f8a-111">**Element**</span></span>|<span data-ttu-id="26f8a-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="26f8a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="26f8a-113">Contact.personname</span><span class="sxs-lookup"><span data-stu-id="26f8a-113">PersonName</span></span>](personname.md) <br/> |<span data-ttu-id="26f8a-114">個人の名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="26f8a-114">Specifies the name of an individual.</span></span>  <br/> |
|[<span data-ttu-id="26f8a-115">Contact.businessname</span><span class="sxs-lookup"><span data-stu-id="26f8a-115">BusinessName</span></span>](businessname.md) <br/> |<span data-ttu-id="26f8a-116">会社の名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="26f8a-116">Specifies the name of a business.</span></span>  <br/> |
|[<span data-ttu-id="26f8a-117">PhoneNumbers</span><span class="sxs-lookup"><span data-stu-id="26f8a-117">PhoneNumbers</span></span>](phonenumbers.md) <br/> |<span data-ttu-id="26f8a-118">連絡先の電話番号のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="26f8a-118">Represents a collection of telephone numbers for a contact.</span></span>  <br/> |
|[<span data-ttu-id="26f8a-119">Urls</span><span class="sxs-lookup"><span data-stu-id="26f8a-119">Urls</span></span>](urls.md) <br/> |<span data-ttu-id="26f8a-120">ペルソナの Url の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="26f8a-120">Specifies an array of URLs for a persona.</span></span>  <br/> |
|[<span data-ttu-id="26f8a-121">EmailAddresses (ArrayOfExtractedEmailAddresses)</span><span class="sxs-lookup"><span data-stu-id="26f8a-121">EmailAddresses (ArrayOfExtractedEmailAddresses)</span></span>](emailaddresses-arrayofextractedemailaddresses.md) <br/> |<span data-ttu-id="26f8a-122">抽出された電子メールアドレスの配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="26f8a-122">Specifies an array of extracted email addresses.</span></span>  <br/> |
|[<span data-ttu-id="26f8a-123">アドレス (ArrayOfAddressesType)</span><span class="sxs-lookup"><span data-stu-id="26f8a-123">Addresses (ArrayOfAddressesType)</span></span>](addresses-arrayofaddressestype.md) <br/> |<span data-ttu-id="26f8a-124">**Address**要素の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="26f8a-124">Specifies an array of **Address** elements.</span></span>  <br/> |
|[<span data-ttu-id="26f8a-125">ContactString</span><span class="sxs-lookup"><span data-stu-id="26f8a-125">ContactString</span></span>](contactstring.md) <br/> |<span data-ttu-id="26f8a-126">連絡先の表示名を指定します。</span><span class="sxs-lookup"><span data-stu-id="26f8a-126">Specifies the display name of a contact.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="26f8a-127">親要素</span><span class="sxs-lookup"><span data-stu-id="26f8a-127">Parent elements</span></span>

|<span data-ttu-id="26f8a-128">**要素**</span><span class="sxs-lookup"><span data-stu-id="26f8a-128">**Element**</span></span>|<span data-ttu-id="26f8a-129">**説明**</span><span class="sxs-lookup"><span data-stu-id="26f8a-129">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="26f8a-130">連絡先 (ArrayOfContactsType)</span><span class="sxs-lookup"><span data-stu-id="26f8a-130">Contacts (ArrayOfContactsType)</span></span>](contacts-arrayofcontactstype.md) <br/> |<span data-ttu-id="26f8a-131">連絡先の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="26f8a-131">Specifies an array of contacts.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="26f8a-132">注釈</span><span class="sxs-lookup"><span data-stu-id="26f8a-132">Remarks</span></span>

<span data-ttu-id="26f8a-133">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="26f8a-133">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="26f8a-134">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="26f8a-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="26f8a-135">要素の情報</span><span class="sxs-lookup"><span data-stu-id="26f8a-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="26f8a-136">Namespace</span><span class="sxs-lookup"><span data-stu-id="26f8a-136">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="26f8a-137">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="26f8a-137">Schema Name</span></span>  <br/> |<span data-ttu-id="26f8a-138">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="26f8a-138">Type schema</span></span>  <br/> |
|<span data-ttu-id="26f8a-139">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="26f8a-139">Validation File</span></span>  <br/> |<span data-ttu-id="26f8a-140">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="26f8a-140">types.xsd</span></span>  <br/> |
|<span data-ttu-id="26f8a-141">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="26f8a-141">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="26f8a-142">関連項目</span><span class="sxs-lookup"><span data-stu-id="26f8a-142">See also</span></span>



- [<span data-ttu-id="26f8a-143">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="26f8a-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

