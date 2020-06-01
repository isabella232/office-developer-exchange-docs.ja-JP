---
title: GetItemResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetItemResponse
api_type:
- schema
ms.assetid: 8b66de1b-26a6-476c-9585-a96059125716
description: GetItemResponse 要素は、GetItem 要求に対する応答を定義します。
ms.openlocfilehash: 9b6ebb96406a59fae95e6e243c81494020a50758
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463315"
---
# <a name="getitemresponse"></a><span data-ttu-id="bee01-103">GetItemResponse</span><span class="sxs-lookup"><span data-stu-id="bee01-103">GetItemResponse</span></span>

<span data-ttu-id="bee01-104">**GetItemResponse**要素は、GetItem 要求に対する応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="bee01-104">The **GetItemResponse** element defines a response to a GetItem request.</span></span> 
  
```xml
<GetItemResponse>
   <ResponseMessages/>
</GetItemResponse>
```

 <span data-ttu-id="bee01-105">**GetItemResponseType**</span><span class="sxs-lookup"><span data-stu-id="bee01-105">**GetItemResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bee01-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="bee01-106">Attributes and elements</span></span>

<span data-ttu-id="bee01-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="bee01-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bee01-108">属性</span><span class="sxs-lookup"><span data-stu-id="bee01-108">Attributes</span></span>

<span data-ttu-id="bee01-109">なし。</span><span class="sxs-lookup"><span data-stu-id="bee01-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bee01-110">子要素</span><span class="sxs-lookup"><span data-stu-id="bee01-110">Child elements</span></span>

|<span data-ttu-id="bee01-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="bee01-111">**Element**</span></span>|<span data-ttu-id="bee01-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="bee01-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bee01-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="bee01-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="bee01-114">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="bee01-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bee01-115">親要素</span><span class="sxs-lookup"><span data-stu-id="bee01-115">Parent elements</span></span>

<span data-ttu-id="bee01-116">なし。</span><span class="sxs-lookup"><span data-stu-id="bee01-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bee01-117">注釈</span><span class="sxs-lookup"><span data-stu-id="bee01-117">Remarks</span></span>

<span data-ttu-id="bee01-118">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="bee01-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bee01-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="bee01-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bee01-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="bee01-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="bee01-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="bee01-121">Schema name</span></span>  <br/> |<span data-ttu-id="bee01-122">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="bee01-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="bee01-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="bee01-123">Validation file</span></span>  <br/> |<span data-ttu-id="bee01-124">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="bee01-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="bee01-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="bee01-125">Can be empty</span></span>  <br/> |<span data-ttu-id="bee01-126">正しくない</span><span class="sxs-lookup"><span data-stu-id="bee01-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bee01-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="bee01-127">See also</span></span>



[<span data-ttu-id="bee01-128">GetItem</span><span class="sxs-lookup"><span data-stu-id="bee01-128">GetItem</span></span>](getitem.md)
  
[<span data-ttu-id="bee01-129">GetItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="bee01-129">GetItemResponseMessage</span></span>](getitemresponsemessage.md)
  
<span data-ttu-id="bee01-130">
  [GetItem 操作](getitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="bee01-130">[GetItem operation](getitem-operation.md)</span></span>

