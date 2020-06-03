---
title: アーカイブ Itemresponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 68109a92-c49e-4c0e-b6ec-e90d38d4be4d
description: アーカイブアイテム要求に対する応答を指定するには、アーカイブアイテム Response 要素を指定します。
ms.openlocfilehash: 86360846a9a12955e7fa651d5b5027d90b5e56c0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463399"
---
# <a name="archiveitemresponse"></a><span data-ttu-id="0e087-103">アーカイブ Itemresponse</span><span class="sxs-lookup"><span data-stu-id="0e087-103">ArchiveItemResponse</span></span>

<span data-ttu-id="0e087-104">アーカイブ**アイテム**要求に対する応答を指定するには、アーカイブアイテム**response**要素を指定します。</span><span class="sxs-lookup"><span data-stu-id="0e087-104">The **ArchiveItemResponse** element specifies the response to an **ArchiveItem** request.</span></span> 
  
```XML
<ArchiveItemResponse>
    <ResponseMessages></ResponseMessages>
</ArchiveItemResponse>
```

 <span data-ttu-id="0e087-105">**アーカイブ Itemresponsetype**</span><span class="sxs-lookup"><span data-stu-id="0e087-105">**ArchiveItemResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0e087-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="0e087-106">Attributes and elements</span></span>

<span data-ttu-id="0e087-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0e087-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0e087-108">属性</span><span class="sxs-lookup"><span data-stu-id="0e087-108">Attributes</span></span>

<span data-ttu-id="0e087-109">なし。</span><span class="sxs-lookup"><span data-stu-id="0e087-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0e087-110">子要素</span><span class="sxs-lookup"><span data-stu-id="0e087-110">Child elements</span></span>

|<span data-ttu-id="0e087-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="0e087-111">**Element**</span></span>|<span data-ttu-id="0e087-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="0e087-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0e087-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="0e087-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="0e087-114">Exchange Web サービス要求への応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="0e087-114">Contains the response messages to an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0e087-115">親要素</span><span class="sxs-lookup"><span data-stu-id="0e087-115">Parent elements</span></span>

<span data-ttu-id="0e087-116">なし。</span><span class="sxs-lookup"><span data-stu-id="0e087-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0e087-117">注釈</span><span class="sxs-lookup"><span data-stu-id="0e087-117">Remarks</span></span>

<span data-ttu-id="0e087-118">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="0e087-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="0e087-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="0e087-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0e087-120">要素の情報</span><span class="sxs-lookup"><span data-stu-id="0e087-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0e087-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="0e087-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0e087-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0e087-122">Schema Name</span></span>  <br/> |<span data-ttu-id="0e087-123">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="0e087-123">Message schema</span></span>  <br/> |
|<span data-ttu-id="0e087-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0e087-124">Validation File</span></span>  <br/> |<span data-ttu-id="0e087-125">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="0e087-125">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0e087-126">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="0e087-126">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="0e087-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="0e087-127">See also</span></span>

- [<span data-ttu-id="0e087-128">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="0e087-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

