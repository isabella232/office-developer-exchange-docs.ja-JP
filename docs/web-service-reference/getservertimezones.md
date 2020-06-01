---
title: GetServerTimeZones
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetServerTimeZones
api_type:
- schema
ms.assetid: 2a89098b-d89b-4d01-827b-50be00f7cbe9
description: GetServerTimeZones 要素は、Exchange サーバーからタイムゾーン定義を取得するための要求のルート要素です。
ms.openlocfilehash: 797e4543c94b0628242bcf544fe9a735ebaa5a63
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460940"
---
# <a name="getservertimezones"></a><span data-ttu-id="b901d-103">GetServerTimeZones</span><span class="sxs-lookup"><span data-stu-id="b901d-103">GetServerTimeZones</span></span>

<span data-ttu-id="b901d-104">**GetServerTimeZones**要素は、Exchange サーバーからタイムゾーン定義を取得するための要求のルート要素です。</span><span class="sxs-lookup"><span data-stu-id="b901d-104">The **GetServerTimeZones** element is the root element in a request to retrieve time zone definitions from the Exchange server.</span></span> 
  
```xml
<GetServerTimeZones ReturnFullTimeZoneData="">   <Ids/></GetServerTimeZones>
```

 <span data-ttu-id="b901d-105">**GetServerTimeZonesType**</span><span class="sxs-lookup"><span data-stu-id="b901d-105">**GetServerTimeZonesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b901d-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="b901d-106">Attributes and elements</span></span>

<span data-ttu-id="b901d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b901d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b901d-108">属性</span><span class="sxs-lookup"><span data-stu-id="b901d-108">Attributes</span></span>

|<span data-ttu-id="b901d-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="b901d-109">**Attribute**</span></span>|<span data-ttu-id="b901d-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="b901d-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b901d-111">**ReturnFullTimeZoneData**</span><span class="sxs-lookup"><span data-stu-id="b901d-111">**ReturnFullTimeZoneData**</span></span> <br/> |<span data-ttu-id="b901d-112">[GetServerTimeZones 操作](getservertimezones-operation.md)が、各タイムゾーンの完全な定義または名前と識別子のみを返すかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="b901d-112">Specifies whether the [GetServerTimeZones operation](getservertimezones-operation.md) returns the complete definition or only the name and identifier for each time zone.</span></span> <span data-ttu-id="b901d-113">この属性は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="b901d-113">This attribute is optional.</span></span> <span data-ttu-id="b901d-114">既定値は **true** です。</span><span class="sxs-lookup"><span data-stu-id="b901d-114">The default value is **true**.</span></span>  <br/> |
   
#### <a name="returnfulltimezonedata-attribute"></a><span data-ttu-id="b901d-115">ReturnFullTimeZoneData 属性</span><span class="sxs-lookup"><span data-stu-id="b901d-115">ReturnFullTimeZoneData Attribute</span></span>

|<span data-ttu-id="b901d-116">**値**</span><span class="sxs-lookup"><span data-stu-id="b901d-116">**Value**</span></span>|<span data-ttu-id="b901d-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="b901d-117">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b901d-118">**false**</span><span class="sxs-lookup"><span data-stu-id="b901d-118">**true**</span></span> <br/> |<span data-ttu-id="b901d-119">各タイムゾーンの完全な定義を返します。</span><span class="sxs-lookup"><span data-stu-id="b901d-119">Return the complete definitions for each time zone.</span></span>  <br/> |
|<span data-ttu-id="b901d-120">**false**</span><span class="sxs-lookup"><span data-stu-id="b901d-120">**false**</span></span> <br/> |<span data-ttu-id="b901d-121">各タイムゾーンの名前と識別子のみを返します。</span><span class="sxs-lookup"><span data-stu-id="b901d-121">Return only the name and identifier for each time zone.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="b901d-122">子要素</span><span class="sxs-lookup"><span data-stu-id="b901d-122">Child elements</span></span>

|<span data-ttu-id="b901d-123">**Element**</span><span class="sxs-lookup"><span data-stu-id="b901d-123">**Element**</span></span>|<span data-ttu-id="b901d-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="b901d-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b901d-125">Rid</span><span class="sxs-lookup"><span data-stu-id="b901d-125">Ids</span></span>](ids.md) <br/> |<span data-ttu-id="b901d-126">要求されたタイムゾーン定義を指定するタイムゾーン定義識別子の配列を含みます。</span><span class="sxs-lookup"><span data-stu-id="b901d-126">Contains an array of time zone definition identifiers that specifies the requested time zone definitions.</span></span> <span data-ttu-id="b901d-127">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="b901d-127">This element is optional.</span></span> <span data-ttu-id="b901d-128">この要素が[GetServerTimeZones 操作](getservertimezones-operation.md)要求に含まれていない場合、サーバー上で使用可能なすべてのタイムゾーン定義が応答で返されます。</span><span class="sxs-lookup"><span data-stu-id="b901d-128">If this element is not included in the [GetServerTimeZones operation](getservertimezones-operation.md) request, all time zone definitions that are available on the server are returned in the response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b901d-129">親要素</span><span class="sxs-lookup"><span data-stu-id="b901d-129">Parent elements</span></span>

<span data-ttu-id="b901d-130">なし。</span><span class="sxs-lookup"><span data-stu-id="b901d-130">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b901d-131">注釈</span><span class="sxs-lookup"><span data-stu-id="b901d-131">Remarks</span></span>

<span data-ttu-id="b901d-132">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="b901d-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b901d-133">要素の情報</span><span class="sxs-lookup"><span data-stu-id="b901d-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b901d-134">Namespace</span><span class="sxs-lookup"><span data-stu-id="b901d-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b901d-135">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b901d-135">Schema Name</span></span>  <br/> |<span data-ttu-id="b901d-136">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="b901d-136">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b901d-137">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b901d-137">Validation File</span></span>  <br/> |<span data-ttu-id="b901d-138">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="b901d-138">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b901d-139">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="b901d-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="b901d-140">正しくない</span><span class="sxs-lookup"><span data-stu-id="b901d-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b901d-141">関連項目</span><span class="sxs-lookup"><span data-stu-id="b901d-141">See also</span></span>



[<span data-ttu-id="b901d-142">GetServerTimeZones 操作</span><span class="sxs-lookup"><span data-stu-id="b901d-142">GetServerTimeZones operation</span></span>](getservertimezones-operation.md)
  
[<span data-ttu-id="b901d-143">GetServerTimeZonesResponse</span><span class="sxs-lookup"><span data-stu-id="b901d-143">GetServerTimeZonesResponse</span></span>](getservertimezonesresponse.md)


- [<span data-ttu-id="b901d-144">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="b901d-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

