---
title: UpdateItemResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateItemResponse
api_type:
- schema
ms.assetid: 023b79b4-c675-4669-9112-d85499ec4fc4
description: UpdateItemResponse 要素は、UpdateItem 要求に対する応答を定義します。
ms.openlocfilehash: f18bb6658bf7a68e2262ebee7ce86255ea527ac4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467145"
---
# <a name="updateitemresponse"></a><span data-ttu-id="385d6-103">UpdateItemResponse</span><span class="sxs-lookup"><span data-stu-id="385d6-103">UpdateItemResponse</span></span>

<span data-ttu-id="385d6-104">**Updateitemresponse**要素は、updateitem 要求に対する応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="385d6-104">The **UpdateItemResponse** element defines a response to an UpdateItem request.</span></span> 
  
```xml
<UpdateItemResponse>
   <ResponseMessages/>
</UpdateItemResponse>
```

 <span data-ttu-id="385d6-105">**UpdateItemResponseType**</span><span class="sxs-lookup"><span data-stu-id="385d6-105">**UpdateItemResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="385d6-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="385d6-106">Attributes and elements</span></span>

<span data-ttu-id="385d6-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="385d6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="385d6-108">属性</span><span class="sxs-lookup"><span data-stu-id="385d6-108">Attributes</span></span>

<span data-ttu-id="385d6-109">なし。</span><span class="sxs-lookup"><span data-stu-id="385d6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="385d6-110">子要素</span><span class="sxs-lookup"><span data-stu-id="385d6-110">Child elements</span></span>

|<span data-ttu-id="385d6-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="385d6-111">**Element**</span></span>|<span data-ttu-id="385d6-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="385d6-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="385d6-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="385d6-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="385d6-114">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="385d6-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="385d6-115">親要素</span><span class="sxs-lookup"><span data-stu-id="385d6-115">Parent elements</span></span>

<span data-ttu-id="385d6-116">なし。</span><span class="sxs-lookup"><span data-stu-id="385d6-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="385d6-117">注釈</span><span class="sxs-lookup"><span data-stu-id="385d6-117">Remarks</span></span>

<span data-ttu-id="385d6-118">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="385d6-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="385d6-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="385d6-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="385d6-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="385d6-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="385d6-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="385d6-121">Schema name</span></span>  <br/> |<span data-ttu-id="385d6-122">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="385d6-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="385d6-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="385d6-123">Validation file</span></span>  <br/> |<span data-ttu-id="385d6-124">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="385d6-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="385d6-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="385d6-125">Can be empty</span></span>  <br/> |<span data-ttu-id="385d6-126">正しくない</span><span class="sxs-lookup"><span data-stu-id="385d6-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="385d6-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="385d6-127">See also</span></span>



<span data-ttu-id="385d6-128">
  [UpdateItem 操作](updateitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="385d6-128">[UpdateItem operation](updateitem-operation.md)</span></span>
  
[<span data-ttu-id="385d6-129">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="385d6-129">UpdateItem</span></span>](updateitem.md)


- [<span data-ttu-id="385d6-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="385d6-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

