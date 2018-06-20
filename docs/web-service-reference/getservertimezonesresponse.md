---
title: GetServerTimeZonesResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetServerTimeZonesResponse
api_type:
- schema
ms.assetid: 97c94d32-10f1-4c3e-ab20-9fd7e8257e50
description: GetServerTimeZonesResponse 要素は、GetServerTimeZones 操作の要求に対する応答を定義します。
ms.openlocfilehash: 119809076c82ff75a6dd061fc976f861e13f4e57
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831664"
---
# <a name="getservertimezonesresponse"></a><span data-ttu-id="dbdc9-103">GetServerTimeZonesResponse</span><span class="sxs-lookup"><span data-stu-id="dbdc9-103">GetServerTimeZonesResponse</span></span>

<span data-ttu-id="dbdc9-104">**GetServerTimeZonesResponse**要素は、 [GetServerTimeZones 操作](getservertimezones-operation.md)の要求に対する応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="dbdc9-104">The **GetServerTimeZonesResponse** element defines a response to a [GetServerTimeZones operation](getservertimezones-operation.md) request.</span></span> 
  
```XML
<GetServerTimeZonesResponse>
   <ResponseMessages/>
</GetServerTimeZonesResponse>
```

 <span data-ttu-id="dbdc9-105">**GetServerTimeZonesResponseType**</span><span class="sxs-lookup"><span data-stu-id="dbdc9-105">**GetServerTimeZonesResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dbdc9-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="dbdc9-106">Attributes and elements</span></span>

<span data-ttu-id="dbdc9-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="dbdc9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dbdc9-108">属性</span><span class="sxs-lookup"><span data-stu-id="dbdc9-108">Attributes</span></span>

<span data-ttu-id="dbdc9-109">なし。</span><span class="sxs-lookup"><span data-stu-id="dbdc9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dbdc9-110">子要素</span><span class="sxs-lookup"><span data-stu-id="dbdc9-110">Child elements</span></span>

|<span data-ttu-id="dbdc9-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="dbdc9-111">**Element**</span></span>|<span data-ttu-id="dbdc9-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="dbdc9-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dbdc9-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="dbdc9-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="dbdc9-114">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="dbdc9-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="dbdc9-115">親要素</span><span class="sxs-lookup"><span data-stu-id="dbdc9-115">Parent elements</span></span>

<span data-ttu-id="dbdc9-116">なし。</span><span class="sxs-lookup"><span data-stu-id="dbdc9-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="dbdc9-117">備考</span><span class="sxs-lookup"><span data-stu-id="dbdc9-117">Remarks</span></span>

<span data-ttu-id="dbdc9-118">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="dbdc9-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dbdc9-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="dbdc9-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dbdc9-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="dbdc9-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="dbdc9-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="dbdc9-121">Schema Name</span></span>  <br/> |<span data-ttu-id="dbdc9-122">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="dbdc9-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="dbdc9-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="dbdc9-123">Validation File</span></span>  <br/> |<span data-ttu-id="dbdc9-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="dbdc9-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="dbdc9-125">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="dbdc9-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="dbdc9-126">False</span><span class="sxs-lookup"><span data-stu-id="dbdc9-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dbdc9-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="dbdc9-127">See also</span></span>



- [<span data-ttu-id="dbdc9-128">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="dbdc9-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

