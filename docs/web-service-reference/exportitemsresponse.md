---
title: ExportItemsResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExportItemsResponse
api_type:
- schema
ms.assetid: ef44354b-fbdb-4f7c-b6bd-b27f56a1d018
description: ExportItemsResponse 要素は、1つの ExportItems 要求への応答を表します。
ms.openlocfilehash: a05a767032c32680cc269459b541446fcaa3d660
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526040"
---
# <a name="exportitemsresponse"></a><span data-ttu-id="a94e1-103">ExportItemsResponse</span><span class="sxs-lookup"><span data-stu-id="a94e1-103">ExportItemsResponse</span></span>

<span data-ttu-id="a94e1-104">**ExportItemsResponse**要素は、1つの**ExportItems**要求への応答を表します。</span><span class="sxs-lookup"><span data-stu-id="a94e1-104">The **ExportItemsResponse** element represents response to a single **ExportItems** request.</span></span> 
  
[<span data-ttu-id="a94e1-105">ExportItemsResponse</span><span class="sxs-lookup"><span data-stu-id="a94e1-105">ExportItemsResponse</span></span>](exportitemsresponse.md)
  
```XML
<ExportItemsResponse>
   <ResponseMessages/>
</ExportItemsResponse>
```

 <span data-ttu-id="a94e1-106">**ExportItemsResponseType**</span><span class="sxs-lookup"><span data-stu-id="a94e1-106">**ExportItemsResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a94e1-107">属性と要素</span><span class="sxs-lookup"><span data-stu-id="a94e1-107">Attributes and elements</span></span>

<span data-ttu-id="a94e1-108">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a94e1-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a94e1-109">属性</span><span class="sxs-lookup"><span data-stu-id="a94e1-109">Attributes</span></span>

<span data-ttu-id="a94e1-110">なし。</span><span class="sxs-lookup"><span data-stu-id="a94e1-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a94e1-111">子要素</span><span class="sxs-lookup"><span data-stu-id="a94e1-111">Child elements</span></span>

|<span data-ttu-id="a94e1-112">**Element**</span><span class="sxs-lookup"><span data-stu-id="a94e1-112">**Element**</span></span>|<span data-ttu-id="a94e1-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="a94e1-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a94e1-114">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="a94e1-114">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="a94e1-115">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="a94e1-115">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a94e1-116">親要素</span><span class="sxs-lookup"><span data-stu-id="a94e1-116">Parent elements</span></span>

<span data-ttu-id="a94e1-117">なし。</span><span class="sxs-lookup"><span data-stu-id="a94e1-117">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="a94e1-118">テキスト値</span><span class="sxs-lookup"><span data-stu-id="a94e1-118">Text value</span></span>

<span data-ttu-id="a94e1-119">なし。</span><span class="sxs-lookup"><span data-stu-id="a94e1-119">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a94e1-120">注釈</span><span class="sxs-lookup"><span data-stu-id="a94e1-120">Remarks</span></span>

<span data-ttu-id="a94e1-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="a94e1-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a94e1-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="a94e1-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a94e1-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="a94e1-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a94e1-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a94e1-124">Schema Name</span></span>  <br/> |<span data-ttu-id="a94e1-125">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="a94e1-125">Message schema</span></span>  <br/> |
|<span data-ttu-id="a94e1-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a94e1-126">Validation File</span></span>  <br/> |<span data-ttu-id="a94e1-127">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="a94e1-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a94e1-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="a94e1-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="a94e1-129">正しくない</span><span class="sxs-lookup"><span data-stu-id="a94e1-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a94e1-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="a94e1-130">See also</span></span>



[<span data-ttu-id="a94e1-131">ExportItems 操作</span><span class="sxs-lookup"><span data-stu-id="a94e1-131">ExportItems operation</span></span>](exportitems-operation.md)
  
[<span data-ttu-id="a94e1-132">UploadItems 操作</span><span class="sxs-lookup"><span data-stu-id="a94e1-132">UploadItems operation</span></span>](uploaditems-operation.md)

