---
title: FindItemResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindItemResponse
api_type:
- schema
ms.assetid: c8b316df-d4ab-49b8-96d4-8e9a016730ef
description: FindItemResponse 要素は、FindItem 要求に対する応答を定義します。
ms.openlocfilehash: 989adc40a69137dd53289fa48cc65a90259a2e38
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460611"
---
# <a name="finditemresponse"></a><span data-ttu-id="8b516-103">FindItemResponse</span><span class="sxs-lookup"><span data-stu-id="8b516-103">FindItemResponse</span></span>

<span data-ttu-id="8b516-104">**Finditemresponse**要素は、FindItem 要求に対する応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="8b516-104">The **FindItemResponse** element defines a response to a FindItem request.</span></span> 
  
[<span data-ttu-id="8b516-105">FindItemResponse</span><span class="sxs-lookup"><span data-stu-id="8b516-105">FindItemResponse</span></span>](finditemresponse.md)
  
```xml
<FindItemResponse>
   <ResponseMessages/>
</FindItemResponse>
```

 <span data-ttu-id="8b516-106">**FindItemResponseType**</span><span class="sxs-lookup"><span data-stu-id="8b516-106">**FindItemResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8b516-107">属性と要素</span><span class="sxs-lookup"><span data-stu-id="8b516-107">Attributes and elements</span></span>

<span data-ttu-id="8b516-108">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8b516-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8b516-109">属性</span><span class="sxs-lookup"><span data-stu-id="8b516-109">Attributes</span></span>

<span data-ttu-id="8b516-110">なし。</span><span class="sxs-lookup"><span data-stu-id="8b516-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8b516-111">子要素</span><span class="sxs-lookup"><span data-stu-id="8b516-111">Child elements</span></span>

|<span data-ttu-id="8b516-112">**Element**</span><span class="sxs-lookup"><span data-stu-id="8b516-112">**Element**</span></span>|<span data-ttu-id="8b516-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="8b516-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8b516-114">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="8b516-114">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="8b516-115">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="8b516-115">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8b516-116">親要素</span><span class="sxs-lookup"><span data-stu-id="8b516-116">Parent elements</span></span>

<span data-ttu-id="8b516-117">なし。</span><span class="sxs-lookup"><span data-stu-id="8b516-117">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8b516-118">注釈</span><span class="sxs-lookup"><span data-stu-id="8b516-118">Remarks</span></span>

<span data-ttu-id="8b516-119">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="8b516-119">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8b516-120">要素の情報</span><span class="sxs-lookup"><span data-stu-id="8b516-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8b516-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="8b516-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="8b516-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8b516-122">Schema name</span></span>  <br/> |<span data-ttu-id="8b516-123">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="8b516-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="8b516-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8b516-124">Validation file</span></span>  <br/> |<span data-ttu-id="8b516-125">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="8b516-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8b516-126">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="8b516-126">Can be empty</span></span>  <br/> |<span data-ttu-id="8b516-127">正しくない</span><span class="sxs-lookup"><span data-stu-id="8b516-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8b516-128">関連項目</span><span class="sxs-lookup"><span data-stu-id="8b516-128">See also</span></span>



[<span data-ttu-id="8b516-129">FindItem 操作</span><span class="sxs-lookup"><span data-stu-id="8b516-129">FindItem operation</span></span>](finditem-operation.md)
  
[<span data-ttu-id="8b516-130">FindItem</span><span class="sxs-lookup"><span data-stu-id="8b516-130">FindItem</span></span>](finditem.md)


[<span data-ttu-id="8b516-131">アイテムの検索</span><span class="sxs-lookup"><span data-stu-id="8b516-131">Finding Items</span></span>](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

