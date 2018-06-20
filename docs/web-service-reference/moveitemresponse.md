---
title: MoveItemResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MoveItemResponse
api_type:
- schema
ms.assetid: 77be5104-1e09-4d50-abec-4fadb3a230e5
description: MoveItemResponse 要素は、MoveItem 要求への応答を定義します。
ms.openlocfilehash: 5d1dd0c64880e819e789a0f9f3935168c65b4b28
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832491"
---
# <a name="moveitemresponse"></a><span data-ttu-id="fb489-103">MoveItemResponse</span><span class="sxs-lookup"><span data-stu-id="fb489-103">MoveItemResponse</span></span>

<span data-ttu-id="fb489-104">**MoveItemResponse**要素は、MoveItem 要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="fb489-104">The **MoveItemResponse** element defines a response to a MoveItem request.</span></span> 
  
```xml
<MoveItemResponse>
   <ResponseMessages/>
</MoveItemResponse>
```

 <span data-ttu-id="fb489-105">**MoveItemResponseType**</span><span class="sxs-lookup"><span data-stu-id="fb489-105">**MoveItemResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fb489-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="fb489-106">Attributes and elements</span></span>

<span data-ttu-id="fb489-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="fb489-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fb489-108">属性</span><span class="sxs-lookup"><span data-stu-id="fb489-108">Attributes</span></span>

<span data-ttu-id="fb489-109">なし。</span><span class="sxs-lookup"><span data-stu-id="fb489-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fb489-110">子要素</span><span class="sxs-lookup"><span data-stu-id="fb489-110">Child elements</span></span>

|<span data-ttu-id="fb489-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="fb489-111">**Element**</span></span>|<span data-ttu-id="fb489-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="fb489-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fb489-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="fb489-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="fb489-114">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="fb489-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fb489-115">親要素</span><span class="sxs-lookup"><span data-stu-id="fb489-115">Parent elements</span></span>

<span data-ttu-id="fb489-116">なし。</span><span class="sxs-lookup"><span data-stu-id="fb489-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="fb489-117">備考</span><span class="sxs-lookup"><span data-stu-id="fb489-117">Remarks</span></span>

<span data-ttu-id="fb489-118">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="fb489-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fb489-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="fb489-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fb489-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="fb489-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="fb489-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="fb489-121">Schema name</span></span>  <br/> |<span data-ttu-id="fb489-122">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="fb489-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="fb489-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="fb489-123">Validation file</span></span>  <br/> |<span data-ttu-id="fb489-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="fb489-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fb489-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="fb489-125">Can be empty</span></span>  <br/> |<span data-ttu-id="fb489-126">いいえ</span><span class="sxs-lookup"><span data-stu-id="fb489-126">False</span></span>  <br/> |
   

