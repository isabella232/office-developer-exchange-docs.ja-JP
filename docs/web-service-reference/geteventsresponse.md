---
title: Getイベント応答
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
description: Getイベント Response 要素は、GetEvents 要求への応答を表します。
ms.openlocfilehash: 27335ec9adb7887514c98be34016cd766dc4127d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462865"
---
# <a name="geteventsresponse"></a><span data-ttu-id="d2528-103">Getイベント応答</span><span class="sxs-lookup"><span data-stu-id="d2528-103">GetEventsResponse</span></span>

<span data-ttu-id="d2528-104">**Getイベント response**要素は、GetEvents 要求への応答を表します。</span><span class="sxs-lookup"><span data-stu-id="d2528-104">The **GetEventsResponse** element represents a response to a GetEvents request.</span></span> 
  
```xml
<GetEventsResponse>
   <ResponseMessages/>
</GetEventsResponse>
```

 <span data-ttu-id="d2528-105">**Getイベント Responsetype**</span><span class="sxs-lookup"><span data-stu-id="d2528-105">**GetEventsResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d2528-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d2528-106">Attributes and elements</span></span>

<span data-ttu-id="d2528-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d2528-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d2528-108">属性</span><span class="sxs-lookup"><span data-stu-id="d2528-108">Attributes</span></span>

<span data-ttu-id="d2528-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d2528-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d2528-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d2528-110">Child elements</span></span>

|<span data-ttu-id="d2528-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="d2528-111">**Element**</span></span>|<span data-ttu-id="d2528-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="d2528-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d2528-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="d2528-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="d2528-114">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="d2528-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d2528-115">親要素</span><span class="sxs-lookup"><span data-stu-id="d2528-115">Parent elements</span></span>

<span data-ttu-id="d2528-116">なし。</span><span class="sxs-lookup"><span data-stu-id="d2528-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d2528-117">注釈</span><span class="sxs-lookup"><span data-stu-id="d2528-117">Remarks</span></span>

<span data-ttu-id="d2528-118">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="d2528-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d2528-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d2528-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d2528-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="d2528-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d2528-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d2528-121">Schema name</span></span>  <br/> |<span data-ttu-id="d2528-122">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="d2528-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d2528-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d2528-123">Validation file</span></span>  <br/> |<span data-ttu-id="d2528-124">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="d2528-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d2528-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="d2528-125">Can be empty</span></span>  <br/> |<span data-ttu-id="d2528-126">いいえ</span><span class="sxs-lookup"><span data-stu-id="d2528-126">False</span></span>  <br/> |
   

