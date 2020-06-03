---
title: UploadItemsResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UploadItemsResponse
api_type:
- schema
ms.assetid: 93044d39-4489-456a-8cce-b6d69873348f
description: UploadItemsResponse 要素は、1つの UploadItems 要求への応答を表します。
ms.openlocfilehash: 8f83c8239709052fe84d80834333d18bea51e489
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468818"
---
# <a name="uploaditemsresponse"></a><span data-ttu-id="5d803-103">UploadItemsResponse</span><span class="sxs-lookup"><span data-stu-id="5d803-103">UploadItemsResponse</span></span>

<span data-ttu-id="5d803-104">**UploadItemsResponse**要素は、1つの UploadItems 要求への応答を表します。</span><span class="sxs-lookup"><span data-stu-id="5d803-104">The **UploadItemsResponse** element represents a response to a single UploadItems request.</span></span> 
  
[<span data-ttu-id="5d803-105">UploadItemsResponse</span><span class="sxs-lookup"><span data-stu-id="5d803-105">UploadItemsResponse</span></span>](uploaditemsresponse.md)
  
```XML
<UploadItemsResponse>
   <ResponseMessages/>
</UploadItemsResponse>
```

 <span data-ttu-id="5d803-106">**UploadItemsResponseType**</span><span class="sxs-lookup"><span data-stu-id="5d803-106">**UploadItemsResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5d803-107">属性と要素</span><span class="sxs-lookup"><span data-stu-id="5d803-107">Attributes and elements</span></span>

<span data-ttu-id="5d803-108">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5d803-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5d803-109">属性</span><span class="sxs-lookup"><span data-stu-id="5d803-109">Attributes</span></span>

<span data-ttu-id="5d803-110">なし。</span><span class="sxs-lookup"><span data-stu-id="5d803-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5d803-111">子要素</span><span class="sxs-lookup"><span data-stu-id="5d803-111">Child elements</span></span>

|<span data-ttu-id="5d803-112">**Element**</span><span class="sxs-lookup"><span data-stu-id="5d803-112">**Element**</span></span>|<span data-ttu-id="5d803-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="5d803-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5d803-114">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="5d803-114">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="5d803-115">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="5d803-115">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5d803-116">親要素</span><span class="sxs-lookup"><span data-stu-id="5d803-116">Parent elements</span></span>

<span data-ttu-id="5d803-117">なし。</span><span class="sxs-lookup"><span data-stu-id="5d803-117">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="5d803-118">テキスト値</span><span class="sxs-lookup"><span data-stu-id="5d803-118">Text value</span></span>

<span data-ttu-id="5d803-119">なし。</span><span class="sxs-lookup"><span data-stu-id="5d803-119">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5d803-120">注釈</span><span class="sxs-lookup"><span data-stu-id="5d803-120">Remarks</span></span>

<span data-ttu-id="5d803-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="5d803-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5d803-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="5d803-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5d803-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="5d803-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5d803-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5d803-124">Schema Name</span></span>  <br/> |<span data-ttu-id="5d803-125">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="5d803-125">Message schema</span></span>  <br/> |
|<span data-ttu-id="5d803-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5d803-126">Validation File</span></span>  <br/> |<span data-ttu-id="5d803-127">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="5d803-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5d803-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="5d803-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="5d803-129">正しくない</span><span class="sxs-lookup"><span data-stu-id="5d803-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5d803-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="5d803-130">See also</span></span>



[<span data-ttu-id="5d803-131">ExportItems 操作</span><span class="sxs-lookup"><span data-stu-id="5d803-131">ExportItems operation</span></span>](exportitems-operation.md)
  
[<span data-ttu-id="5d803-132">UploadItems 操作</span><span class="sxs-lookup"><span data-stu-id="5d803-132">UploadItems operation</span></span>](uploaditems-operation.md)


- [<span data-ttu-id="5d803-133">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="5d803-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

