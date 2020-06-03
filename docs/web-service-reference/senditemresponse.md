---
title: SendItemResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SendItemResponse
api_type:
- schema
ms.assetid: 26ac41c7-57d9-473e-ab7a-bae93e1d2aba
description: SendItemResponse 要素は、SendItem 要求への応答を定義します。
ms.openlocfilehash: dd90510547c3db8c3531663c23d05055bd774fab
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462130"
---
# <a name="senditemresponse"></a><span data-ttu-id="4ac14-103">SendItemResponse</span><span class="sxs-lookup"><span data-stu-id="4ac14-103">SendItemResponse</span></span>

<span data-ttu-id="4ac14-104">**Senditemresponse**要素は、SendItem 要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="4ac14-104">The **SendItemResponse** element defines a response to a SendItem request.</span></span> 
  
```xml
<SendItemResponse>
   <ResponseMessages/>
</SendItemResponse>
```

 <span data-ttu-id="4ac14-105">**SendItemResponseType**</span><span class="sxs-lookup"><span data-stu-id="4ac14-105">**SendItemResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4ac14-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="4ac14-106">Attributes and elements</span></span>

<span data-ttu-id="4ac14-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4ac14-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4ac14-108">属性</span><span class="sxs-lookup"><span data-stu-id="4ac14-108">Attributes</span></span>

<span data-ttu-id="4ac14-109">なし。</span><span class="sxs-lookup"><span data-stu-id="4ac14-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4ac14-110">子要素</span><span class="sxs-lookup"><span data-stu-id="4ac14-110">Child elements</span></span>

|<span data-ttu-id="4ac14-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="4ac14-111">**Element**</span></span>|<span data-ttu-id="4ac14-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="4ac14-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4ac14-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="4ac14-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="4ac14-114">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="4ac14-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4ac14-115">親要素</span><span class="sxs-lookup"><span data-stu-id="4ac14-115">Parent elements</span></span>

<span data-ttu-id="4ac14-116">なし。</span><span class="sxs-lookup"><span data-stu-id="4ac14-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4ac14-117">注釈</span><span class="sxs-lookup"><span data-stu-id="4ac14-117">Remarks</span></span>

<span data-ttu-id="4ac14-118">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="4ac14-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4ac14-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="4ac14-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4ac14-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="4ac14-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4ac14-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4ac14-121">Schema name</span></span>  <br/> |<span data-ttu-id="4ac14-122">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="4ac14-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4ac14-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4ac14-123">Validation file</span></span>  <br/> |<span data-ttu-id="4ac14-124">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="4ac14-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4ac14-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="4ac14-125">Can be empty</span></span>  <br/> |<span data-ttu-id="4ac14-126">正しくない</span><span class="sxs-lookup"><span data-stu-id="4ac14-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4ac14-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="4ac14-127">See also</span></span>



[<span data-ttu-id="4ac14-128">SendItem 操作</span><span class="sxs-lookup"><span data-stu-id="4ac14-128">SendItem operation</span></span>](senditem-operation.md)
  
[<span data-ttu-id="4ac14-129">SendItem</span><span class="sxs-lookup"><span data-stu-id="4ac14-129">SendItem</span></span>](senditem.md)


- [<span data-ttu-id="4ac14-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="4ac14-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

