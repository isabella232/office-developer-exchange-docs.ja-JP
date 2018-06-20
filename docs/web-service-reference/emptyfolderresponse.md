---
title: EmptyFolderResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c900be49-3c90-41aa-aba5-bcf1116ec2aa
description: EmptyFolderResponse 要素は、EmptyFolder 操作要求への応答を定義します。
ms.openlocfilehash: ab753351a1eb7deba83823875989816ba75b9809
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760267"
---
# <a name="emptyfolderresponse"></a><span data-ttu-id="d0c05-103">EmptyFolderResponse</span><span class="sxs-lookup"><span data-stu-id="d0c05-103">EmptyFolderResponse</span></span>

<span data-ttu-id="d0c05-104">**EmptyFolderResponse**要素は、[操作の EmptyFolder](emptyfolder-operation.md)要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="d0c05-104">The **EmptyFolderResponse** element defines a response to an [EmptyFolder operation](emptyfolder-operation.md) request.</span></span> 
  
```XML
<EmptyFolderResponse>
   <ResponseMessages/>
</EmptyFolderResponse>
```

 <span data-ttu-id="d0c05-105">**EmptyFolderResponseType**</span><span class="sxs-lookup"><span data-stu-id="d0c05-105">**EmptyFolderResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d0c05-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="d0c05-106">Attributes and elements</span></span>

<span data-ttu-id="d0c05-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d0c05-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d0c05-108">属性</span><span class="sxs-lookup"><span data-stu-id="d0c05-108">Attributes</span></span>

<span data-ttu-id="d0c05-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d0c05-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d0c05-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d0c05-110">Child elements</span></span>

|<span data-ttu-id="d0c05-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="d0c05-111">**Element**</span></span>|<span data-ttu-id="d0c05-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="d0c05-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d0c05-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="d0c05-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="d0c05-114">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="d0c05-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d0c05-115">親要素</span><span class="sxs-lookup"><span data-stu-id="d0c05-115">Parent elements</span></span>

<span data-ttu-id="d0c05-116">なし。</span><span class="sxs-lookup"><span data-stu-id="d0c05-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d0c05-117">備考</span><span class="sxs-lookup"><span data-stu-id="d0c05-117">Remarks</span></span>

<span data-ttu-id="d0c05-118">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="d0c05-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d0c05-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="d0c05-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d0c05-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="d0c05-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d0c05-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d0c05-121">Schema name</span></span>  <br/> |<span data-ttu-id="d0c05-122">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="d0c05-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d0c05-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d0c05-123">Validation file</span></span>  <br/> |<span data-ttu-id="d0c05-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d0c05-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d0c05-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="d0c05-125">Can be empty</span></span>  <br/> |<span data-ttu-id="d0c05-126">False</span><span class="sxs-lookup"><span data-stu-id="d0c05-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d0c05-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="d0c05-127">See also</span></span>



[<span data-ttu-id="d0c05-128">EmptyFolder 操作</span><span class="sxs-lookup"><span data-stu-id="d0c05-128">EmptyFolder operation</span></span>](emptyfolder-operation.md)
  
[<span data-ttu-id="d0c05-129">EmptyFolder</span><span class="sxs-lookup"><span data-stu-id="d0c05-129">EmptyFolder</span></span>](emptyfolder.md)


- [<span data-ttu-id="d0c05-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="d0c05-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

