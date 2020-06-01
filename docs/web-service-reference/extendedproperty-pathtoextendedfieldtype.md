---
title: ExtendedProperty (PathToExtendedFieldType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fa620b48-2ce3-437d-b51e-541247eea1d9
description: ExtendedProperty 要素は、統合連絡先ストアの拡張プロパティを指定します。
ms.openlocfilehash: f6c283d5cce3bc927662ad0d9c796c0589e7054c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460142"
---
# <a name="extendedproperty-pathtoextendedfieldtype"></a><span data-ttu-id="a8a7f-103">ExtendedProperty (PathToExtendedFieldType)</span><span class="sxs-lookup"><span data-stu-id="a8a7f-103">ExtendedProperty (PathToExtendedFieldType)</span></span>

<span data-ttu-id="a8a7f-104">**Extendedproperty**要素は、統合連絡先ストアの拡張プロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-104">The **ExtendedProperty** element specifies an extended property for the Unified Contact Store.</span></span> 
  
```xml
<ExtendedProperty DistinguishedPropertySetId="" PropertySetId="" PropertyTag="" PropertyName="" PropertyId="" PropertyType="" FieldURI="">
</ExtendedProperty>
```

<span data-ttu-id="a8a7f-105">**PathToExtendedFieldType**</span><span class="sxs-lookup"><span data-stu-id="a8a7f-105">**PathToExtendedFieldType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="a8a7f-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="a8a7f-106">Attributes and elements</span></span>

<span data-ttu-id="a8a7f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a8a7f-108">属性</span><span class="sxs-lookup"><span data-stu-id="a8a7f-108">Attributes</span></span>

|<span data-ttu-id="a8a7f-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="a8a7f-109">**Attribute**</span></span>|<span data-ttu-id="a8a7f-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="a8a7f-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a8a7f-111">DistinguishedPropertySetId</span><span class="sxs-lookup"><span data-stu-id="a8a7f-111">DistinguishedPropertySetId</span></span>  <br/> |<span data-ttu-id="a8a7f-112">識別プロパティセット識別子を示します。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-112">Indicates the distinguished property set identifier.</span></span> <span data-ttu-id="a8a7f-113">この属性は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-113">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="a8a7f-114">PropertySetId</span><span class="sxs-lookup"><span data-stu-id="a8a7f-114">PropertySetId</span></span>  <br/> |<span data-ttu-id="a8a7f-115">GUID プロパティセット識別子を示します。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-115">Indicates the GUID property set identifier.</span></span> <span data-ttu-id="a8a7f-116">この属性は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-116">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="a8a7f-117">PropertyTag</span><span class="sxs-lookup"><span data-stu-id="a8a7f-117">PropertyTag</span></span>  <br/> | <span data-ttu-id="a8a7f-118">プロパティタグから type part を引いたものを表します。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-118">Represents the property tag minus the type part.</span></span><br/><br/><span data-ttu-id="a8a7f-119">表現には、次の2つのオプションがあります。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-119">There are two options for representation:</span></span>  <br/><br/><span data-ttu-id="a8a7f-120">-16 進: 0x3fa4</span><span class="sxs-lookup"><span data-stu-id="a8a7f-120">-  Hexadecimal: 0x3fa4</span></span>  <br/><span data-ttu-id="a8a7f-121">-10 進: 0-65535</span><span class="sxs-lookup"><span data-stu-id="a8a7f-121">-  Decimal: 0-65535</span></span><br/><br/>  <span data-ttu-id="a8a7f-122">この属性は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-122">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="a8a7f-123">PropertyName</span><span class="sxs-lookup"><span data-stu-id="a8a7f-123">PropertyName</span></span>  <br/> |<span data-ttu-id="a8a7f-124">プロパティ名を示す文字列。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-124">String that indicates the property name.</span></span> <span data-ttu-id="a8a7f-125">この属性は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-125">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="a8a7f-126">PropertyId</span><span class="sxs-lookup"><span data-stu-id="a8a7f-126">PropertyId</span></span>  <br/> |<span data-ttu-id="a8a7f-127">プロパティ識別子を示す整数。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-127">Integer that indicates the property identifier.</span></span> <span data-ttu-id="a8a7f-128">この属性は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-128">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="a8a7f-129">Recordtype</span><span class="sxs-lookup"><span data-stu-id="a8a7f-129">PropertyType</span></span>  <br/> |<span data-ttu-id="a8a7f-130">プロパティの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-130">Indicates the property type.</span></span> <span data-ttu-id="a8a7f-131">この属性は必須です。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-131">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="a8a7f-132">FieldURI</span><span class="sxs-lookup"><span data-stu-id="a8a7f-132">FieldURI</span></span>  <br/> |<span data-ttu-id="a8a7f-133">フィールド URI (Uniform Resource Identifier) を示します。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-133">Indicates the field Uniform Resource Identifier (URI).</span></span> <span data-ttu-id="a8a7f-134">この属性は必須です。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-134">This attribute is required.</span></span> <span data-ttu-id="a8a7f-135">可能な値については、 [FieldURI](fielduri.md)要素を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-135">For possible values, see the [FieldURI](fielduri.md) element.</span></span>  <br/> |
   
#### <a name="distinguishedpropertysetid"></a><span data-ttu-id="a8a7f-136">DistinguishedPropertySetId</span><span class="sxs-lookup"><span data-stu-id="a8a7f-136">DistinguishedPropertySetId</span></span>

|<span data-ttu-id="a8a7f-137">**値**</span><span class="sxs-lookup"><span data-stu-id="a8a7f-137">**Value**</span></span>|<span data-ttu-id="a8a7f-138">**説明**</span><span class="sxs-lookup"><span data-stu-id="a8a7f-138">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a8a7f-139">会議</span><span class="sxs-lookup"><span data-stu-id="a8a7f-139">Meeting</span></span>  <br/> |<span data-ttu-id="a8a7f-140">会議を示します。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-140">Indicates a meeting.</span></span>  <br/> |
|<span data-ttu-id="a8a7f-141">Appointment</span><span class="sxs-lookup"><span data-stu-id="a8a7f-141">Appointment</span></span>  <br/> |<span data-ttu-id="a8a7f-142">予定を示します。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-142">Indicates an appointment.</span></span>  <br/> |
|<span data-ttu-id="a8a7f-143">共通</span><span class="sxs-lookup"><span data-stu-id="a8a7f-143">Common</span></span>  <br/> |<span data-ttu-id="a8a7f-144">Common プロパティセットを示します。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-144">Indicates the common property set.</span></span>  <br/> |
|<span data-ttu-id="a8a7f-145">PublicStrings</span><span class="sxs-lookup"><span data-stu-id="a8a7f-145">PublicStrings</span></span>  <br/> |<span data-ttu-id="a8a7f-146">パブリック文字列を示します。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-146">Indicates public strings.</span></span>  <br/> |
|<span data-ttu-id="a8a7f-147">Address</span><span class="sxs-lookup"><span data-stu-id="a8a7f-147">Address</span></span>  <br/> |<span data-ttu-id="a8a7f-148">アドレスを示します。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-148">Indicates an address.</span></span>  <br/> |
|<span data-ttu-id="a8a7f-149">InternetHeaders</span><span class="sxs-lookup"><span data-stu-id="a8a7f-149">InternetHeaders</span></span>  <br/> |<span data-ttu-id="a8a7f-150">インターネットヘッダーを示します。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-150">Indicates Internet headers.</span></span>  <br/> |
|<span data-ttu-id="a8a7f-151">CalendarAssistant</span><span class="sxs-lookup"><span data-stu-id="a8a7f-151">CalendarAssistant</span></span>  <br/> |<span data-ttu-id="a8a7f-152">カレンダーアシスタントを示します。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-152">Indicates the Calendar Assistant.</span></span>  <br/> |
|<span data-ttu-id="a8a7f-153">UnifiedMessaging</span><span class="sxs-lookup"><span data-stu-id="a8a7f-153">UnifiedMessaging</span></span>  <br/> |<span data-ttu-id="a8a7f-154">ユニファイドメッセージングを示します。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-154">Indicates Unified Messaging.</span></span>  <br/> |
|<span data-ttu-id="a8a7f-155">タスク</span><span class="sxs-lookup"><span data-stu-id="a8a7f-155">Task</span></span>  <br/> |<span data-ttu-id="a8a7f-156">タスクを示します。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-156">Indicates a task.</span></span>  <br/> |
   
#### <a name="propertytype"></a><span data-ttu-id="a8a7f-157">Recordtype</span><span class="sxs-lookup"><span data-stu-id="a8a7f-157">PropertyType</span></span>

|<span data-ttu-id="a8a7f-158">**値**</span><span class="sxs-lookup"><span data-stu-id="a8a7f-158">**Value**</span></span>|<span data-ttu-id="a8a7f-159">**説明**</span><span class="sxs-lookup"><span data-stu-id="a8a7f-159">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a8a7f-160">ApplicationTime</span><span class="sxs-lookup"><span data-stu-id="a8a7f-160">ApplicationTime</span></span>  <br/> |<span data-ttu-id="a8a7f-161">アプリケーション時間を示します。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-161">Indicates the application time.</span></span>  <br/> |
|<span data-ttu-id="a8a7f-162">ApplicationTimeArray</span><span class="sxs-lookup"><span data-stu-id="a8a7f-162">ApplicationTimeArray</span></span>  <br/> |<span data-ttu-id="a8a7f-163">アプリケーション時間の配列を示します。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-163">Indicates an array of application times.</span></span>  <br/> |
|<span data-ttu-id="a8a7f-164">バイナリ</span><span class="sxs-lookup"><span data-stu-id="a8a7f-164">Binary</span></span>  <br/> |<span data-ttu-id="a8a7f-165">バイナリ値を示します。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-165">Indicates a binary value.</span></span>  <br/> |
|<span data-ttu-id="a8a7f-166">BinaryArray</span><span class="sxs-lookup"><span data-stu-id="a8a7f-166">BinaryArray</span></span>  <br/> |<span data-ttu-id="a8a7f-167">バイナリ値の配列を示します。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-167">Indicates an array of binary values.</span></span>  <br/> |
|<span data-ttu-id="a8a7f-168">ブール型</span><span class="sxs-lookup"><span data-stu-id="a8a7f-168">Boolean</span></span>  <br/> |<span data-ttu-id="a8a7f-169">ブール値を示します。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-169">Indicates a Boolean value.</span></span>  <br/> |
|<span data-ttu-id="a8a7f-170">CLSID</span><span class="sxs-lookup"><span data-stu-id="a8a7f-170">CLSID</span></span>  <br/> |<span data-ttu-id="a8a7f-171">CLSID を示します。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-171">Indicates a CLSID.</span></span>  <br/> |
|<span data-ttu-id="a8a7f-172">CLSIDArray</span><span class="sxs-lookup"><span data-stu-id="a8a7f-172">CLSIDArray</span></span>  <br/> |<span data-ttu-id="a8a7f-173">Clsid の配列を示します。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-173">Indicates an array of CLSIDs.</span></span>  <br/> |
|<span data-ttu-id="a8a7f-174">通貨</span><span class="sxs-lookup"><span data-stu-id="a8a7f-174">Currency</span></span>  <br/> |<span data-ttu-id="a8a7f-175">通貨値を示します。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-175">Indicates a currency value.</span></span>  <br/> |
|<span data-ttu-id="a8a7f-176">CurrencyArray</span><span class="sxs-lookup"><span data-stu-id="a8a7f-176">CurrencyArray</span></span>  <br/> |<span data-ttu-id="a8a7f-177">通貨値の配列を示します。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-177">Indicates an array of currency values.</span></span>  <br/> |
|<span data-ttu-id="a8a7f-178">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="a8a7f-178">Double</span></span>  <br/> |<span data-ttu-id="a8a7f-179">**倍精度浮動小数点**型を示します。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-179">Indicates a **double**.</span></span>  <br/> |
|<span data-ttu-id="a8a7f-180">DoubleArray</span><span class="sxs-lookup"><span data-stu-id="a8a7f-180">DoubleArray</span></span>  <br/> |<span data-ttu-id="a8a7f-181">**倍精度浮動小数点**型の値の配列を示します。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-181">Indicates an array of **double** values.</span></span>  <br/> |
|<span data-ttu-id="a8a7f-182">Error</span><span class="sxs-lookup"><span data-stu-id="a8a7f-182">Error</span></span>  <br/> |<span data-ttu-id="a8a7f-183">エラーを示します。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-183">Indicates an error.</span></span> <span data-ttu-id="a8a7f-184">これはエラーレポートのためのものです。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-184">This is for error-reporting purposes.</span></span> <span data-ttu-id="a8a7f-185">制限で、または値を取得または設定するために使用することはできません。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-185">It cannot be used in restrictions or for getting or setting values.</span></span>  <br/> |
|<span data-ttu-id="a8a7f-186">浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="a8a7f-186">Float</span></span>  <br/> |<span data-ttu-id="a8a7f-187">**Float**を示します。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-187">Indicates a **float**.</span></span>  <br/> |
|<span data-ttu-id="a8a7f-188">FloatArray</span><span class="sxs-lookup"><span data-stu-id="a8a7f-188">FloatArray</span></span>  <br/> |<span data-ttu-id="a8a7f-189">**Float**値の配列を示します。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-189">Indicates an array of **float** values.</span></span>  <br/> |
|<span data-ttu-id="a8a7f-190">整数</span><span class="sxs-lookup"><span data-stu-id="a8a7f-190">Integer</span></span>  <br/> |<span data-ttu-id="a8a7f-191">整数を示します。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-191">Indicates an integer.</span></span>  <br/> |
|<span data-ttu-id="a8a7f-192">整数配列</span><span class="sxs-lookup"><span data-stu-id="a8a7f-192">IntegerArray</span></span>  <br/> |<span data-ttu-id="a8a7f-193">整数の配列を示します。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-193">Indicates an array of integers.</span></span>  <br/> |
|<span data-ttu-id="a8a7f-194">Long</span><span class="sxs-lookup"><span data-stu-id="a8a7f-194">Long</span></span>  <br/> |<span data-ttu-id="a8a7f-195">**Long**を示します。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-195">Indicates a **long**.</span></span>  <br/> |
|<span data-ttu-id="a8a7f-196">LongArray</span><span class="sxs-lookup"><span data-stu-id="a8a7f-196">LongArray</span></span>  <br/> |<span data-ttu-id="a8a7f-197">**長整数型 (long)** の値の配列を示します。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-197">Indicates an array of **long** values.</span></span>  <br/> |
|<span data-ttu-id="a8a7f-198">Null</span><span class="sxs-lookup"><span data-stu-id="a8a7f-198">Null</span></span>  <br/> |<span data-ttu-id="a8a7f-199">Null 値を示します。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-199">Indicates a null value.</span></span> <span data-ttu-id="a8a7f-200">これはエラーレポートのためのものです。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-200">This is for error-reporting purposes.</span></span> <span data-ttu-id="a8a7f-201">制限で、または値を取得または設定するために使用することはできません。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-201">It cannot be used in restrictions or for getting or setting values.</span></span>  <br/> |
|<span data-ttu-id="a8a7f-202">オブジェクト</span><span class="sxs-lookup"><span data-stu-id="a8a7f-202">Object</span></span>  <br/> |<span data-ttu-id="a8a7f-203">オブジェクトを示します。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-203">Indicates an object.</span></span> <span data-ttu-id="a8a7f-204">これはエラーレポートのためのものです。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-204">This is for error-reporting purposes.</span></span> <span data-ttu-id="a8a7f-205">制限で、または値を取得または設定するために使用することはできません。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-205">It cannot be used in restrictions or for getting or setting values.</span></span>  <br/> |
|<span data-ttu-id="a8a7f-206">ObjectArray</span><span class="sxs-lookup"><span data-stu-id="a8a7f-206">ObjectArray</span></span>  <br/> |<span data-ttu-id="a8a7f-207">オブジェクトの配列を示します。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-207">Indicates an array of objects.</span></span> <span data-ttu-id="a8a7f-208">これはエラーレポートのためのものです。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-208">This is for error-reporting purposes.</span></span> <span data-ttu-id="a8a7f-209">制限で、または値を取得または設定するために使用することはできません。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-209">It cannot be used in restrictions or for getting or setting values.</span></span>  <br/> |
|<span data-ttu-id="a8a7f-210">長い形式の日付 (スラッシュ区切り)</span><span class="sxs-lookup"><span data-stu-id="a8a7f-210">Short</span></span>  <br/> |<span data-ttu-id="a8a7f-211">**Short**を示します。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-211">Indicates a **short**.</span></span>  <br/> |
|<span data-ttu-id="a8a7f-212">Short 配列</span><span class="sxs-lookup"><span data-stu-id="a8a7f-212">ShortArray</span></span>  <br/> |<span data-ttu-id="a8a7f-213">**Short**値の配列を示します。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-213">Indicates an array of **short** values.</span></span>  <br/> |
|<span data-ttu-id="a8a7f-214">SystemTime</span><span class="sxs-lookup"><span data-stu-id="a8a7f-214">SystemTime</span></span>  <br/> |<span data-ttu-id="a8a7f-215">システム時間の値を示します。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-215">Indicates a system time value.</span></span>  <br/> |
|<span data-ttu-id="a8a7f-216">SystemTimeArray</span><span class="sxs-lookup"><span data-stu-id="a8a7f-216">SystemTimeArray</span></span>  <br/> |<span data-ttu-id="a8a7f-217">システム時間の値の配列を示します。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-217">Indicates an array of system time values.</span></span>  <br/> |
|<span data-ttu-id="a8a7f-218">String</span><span class="sxs-lookup"><span data-stu-id="a8a7f-218">String</span></span>  <br/> |<span data-ttu-id="a8a7f-219">文字列を示します。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-219">Indicates a string.</span></span>  <br/> |
|<span data-ttu-id="a8a7f-220">StringArray</span><span class="sxs-lookup"><span data-stu-id="a8a7f-220">StringArray</span></span>  <br/> |<span data-ttu-id="a8a7f-221">文字列の配列を示します。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-221">Indicates an array of strings.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="a8a7f-222">子要素</span><span class="sxs-lookup"><span data-stu-id="a8a7f-222">Child elements</span></span>

<span data-ttu-id="a8a7f-223">なし。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-223">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a8a7f-224">親要素</span><span class="sxs-lookup"><span data-stu-id="a8a7f-224">Parent elements</span></span>

|<span data-ttu-id="a8a7f-225">**要素**</span><span class="sxs-lookup"><span data-stu-id="a8a7f-225">**Element**</span></span>|<span data-ttu-id="a8a7f-226">**説明**</span><span class="sxs-lookup"><span data-stu-id="a8a7f-226">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a8a7f-227">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="a8a7f-227">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="a8a7f-228">拡張 MAPI プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-228">Identifies an extended MAPI property.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a8a7f-229">注釈</span><span class="sxs-lookup"><span data-stu-id="a8a7f-229">Remarks</span></span>

<span data-ttu-id="a8a7f-230">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-230">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="a8a7f-231">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-231">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a8a7f-232">要素の情報</span><span class="sxs-lookup"><span data-stu-id="a8a7f-232">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a8a7f-233">Namespace</span><span class="sxs-lookup"><span data-stu-id="a8a7f-233">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a8a7f-234">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a8a7f-234">Schema Name</span></span>  <br/> |<span data-ttu-id="a8a7f-235">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="a8a7f-235">Type schema</span></span>  <br/> |
|<span data-ttu-id="a8a7f-236">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a8a7f-236">Validation File</span></span>  <br/> |<span data-ttu-id="a8a7f-237">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="a8a7f-237">types.xsd</span></span>  <br/> |
|<span data-ttu-id="a8a7f-238">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="a8a7f-238">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="a8a7f-239">関連項目</span><span class="sxs-lookup"><span data-stu-id="a8a7f-239">See also</span></span>

- [<span data-ttu-id="a8a7f-240">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="a8a7f-240">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

