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
description: GetServerTimeZones 要素は、Exchange サーバーからのタイム ゾーン定義を取得する要求のルート要素です。
ms.openlocfilehash: 1ad503ff312497189f57bce9a3670571aedad5ce
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760862"
---
# <a name="getservertimezones"></a><span data-ttu-id="82ae1-103">GetServerTimeZones</span><span class="sxs-lookup"><span data-stu-id="82ae1-103">GetServerTimeZones</span></span>

<span data-ttu-id="82ae1-104">**GetServerTimeZones**要素は、Exchange サーバーからのタイム ゾーン定義を取得する要求のルート要素です。</span><span class="sxs-lookup"><span data-stu-id="82ae1-104">The **GetServerTimeZones** element is the root element in a request to retrieve time zone definitions from the Exchange server.</span></span> 
  
```xml
<GetServerTimeZones ReturnFullTimeZoneData="">   <Ids/></GetServerTimeZones>
```

 <span data-ttu-id="82ae1-105">**GetServerTimeZonesType**</span><span class="sxs-lookup"><span data-stu-id="82ae1-105">**GetServerTimeZonesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="82ae1-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="82ae1-106">Attributes and elements</span></span>

<span data-ttu-id="82ae1-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="82ae1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="82ae1-108">属性</span><span class="sxs-lookup"><span data-stu-id="82ae1-108">Attributes</span></span>

|<span data-ttu-id="82ae1-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="82ae1-109">**Attribute**</span></span>|<span data-ttu-id="82ae1-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="82ae1-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="82ae1-111">**ReturnFullTimeZoneData**</span><span class="sxs-lookup"><span data-stu-id="82ae1-111">**ReturnFullTimeZoneData**</span></span> <br/> |<span data-ttu-id="82ae1-112">[GetServerTimeZones 操作](getservertimezones-operation.md)が完全な定義のみの名前や各タイム ゾーンの識別子を返すかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="82ae1-112">Specifies whether the [GetServerTimeZones operation](getservertimezones-operation.md) returns the complete definition or only the name and identifier for each time zone.</span></span> <span data-ttu-id="82ae1-113">この属性は、省略可能です。</span><span class="sxs-lookup"><span data-stu-id="82ae1-113">This attribute is optional.</span></span> <span data-ttu-id="82ae1-114">既定値は、 **true を指定**します。</span><span class="sxs-lookup"><span data-stu-id="82ae1-114">The default value is **true**.</span></span>  <br/> |
   
#### <a name="returnfulltimezonedata-attribute"></a><span data-ttu-id="82ae1-115">ReturnFullTimeZoneData 属性</span><span class="sxs-lookup"><span data-stu-id="82ae1-115">ReturnFullTimeZoneData Attribute</span></span>

|<span data-ttu-id="82ae1-116">**値**</span><span class="sxs-lookup"><span data-stu-id="82ae1-116">**Value**</span></span>|<span data-ttu-id="82ae1-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="82ae1-117">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="82ae1-118">**true**</span><span class="sxs-lookup"><span data-stu-id="82ae1-118">**true**</span></span> <br/> |<span data-ttu-id="82ae1-119">各タイム ゾーンの完全な定義を返します。</span><span class="sxs-lookup"><span data-stu-id="82ae1-119">Return the complete definitions for each time zone.</span></span>  <br/> |
|<span data-ttu-id="82ae1-120">**false**</span><span class="sxs-lookup"><span data-stu-id="82ae1-120">**false**</span></span> <br/> |<span data-ttu-id="82ae1-121">名と各タイム ゾーンの識別子を返します。</span><span class="sxs-lookup"><span data-stu-id="82ae1-121">Return only the name and identifier for each time zone.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="82ae1-122">子要素</span><span class="sxs-lookup"><span data-stu-id="82ae1-122">Child elements</span></span>

|<span data-ttu-id="82ae1-123">**要素**</span><span class="sxs-lookup"><span data-stu-id="82ae1-123">**Element**</span></span>|<span data-ttu-id="82ae1-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="82ae1-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="82ae1-125">Id</span><span class="sxs-lookup"><span data-stu-id="82ae1-125">Ids</span></span>](ids.md) <br/> |<span data-ttu-id="82ae1-126">要求されたタイム ゾーン定義を指定するタイム ゾーン定義の識別子の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="82ae1-126">Contains an array of time zone definition identifiers that specifies the requested time zone definitions.</span></span> <span data-ttu-id="82ae1-127">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="82ae1-127">This element is optional.</span></span> <span data-ttu-id="82ae1-128">[GetServerTimeZones 操作](getservertimezones-operation.md)の要求には、この要素が含まれていない、サーバーで利用可能なすべてのタイム ゾーン定義が応答で返されます。</span><span class="sxs-lookup"><span data-stu-id="82ae1-128">If this element is not included in the [GetServerTimeZones operation](getservertimezones-operation.md) request, all time zone definitions that are available on the server are returned in the response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="82ae1-129">親要素</span><span class="sxs-lookup"><span data-stu-id="82ae1-129">Parent elements</span></span>

<span data-ttu-id="82ae1-130">なし。</span><span class="sxs-lookup"><span data-stu-id="82ae1-130">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="82ae1-131">備考</span><span class="sxs-lookup"><span data-stu-id="82ae1-131">Remarks</span></span>

<span data-ttu-id="82ae1-132">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="82ae1-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="82ae1-133">要素情報</span><span class="sxs-lookup"><span data-stu-id="82ae1-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="82ae1-134">名前空間</span><span class="sxs-lookup"><span data-stu-id="82ae1-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="82ae1-135">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="82ae1-135">Schema Name</span></span>  <br/> |<span data-ttu-id="82ae1-136">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="82ae1-136">Messages schema</span></span>  <br/> |
|<span data-ttu-id="82ae1-137">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="82ae1-137">Validation File</span></span>  <br/> |<span data-ttu-id="82ae1-138">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="82ae1-138">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="82ae1-139">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="82ae1-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="82ae1-140">False</span><span class="sxs-lookup"><span data-stu-id="82ae1-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="82ae1-141">関連項目</span><span class="sxs-lookup"><span data-stu-id="82ae1-141">See also</span></span>



[<span data-ttu-id="82ae1-142">GetServerTimeZones 操作</span><span class="sxs-lookup"><span data-stu-id="82ae1-142">GetServerTimeZones operation</span></span>](getservertimezones-operation.md)
  
[<span data-ttu-id="82ae1-143">GetServerTimeZonesResponse</span><span class="sxs-lookup"><span data-stu-id="82ae1-143">GetServerTimeZonesResponse</span></span>](getservertimezonesresponse.md)


- [<span data-ttu-id="82ae1-144">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="82ae1-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

