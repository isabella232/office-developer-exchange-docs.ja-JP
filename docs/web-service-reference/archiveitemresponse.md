---
title: ArchiveItemResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 68109a92-c49e-4c0e-b6ec-e90d38d4be4d
description: ArchiveItemResponse 要素は、ArchiveItem 要求への応答を指定します。
ms.openlocfilehash: bfd1b9d76c2b49e00a82bd8f6f57742007d0adf7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759431"
---
# <a name="archiveitemresponse"></a><span data-ttu-id="3f0f8-103">ArchiveItemResponse</span><span class="sxs-lookup"><span data-stu-id="3f0f8-103">ArchiveItemResponse</span></span>

<span data-ttu-id="3f0f8-104">**ArchiveItemResponse**要素は、 **ArchiveItem**要求への応答を指定します。</span><span class="sxs-lookup"><span data-stu-id="3f0f8-104">The **ArchiveItemResponse** element specifies the response to an **ArchiveItem** request.</span></span> 
  
```XML
<ArchiveItemResponse>
    <ResponseMessages></ResponseMessages>
</ArchiveItemResponse>
```

 <span data-ttu-id="3f0f8-105">**ArchiveItemResponseType**</span><span class="sxs-lookup"><span data-stu-id="3f0f8-105">**ArchiveItemResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3f0f8-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="3f0f8-106">Attributes and elements</span></span>

<span data-ttu-id="3f0f8-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3f0f8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3f0f8-108">属性</span><span class="sxs-lookup"><span data-stu-id="3f0f8-108">Attributes</span></span>

<span data-ttu-id="3f0f8-109">なし。</span><span class="sxs-lookup"><span data-stu-id="3f0f8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3f0f8-110">子要素</span><span class="sxs-lookup"><span data-stu-id="3f0f8-110">Child elements</span></span>

|<span data-ttu-id="3f0f8-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="3f0f8-111">**Element**</span></span>|<span data-ttu-id="3f0f8-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="3f0f8-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3f0f8-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="3f0f8-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="3f0f8-114">Exchange Web サービス要求への応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="3f0f8-114">Contains the response messages to an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3f0f8-115">親要素</span><span class="sxs-lookup"><span data-stu-id="3f0f8-115">Parent elements</span></span>

<span data-ttu-id="3f0f8-116">なし。</span><span class="sxs-lookup"><span data-stu-id="3f0f8-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3f0f8-117">備考</span><span class="sxs-lookup"><span data-stu-id="3f0f8-117">Remarks</span></span>

<span data-ttu-id="3f0f8-118">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="3f0f8-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="3f0f8-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="3f0f8-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3f0f8-120">要素情報</span><span class="sxs-lookup"><span data-stu-id="3f0f8-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3f0f8-121">名前空間</span><span class="sxs-lookup"><span data-stu-id="3f0f8-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3f0f8-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3f0f8-122">Schema Name</span></span>  <br/> |<span data-ttu-id="3f0f8-123">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="3f0f8-123">Message schema</span></span>  <br/> |
|<span data-ttu-id="3f0f8-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3f0f8-124">Validation File</span></span>  <br/> |<span data-ttu-id="3f0f8-125">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="3f0f8-125">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3f0f8-126">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="3f0f8-126">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="3f0f8-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="3f0f8-127">See also</span></span>

- [<span data-ttu-id="3f0f8-128">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="3f0f8-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

