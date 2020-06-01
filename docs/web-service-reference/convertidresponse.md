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
description: ConvertIdResponse 要素には、[コンバーター Tid 要求への応答が含まれます。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: 690f0f2109dfc36dd8f359b7cef1e65beb47fc6e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44452525"
---
# <a name="convertidresponse"></a><span data-ttu-id="5f1f1-104">ConvertIdResponse</span><span class="sxs-lookup"><span data-stu-id="5f1f1-104">ConvertIdResponse</span></span>

<span data-ttu-id="5f1f1-105">**ConvertIdResponse**要素には、[コンバーター tid 要求への応答が含まれます。</span><span class="sxs-lookup"><span data-stu-id="5f1f1-105">The **ConvertIdResponse** element contains a response to a ConvertId request.</span></span> <span data-ttu-id="5f1f1-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="5f1f1-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<ConvertIdResponse>
   <ResponseMessages/>
</ConvertIdResponse>
```

 <span data-ttu-id="5f1f1-107">**ConvertIdResponseType**</span><span class="sxs-lookup"><span data-stu-id="5f1f1-107">**ConvertIdResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5f1f1-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="5f1f1-108">Attributes and elements</span></span>

<span data-ttu-id="5f1f1-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5f1f1-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5f1f1-110">属性</span><span class="sxs-lookup"><span data-stu-id="5f1f1-110">Attributes</span></span>

<span data-ttu-id="5f1f1-111">なし。</span><span class="sxs-lookup"><span data-stu-id="5f1f1-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5f1f1-112">子要素</span><span class="sxs-lookup"><span data-stu-id="5f1f1-112">Child elements</span></span>

|<span data-ttu-id="5f1f1-113">**Element**</span><span class="sxs-lookup"><span data-stu-id="5f1f1-113">**Element**</span></span>|<span data-ttu-id="5f1f1-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="5f1f1-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5f1f1-115">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="5f1f1-115">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="5f1f1-116">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="5f1f1-116">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5f1f1-117">親要素</span><span class="sxs-lookup"><span data-stu-id="5f1f1-117">Parent elements</span></span>

<span data-ttu-id="5f1f1-118">なし。</span><span class="sxs-lookup"><span data-stu-id="5f1f1-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5f1f1-119">注釈</span><span class="sxs-lookup"><span data-stu-id="5f1f1-119">Remarks</span></span>

<span data-ttu-id="5f1f1-120">[Responsemessages](responsemessages.md)要素内に含まれる応答メッセージは、ConvertIdResponseMessageType のインスタンスになります。</span><span class="sxs-lookup"><span data-stu-id="5f1f1-120">The response messages that are contained within the [ResponseMessages](responsemessages.md) element will be instances of ConvertIdResponseMessageType.</span></span> 
  
<span data-ttu-id="5f1f1-121">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="5f1f1-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5f1f1-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="5f1f1-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5f1f1-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="5f1f1-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5f1f1-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5f1f1-124">Schema Name</span></span>  <br/> |<span data-ttu-id="5f1f1-125">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="5f1f1-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5f1f1-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5f1f1-126">Validation File</span></span>  <br/> |<span data-ttu-id="5f1f1-127">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="5f1f1-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5f1f1-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="5f1f1-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="5f1f1-129">正しくない</span><span class="sxs-lookup"><span data-stu-id="5f1f1-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5f1f1-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="5f1f1-130">See also</span></span>



[<span data-ttu-id="5f1f1-131">ConvertId 操作</span><span class="sxs-lookup"><span data-stu-id="5f1f1-131">ConvertId operation</span></span>](convertid-operation.md)


- [<span data-ttu-id="5f1f1-132">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="5f1f1-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="5f1f1-133">識別子の変換</span><span class="sxs-lookup"><span data-stu-id="5f1f1-133">Converting Identifiers</span></span>](https://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

