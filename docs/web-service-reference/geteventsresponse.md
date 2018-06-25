---
title: GetEventsResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetEventsResponse
api_type:
- schema
ms.assetid: 5b735d19-55ae-4e6f-a5e3-2bfbdf3d8749
description: GetEventsResponse 要素は、GetEvents 要求への応答を表します。
ms.openlocfilehash: caef7a28a6e644bf2818b57d53e6f22d6e7896f8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760713"
---
# <a name="geteventsresponse"></a><span data-ttu-id="169a6-103">GetEventsResponse</span><span class="sxs-lookup"><span data-stu-id="169a6-103">GetEventsResponse</span></span>

<span data-ttu-id="169a6-104">**GetEventsResponse**要素は、GetEvents 要求への応答を表します。</span><span class="sxs-lookup"><span data-stu-id="169a6-104">The **GetEventsResponse** element represents a response to a GetEvents request.</span></span> 
  
```xml
<GetEventsResponse>
   <ResponseMessages/>
</GetEventsResponse>
```

 <span data-ttu-id="169a6-105">**GetEventsResponseType**</span><span class="sxs-lookup"><span data-stu-id="169a6-105">**GetEventsResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="169a6-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="169a6-106">Attributes and elements</span></span>

<span data-ttu-id="169a6-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="169a6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="169a6-108">属性</span><span class="sxs-lookup"><span data-stu-id="169a6-108">Attributes</span></span>

<span data-ttu-id="169a6-109">なし。</span><span class="sxs-lookup"><span data-stu-id="169a6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="169a6-110">子要素</span><span class="sxs-lookup"><span data-stu-id="169a6-110">Child elements</span></span>

|<span data-ttu-id="169a6-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="169a6-111">**Element**</span></span>|<span data-ttu-id="169a6-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="169a6-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="169a6-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="169a6-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="169a6-114">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="169a6-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="169a6-115">親要素</span><span class="sxs-lookup"><span data-stu-id="169a6-115">Parent elements</span></span>

<span data-ttu-id="169a6-116">なし。</span><span class="sxs-lookup"><span data-stu-id="169a6-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="169a6-117">備考</span><span class="sxs-lookup"><span data-stu-id="169a6-117">Remarks</span></span>

<span data-ttu-id="169a6-118">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="169a6-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="169a6-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="169a6-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="169a6-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="169a6-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="169a6-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="169a6-121">Schema name</span></span>  <br/> |<span data-ttu-id="169a6-122">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="169a6-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="169a6-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="169a6-123">Validation file</span></span>  <br/> |<span data-ttu-id="169a6-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="169a6-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="169a6-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="169a6-125">Can be empty</span></span>  <br/> |<span data-ttu-id="169a6-126">いいえ</span><span class="sxs-lookup"><span data-stu-id="169a6-126">False</span></span>  <br/> |
   

