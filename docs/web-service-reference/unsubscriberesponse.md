---
title: UnsubscribeResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UnsubscribeResponse
api_type:
- schema
ms.assetid: 125e0326-6522-42cd-b20e-6977e6fde249
description: UnsubscribeResponse 要素は、購読の取り消し要求への応答を定義します。
ms.openlocfilehash: a5d90a6631cba7f18da0261be52488c7f6793dcd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839818"
---
# <a name="unsubscriberesponse"></a><span data-ttu-id="3401d-103">UnsubscribeResponse</span><span class="sxs-lookup"><span data-stu-id="3401d-103">UnsubscribeResponse</span></span>

<span data-ttu-id="3401d-104">**UnsubscribeResponse**要素は、購読の取り消し要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="3401d-104">The **UnsubscribeResponse** element defines a response to an Unsubscribe request.</span></span> 
  
```xml
<UnsubscribeResponse>
   <ResponseMessages/>
</UnsubscribeResponse>
```

 <span data-ttu-id="3401d-105">**UnsubscribeResponseType**</span><span class="sxs-lookup"><span data-stu-id="3401d-105">**UnsubscribeResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3401d-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="3401d-106">Attributes and elements</span></span>

<span data-ttu-id="3401d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3401d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3401d-108">属性</span><span class="sxs-lookup"><span data-stu-id="3401d-108">Attributes</span></span>

<span data-ttu-id="3401d-109">なし。</span><span class="sxs-lookup"><span data-stu-id="3401d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3401d-110">子要素</span><span class="sxs-lookup"><span data-stu-id="3401d-110">Child elements</span></span>

|<span data-ttu-id="3401d-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="3401d-111">**Element**</span></span>|<span data-ttu-id="3401d-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="3401d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3401d-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="3401d-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="3401d-114">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="3401d-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3401d-115">親要素</span><span class="sxs-lookup"><span data-stu-id="3401d-115">Parent elements</span></span>

<span data-ttu-id="3401d-116">なし。</span><span class="sxs-lookup"><span data-stu-id="3401d-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3401d-117">備考</span><span class="sxs-lookup"><span data-stu-id="3401d-117">Remarks</span></span>

<span data-ttu-id="3401d-118">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="3401d-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3401d-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="3401d-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3401d-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="3401d-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3401d-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3401d-121">Schema name</span></span>  <br/> |<span data-ttu-id="3401d-122">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="3401d-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3401d-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3401d-123">Validation file</span></span>  <br/> |<span data-ttu-id="3401d-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="3401d-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3401d-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="3401d-125">Can be empty</span></span>  <br/> |<span data-ttu-id="3401d-126">False</span><span class="sxs-lookup"><span data-stu-id="3401d-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3401d-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="3401d-127">See also</span></span>



- [<span data-ttu-id="3401d-128">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="3401d-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

