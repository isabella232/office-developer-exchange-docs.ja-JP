---
title: ConvertIdResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConvertIdResponse
api_type:
- schema
ms.assetid: ac1f044f-04a4-42ef-b762-cac5cd37894d
description: ConvertIdResponse 要素には、ConvertId 要求への応答が含まれています。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: 80299afebcebf15546b0fdbe14f0b08960527a47
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759770"
---
# <a name="convertidresponse"></a><span data-ttu-id="26f2a-104">ConvertIdResponse</span><span class="sxs-lookup"><span data-stu-id="26f2a-104">ConvertIdResponse</span></span>

<span data-ttu-id="26f2a-105">**ConvertIdResponse**要素には、ConvertId 要求への応答が含まれています。</span><span class="sxs-lookup"><span data-stu-id="26f2a-105">The **ConvertIdResponse** element contains a response to a ConvertId request.</span></span> <span data-ttu-id="26f2a-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="26f2a-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<ConvertIdResponse>
   <ResponseMessages/>
</ConvertIdResponse>
```

 <span data-ttu-id="26f2a-107">**ConvertIdResponseType**</span><span class="sxs-lookup"><span data-stu-id="26f2a-107">**ConvertIdResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="26f2a-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="26f2a-108">Attributes and elements</span></span>

<span data-ttu-id="26f2a-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="26f2a-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="26f2a-110">属性</span><span class="sxs-lookup"><span data-stu-id="26f2a-110">Attributes</span></span>

<span data-ttu-id="26f2a-111">なし。</span><span class="sxs-lookup"><span data-stu-id="26f2a-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="26f2a-112">子要素</span><span class="sxs-lookup"><span data-stu-id="26f2a-112">Child elements</span></span>

|<span data-ttu-id="26f2a-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="26f2a-113">**Element**</span></span>|<span data-ttu-id="26f2a-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="26f2a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="26f2a-115">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="26f2a-115">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="26f2a-116">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="26f2a-116">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="26f2a-117">親要素</span><span class="sxs-lookup"><span data-stu-id="26f2a-117">Parent elements</span></span>

<span data-ttu-id="26f2a-118">なし。</span><span class="sxs-lookup"><span data-stu-id="26f2a-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="26f2a-119">備考</span><span class="sxs-lookup"><span data-stu-id="26f2a-119">Remarks</span></span>

<span data-ttu-id="26f2a-120">[ResponseMessages](responsemessages.md)要素内に含まれる応答メッセージは、ConvertIdResponseMessageType のインスタンスになります。</span><span class="sxs-lookup"><span data-stu-id="26f2a-120">The response messages that are contained within the [ResponseMessages](responsemessages.md) element will be instances of ConvertIdResponseMessageType.</span></span> 
  
<span data-ttu-id="26f2a-121">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="26f2a-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="26f2a-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="26f2a-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="26f2a-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="26f2a-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="26f2a-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="26f2a-124">Schema Name</span></span>  <br/> |<span data-ttu-id="26f2a-125">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="26f2a-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="26f2a-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="26f2a-126">Validation File</span></span>  <br/> |<span data-ttu-id="26f2a-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="26f2a-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="26f2a-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="26f2a-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="26f2a-129">False</span><span class="sxs-lookup"><span data-stu-id="26f2a-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="26f2a-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="26f2a-130">See also</span></span>



[<span data-ttu-id="26f2a-131">ConvertId 操作</span><span class="sxs-lookup"><span data-stu-id="26f2a-131">ConvertId operation</span></span>](convertid-operation.md)


- [<span data-ttu-id="26f2a-132">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="26f2a-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="26f2a-133">識別子に変換します。</span><span class="sxs-lookup"><span data-stu-id="26f2a-133">Converting Identifiers</span></span>](http://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

