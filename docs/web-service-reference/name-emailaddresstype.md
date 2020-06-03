---
title: Name (EmailAddressType)
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
description: Name 要素は、メールボックスユーザーの名前を表します。
ms.openlocfilehash: db6eb547b5c848dc31bbaa377692989b16771673
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466928"
---
# <a name="name-emailaddresstype"></a><span data-ttu-id="83a85-103">Name (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="83a85-103">Name (EmailAddressType)</span></span>

<span data-ttu-id="83a85-104">**Name**要素は、メールボックスユーザーの名前を表します。</span><span class="sxs-lookup"><span data-stu-id="83a85-104">The **Name** element represents the name of a mailbox user.</span></span> 
  
```xml
<Name/>
```

<span data-ttu-id="83a85-105">**string**</span><span class="sxs-lookup"><span data-stu-id="83a85-105">**string**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="83a85-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="83a85-106">Attributes and elements</span></span>

<span data-ttu-id="83a85-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="83a85-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="83a85-108">属性</span><span class="sxs-lookup"><span data-stu-id="83a85-108">Attributes</span></span>

<span data-ttu-id="83a85-109">なし。</span><span class="sxs-lookup"><span data-stu-id="83a85-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="83a85-110">子要素</span><span class="sxs-lookup"><span data-stu-id="83a85-110">Child elements</span></span>

<span data-ttu-id="83a85-111">なし。</span><span class="sxs-lookup"><span data-stu-id="83a85-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="83a85-112">親要素</span><span class="sxs-lookup"><span data-stu-id="83a85-112">Parent elements</span></span>

|<span data-ttu-id="83a85-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="83a85-113">**Element**</span></span>|<span data-ttu-id="83a85-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="83a85-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="83a85-115">メールボックス</span><span class="sxs-lookup"><span data-stu-id="83a85-115">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="83a85-116">完全に解決された電子メールアドレスを識別します。</span><span class="sxs-lookup"><span data-stu-id="83a85-116">Identifies a fully resolved e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="83a85-117">RoomList</span><span class="sxs-lookup"><span data-stu-id="83a85-117">RoomList</span></span>](roomlist.md) <br/> |<span data-ttu-id="83a85-118">会議室のリストを識別します。</span><span class="sxs-lookup"><span data-stu-id="83a85-118">Identifies a list of meeting rooms.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="83a85-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="83a85-119">Text value</span></span>

<span data-ttu-id="83a85-120">この要素を使用する場合は、文字列を表すテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="83a85-120">A text value that represents a string is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="83a85-121">注釈</span><span class="sxs-lookup"><span data-stu-id="83a85-121">Remarks</span></span>

<span data-ttu-id="83a85-122">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="83a85-122">This element is optional.</span></span> <span data-ttu-id="83a85-123">**Name**要素は、 **attachmenttype**、 **emailaddresstype**、および**EmailAddress**型に存在します。</span><span class="sxs-lookup"><span data-stu-id="83a85-123">The **Name** element exists in the **AttachmentType**, **EmailAddressType**, and **EmailAddress** types.</span></span> <span data-ttu-id="83a85-124">**EmailAddress**型の**name**要素については、「 [name (EmailAddress)](name-emailaddress.md)要素のトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="83a85-124">The **Name** element in the **EmailAddress** type is described in the [Name (EmailAddress)](name-emailaddress.md) element topic.</span></span> 
  
<span data-ttu-id="83a85-125">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="83a85-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="83a85-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="83a85-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="83a85-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="83a85-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="83a85-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="83a85-128">Schema Name</span></span>  <br/> |<span data-ttu-id="83a85-129">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="83a85-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="83a85-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="83a85-130">Validation File</span></span>  <br/> |<span data-ttu-id="83a85-131">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="83a85-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="83a85-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="83a85-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="83a85-133">正しくない</span><span class="sxs-lookup"><span data-stu-id="83a85-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="83a85-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="83a85-134">See also</span></span>

- [<span data-ttu-id="83a85-135">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="83a85-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

