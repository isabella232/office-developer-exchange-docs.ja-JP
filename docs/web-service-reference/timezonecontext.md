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
description: Simple Object Access Protocol (SOAP) ヘッダーで、DateTime オブジェクトのプロパティを作成、更新、および取得のタイム ゾーンを割り当てるときに既定値として使用されるタイム ゾーン定義を指定する TimeZoneContext 要素が使用されます。Exchange Web サービス (EWS) を使用します。
ms.openlocfilehash: 38b7ab4c587adac45fc3bcf351f417ea72313a97
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839703"
---
# <a name="timezonecontext"></a><span data-ttu-id="d0473-103">TimeZoneContext</span><span class="sxs-lookup"><span data-stu-id="d0473-103">TimeZoneContext</span></span>

<span data-ttu-id="d0473-104">、更新、作成されたオブジェクトの日付プロパティのタイム ゾーンを割り当てるときに既定値として使用されるタイム ゾーンの定義を指定するのには、Simple Object Access Protocol (SOAP) ヘッダーに**TimeZoneContext**要素を使用し、Exchange Web サービス (EWS) を使用して取得します。</span><span class="sxs-lookup"><span data-stu-id="d0473-104">The **TimeZoneContext** element is used in the Simple Object Access Protocol (SOAP) header to specify the time zone definition that is to be used as the default when assigning the time zone for the DateTime properties of objects that are created, updated, and retrieved by using Exchange Web Services (EWS).</span></span> 
  
```xml
<TimeZoneContext>
   <TimeZoneDefinition/>
</TimeZoneContext>
```

 <span data-ttu-id="d0473-105">**TimeZoneContextType**</span><span class="sxs-lookup"><span data-stu-id="d0473-105">**TimeZoneContextType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d0473-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="d0473-106">Attributes and elements</span></span>

<span data-ttu-id="d0473-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d0473-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d0473-108">属性</span><span class="sxs-lookup"><span data-stu-id="d0473-108">Attributes</span></span>

<span data-ttu-id="d0473-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d0473-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d0473-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d0473-110">Child elements</span></span>

|<span data-ttu-id="d0473-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="d0473-111">**Element**</span></span>|<span data-ttu-id="d0473-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="d0473-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d0473-113">タイム</span><span class="sxs-lookup"><span data-stu-id="d0473-113">TimeZoneDefinition</span></span>](timezonedefinition.md) <br/> |<span data-ttu-id="d0473-114">期間とタイム ゾーンを定義するための遷移を指定します。</span><span class="sxs-lookup"><span data-stu-id="d0473-114">Specifies the periods and transitions that define a time zone.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d0473-115">親要素</span><span class="sxs-lookup"><span data-stu-id="d0473-115">Parent elements</span></span>

<span data-ttu-id="d0473-116">なし。</span><span class="sxs-lookup"><span data-stu-id="d0473-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d0473-117">備考</span><span class="sxs-lookup"><span data-stu-id="d0473-117">Remarks</span></span>

<span data-ttu-id="d0473-118">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="d0473-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d0473-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="d0473-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d0473-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="d0473-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d0473-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d0473-121">Schema Name</span></span>  <br/> |<span data-ttu-id="d0473-122">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="d0473-122">Types schema</span></span>  <br/> |
|<span data-ttu-id="d0473-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d0473-123">Validation File</span></span>  <br/> |<span data-ttu-id="d0473-124">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d0473-124">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d0473-125">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d0473-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="d0473-126">False</span><span class="sxs-lookup"><span data-stu-id="d0473-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d0473-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="d0473-127">See also</span></span>



- [<span data-ttu-id="d0473-128">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="d0473-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

