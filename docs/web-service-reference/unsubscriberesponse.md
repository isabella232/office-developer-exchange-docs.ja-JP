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
description: UnsubscribeResponse 要素は、購読中止要求への応答を定義します。
ms.openlocfilehash: 1a8ddf93499acb7aa369ec9e91a7106e5cb4bd53
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/01/2020
ms.locfileid: "44467201"
---
# <a name="unsubscriberesponse"></a><span data-ttu-id="a14b9-103">UnsubscribeResponse</span><span class="sxs-lookup"><span data-stu-id="a14b9-103">UnsubscribeResponse</span></span>

<span data-ttu-id="a14b9-104">**UnsubscribeResponse**要素は、購読中止要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="a14b9-104">The **UnsubscribeResponse** element defines a response to an Unsubscribe request.</span></span> 
  
```xml
<UnsubscribeResponse>
   <ResponseMessages/>
</UnsubscribeResponse>
```

 <span data-ttu-id="a14b9-105">**未登録の種類**</span><span class="sxs-lookup"><span data-stu-id="a14b9-105">**UnsubscribeResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a14b9-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="a14b9-106">Attributes and elements</span></span>

<span data-ttu-id="a14b9-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a14b9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a14b9-108">属性</span><span class="sxs-lookup"><span data-stu-id="a14b9-108">Attributes</span></span>

<span data-ttu-id="a14b9-109">なし。</span><span class="sxs-lookup"><span data-stu-id="a14b9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a14b9-110">子要素</span><span class="sxs-lookup"><span data-stu-id="a14b9-110">Child elements</span></span>

|<span data-ttu-id="a14b9-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="a14b9-111">**Element**</span></span>|<span data-ttu-id="a14b9-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="a14b9-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a14b9-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="a14b9-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="a14b9-114">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="a14b9-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a14b9-115">親要素</span><span class="sxs-lookup"><span data-stu-id="a14b9-115">Parent elements</span></span>

<span data-ttu-id="a14b9-116">なし。</span><span class="sxs-lookup"><span data-stu-id="a14b9-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a14b9-117">注釈</span><span class="sxs-lookup"><span data-stu-id="a14b9-117">Remarks</span></span>

<span data-ttu-id="a14b9-118">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="a14b9-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a14b9-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="a14b9-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a14b9-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="a14b9-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a14b9-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a14b9-121">Schema name</span></span>  <br/> |<span data-ttu-id="a14b9-122">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="a14b9-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a14b9-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a14b9-123">Validation file</span></span>  <br/> |<span data-ttu-id="a14b9-124">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="a14b9-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a14b9-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="a14b9-125">Can be empty</span></span>  <br/> |<span data-ttu-id="a14b9-126">正しくない</span><span class="sxs-lookup"><span data-stu-id="a14b9-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a14b9-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="a14b9-127">See also</span></span>



- [<span data-ttu-id="a14b9-128">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="a14b9-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

