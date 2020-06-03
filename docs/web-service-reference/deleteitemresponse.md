---
title: DeleteItemResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteItemResponse
api_type:
- schema
ms.assetid: 86463d66-fe47-4a19-a81b-e24841e816ab
description: DeleteItemResponse 要素は、1つの DeleteItem 要求に対する応答を定義します。
ms.openlocfilehash: 6aad30077e8867486012dd34bb1def97accffc2b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529197"
---
# <a name="deleteitemresponse"></a><span data-ttu-id="89169-103">DeleteItemResponse</span><span class="sxs-lookup"><span data-stu-id="89169-103">DeleteItemResponse</span></span>

<span data-ttu-id="89169-104">**Deleteitemresponse**要素は、1つの DeleteItem 要求に対する応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="89169-104">The **DeleteItemResponse** element defines a response to a single DeleteItem request.</span></span> 
  
```xml
<DeleteItemResponse>
   <ResponseMessages/>
</DeleteItemResponse>
```

 <span data-ttu-id="89169-105">**DeleteItemResponseType**</span><span class="sxs-lookup"><span data-stu-id="89169-105">**DeleteItemResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="89169-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="89169-106">Attributes and elements</span></span>

<span data-ttu-id="89169-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="89169-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="89169-108">属性</span><span class="sxs-lookup"><span data-stu-id="89169-108">Attributes</span></span>

<span data-ttu-id="89169-109">なし。</span><span class="sxs-lookup"><span data-stu-id="89169-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="89169-110">子要素</span><span class="sxs-lookup"><span data-stu-id="89169-110">Child elements</span></span>

|<span data-ttu-id="89169-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="89169-111">**Element**</span></span>|<span data-ttu-id="89169-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="89169-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="89169-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="89169-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="89169-114">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="89169-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="89169-115">親要素</span><span class="sxs-lookup"><span data-stu-id="89169-115">Parent elements</span></span>

<span data-ttu-id="89169-116">なし。</span><span class="sxs-lookup"><span data-stu-id="89169-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="89169-117">注釈</span><span class="sxs-lookup"><span data-stu-id="89169-117">Remarks</span></span>

<span data-ttu-id="89169-118">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="89169-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="89169-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="89169-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="89169-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="89169-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="89169-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="89169-121">Schema Name</span></span>  <br/> |<span data-ttu-id="89169-122">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="89169-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="89169-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="89169-123">Validation File</span></span>  <br/> |<span data-ttu-id="89169-124">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="89169-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="89169-125">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="89169-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="89169-126">正しくない</span><span class="sxs-lookup"><span data-stu-id="89169-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="89169-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="89169-127">See also</span></span>

- [<span data-ttu-id="89169-128">DeleteItem 操作</span><span class="sxs-lookup"><span data-stu-id="89169-128">DeleteItem operation</span></span>](deleteitem-operation.md)  
- [<span data-ttu-id="89169-129">DeleteItem</span><span class="sxs-lookup"><span data-stu-id="89169-129">DeleteItem</span></span>](deleteitem.md)
- [<span data-ttu-id="89169-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="89169-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

