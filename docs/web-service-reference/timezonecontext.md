---
title: TimeZoneContext
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TimeZoneContext
api_type:
- schema
ms.assetid: 573c462b-aa1d-4ba0-8852-e3f48b26873b
description: TimeZoneContext 要素は、簡易オブジェクトアクセスプロトコル (SOAP) ヘッダーで使用され、Exchange Web サービス (EWS) を使用して作成、更新、および取得されるオブジェクトの DateTime プロパティのタイムゾーンを割り当てるときに既定として使用されるタイムゾーン定義を指定します。
ms.openlocfilehash: 26727317ccf34338e8d62ec92bd7a44d43a6cfdb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460254"
---
# <a name="timezonecontext"></a><span data-ttu-id="71f40-103">TimeZoneContext</span><span class="sxs-lookup"><span data-stu-id="71f40-103">TimeZoneContext</span></span>

<span data-ttu-id="71f40-104">**TimeZoneContext**要素は、簡易オブジェクトアクセスプロトコル (SOAP) ヘッダーで使用され、Exchange Web サービス (EWS) を使用して作成、更新、および取得されるオブジェクトの DateTime プロパティのタイムゾーンを割り当てるときに既定として使用されるタイムゾーン定義を指定します。</span><span class="sxs-lookup"><span data-stu-id="71f40-104">The **TimeZoneContext** element is used in the Simple Object Access Protocol (SOAP) header to specify the time zone definition that is to be used as the default when assigning the time zone for the DateTime properties of objects that are created, updated, and retrieved by using Exchange Web Services (EWS).</span></span> 
  
```xml
<TimeZoneContext>
   <TimeZoneDefinition/>
</TimeZoneContext>
```

 <span data-ttu-id="71f40-105">**TimeZoneContextType**</span><span class="sxs-lookup"><span data-stu-id="71f40-105">**TimeZoneContextType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="71f40-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="71f40-106">Attributes and elements</span></span>

<span data-ttu-id="71f40-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="71f40-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="71f40-108">属性</span><span class="sxs-lookup"><span data-stu-id="71f40-108">Attributes</span></span>

<span data-ttu-id="71f40-109">なし。</span><span class="sxs-lookup"><span data-stu-id="71f40-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="71f40-110">子要素</span><span class="sxs-lookup"><span data-stu-id="71f40-110">Child elements</span></span>

|<span data-ttu-id="71f40-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="71f40-111">**Element**</span></span>|<span data-ttu-id="71f40-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="71f40-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="71f40-113">TimeZoneDefinition</span><span class="sxs-lookup"><span data-stu-id="71f40-113">TimeZoneDefinition</span></span>](timezonedefinition.md) <br/> |<span data-ttu-id="71f40-114">タイムゾーンを定義する期間と切り替えを指定します。</span><span class="sxs-lookup"><span data-stu-id="71f40-114">Specifies the periods and transitions that define a time zone.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="71f40-115">親要素</span><span class="sxs-lookup"><span data-stu-id="71f40-115">Parent elements</span></span>

<span data-ttu-id="71f40-116">なし。</span><span class="sxs-lookup"><span data-stu-id="71f40-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="71f40-117">注釈</span><span class="sxs-lookup"><span data-stu-id="71f40-117">Remarks</span></span>

<span data-ttu-id="71f40-118">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="71f40-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="71f40-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="71f40-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="71f40-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="71f40-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="71f40-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="71f40-121">Schema Name</span></span>  <br/> |<span data-ttu-id="71f40-122">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="71f40-122">Types schema</span></span>  <br/> |
|<span data-ttu-id="71f40-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="71f40-123">Validation File</span></span>  <br/> |<span data-ttu-id="71f40-124">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="71f40-124">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="71f40-125">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="71f40-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="71f40-126">正しくない</span><span class="sxs-lookup"><span data-stu-id="71f40-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="71f40-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="71f40-127">See also</span></span>



- [<span data-ttu-id="71f40-128">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="71f40-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

