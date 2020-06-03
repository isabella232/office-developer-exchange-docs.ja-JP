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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460142"
---
# <a name="extendedproperty-pathtoextendedfieldtype"></a><span data-ttu-id="a9254-103">ExtendedProperty (PathToExtendedFieldType)</span><span class="sxs-lookup"><span data-stu-id="a9254-103">ExtendedProperty (PathToExtendedFieldType)</span></span>

<span data-ttu-id="a9254-104">**Extendedproperty**要素は、統合連絡先ストアの拡張プロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="a9254-104">The **ExtendedProperty** element specifies an extended property for the Unified Contact Store.</span></span> 
  
```xml
<ExtendedProperty DistinguishedPropertySetId="" PropertySetId="" PropertyTag="" PropertyName="" PropertyId="" PropertyType="" FieldURI="">
</ExtendedProperty>
```

<span data-ttu-id="a9254-105">**PathToExtendedFieldType**</span><span class="sxs-lookup"><span data-stu-id="a9254-105">**PathToExtendedFieldType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="a9254-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="a9254-106">Attributes and elements</span></span>

<span data-ttu-id="a9254-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a9254-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a9254-108">属性</span><span class="sxs-lookup"><span data-stu-id="a9254-108">Attributes</span></span>

|<span data-ttu-id="a9254-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="a9254-109">**Attribute**</span></span>|<span data-ttu-id="a9254-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="a9254-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a9254-111">DistinguishedPropertySetId</span><span class="sxs-lookup"><span data-stu-id="a9254-111">DistinguishedPropertySetId</span></span>  <br/> |<span data-ttu-id="a9254-112">識別プロパティセット識別子を示します。</span><span class="sxs-lookup"><span data-stu-id="a9254-112">Indicates the distinguished property set identifier.</span></span> <span data-ttu-id="a9254-113">この属性は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="a9254-113">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="a9254-114">PropertySetId</span><span class="sxs-lookup"><span data-stu-id="a9254-114">PropertySetId</span></span>  <br/> |<span data-ttu-id="a9254-115">GUID プロパティセット識別子を示します。</span><span class="sxs-lookup"><span data-stu-id="a9254-115">Indicates the GUID property set identifier.</span></span> <span data-ttu-id="a9254-116">この属性は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="a9254-116">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="a9254-117">PropertyTag</span><span class="sxs-lookup"><span data-stu-id="a9254-117">PropertyTag</span></span>  <br/> | <span data-ttu-id="a9254-118">プロパティタグから type part を引いたものを表します。</span><span class="sxs-lookup"><span data-stu-id="a9254-118">Represents the property tag minus the type part.</span></span><br/><br/><span data-ttu-id="a9254-119">表現には、次の2つのオプションがあります。</span><span class="sxs-lookup"><span data-stu-id="a9254-119">There are two options for representation:</span></span>  <br/><br/><span data-ttu-id="a9254-120">-16 進: 0x3fa4</span><span class="sxs-lookup"><span data-stu-id="a9254-120">-  Hexadecimal: 0x3fa4</span></span>  <br/><span data-ttu-id="a9254-121">-10 進: 0-65535</span><span class="sxs-lookup"><span data-stu-id="a9254-121">-  Decimal: 0-65535</span></span><br/><br/>  <span data-ttu-id="a9254-122">この属性は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="a9254-122">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="a9254-123">PropertyName</span><span class="sxs-lookup"><span data-stu-id="a9254-123">PropertyName</span></span>  <br/> |<span data-ttu-id="a9254-124">プロパティ名を示す文字列。</span><span class="sxs-lookup"><span data-stu-id="a9254-124">String that indicates the property name.</span></span> <span data-ttu-id="a9254-125">この属性は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="a9254-125">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="a9254-126">PropertyId</span><span class="sxs-lookup"><span data-stu-id="a9254-126">PropertyId</span></span>  <br/> |<span data-ttu-id="a9254-127">プロパティ識別子を示す整数。</span><span class="sxs-lookup"><span data-stu-id="a9254-127">Integer that indicates the property identifier.</span></span> <span data-ttu-id="a9254-128">この属性は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="a9254-128">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="a9254-129">Recordtype</span><span class="sxs-lookup"><span data-stu-id="a9254-129">PropertyType</span></span>  <br/> |<span data-ttu-id="a9254-130">プロパティの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="a9254-130">Indicates the property type.</span></span> <span data-ttu-id="a9254-131">この属性は必須です。</span><span class="sxs-lookup"><span data-stu-id="a9254-131">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="a9254-132">FieldURI</span><span class="sxs-lookup"><span data-stu-id="a9254-132">FieldURI</span></span>  <br/> |<span data-ttu-id="a9254-133">フィールド URI (Uniform Resource Identifier) を示します。</span><span class="sxs-lookup"><span data-stu-id="a9254-133">Indicates the field Uniform Resource Identifier (URI).</span></span> <span data-ttu-id="a9254-134">この属性は必須です。</span><span class="sxs-lookup"><span data-stu-id="a9254-134">This attribute is required.</span></span> <span data-ttu-id="a9254-135">可能な値については、 [FieldURI](fielduri.md)要素を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a9254-135">For possible values, see the [FieldURI](fielduri.md) element.</span></span>  <br/> |
   
#### <a name="distinguishedpropertysetid"></a><span data-ttu-id="a9254-136">DistinguishedPropertySetId</span><span class="sxs-lookup"><span data-stu-id="a9254-136">DistinguishedPropertySetId</span></span>

|<span data-ttu-id="a9254-137">**値**</span><span class="sxs-lookup"><span data-stu-id="a9254-137">**Value**</span></span>|<span data-ttu-id="a9254-138">**説明**</span><span class="sxs-lookup"><span data-stu-id="a9254-138">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a9254-139">会議</span><span class="sxs-lookup"><span data-stu-id="a9254-139">Meeting</span></span>  <br/> |<span data-ttu-id="a9254-140">会議を示します。</span><span class="sxs-lookup"><span data-stu-id="a9254-140">Indicates a meeting.</span></span>  <br/> |
|<span data-ttu-id="a9254-141">Appointment</span><span class="sxs-lookup"><span data-stu-id="a9254-141">Appointment</span></span>  <br/> |<span data-ttu-id="a9254-142">予定を示します。</span><span class="sxs-lookup"><span data-stu-id="a9254-142">Indicates an appointment.</span></span>  <br/> |
|<span data-ttu-id="a9254-143">共通</span><span class="sxs-lookup"><span data-stu-id="a9254-143">Common</span></span>  <br/> |<span data-ttu-id="a9254-144">Common プロパティセットを示します。</span><span class="sxs-lookup"><span data-stu-id="a9254-144">Indicates the common property set.</span></span>  <br/> |
|<span data-ttu-id="a9254-145">PublicStrings</span><span class="sxs-lookup"><span data-stu-id="a9254-145">PublicStrings</span></span>  <br/> |<span data-ttu-id="a9254-146">パブリック文字列を示します。</span><span class="sxs-lookup"><span data-stu-id="a9254-146">Indicates public strings.</span></span>  <br/> |
|<span data-ttu-id="a9254-147">Address</span><span class="sxs-lookup"><span data-stu-id="a9254-147">Address</span></span>  <br/> |<span data-ttu-id="a9254-148">アドレスを示します。</span><span class="sxs-lookup"><span data-stu-id="a9254-148">Indicates an address.</span></span>  <br/> |
|<span data-ttu-id="a9254-149">InternetHeaders</span><span class="sxs-lookup"><span data-stu-id="a9254-149">InternetHeaders</span></span>  <br/> |<span data-ttu-id="a9254-150">インターネットヘッダーを示します。</span><span class="sxs-lookup"><span data-stu-id="a9254-150">Indicates Internet headers.</span></span>  <br/> |
|<span data-ttu-id="a9254-151">CalendarAssistant</span><span class="sxs-lookup"><span data-stu-id="a9254-151">CalendarAssistant</span></span>  <br/> |<span data-ttu-id="a9254-152">カレンダーアシスタントを示します。</span><span class="sxs-lookup"><span data-stu-id="a9254-152">Indicates the Calendar Assistant.</span></span>  <br/> |
|<span data-ttu-id="a9254-153">UnifiedMessaging</span><span class="sxs-lookup"><span data-stu-id="a9254-153">UnifiedMessaging</span></span>  <br/> |<span data-ttu-id="a9254-154">ユニファイドメッセージングを示します。</span><span class="sxs-lookup"><span data-stu-id="a9254-154">Indicates Unified Messaging.</span></span>  <br/> |
|<span data-ttu-id="a9254-155">タスク</span><span class="sxs-lookup"><span data-stu-id="a9254-155">Task</span></span>  <br/> |<span data-ttu-id="a9254-156">タスクを示します。</span><span class="sxs-lookup"><span data-stu-id="a9254-156">Indicates a task.</span></span>  <br/> |
   
#### <a name="propertytype"></a><span data-ttu-id="a9254-157">Recordtype</span><span class="sxs-lookup"><span data-stu-id="a9254-157">PropertyType</span></span>

|<span data-ttu-id="a9254-158">**値**</span><span class="sxs-lookup"><span data-stu-id="a9254-158">**Value**</span></span>|<span data-ttu-id="a9254-159">**説明**</span><span class="sxs-lookup"><span data-stu-id="a9254-159">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a9254-160">ApplicationTime</span><span class="sxs-lookup"><span data-stu-id="a9254-160">ApplicationTime</span></span>  <br/> |<span data-ttu-id="a9254-161">アプリケーション時間を示します。</span><span class="sxs-lookup"><span data-stu-id="a9254-161">Indicates the application time.</span></span>  <br/> |
|<span data-ttu-id="a9254-162">ApplicationTimeArray</span><span class="sxs-lookup"><span data-stu-id="a9254-162">ApplicationTimeArray</span></span>  <br/> |<span data-ttu-id="a9254-163">アプリケーション時間の配列を示します。</span><span class="sxs-lookup"><span data-stu-id="a9254-163">Indicates an array of application times.</span></span>  <br/> |
|<span data-ttu-id="a9254-164">バイナリ</span><span class="sxs-lookup"><span data-stu-id="a9254-164">Binary</span></span>  <br/> |<span data-ttu-id="a9254-165">バイナリ値を示します。</span><span class="sxs-lookup"><span data-stu-id="a9254-165">Indicates a binary value.</span></span>  <br/> |
|<span data-ttu-id="a9254-166">BinaryArray</span><span class="sxs-lookup"><span data-stu-id="a9254-166">BinaryArray</span></span>  <br/> |<span data-ttu-id="a9254-167">バイナリ値の配列を示します。</span><span class="sxs-lookup"><span data-stu-id="a9254-167">Indicates an array of binary values.</span></span>  <br/> |
|<span data-ttu-id="a9254-168">ブール型</span><span class="sxs-lookup"><span data-stu-id="a9254-168">Boolean</span></span>  <br/> |<span data-ttu-id="a9254-169">ブール値を示します。</span><span class="sxs-lookup"><span data-stu-id="a9254-169">Indicates a Boolean value.</span></span>  <br/> |
|<span data-ttu-id="a9254-170">CLSID</span><span class="sxs-lookup"><span data-stu-id="a9254-170">CLSID</span></span>  <br/> |<span data-ttu-id="a9254-171">CLSID を示します。</span><span class="sxs-lookup"><span data-stu-id="a9254-171">Indicates a CLSID.</span></span>  <br/> |
|<span data-ttu-id="a9254-172">CLSIDArray</span><span class="sxs-lookup"><span data-stu-id="a9254-172">CLSIDArray</span></span>  <br/> |<span data-ttu-id="a9254-173">Clsid の配列を示します。</span><span class="sxs-lookup"><span data-stu-id="a9254-173">Indicates an array of CLSIDs.</span></span>  <br/> |
|<span data-ttu-id="a9254-174">通貨</span><span class="sxs-lookup"><span data-stu-id="a9254-174">Currency</span></span>  <br/> |<span data-ttu-id="a9254-175">通貨値を示します。</span><span class="sxs-lookup"><span data-stu-id="a9254-175">Indicates a currency value.</span></span>  <br/> |
|<span data-ttu-id="a9254-176">CurrencyArray</span><span class="sxs-lookup"><span data-stu-id="a9254-176">CurrencyArray</span></span>  <br/> |<span data-ttu-id="a9254-177">通貨値の配列を示します。</span><span class="sxs-lookup"><span data-stu-id="a9254-177">Indicates an array of currency values.</span></span>  <br/> |
|<span data-ttu-id="a9254-178">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="a9254-178">Double</span></span>  <br/> |<span data-ttu-id="a9254-179">**倍精度浮動小数点**型を示します。</span><span class="sxs-lookup"><span data-stu-id="a9254-179">Indicates a **double**.</span></span>  <br/> |
|<span data-ttu-id="a9254-180">DoubleArray</span><span class="sxs-lookup"><span data-stu-id="a9254-180">DoubleArray</span></span>  <br/> |<span data-ttu-id="a9254-181">**倍精度浮動小数点**型の値の配列を示します。</span><span class="sxs-lookup"><span data-stu-id="a9254-181">Indicates an array of **double** values.</span></span>  <br/> |
|<span data-ttu-id="a9254-182">Error</span><span class="sxs-lookup"><span data-stu-id="a9254-182">Error</span></span>  <br/> |<span data-ttu-id="a9254-183">エラーを示します。</span><span class="sxs-lookup"><span data-stu-id="a9254-183">Indicates an error.</span></span> <span data-ttu-id="a9254-184">これはエラーレポートのためのものです。</span><span class="sxs-lookup"><span data-stu-id="a9254-184">This is for error-reporting purposes.</span></span> <span data-ttu-id="a9254-185">制限で、または値を取得または設定するために使用することはできません。</span><span class="sxs-lookup"><span data-stu-id="a9254-185">It cannot be used in restrictions or for getting or setting values.</span></span>  <br/> |
|<span data-ttu-id="a9254-186">浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="a9254-186">Float</span></span>  <br/> |<span data-ttu-id="a9254-187">**Float**を示します。</span><span class="sxs-lookup"><span data-stu-id="a9254-187">Indicates a **float**.</span></span>  <br/> |
|<span data-ttu-id="a9254-188">FloatArray</span><span class="sxs-lookup"><span data-stu-id="a9254-188">FloatArray</span></span>  <br/> |<span data-ttu-id="a9254-189">**Float**値の配列を示します。</span><span class="sxs-lookup"><span data-stu-id="a9254-189">Indicates an array of **float** values.</span></span>  <br/> |
|<span data-ttu-id="a9254-190">整数</span><span class="sxs-lookup"><span data-stu-id="a9254-190">Integer</span></span>  <br/> |<span data-ttu-id="a9254-191">整数を示します。</span><span class="sxs-lookup"><span data-stu-id="a9254-191">Indicates an integer.</span></span>  <br/> |
|<span data-ttu-id="a9254-192">整数配列</span><span class="sxs-lookup"><span data-stu-id="a9254-192">IntegerArray</span></span>  <br/> |<span data-ttu-id="a9254-193">整数の配列を示します。</span><span class="sxs-lookup"><span data-stu-id="a9254-193">Indicates an array of integers.</span></span>  <br/> |
|<span data-ttu-id="a9254-194">Long</span><span class="sxs-lookup"><span data-stu-id="a9254-194">Long</span></span>  <br/> |<span data-ttu-id="a9254-195">**Long**を示します。</span><span class="sxs-lookup"><span data-stu-id="a9254-195">Indicates a **long**.</span></span>  <br/> |
|<span data-ttu-id="a9254-196">LongArray</span><span class="sxs-lookup"><span data-stu-id="a9254-196">LongArray</span></span>  <br/> |<span data-ttu-id="a9254-197">**長整数型 (long)** の値の配列を示します。</span><span class="sxs-lookup"><span data-stu-id="a9254-197">Indicates an array of **long** values.</span></span>  <br/> |
|<span data-ttu-id="a9254-198">Null</span><span class="sxs-lookup"><span data-stu-id="a9254-198">Null</span></span>  <br/> |<span data-ttu-id="a9254-199">Null 値を示します。</span><span class="sxs-lookup"><span data-stu-id="a9254-199">Indicates a null value.</span></span> <span data-ttu-id="a9254-200">これはエラーレポートのためのものです。</span><span class="sxs-lookup"><span data-stu-id="a9254-200">This is for error-reporting purposes.</span></span> <span data-ttu-id="a9254-201">制限で、または値を取得または設定するために使用することはできません。</span><span class="sxs-lookup"><span data-stu-id="a9254-201">It cannot be used in restrictions or for getting or setting values.</span></span>  <br/> |
|<span data-ttu-id="a9254-202">オブジェクト</span><span class="sxs-lookup"><span data-stu-id="a9254-202">Object</span></span>  <br/> |<span data-ttu-id="a9254-203">オブジェクトを示します。</span><span class="sxs-lookup"><span data-stu-id="a9254-203">Indicates an object.</span></span> <span data-ttu-id="a9254-204">これはエラーレポートのためのものです。</span><span class="sxs-lookup"><span data-stu-id="a9254-204">This is for error-reporting purposes.</span></span> <span data-ttu-id="a9254-205">制限で、または値を取得または設定するために使用することはできません。</span><span class="sxs-lookup"><span data-stu-id="a9254-205">It cannot be used in restrictions or for getting or setting values.</span></span>  <br/> |
|<span data-ttu-id="a9254-206">ObjectArray</span><span class="sxs-lookup"><span data-stu-id="a9254-206">ObjectArray</span></span>  <br/> |<span data-ttu-id="a9254-207">オブジェクトの配列を示します。</span><span class="sxs-lookup"><span data-stu-id="a9254-207">Indicates an array of objects.</span></span> <span data-ttu-id="a9254-208">これはエラーレポートのためのものです。</span><span class="sxs-lookup"><span data-stu-id="a9254-208">This is for error-reporting purposes.</span></span> <span data-ttu-id="a9254-209">制限で、または値を取得または設定するために使用することはできません。</span><span class="sxs-lookup"><span data-stu-id="a9254-209">It cannot be used in restrictions or for getting or setting values.</span></span>  <br/> |
|<span data-ttu-id="a9254-210">長い形式の日付 (スラッシュ区切り)</span><span class="sxs-lookup"><span data-stu-id="a9254-210">Short</span></span>  <br/> |<span data-ttu-id="a9254-211">**Short**を示します。</span><span class="sxs-lookup"><span data-stu-id="a9254-211">Indicates a **short**.</span></span>  <br/> |
|<span data-ttu-id="a9254-212">Short 配列</span><span class="sxs-lookup"><span data-stu-id="a9254-212">ShortArray</span></span>  <br/> |<span data-ttu-id="a9254-213">**Short**値の配列を示します。</span><span class="sxs-lookup"><span data-stu-id="a9254-213">Indicates an array of **short** values.</span></span>  <br/> |
|<span data-ttu-id="a9254-214">SystemTime</span><span class="sxs-lookup"><span data-stu-id="a9254-214">SystemTime</span></span>  <br/> |<span data-ttu-id="a9254-215">システム時間の値を示します。</span><span class="sxs-lookup"><span data-stu-id="a9254-215">Indicates a system time value.</span></span>  <br/> |
|<span data-ttu-id="a9254-216">SystemTimeArray</span><span class="sxs-lookup"><span data-stu-id="a9254-216">SystemTimeArray</span></span>  <br/> |<span data-ttu-id="a9254-217">システム時間の値の配列を示します。</span><span class="sxs-lookup"><span data-stu-id="a9254-217">Indicates an array of system time values.</span></span>  <br/> |
|<span data-ttu-id="a9254-218">文字列</span><span class="sxs-lookup"><span data-stu-id="a9254-218">String</span></span>  <br/> |<span data-ttu-id="a9254-219">文字列を示します。</span><span class="sxs-lookup"><span data-stu-id="a9254-219">Indicates a string.</span></span>  <br/> |
|<span data-ttu-id="a9254-220">StringArray</span><span class="sxs-lookup"><span data-stu-id="a9254-220">StringArray</span></span>  <br/> |<span data-ttu-id="a9254-221">文字列の配列を示します。</span><span class="sxs-lookup"><span data-stu-id="a9254-221">Indicates an array of strings.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="a9254-222">子要素</span><span class="sxs-lookup"><span data-stu-id="a9254-222">Child elements</span></span>

<span data-ttu-id="a9254-223">なし。</span><span class="sxs-lookup"><span data-stu-id="a9254-223">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a9254-224">親要素</span><span class="sxs-lookup"><span data-stu-id="a9254-224">Parent elements</span></span>

|<span data-ttu-id="a9254-225">**要素**</span><span class="sxs-lookup"><span data-stu-id="a9254-225">**Element**</span></span>|<span data-ttu-id="a9254-226">**説明**</span><span class="sxs-lookup"><span data-stu-id="a9254-226">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a9254-227">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="a9254-227">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="a9254-228">拡張 MAPI プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="a9254-228">Identifies an extended MAPI property.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a9254-229">注釈</span><span class="sxs-lookup"><span data-stu-id="a9254-229">Remarks</span></span>

<span data-ttu-id="a9254-230">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="a9254-230">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="a9254-231">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="a9254-231">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a9254-232">要素の情報</span><span class="sxs-lookup"><span data-stu-id="a9254-232">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a9254-233">Namespace</span><span class="sxs-lookup"><span data-stu-id="a9254-233">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a9254-234">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a9254-234">Schema Name</span></span>  <br/> |<span data-ttu-id="a9254-235">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="a9254-235">Type schema</span></span>  <br/> |
|<span data-ttu-id="a9254-236">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a9254-236">Validation File</span></span>  <br/> |<span data-ttu-id="a9254-237">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="a9254-237">types.xsd</span></span>  <br/> |
|<span data-ttu-id="a9254-238">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="a9254-238">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="a9254-239">関連項目</span><span class="sxs-lookup"><span data-stu-id="a9254-239">See also</span></span>

- [<span data-ttu-id="a9254-240">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="a9254-240">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

