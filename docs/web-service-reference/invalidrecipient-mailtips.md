---
title: InvalidRecipient (メールヒント)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- InvalidRecipient
api_type:
- schema
ms.assetid: 48959a99-bb0d-4004-963e-5a5baaa96476
description: InvalidRecipient 要素は、受信者が無効であるかどうかを示します。
ms.openlocfilehash: fddd75beb2228c50084bd38b4f4745064cc281dc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530003"
---
# <a name="invalidrecipient-mailtips"></a><span data-ttu-id="93991-103">InvalidRecipient (メールヒント)</span><span class="sxs-lookup"><span data-stu-id="93991-103">InvalidRecipient (MailTips)</span></span>

<span data-ttu-id="93991-104">**Invalidrecipient**要素は、受信者が無効であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="93991-104">The **InvalidRecipient** element indicates whether the recipient is invalid.</span></span> 
  
```XML
<InvalidRecipient>true | false</InvalidRecipient>
```

 <span data-ttu-id="93991-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="93991-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="93991-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="93991-106">Attributes and elements</span></span>

<span data-ttu-id="93991-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="93991-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="93991-108">属性</span><span class="sxs-lookup"><span data-stu-id="93991-108">Attributes</span></span>

<span data-ttu-id="93991-109">なし。</span><span class="sxs-lookup"><span data-stu-id="93991-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="93991-110">子要素</span><span class="sxs-lookup"><span data-stu-id="93991-110">Child elements</span></span>

<span data-ttu-id="93991-111">なし。</span><span class="sxs-lookup"><span data-stu-id="93991-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="93991-112">親要素</span><span class="sxs-lookup"><span data-stu-id="93991-112">Parent elements</span></span>

|<span data-ttu-id="93991-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="93991-113">**Element**</span></span>|<span data-ttu-id="93991-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="93991-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="93991-115">メールヒント</span><span class="sxs-lookup"><span data-stu-id="93991-115">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="93991-116">さまざまな種類のメールヒントの値を表します。</span><span class="sxs-lookup"><span data-stu-id="93991-116">Represents values for various types of mail tips.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="93991-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="93991-117">Text value</span></span>

<span data-ttu-id="93991-118">この要素のテキスト値は、受信者が無効な場合は**true**です。</span><span class="sxs-lookup"><span data-stu-id="93991-118">The text value of this element is **true** if the recipient is invalid.</span></span> <span data-ttu-id="93991-119">受信者が無効である場合、値は**false**になります。</span><span class="sxs-lookup"><span data-stu-id="93991-119">The value is **false** if the recipient is not invalid.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="93991-120">注釈</span><span class="sxs-lookup"><span data-stu-id="93991-120">Remarks</span></span>

<span data-ttu-id="93991-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="93991-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="93991-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="93991-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="93991-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="93991-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="93991-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="93991-124">Schema Name</span></span>  <br/> |<span data-ttu-id="93991-125">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="93991-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="93991-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="93991-126">Validation File</span></span>  <br/> |<span data-ttu-id="93991-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="93991-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="93991-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="93991-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="93991-129">正しくない</span><span class="sxs-lookup"><span data-stu-id="93991-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="93991-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="93991-130">See also</span></span>



- [<span data-ttu-id="93991-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="93991-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

