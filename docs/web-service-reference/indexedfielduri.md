---
title: IndexedFieldURI
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IndexedFieldURI
api_type:
- schema
ms.assetid: 5c9cd0b5-7eca-480a-8730-fe98b1779afa
description: IndexedFieldURI 要素は、辞書の個々のメンバーを識別します。
ms.openlocfilehash: f794d9970590417d916925f7258b28d4f0920d0e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467019"
---
# <a name="indexedfielduri"></a><span data-ttu-id="d6200-103">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="d6200-103">IndexedFieldURI</span></span>

<span data-ttu-id="d6200-104">**IndexedFieldURI**要素は、辞書の個々のメンバーを識別します。</span><span class="sxs-lookup"><span data-stu-id="d6200-104">The **IndexedFieldURI** element identifies individual members of a dictionary.</span></span> 
  
```xml
<IndexedFieldURI FieldURI="" FieldIndex="" />
```

 <span data-ttu-id="d6200-105">**PathToIndexedFieldType**</span><span class="sxs-lookup"><span data-stu-id="d6200-105">**PathToIndexedFieldType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d6200-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d6200-106">Attributes and elements</span></span>

<span data-ttu-id="d6200-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d6200-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d6200-108">属性</span><span class="sxs-lookup"><span data-stu-id="d6200-108">Attributes</span></span>

|<span data-ttu-id="d6200-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="d6200-109">**Attribute**</span></span>|<span data-ttu-id="d6200-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="d6200-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d6200-111">**FieldURI**</span><span class="sxs-lookup"><span data-stu-id="d6200-111">**FieldURI**</span></span> <br/> |<span data-ttu-id="d6200-112">返すメンバーを含むディクショナリを識別します。</span><span class="sxs-lookup"><span data-stu-id="d6200-112">Identifies the dictionary that contains the member to return.</span></span> <span data-ttu-id="d6200-113">この属性は必須です。</span><span class="sxs-lookup"><span data-stu-id="d6200-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="d6200-114">**FieldIndex**</span><span class="sxs-lookup"><span data-stu-id="d6200-114">**FieldIndex**</span></span> <br/> |<span data-ttu-id="d6200-115">取得する辞書のメンバを識別します。</span><span class="sxs-lookup"><span data-stu-id="d6200-115">Identifies the member of the dictionary to return.</span></span> <span data-ttu-id="d6200-116">この属性は必須です。</span><span class="sxs-lookup"><span data-stu-id="d6200-116">This attribute is required.</span></span>  <br/> |
   
#### <a name="fielduri-attribute"></a><span data-ttu-id="d6200-117">FieldURI 属性</span><span class="sxs-lookup"><span data-stu-id="d6200-117">FieldURI Attribute</span></span>

|<span data-ttu-id="d6200-118">**値**</span><span class="sxs-lookup"><span data-stu-id="d6200-118">**Value**</span></span>|<span data-ttu-id="d6200-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="d6200-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d6200-120">アイテム: InternetMessageHeader</span><span class="sxs-lookup"><span data-stu-id="d6200-120">item:InternetMessageHeader</span></span>  <br/> |<span data-ttu-id="d6200-121">アイテムのメッセージヘッダーを表します。</span><span class="sxs-lookup"><span data-stu-id="d6200-121">Represents the message header of an item.</span></span>  <br/> |
|<span data-ttu-id="d6200-122">連絡先: ImAddress</span><span class="sxs-lookup"><span data-stu-id="d6200-122">contacts:ImAddress</span></span>  <br/> |<span data-ttu-id="d6200-123">連絡先のインスタントメッセージングアドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="d6200-123">Represents the instant messaging address of a contact.</span></span>  <br/> |
|<span data-ttu-id="d6200-124">連絡先: PhysicalAddress: ストリート</span><span class="sxs-lookup"><span data-stu-id="d6200-124">contacts:PhysicalAddress:Street</span></span>  <br/> |<span data-ttu-id="d6200-125">連絡先の住所を表します。</span><span class="sxs-lookup"><span data-stu-id="d6200-125">Represents the street address of a contact.</span></span>  <br/> |
|<span data-ttu-id="d6200-126">連絡先: PhysicalAddress: City</span><span class="sxs-lookup"><span data-stu-id="d6200-126">contacts:PhysicalAddress:City</span></span>  <br/> |<span data-ttu-id="d6200-127">連絡先の市町村を表します。</span><span class="sxs-lookup"><span data-stu-id="d6200-127">Represents the city of a contact.</span></span>  <br/> |
|<span data-ttu-id="d6200-128">連絡先: PhysicalAddress: State</span><span class="sxs-lookup"><span data-stu-id="d6200-128">contacts:PhysicalAddress:State</span></span>  <br/> |<span data-ttu-id="d6200-129">連絡先の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="d6200-129">Represents the state of a contact.</span></span>  <br/> |
|<span data-ttu-id="d6200-130">連絡先: PhysicalAddress: Country</span><span class="sxs-lookup"><span data-stu-id="d6200-130">contacts:PhysicalAddress:Country</span></span>  <br/> |<span data-ttu-id="d6200-131">連絡先の国/地域を表します。</span><span class="sxs-lookup"><span data-stu-id="d6200-131">Represents the country/region of a contact.</span></span>  <br/> |
|<span data-ttu-id="d6200-132">連絡先: PhysicalAddress: 郵便番号</span><span class="sxs-lookup"><span data-stu-id="d6200-132">contacts:PhysicalAddress:PostalCode</span></span>  <br/> |<span data-ttu-id="d6200-133">連絡先の郵便番号を表します。</span><span class="sxs-lookup"><span data-stu-id="d6200-133">Represents the postal code of a contact.</span></span>  <br/> |
|<span data-ttu-id="d6200-134">連絡先: PhoneNumber</span><span class="sxs-lookup"><span data-stu-id="d6200-134">contacts:PhoneNumber</span></span>  <br/> |<span data-ttu-id="d6200-135">連絡先の電話番号を表します。</span><span class="sxs-lookup"><span data-stu-id="d6200-135">Represents the phone number of a contact.</span></span>  <br/> |
|<span data-ttu-id="d6200-136">連絡先: EmailAddress</span><span class="sxs-lookup"><span data-stu-id="d6200-136">contacts:EmailAddress</span></span>  <br/> |<span data-ttu-id="d6200-137">連絡先の電子メールアドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="d6200-137">Represents the e-mail address of a contact.</span></span>  <br/> |
|<span data-ttu-id="d6200-138">distributionlist: Members: Member</span><span class="sxs-lookup"><span data-stu-id="d6200-138">distributionlist:Members:Member</span></span>  <br/> |<span data-ttu-id="d6200-139">配布リストのメンバーを表します。</span><span class="sxs-lookup"><span data-stu-id="d6200-139">Represents a member of a distribution list.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d6200-140">子要素</span><span class="sxs-lookup"><span data-stu-id="d6200-140">Child elements</span></span>

<span data-ttu-id="d6200-141">なし。</span><span class="sxs-lookup"><span data-stu-id="d6200-141">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d6200-142">親要素</span><span class="sxs-lookup"><span data-stu-id="d6200-142">Parent elements</span></span>

|<span data-ttu-id="d6200-143">**要素**</span><span class="sxs-lookup"><span data-stu-id="d6200-143">**Element**</span></span>|<span data-ttu-id="d6200-144">**説明**</span><span class="sxs-lookup"><span data-stu-id="d6200-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d6200-145">AdditionalProperties</span><span class="sxs-lookup"><span data-stu-id="d6200-145">AdditionalProperties</span></span>](additionalproperties.md) <br/> |<span data-ttu-id="d6200-146">取得、設定、または作成する追加のプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="d6200-146">Identifies additional properties to get, set, or create.</span></span>  <br/> |
|[<span data-ttu-id="d6200-147">AggregateOn</span><span class="sxs-lookup"><span data-stu-id="d6200-147">AggregateOn</span></span>](aggregateon.md) <br/> |<span data-ttu-id="d6200-148">グループ化された FindItem 結果セットのグループ化されたアイテムの順序を決定するために使用されるプロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="d6200-148">Represents the property that is used to determine the order of grouped items for a grouped FindItem result set.</span></span>  <br/> |
|[<span data-ttu-id="d6200-149">GroupBy</span><span class="sxs-lookup"><span data-stu-id="d6200-149">GroupBy</span></span>](groupby.md) <br/> |<span data-ttu-id="d6200-150">FindItem クエリの任意のグループを指定します。</span><span class="sxs-lookup"><span data-stu-id="d6200-150">Specifies an arbitrary grouping for FindItem queries.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d6200-151">注釈</span><span class="sxs-lookup"><span data-stu-id="d6200-151">Remarks</span></span>

<span data-ttu-id="d6200-152">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="d6200-152">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d6200-153">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d6200-153">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d6200-154">Namespace</span><span class="sxs-lookup"><span data-stu-id="d6200-154">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d6200-155">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d6200-155">Schema Name</span></span>  <br/> |<span data-ttu-id="d6200-156">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="d6200-156">Types schema</span></span>  <br/> |
|<span data-ttu-id="d6200-157">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d6200-157">Validation File</span></span>  <br/> |<span data-ttu-id="d6200-158">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="d6200-158">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d6200-159">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d6200-159">Can be Empty</span></span>  <br/> |<span data-ttu-id="d6200-160">正しくない</span><span class="sxs-lookup"><span data-stu-id="d6200-160">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d6200-161">関連項目</span><span class="sxs-lookup"><span data-stu-id="d6200-161">See also</span></span>



- [<span data-ttu-id="d6200-162">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="d6200-162">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

