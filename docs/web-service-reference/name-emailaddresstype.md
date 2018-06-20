---
title: 名 (EmailAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Name
api_type:
- schema
ms.assetid: 98c58c53-9acc-4e89-9fcf-03f1b05abee1
description: Name 要素は、メールボックス ユーザーの名前を表します。
ms.openlocfilehash: b140fd46608a04f9aaba17f917cc4171c056dcf2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832504"
---
# <a name="name-emailaddresstype"></a><span data-ttu-id="b2a52-103">名 (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="b2a52-103">Name (EmailAddressType)</span></span>

<span data-ttu-id="b2a52-104">**Name**要素は、メールボックス ユーザーの名前を表します。</span><span class="sxs-lookup"><span data-stu-id="b2a52-104">The **Name** element represents the name of a mailbox user.</span></span> 
  
```xml
<Name/>
```

<span data-ttu-id="b2a52-105">**string**</span><span class="sxs-lookup"><span data-stu-id="b2a52-105">**string**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="b2a52-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="b2a52-106">Attributes and elements</span></span>

<span data-ttu-id="b2a52-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b2a52-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b2a52-108">属性</span><span class="sxs-lookup"><span data-stu-id="b2a52-108">Attributes</span></span>

<span data-ttu-id="b2a52-109">なし。</span><span class="sxs-lookup"><span data-stu-id="b2a52-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b2a52-110">子要素</span><span class="sxs-lookup"><span data-stu-id="b2a52-110">Child elements</span></span>

<span data-ttu-id="b2a52-111">なし。</span><span class="sxs-lookup"><span data-stu-id="b2a52-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b2a52-112">親要素</span><span class="sxs-lookup"><span data-stu-id="b2a52-112">Parent elements</span></span>

|<span data-ttu-id="b2a52-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="b2a52-113">**Element**</span></span>|<span data-ttu-id="b2a52-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="b2a52-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b2a52-115">メールボックス</span><span class="sxs-lookup"><span data-stu-id="b2a52-115">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="b2a52-116">完全に解決された電子メール アドレスを識別します。</span><span class="sxs-lookup"><span data-stu-id="b2a52-116">Identifies a fully resolved e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="b2a52-117">RoomList</span><span class="sxs-lookup"><span data-stu-id="b2a52-117">RoomList</span></span>](roomlist.md) <br/> |<span data-ttu-id="b2a52-118">会議室の一覧を識別します。</span><span class="sxs-lookup"><span data-stu-id="b2a52-118">Identifies a list of meeting rooms.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b2a52-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="b2a52-119">Text value</span></span>

<span data-ttu-id="b2a52-120">文字列を表す文字列値は、この要素を使用する場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="b2a52-120">A text value that represents a string is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b2a52-121">備考</span><span class="sxs-lookup"><span data-stu-id="b2a52-121">Remarks</span></span>

<span data-ttu-id="b2a52-122">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="b2a52-122">This element is optional.</span></span> <span data-ttu-id="b2a52-123">**AttachmentType**、 **EmailAddressType**、および**EmailAddress**の種類の**名前**の要素が存在しています。</span><span class="sxs-lookup"><span data-stu-id="b2a52-123">The **Name** element exists in the **AttachmentType**, **EmailAddressType**, and **EmailAddress** types.</span></span> <span data-ttu-id="b2a52-124">**EmailAddress**の型の**名前**の要素は、[名前 (EmailAddress)](name-emailaddress.md)要素のトピックで説明します。</span><span class="sxs-lookup"><span data-stu-id="b2a52-124">The **Name** element in the **EmailAddress** type is described in the [Name (EmailAddress)](name-emailaddress.md) element topic.</span></span> 
  
<span data-ttu-id="b2a52-125">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="b2a52-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b2a52-126">要素情報</span><span class="sxs-lookup"><span data-stu-id="b2a52-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b2a52-127">名前空間</span><span class="sxs-lookup"><span data-stu-id="b2a52-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b2a52-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b2a52-128">Schema Name</span></span>  <br/> |<span data-ttu-id="b2a52-129">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="b2a52-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="b2a52-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b2a52-130">Validation File</span></span>  <br/> |<span data-ttu-id="b2a52-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b2a52-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b2a52-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="b2a52-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="b2a52-133">False</span><span class="sxs-lookup"><span data-stu-id="b2a52-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b2a52-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="b2a52-134">See also</span></span>

- [<span data-ttu-id="b2a52-135">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="b2a52-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

