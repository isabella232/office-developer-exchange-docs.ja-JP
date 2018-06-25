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
description: IndexedFieldURI 要素は、辞書の個々 のメンバーを識別します。
ms.openlocfilehash: 6a75e8855ecabf15ca31bb1e05d569c258a43b0b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831909"
---
# <a name="indexedfielduri"></a><span data-ttu-id="2c66a-103">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="2c66a-103">IndexedFieldURI</span></span>

<span data-ttu-id="2c66a-104">**IndexedFieldURI**要素は、辞書の個々 のメンバーを識別します。</span><span class="sxs-lookup"><span data-stu-id="2c66a-104">The **IndexedFieldURI** element identifies individual members of a dictionary.</span></span> 
  
```xml
<IndexedFieldURI FieldURI="" FieldIndex="" />
```

 <span data-ttu-id="2c66a-105">**PathToIndexedFieldType**</span><span class="sxs-lookup"><span data-stu-id="2c66a-105">**PathToIndexedFieldType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2c66a-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="2c66a-106">Attributes and elements</span></span>

<span data-ttu-id="2c66a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2c66a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2c66a-108">属性</span><span class="sxs-lookup"><span data-stu-id="2c66a-108">Attributes</span></span>

|<span data-ttu-id="2c66a-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="2c66a-109">**Attribute**</span></span>|<span data-ttu-id="2c66a-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="2c66a-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2c66a-111">**FieldURI**</span><span class="sxs-lookup"><span data-stu-id="2c66a-111">**FieldURI**</span></span> <br/> |<span data-ttu-id="2c66a-112">返すメンバーを格納しているディクショナリを識別します。</span><span class="sxs-lookup"><span data-stu-id="2c66a-112">Identifies the dictionary that contains the member to return.</span></span> <span data-ttu-id="2c66a-113">この属性は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="2c66a-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="2c66a-114">**FieldIndex**</span><span class="sxs-lookup"><span data-stu-id="2c66a-114">**FieldIndex**</span></span> <br/> |<span data-ttu-id="2c66a-115">返すディクショナリのメンバーを識別します。</span><span class="sxs-lookup"><span data-stu-id="2c66a-115">Identifies the member of the dictionary to return.</span></span> <span data-ttu-id="2c66a-116">この属性は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="2c66a-116">This attribute is required.</span></span>  <br/> |
   
#### <a name="fielduri-attribute"></a><span data-ttu-id="2c66a-117">FieldURI 属性</span><span class="sxs-lookup"><span data-stu-id="2c66a-117">FieldURI Attribute</span></span>

|<span data-ttu-id="2c66a-118">**値**</span><span class="sxs-lookup"><span data-stu-id="2c66a-118">**Value**</span></span>|<span data-ttu-id="2c66a-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="2c66a-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2c66a-120">アイテム: InternetMessageHeader</span><span class="sxs-lookup"><span data-stu-id="2c66a-120">item:InternetMessageHeader</span></span>  <br/> |<span data-ttu-id="2c66a-121">アイテムのメッセージのヘッダーを表します。</span><span class="sxs-lookup"><span data-stu-id="2c66a-121">Represents the message header of an item.</span></span>  <br/> |
|<span data-ttu-id="2c66a-122">連絡先: ImAddress</span><span class="sxs-lookup"><span data-stu-id="2c66a-122">contacts:ImAddress</span></span>  <br/> |<span data-ttu-id="2c66a-123">インスタント メッセージの連絡先のアドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="2c66a-123">Represents the instant messaging address of a contact.</span></span>  <br/> |
|<span data-ttu-id="2c66a-124">連絡先: PhysicalAddress:Street</span><span class="sxs-lookup"><span data-stu-id="2c66a-124">contacts:PhysicalAddress:Street</span></span>  <br/> |<span data-ttu-id="2c66a-125">連絡先の住所を表します。</span><span class="sxs-lookup"><span data-stu-id="2c66a-125">Represents the street address of a contact.</span></span>  <br/> |
|<span data-ttu-id="2c66a-126">連絡先: PhysicalAddress:City</span><span class="sxs-lookup"><span data-stu-id="2c66a-126">contacts:PhysicalAddress:City</span></span>  <br/> |<span data-ttu-id="2c66a-127">連絡先の市区町村を表します。</span><span class="sxs-lookup"><span data-stu-id="2c66a-127">Represents the city of a contact.</span></span>  <br/> |
|<span data-ttu-id="2c66a-128">連絡先: PhysicalAddress:State</span><span class="sxs-lookup"><span data-stu-id="2c66a-128">contacts:PhysicalAddress:State</span></span>  <br/> |<span data-ttu-id="2c66a-129">連絡先の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="2c66a-129">Represents the state of a contact.</span></span>  <br/> |
|<span data-ttu-id="2c66a-130">連絡先: PhysicalAddress:Country</span><span class="sxs-lookup"><span data-stu-id="2c66a-130">contacts:PhysicalAddress:Country</span></span>  <br/> |<span data-ttu-id="2c66a-131">連絡先の国/地域を表します。</span><span class="sxs-lookup"><span data-stu-id="2c66a-131">Represents the country/region of a contact.</span></span>  <br/> |
|<span data-ttu-id="2c66a-132">連絡先: PhysicalAddress:PostalCode</span><span class="sxs-lookup"><span data-stu-id="2c66a-132">contacts:PhysicalAddress:PostalCode</span></span>  <br/> |<span data-ttu-id="2c66a-133">連絡先の郵便番号コードを表します。</span><span class="sxs-lookup"><span data-stu-id="2c66a-133">Represents the postal code of a contact.</span></span>  <br/> |
|<span data-ttu-id="2c66a-134">連絡先: 電話番号</span><span class="sxs-lookup"><span data-stu-id="2c66a-134">contacts:PhoneNumber</span></span>  <br/> |<span data-ttu-id="2c66a-135">連絡先の電話番号を表します。</span><span class="sxs-lookup"><span data-stu-id="2c66a-135">Represents the phone number of a contact.</span></span>  <br/> |
|<span data-ttu-id="2c66a-136">EmailAddress の連絡先:</span><span class="sxs-lookup"><span data-stu-id="2c66a-136">contacts:EmailAddress</span></span>  <br/> |<span data-ttu-id="2c66a-137">連絡先の電子メール アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="2c66a-137">Represents the e-mail address of a contact.</span></span>  <br/> |
|<span data-ttu-id="2c66a-138">distributionlist:Members:Member</span><span class="sxs-lookup"><span data-stu-id="2c66a-138">distributionlist:Members:Member</span></span>  <br/> |<span data-ttu-id="2c66a-139">配布リストのメンバーを表します。</span><span class="sxs-lookup"><span data-stu-id="2c66a-139">Represents a member of a distribution list.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="2c66a-140">子要素</span><span class="sxs-lookup"><span data-stu-id="2c66a-140">Child elements</span></span>

<span data-ttu-id="2c66a-141">なし。</span><span class="sxs-lookup"><span data-stu-id="2c66a-141">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2c66a-142">親要素</span><span class="sxs-lookup"><span data-stu-id="2c66a-142">Parent elements</span></span>

|<span data-ttu-id="2c66a-143">**要素**</span><span class="sxs-lookup"><span data-stu-id="2c66a-143">**Element**</span></span>|<span data-ttu-id="2c66a-144">**説明**</span><span class="sxs-lookup"><span data-stu-id="2c66a-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2c66a-145">AdditionalProperties</span><span class="sxs-lookup"><span data-stu-id="2c66a-145">AdditionalProperties</span></span>](additionalproperties.md) <br/> |<span data-ttu-id="2c66a-146">取得、設定、または作成する追加のプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="2c66a-146">Identifies additional properties to get, set, or create.</span></span>  <br/> |
|[<span data-ttu-id="2c66a-147">AggregateOn</span><span class="sxs-lookup"><span data-stu-id="2c66a-147">AggregateOn</span></span>](aggregateon.md) <br/> |<span data-ttu-id="2c66a-148">グループ化された FindItem 結果セットをグループ化した項目の順序を決定するために使用されるプロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="2c66a-148">Represents the property that is used to determine the order of grouped items for a grouped FindItem result set.</span></span>  <br/> |
|[<span data-ttu-id="2c66a-149">GroupBy</span><span class="sxs-lookup"><span data-stu-id="2c66a-149">GroupBy</span></span>](groupby.md) <br/> |<span data-ttu-id="2c66a-150">FindItem クエリの任意のグループ化を指定します。</span><span class="sxs-lookup"><span data-stu-id="2c66a-150">Specifies an arbitrary grouping for FindItem queries.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2c66a-151">備考</span><span class="sxs-lookup"><span data-stu-id="2c66a-151">Remarks</span></span>

<span data-ttu-id="2c66a-152">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="2c66a-152">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2c66a-153">要素情報</span><span class="sxs-lookup"><span data-stu-id="2c66a-153">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2c66a-154">名前空間</span><span class="sxs-lookup"><span data-stu-id="2c66a-154">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2c66a-155">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2c66a-155">Schema Name</span></span>  <br/> |<span data-ttu-id="2c66a-156">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="2c66a-156">Types schema</span></span>  <br/> |
|<span data-ttu-id="2c66a-157">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2c66a-157">Validation File</span></span>  <br/> |<span data-ttu-id="2c66a-158">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2c66a-158">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2c66a-159">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="2c66a-159">Can be Empty</span></span>  <br/> |<span data-ttu-id="2c66a-160">False</span><span class="sxs-lookup"><span data-stu-id="2c66a-160">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2c66a-161">関連項目</span><span class="sxs-lookup"><span data-stu-id="2c66a-161">See also</span></span>



- [<span data-ttu-id="2c66a-162">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="2c66a-162">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

