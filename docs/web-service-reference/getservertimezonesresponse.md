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
description: GetServerTimeZonesResponse 要素は、GetServerTimeZones 操作要求への応答を定義します。
ms.openlocfilehash: 5a8dbe19055e3b697149c10df610d081cb65430b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460926"
---
# <a name="getservertimezonesresponse"></a><span data-ttu-id="71194-103">GetServerTimeZonesResponse</span><span class="sxs-lookup"><span data-stu-id="71194-103">GetServerTimeZonesResponse</span></span>

<span data-ttu-id="71194-104">**GetServerTimeZonesResponse**要素は、 [GetServerTimeZones 操作](getservertimezones-operation.md)要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="71194-104">The **GetServerTimeZonesResponse** element defines a response to a [GetServerTimeZones operation](getservertimezones-operation.md) request.</span></span> 
  
```XML
<GetServerTimeZonesResponse>
   <ResponseMessages/>
</GetServerTimeZonesResponse>
```

 <span data-ttu-id="71194-105">**GetServerTimeZonesResponseType**</span><span class="sxs-lookup"><span data-stu-id="71194-105">**GetServerTimeZonesResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="71194-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="71194-106">Attributes and elements</span></span>

<span data-ttu-id="71194-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="71194-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="71194-108">属性</span><span class="sxs-lookup"><span data-stu-id="71194-108">Attributes</span></span>

<span data-ttu-id="71194-109">なし。</span><span class="sxs-lookup"><span data-stu-id="71194-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="71194-110">子要素</span><span class="sxs-lookup"><span data-stu-id="71194-110">Child elements</span></span>

|<span data-ttu-id="71194-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="71194-111">**Element**</span></span>|<span data-ttu-id="71194-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="71194-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="71194-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="71194-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="71194-114">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="71194-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="71194-115">親要素</span><span class="sxs-lookup"><span data-stu-id="71194-115">Parent elements</span></span>

<span data-ttu-id="71194-116">なし。</span><span class="sxs-lookup"><span data-stu-id="71194-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="71194-117">注釈</span><span class="sxs-lookup"><span data-stu-id="71194-117">Remarks</span></span>

<span data-ttu-id="71194-118">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="71194-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="71194-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="71194-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="71194-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="71194-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="71194-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="71194-121">Schema Name</span></span>  <br/> |<span data-ttu-id="71194-122">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="71194-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="71194-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="71194-123">Validation File</span></span>  <br/> |<span data-ttu-id="71194-124">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="71194-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="71194-125">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="71194-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="71194-126">正しくない</span><span class="sxs-lookup"><span data-stu-id="71194-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="71194-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="71194-127">See also</span></span>



- [<span data-ttu-id="71194-128">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="71194-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

