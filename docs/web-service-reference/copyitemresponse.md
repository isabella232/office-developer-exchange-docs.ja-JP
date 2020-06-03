---
title: CopyItemResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopyItemResponse
api_type:
- schema
ms.assetid: ae402bc1-4589-45e0-a929-f368c916a7e4
description: CopyItemResponse 要素は、CopyItem 要求に対する応答を定義します。
ms.openlocfilehash: 601c44dbaa50a8cccbb911a85daee47841152b17
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466767"
---
# <a name="copyitemresponse"></a><span data-ttu-id="66a07-103">CopyItemResponse</span><span class="sxs-lookup"><span data-stu-id="66a07-103">CopyItemResponse</span></span>

<span data-ttu-id="66a07-104">**Copyitemresponse**要素は、copyitem 要求に対する応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="66a07-104">The **CopyItemResponse** element defines a response to a CopyItem request.</span></span> 
  
```xml
<CopyItemResponse>
   <ResponseMessages/>
</CopyItemResponse>
```

 <span data-ttu-id="66a07-105">**CopyItemResponseType**</span><span class="sxs-lookup"><span data-stu-id="66a07-105">**CopyItemResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="66a07-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="66a07-106">Attributes and elements</span></span>

<span data-ttu-id="66a07-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="66a07-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="66a07-108">属性</span><span class="sxs-lookup"><span data-stu-id="66a07-108">Attributes</span></span>

<span data-ttu-id="66a07-109">なし。</span><span class="sxs-lookup"><span data-stu-id="66a07-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="66a07-110">子要素</span><span class="sxs-lookup"><span data-stu-id="66a07-110">Child elements</span></span>

|<span data-ttu-id="66a07-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="66a07-111">**Element**</span></span>|<span data-ttu-id="66a07-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="66a07-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="66a07-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="66a07-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="66a07-114">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="66a07-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="66a07-115">親要素</span><span class="sxs-lookup"><span data-stu-id="66a07-115">Parent elements</span></span>

<span data-ttu-id="66a07-116">なし。</span><span class="sxs-lookup"><span data-stu-id="66a07-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="66a07-117">注釈</span><span class="sxs-lookup"><span data-stu-id="66a07-117">Remarks</span></span>

<span data-ttu-id="66a07-118">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="66a07-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="66a07-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="66a07-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="66a07-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="66a07-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="66a07-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="66a07-121">Schema name</span></span>  <br/> |<span data-ttu-id="66a07-122">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="66a07-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="66a07-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="66a07-123">Validation file</span></span>  <br/> |<span data-ttu-id="66a07-124">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="66a07-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="66a07-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="66a07-125">Can be empty</span></span>  <br/> |<span data-ttu-id="66a07-126">正しくない</span><span class="sxs-lookup"><span data-stu-id="66a07-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="66a07-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="66a07-127">See also</span></span>



[<span data-ttu-id="66a07-128">CopyItem 操作</span><span class="sxs-lookup"><span data-stu-id="66a07-128">CopyItem operation</span></span>](copyitem-operation.md)
  
[<span data-ttu-id="66a07-129">CopyItem</span><span class="sxs-lookup"><span data-stu-id="66a07-129">CopyItem</span></span>](copyitem.md)


- [<span data-ttu-id="66a07-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="66a07-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

