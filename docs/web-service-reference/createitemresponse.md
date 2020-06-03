---
title: CreateItemResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateItemResponse
api_type:
- schema
ms.assetid: 742a46a0-2475-45a0-b44f-90639a3f5a43
description: CreateItemResponse 要素は、CreateItem 要求への応答を定義します。
ms.openlocfilehash: af7349888a2f194a8f4ff1043ec8c38a90b3dfff
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458846"
---
# <a name="createitemresponse"></a><span data-ttu-id="9f208-103">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="9f208-103">CreateItemResponse</span></span>

<span data-ttu-id="9f208-104">**Createitemresponse**要素は、CreateItem 要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="9f208-104">The **CreateItemResponse** element defines a response to a CreateItem request.</span></span> 
  
```xml
<CreateItemResponse>
   <ResponseMessages/>
</CreateItemResponse>
```

 <span data-ttu-id="9f208-105">**CreateItemResponseType**</span><span class="sxs-lookup"><span data-stu-id="9f208-105">**CreateItemResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9f208-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="9f208-106">Attributes and elements</span></span>

<span data-ttu-id="9f208-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9f208-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9f208-108">属性</span><span class="sxs-lookup"><span data-stu-id="9f208-108">Attributes</span></span>

<span data-ttu-id="9f208-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9f208-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9f208-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9f208-110">Child elements</span></span>

|<span data-ttu-id="9f208-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="9f208-111">**Element**</span></span>|<span data-ttu-id="9f208-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="9f208-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9f208-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="9f208-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="9f208-114">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="9f208-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9f208-115">親要素</span><span class="sxs-lookup"><span data-stu-id="9f208-115">Parent elements</span></span>

<span data-ttu-id="9f208-116">なし。</span><span class="sxs-lookup"><span data-stu-id="9f208-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9f208-117">注釈</span><span class="sxs-lookup"><span data-stu-id="9f208-117">Remarks</span></span>

<span data-ttu-id="9f208-118">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="9f208-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9f208-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="9f208-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9f208-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="9f208-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9f208-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9f208-121">Schema name</span></span>  <br/> |<span data-ttu-id="9f208-122">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="9f208-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9f208-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9f208-123">Validation file</span></span>  <br/> |<span data-ttu-id="9f208-124">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="9f208-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9f208-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="9f208-125">Can be empty</span></span>  <br/> |<span data-ttu-id="9f208-126">正しくない</span><span class="sxs-lookup"><span data-stu-id="9f208-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9f208-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="9f208-127">See also</span></span>



[<span data-ttu-id="9f208-128">CreateItem 操作</span><span class="sxs-lookup"><span data-stu-id="9f208-128">CreateItem operation</span></span>](createitem-operation.md)
  
[<span data-ttu-id="9f208-129">CreateItem</span><span class="sxs-lookup"><span data-stu-id="9f208-129">CreateItem</span></span>](createitem.md)


- [<span data-ttu-id="9f208-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="9f208-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

