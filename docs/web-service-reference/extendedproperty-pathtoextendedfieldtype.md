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
ms.openlocfilehash: 7541fa6330ee96f7791febfabc672dbcf0e95b54
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760419"
---
# <a name="extendedproperty-pathtoextendedfieldtype"></a><span data-ttu-id="63576-103">ExtendedProperty (PathToExtendedFieldType)</span><span class="sxs-lookup"><span data-stu-id="63576-103">ExtendedProperty (PathToExtendedFieldType)</span></span>

<span data-ttu-id="63576-104">**ExtendedProperty**要素は、統合連絡先ストアの拡張プロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="63576-104">The **ExtendedProperty** element specifies an extended property for the Unified Contact Store.</span></span> 
  
```xml
<ExtendedProperty DistinguishedPropertySetId="" PropertySetId="" PropertyTag="" PropertyName="" PropertyId="" PropertyType="" FieldURI="">
</ExtendedProperty>
```

<span data-ttu-id="63576-105">**PathToExtendedFieldType**</span><span class="sxs-lookup"><span data-stu-id="63576-105">**PathToExtendedFieldType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="63576-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="63576-106">Attributes and elements</span></span>

<span data-ttu-id="63576-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="63576-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="63576-108">属性</span><span class="sxs-lookup"><span data-stu-id="63576-108">Attributes</span></span>

|<span data-ttu-id="63576-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="63576-109">**Attribute**</span></span>|<span data-ttu-id="63576-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="63576-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="63576-111">DistinguishedPropertySetId</span><span class="sxs-lookup"><span data-stu-id="63576-111">DistinguishedPropertySetId</span></span>  <br/> |<span data-ttu-id="63576-112">識別プロパティ セットの識別子を示します。</span><span class="sxs-lookup"><span data-stu-id="63576-112">Indicates the distinguished property set identifier.</span></span> <span data-ttu-id="63576-113">この属性は、省略可能です。</span><span class="sxs-lookup"><span data-stu-id="63576-113">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="63576-114">PropertySetId</span><span class="sxs-lookup"><span data-stu-id="63576-114">PropertySetId</span></span>  <br/> |<span data-ttu-id="63576-115">GUID プロパティ セットの識別子を示します。</span><span class="sxs-lookup"><span data-stu-id="63576-115">Indicates the GUID property set identifier.</span></span> <span data-ttu-id="63576-116">この属性は、省略可能です。</span><span class="sxs-lookup"><span data-stu-id="63576-116">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="63576-117">PropertyTag</span><span class="sxs-lookup"><span data-stu-id="63576-117">PropertyTag</span></span>  <br/> | <span data-ttu-id="63576-118">型部分を差し引いたプロパティ タグを表します。</span><span class="sxs-lookup"><span data-stu-id="63576-118">Represents the property tag minus the type part.</span></span><br/><br/><span data-ttu-id="63576-119">表現の 2 つのオプションがあります。</span><span class="sxs-lookup"><span data-stu-id="63576-119">There are two options for representation:</span></span>  <br/><br/><span data-ttu-id="63576-120">-16 進数: 0x3fa4</span><span class="sxs-lookup"><span data-stu-id="63576-120">-  Hexadecimal: 0x3fa4</span></span>  <br/><span data-ttu-id="63576-121">0 ~ 65535 の 10 進数。</span><span class="sxs-lookup"><span data-stu-id="63576-121">-  Decimal: 0-65535</span></span><br/><br/>  <span data-ttu-id="63576-122">この属性は、省略可能です。</span><span class="sxs-lookup"><span data-stu-id="63576-122">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="63576-123">PropertyName</span><span class="sxs-lookup"><span data-stu-id="63576-123">PropertyName</span></span>  <br/> |<span data-ttu-id="63576-124">プロパティ名を示す文字列です。</span><span class="sxs-lookup"><span data-stu-id="63576-124">String that indicates the property name.</span></span> <span data-ttu-id="63576-125">この属性は、省略可能です。</span><span class="sxs-lookup"><span data-stu-id="63576-125">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="63576-126">PropertyId</span><span class="sxs-lookup"><span data-stu-id="63576-126">PropertyId</span></span>  <br/> |<span data-ttu-id="63576-127">プロパティの識別子を示す整数。</span><span class="sxs-lookup"><span data-stu-id="63576-127">Integer that indicates the property identifier.</span></span> <span data-ttu-id="63576-128">この属性は、省略可能です。</span><span class="sxs-lookup"><span data-stu-id="63576-128">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="63576-129">PropertyType</span><span class="sxs-lookup"><span data-stu-id="63576-129">PropertyType</span></span>  <br/> |<span data-ttu-id="63576-130">プロパティの型を示します。</span><span class="sxs-lookup"><span data-stu-id="63576-130">Indicates the property type.</span></span> <span data-ttu-id="63576-131">この属性は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="63576-131">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="63576-132">FieldURI</span><span class="sxs-lookup"><span data-stu-id="63576-132">FieldURI</span></span>  <br/> |<span data-ttu-id="63576-133">統一リソース識別子 (URI) のフィールドを示します。</span><span class="sxs-lookup"><span data-stu-id="63576-133">Indicates the field Uniform Resource Identifier (URI).</span></span> <span data-ttu-id="63576-134">この属性は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="63576-134">This attribute is required.</span></span> <span data-ttu-id="63576-135">使用可能な値は、 [FieldURI](fielduri.md)要素を参照してください。</span><span class="sxs-lookup"><span data-stu-id="63576-135">For possible values, see the [FieldURI](fielduri.md) element.</span></span>  <br/> |
   
#### <a name="distinguishedpropertysetid"></a><span data-ttu-id="63576-136">DistinguishedPropertySetId</span><span class="sxs-lookup"><span data-stu-id="63576-136">DistinguishedPropertySetId</span></span>

|<span data-ttu-id="63576-137">**値**</span><span class="sxs-lookup"><span data-stu-id="63576-137">**Value**</span></span>|<span data-ttu-id="63576-138">**説明**</span><span class="sxs-lookup"><span data-stu-id="63576-138">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="63576-139">会議</span><span class="sxs-lookup"><span data-stu-id="63576-139">Meeting</span></span>  <br/> |<span data-ttu-id="63576-140">会議を示しています。</span><span class="sxs-lookup"><span data-stu-id="63576-140">Indicates a meeting.</span></span>  <br/> |
|<span data-ttu-id="63576-141">Appointment</span><span class="sxs-lookup"><span data-stu-id="63576-141">Appointment</span></span>  <br/> |<span data-ttu-id="63576-142">予定を示します。</span><span class="sxs-lookup"><span data-stu-id="63576-142">Indicates an appointment.</span></span>  <br/> |
|<span data-ttu-id="63576-143">Common</span><span class="sxs-lookup"><span data-stu-id="63576-143">Common</span></span>  <br/> |<span data-ttu-id="63576-144">共通のプロパティ セットを示します。</span><span class="sxs-lookup"><span data-stu-id="63576-144">Indicates the common property set.</span></span>  <br/> |
|<span data-ttu-id="63576-145">PublicStrings</span><span class="sxs-lookup"><span data-stu-id="63576-145">PublicStrings</span></span>  <br/> |<span data-ttu-id="63576-146">パブリック文字列を示します。</span><span class="sxs-lookup"><span data-stu-id="63576-146">Indicates public strings.</span></span>  <br/> |
|<span data-ttu-id="63576-147">Address</span><span class="sxs-lookup"><span data-stu-id="63576-147">Address</span></span>  <br/> |<span data-ttu-id="63576-148">アドレスを示します。</span><span class="sxs-lookup"><span data-stu-id="63576-148">Indicates an address.</span></span>  <br/> |
|<span data-ttu-id="63576-149">InternetHeaders</span><span class="sxs-lookup"><span data-stu-id="63576-149">InternetHeaders</span></span>  <br/> |<span data-ttu-id="63576-150">インターネット ヘッダーを示します。</span><span class="sxs-lookup"><span data-stu-id="63576-150">Indicates Internet headers.</span></span>  <br/> |
|<span data-ttu-id="63576-151">CalendarAssistant</span><span class="sxs-lookup"><span data-stu-id="63576-151">CalendarAssistant</span></span>  <br/> |<span data-ttu-id="63576-152">予定表のアシスタントを示します。</span><span class="sxs-lookup"><span data-stu-id="63576-152">Indicates the Calendar Assistant.</span></span>  <br/> |
|<span data-ttu-id="63576-153">UnifiedMessaging</span><span class="sxs-lookup"><span data-stu-id="63576-153">UnifiedMessaging</span></span>  <br/> |<span data-ttu-id="63576-154">ユニファイド メッセージングを示します。</span><span class="sxs-lookup"><span data-stu-id="63576-154">Indicates Unified Messaging.</span></span>  <br/> |
|<span data-ttu-id="63576-155">タスク</span><span class="sxs-lookup"><span data-stu-id="63576-155">Task</span></span>  <br/> |<span data-ttu-id="63576-156">タスクを示します。</span><span class="sxs-lookup"><span data-stu-id="63576-156">Indicates a task.</span></span>  <br/> |
   
#### <a name="propertytype"></a><span data-ttu-id="63576-157">PropertyType</span><span class="sxs-lookup"><span data-stu-id="63576-157">PropertyType</span></span>

|<span data-ttu-id="63576-158">**値**</span><span class="sxs-lookup"><span data-stu-id="63576-158">**Value**</span></span>|<span data-ttu-id="63576-159">**説明**</span><span class="sxs-lookup"><span data-stu-id="63576-159">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="63576-160">ApplicationTime</span><span class="sxs-lookup"><span data-stu-id="63576-160">ApplicationTime</span></span>  <br/> |<span data-ttu-id="63576-161">アプリケーション時刻を示します。</span><span class="sxs-lookup"><span data-stu-id="63576-161">Indicates the application time.</span></span>  <br/> |
|<span data-ttu-id="63576-162">ApplicationTimeArray</span><span class="sxs-lookup"><span data-stu-id="63576-162">ApplicationTimeArray</span></span>  <br/> |<span data-ttu-id="63576-163">アプリケーション時間の配列を示します。</span><span class="sxs-lookup"><span data-stu-id="63576-163">Indicates an array of application times.</span></span>  <br/> |
|<span data-ttu-id="63576-164">バイナリ型 (Binary)</span><span class="sxs-lookup"><span data-stu-id="63576-164">Binary</span></span>  <br/> |<span data-ttu-id="63576-165">バイナリ値を示します。</span><span class="sxs-lookup"><span data-stu-id="63576-165">Indicates a binary value.</span></span>  <br/> |
|<span data-ttu-id="63576-166">BinaryArray</span><span class="sxs-lookup"><span data-stu-id="63576-166">BinaryArray</span></span>  <br/> |<span data-ttu-id="63576-167">バイナリ値の配列を示します。</span><span class="sxs-lookup"><span data-stu-id="63576-167">Indicates an array of binary values.</span></span>  <br/> |
|<span data-ttu-id="63576-168">ブール型</span><span class="sxs-lookup"><span data-stu-id="63576-168">Boolean</span></span>  <br/> |<span data-ttu-id="63576-169">ブール値を示します。</span><span class="sxs-lookup"><span data-stu-id="63576-169">Indicates a Boolean value.</span></span>  <br/> |
|<span data-ttu-id="63576-170">CLSID</span><span class="sxs-lookup"><span data-stu-id="63576-170">CLSID</span></span>  <br/> |<span data-ttu-id="63576-171">CLSID を指定します。</span><span class="sxs-lookup"><span data-stu-id="63576-171">Indicates a CLSID.</span></span>  <br/> |
|<span data-ttu-id="63576-172">CLSIDArray</span><span class="sxs-lookup"><span data-stu-id="63576-172">CLSIDArray</span></span>  <br/> |<span data-ttu-id="63576-173">Clsid の配列を示します。</span><span class="sxs-lookup"><span data-stu-id="63576-173">Indicates an array of CLSIDs.</span></span>  <br/> |
|<span data-ttu-id="63576-174">通貨型 (Currency)</span><span class="sxs-lookup"><span data-stu-id="63576-174">Currency</span></span>  <br/> |<span data-ttu-id="63576-175">通貨値を示します。</span><span class="sxs-lookup"><span data-stu-id="63576-175">Indicates a currency value.</span></span>  <br/> |
|<span data-ttu-id="63576-176">CurrencyArray</span><span class="sxs-lookup"><span data-stu-id="63576-176">CurrencyArray</span></span>  <br/> |<span data-ttu-id="63576-177">通貨の値の配列を示します。</span><span class="sxs-lookup"><span data-stu-id="63576-177">Indicates an array of currency values.</span></span>  <br/> |
|<span data-ttu-id="63576-178">倍精度浮動小数点型 (Double)</span><span class="sxs-lookup"><span data-stu-id="63576-178">Double</span></span>  <br/> |<span data-ttu-id="63576-179">**二重**のことを示します。</span><span class="sxs-lookup"><span data-stu-id="63576-179">Indicates a **double**.</span></span>  <br/> |
|<span data-ttu-id="63576-180">DoubleArray</span><span class="sxs-lookup"><span data-stu-id="63576-180">DoubleArray</span></span>  <br/> |<span data-ttu-id="63576-181">**Double**値の配列を示します。</span><span class="sxs-lookup"><span data-stu-id="63576-181">Indicates an array of **double** values.</span></span>  <br/> |
|<span data-ttu-id="63576-182">エラー</span><span class="sxs-lookup"><span data-stu-id="63576-182">Error</span></span>  <br/> |<span data-ttu-id="63576-183">エラーを示します。</span><span class="sxs-lookup"><span data-stu-id="63576-183">Indicates an error.</span></span> <span data-ttu-id="63576-184">これは、エラー報告用です。</span><span class="sxs-lookup"><span data-stu-id="63576-184">This is for error-reporting purposes.</span></span> <span data-ttu-id="63576-185">制限や値の設定を取得または使用できません。</span><span class="sxs-lookup"><span data-stu-id="63576-185">It cannot be used in restrictions or for getting or setting values.</span></span>  <br/> |
|<span data-ttu-id="63576-186">浮動小数点型 (Float)</span><span class="sxs-lookup"><span data-stu-id="63576-186">Float</span></span>  <br/> |<span data-ttu-id="63576-187">**浮動小数点数**を示します。</span><span class="sxs-lookup"><span data-stu-id="63576-187">Indicates a **float**.</span></span>  <br/> |
|<span data-ttu-id="63576-188">FloatArray</span><span class="sxs-lookup"><span data-stu-id="63576-188">FloatArray</span></span>  <br/> |<span data-ttu-id="63576-189">**Float**値の配列を示します。</span><span class="sxs-lookup"><span data-stu-id="63576-189">Indicates an array of **float** values.</span></span>  <br/> |
|<span data-ttu-id="63576-190">整数型 (Integer)</span><span class="sxs-lookup"><span data-stu-id="63576-190">Integer</span></span>  <br/> |<span data-ttu-id="63576-191">整数を示します。</span><span class="sxs-lookup"><span data-stu-id="63576-191">Indicates an integer.</span></span>  <br/> |
|<span data-ttu-id="63576-192">IntegerArray</span><span class="sxs-lookup"><span data-stu-id="63576-192">IntegerArray</span></span>  <br/> |<span data-ttu-id="63576-193">整数の配列を示します。</span><span class="sxs-lookup"><span data-stu-id="63576-193">Indicates an array of integers.</span></span>  <br/> |
|<span data-ttu-id="63576-194">Long 型 (Long)</span><span class="sxs-lookup"><span data-stu-id="63576-194">Long</span></span>  <br/> |<span data-ttu-id="63576-195">**長い**ことを示します。</span><span class="sxs-lookup"><span data-stu-id="63576-195">Indicates a **long**.</span></span>  <br/> |
|<span data-ttu-id="63576-196">LongArray</span><span class="sxs-lookup"><span data-stu-id="63576-196">LongArray</span></span>  <br/> |<span data-ttu-id="63576-197">**Long**値の配列を示します。</span><span class="sxs-lookup"><span data-stu-id="63576-197">Indicates an array of **long** values.</span></span>  <br/> |
|<span data-ttu-id="63576-198">Null</span><span class="sxs-lookup"><span data-stu-id="63576-198">Null</span></span>  <br/> |<span data-ttu-id="63576-199">Null 値を示します。</span><span class="sxs-lookup"><span data-stu-id="63576-199">Indicates a null value.</span></span> <span data-ttu-id="63576-200">これは、エラー報告用です。</span><span class="sxs-lookup"><span data-stu-id="63576-200">This is for error-reporting purposes.</span></span> <span data-ttu-id="63576-201">制限や値の設定を取得または使用できません。</span><span class="sxs-lookup"><span data-stu-id="63576-201">It cannot be used in restrictions or for getting or setting values.</span></span>  <br/> |
|<span data-ttu-id="63576-202">オブジェクト</span><span class="sxs-lookup"><span data-stu-id="63576-202">Object</span></span>  <br/> |<span data-ttu-id="63576-203">オブジェクトを示します。</span><span class="sxs-lookup"><span data-stu-id="63576-203">Indicates an object.</span></span> <span data-ttu-id="63576-204">これは、エラー報告用です。</span><span class="sxs-lookup"><span data-stu-id="63576-204">This is for error-reporting purposes.</span></span> <span data-ttu-id="63576-205">制限や値の設定を取得または使用できません。</span><span class="sxs-lookup"><span data-stu-id="63576-205">It cannot be used in restrictions or for getting or setting values.</span></span>  <br/> |
|<span data-ttu-id="63576-206">ObjectArray</span><span class="sxs-lookup"><span data-stu-id="63576-206">ObjectArray</span></span>  <br/> |<span data-ttu-id="63576-207">オブジェクトの配列を示します。</span><span class="sxs-lookup"><span data-stu-id="63576-207">Indicates an array of objects.</span></span> <span data-ttu-id="63576-208">これは、エラー報告用です。</span><span class="sxs-lookup"><span data-stu-id="63576-208">This is for error-reporting purposes.</span></span> <span data-ttu-id="63576-209">制限や値の設定を取得または使用できません。</span><span class="sxs-lookup"><span data-stu-id="63576-209">It cannot be used in restrictions or for getting or setting values.</span></span>  <br/> |
|<span data-ttu-id="63576-210">長い形式の日付 (スラッシュ区切り)</span><span class="sxs-lookup"><span data-stu-id="63576-210">Short</span></span>  <br/> |<span data-ttu-id="63576-211">**短い**ことを示します。</span><span class="sxs-lookup"><span data-stu-id="63576-211">Indicates a **short**.</span></span>  <br/> |
|<span data-ttu-id="63576-212">ShortArray</span><span class="sxs-lookup"><span data-stu-id="63576-212">ShortArray</span></span>  <br/> |<span data-ttu-id="63576-213">**Short**値の配列を示します。</span><span class="sxs-lookup"><span data-stu-id="63576-213">Indicates an array of **short** values.</span></span>  <br/> |
|<span data-ttu-id="63576-214">SystemTime</span><span class="sxs-lookup"><span data-stu-id="63576-214">SystemTime</span></span>  <br/> |<span data-ttu-id="63576-215">システム時刻の値を示します。</span><span class="sxs-lookup"><span data-stu-id="63576-215">Indicates a system time value.</span></span>  <br/> |
|<span data-ttu-id="63576-216">SystemTimeArray</span><span class="sxs-lookup"><span data-stu-id="63576-216">SystemTimeArray</span></span>  <br/> |<span data-ttu-id="63576-217">システム時刻の値の配列を示します。</span><span class="sxs-lookup"><span data-stu-id="63576-217">Indicates an array of system time values.</span></span>  <br/> |
|<span data-ttu-id="63576-218">String</span><span class="sxs-lookup"><span data-stu-id="63576-218">String</span></span>  <br/> |<span data-ttu-id="63576-219">文字列を示します。</span><span class="sxs-lookup"><span data-stu-id="63576-219">Indicates a string.</span></span>  <br/> |
|<span data-ttu-id="63576-220">自己責任で使用</span><span class="sxs-lookup"><span data-stu-id="63576-220">StringArray</span></span>  <br/> |<span data-ttu-id="63576-221">文字列の配列を示します。</span><span class="sxs-lookup"><span data-stu-id="63576-221">Indicates an array of strings.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="63576-222">子要素</span><span class="sxs-lookup"><span data-stu-id="63576-222">Child elements</span></span>

<span data-ttu-id="63576-223">なし。</span><span class="sxs-lookup"><span data-stu-id="63576-223">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="63576-224">親要素</span><span class="sxs-lookup"><span data-stu-id="63576-224">Parent elements</span></span>

|<span data-ttu-id="63576-225">**要素**</span><span class="sxs-lookup"><span data-stu-id="63576-225">**Element**</span></span>|<span data-ttu-id="63576-226">**説明**</span><span class="sxs-lookup"><span data-stu-id="63576-226">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="63576-227">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="63576-227">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="63576-228">拡張 MAPI プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="63576-228">Identifies an extended MAPI property.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="63576-229">備考</span><span class="sxs-lookup"><span data-stu-id="63576-229">Remarks</span></span>

<span data-ttu-id="63576-230">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="63576-230">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="63576-231">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="63576-231">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="63576-232">要素情報</span><span class="sxs-lookup"><span data-stu-id="63576-232">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="63576-233">名前空間</span><span class="sxs-lookup"><span data-stu-id="63576-233">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="63576-234">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="63576-234">Schema Name</span></span>  <br/> |<span data-ttu-id="63576-235">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="63576-235">Type schema</span></span>  <br/> |
|<span data-ttu-id="63576-236">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="63576-236">Validation File</span></span>  <br/> |<span data-ttu-id="63576-237">types.xsd</span><span class="sxs-lookup"><span data-stu-id="63576-237">types.xsd</span></span>  <br/> |
|<span data-ttu-id="63576-238">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="63576-238">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="63576-239">関連項目</span><span class="sxs-lookup"><span data-stu-id="63576-239">See also</span></span>

- [<span data-ttu-id="63576-240">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="63576-240">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

