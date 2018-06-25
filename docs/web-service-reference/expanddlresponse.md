---
title: ExpandDLResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExpandDLResponse
api_type:
- schema
ms.assetid: 1c60dd64-a083-460a-9840-021d30f871d6
description: ExpandDLResponse 要素は、配布リストを展開するための要求に対する応答を定義します。
ms.openlocfilehash: dbcb0ff8e5c11460c070b8a87da53cecca279b88
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760370"
---
# <a name="expanddlresponse"></a><span data-ttu-id="d8216-103">ExpandDLResponse</span><span class="sxs-lookup"><span data-stu-id="d8216-103">ExpandDLResponse</span></span>

<span data-ttu-id="d8216-104">**ExpandDLResponse**要素は、配布リストを展開するための要求に対する応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="d8216-104">The **ExpandDLResponse** element defines a response to a request to expand a distribution list.</span></span> 
  
[<span data-ttu-id="d8216-105">ExpandDLResponse</span><span class="sxs-lookup"><span data-stu-id="d8216-105">ExpandDLResponse</span></span>](expanddlresponse.md)
  
```xml
<ExpandDLResponse>
   <ResponseMessages/>
</ExpandDLResponse>
```

 <span data-ttu-id="d8216-106">**ExpandDLResponseType**</span><span class="sxs-lookup"><span data-stu-id="d8216-106">**ExpandDLResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d8216-107">属性および要素</span><span class="sxs-lookup"><span data-stu-id="d8216-107">Attributes and elements</span></span>

<span data-ttu-id="d8216-108">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d8216-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d8216-109">属性</span><span class="sxs-lookup"><span data-stu-id="d8216-109">Attributes</span></span>

<span data-ttu-id="d8216-110">なし。</span><span class="sxs-lookup"><span data-stu-id="d8216-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d8216-111">子要素</span><span class="sxs-lookup"><span data-stu-id="d8216-111">Child elements</span></span>

|<span data-ttu-id="d8216-112">**要素**</span><span class="sxs-lookup"><span data-stu-id="d8216-112">**Element**</span></span>|<span data-ttu-id="d8216-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="d8216-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d8216-114">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="d8216-114">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="d8216-115">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="d8216-115">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d8216-116">親要素</span><span class="sxs-lookup"><span data-stu-id="d8216-116">Parent elements</span></span>

<span data-ttu-id="d8216-117">なし。</span><span class="sxs-lookup"><span data-stu-id="d8216-117">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d8216-118">備考</span><span class="sxs-lookup"><span data-stu-id="d8216-118">Remarks</span></span>

<span data-ttu-id="d8216-119">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="d8216-119">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d8216-120">要素情報</span><span class="sxs-lookup"><span data-stu-id="d8216-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d8216-121">名前空間</span><span class="sxs-lookup"><span data-stu-id="d8216-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d8216-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d8216-122">Schema name</span></span>  <br/> |<span data-ttu-id="d8216-123">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="d8216-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="d8216-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d8216-124">Validation file</span></span>  <br/> |<span data-ttu-id="d8216-125">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d8216-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d8216-126">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="d8216-126">Can be empty</span></span>  <br/> |<span data-ttu-id="d8216-127">False</span><span class="sxs-lookup"><span data-stu-id="d8216-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d8216-128">関連項目</span><span class="sxs-lookup"><span data-stu-id="d8216-128">See also</span></span>



[<span data-ttu-id="d8216-129">ExpandDL</span><span class="sxs-lookup"><span data-stu-id="d8216-129">ExpandDL</span></span>](expanddl.md)
  
[<span data-ttu-id="d8216-130">ExpandDL 操作</span><span class="sxs-lookup"><span data-stu-id="d8216-130">ExpandDL operation</span></span>](expanddl-operation.md)

