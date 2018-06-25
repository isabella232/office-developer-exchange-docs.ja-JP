---
title: IsModerated
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsModerated
api_type:
- schema
ms.assetid: a7562256-feb9-41a1-857e-b5d41cbed680
description: IsModerated 要素は、受信者のメールボックスがモデレートされているかどうかを示します。
ms.openlocfilehash: 8db234f9706bb8187978a76f745323749d7a640a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832055"
---
# <a name="ismoderated"></a><span data-ttu-id="db52d-103">IsModerated</span><span class="sxs-lookup"><span data-stu-id="db52d-103">IsModerated</span></span>

<span data-ttu-id="db52d-104">**IsModerated**要素は、受信者のメールボックスがモデレートされているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="db52d-104">The **IsModerated** element indicates whether the recipient's mailbox is being moderated.</span></span> 
  
```XML
<IsModerated>true | false</IsModerated>
```

 <span data-ttu-id="db52d-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="db52d-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="db52d-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="db52d-106">Attributes and elements</span></span>

<span data-ttu-id="db52d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="db52d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="db52d-108">属性</span><span class="sxs-lookup"><span data-stu-id="db52d-108">Attributes</span></span>

<span data-ttu-id="db52d-109">なし。</span><span class="sxs-lookup"><span data-stu-id="db52d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="db52d-110">子要素</span><span class="sxs-lookup"><span data-stu-id="db52d-110">Child elements</span></span>

<span data-ttu-id="db52d-111">なし。</span><span class="sxs-lookup"><span data-stu-id="db52d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="db52d-112">親要素</span><span class="sxs-lookup"><span data-stu-id="db52d-112">Parent elements</span></span>

|<span data-ttu-id="db52d-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="db52d-113">**Element**</span></span>|<span data-ttu-id="db52d-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="db52d-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="db52d-115">メール ヒント</span><span class="sxs-lookup"><span data-stu-id="db52d-115">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="db52d-116">さまざまな種類のメール ヒントの値を表します。</span><span class="sxs-lookup"><span data-stu-id="db52d-116">Represents values for various types of mail tips.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="db52d-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="db52d-117">Text value</span></span>

<span data-ttu-id="db52d-118">**受信者のメールボックスがモデレートされる場合は、この要素のテキスト値は**</span><span class="sxs-lookup"><span data-stu-id="db52d-118">The text value for this element is **true** if the recipient's mailbox is being moderated.</span></span> <span data-ttu-id="db52d-119">受信者のメールボックスがモデレートされていない場合に、値は**false**です。</span><span class="sxs-lookup"><span data-stu-id="db52d-119">The value is **false** if the recipient's mailbox is not being moderated.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="db52d-120">備考</span><span class="sxs-lookup"><span data-stu-id="db52d-120">Remarks</span></span>

<span data-ttu-id="db52d-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="db52d-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="db52d-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="db52d-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="db52d-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="db52d-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="db52d-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="db52d-124">Schema Name</span></span>  <br/> |<span data-ttu-id="db52d-125">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="db52d-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="db52d-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="db52d-126">Validation File</span></span>  <br/> |<span data-ttu-id="db52d-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="db52d-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="db52d-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="db52d-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="db52d-129">False</span><span class="sxs-lookup"><span data-stu-id="db52d-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="db52d-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="db52d-130">See also</span></span>



- [<span data-ttu-id="db52d-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="db52d-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

