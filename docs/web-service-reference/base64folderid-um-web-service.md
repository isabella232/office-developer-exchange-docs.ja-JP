---
title: base64FolderId (UM web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- base64FolderId
api_type:
- schema
ms.assetid: 662f8f2f-49a7-4c7a-9065-98a02a49cfcd
description: Base64FolderId 要素には、ユニファイドメッセージングが SetTelephoneAccessFolderEmail 操作 (UM web サービス) 要求で電話でメッセージを読み取る既定の電子メールフォルダーとして指定するフォルダーの識別子が含まれています。
ms.openlocfilehash: ea31c7a0f93188e563bf95c4a3e6e91f0866746c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458048"
---
# <a name="base64folderid-um-web-service"></a><span data-ttu-id="4ca89-103">base64FolderId (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="4ca89-103">base64FolderId (UM web service)</span></span>

<span data-ttu-id="4ca89-104">**Base64FolderId**要素には、ユニファイドメッセージングが[SETTELEPHONEACCESSFOLDEREMAIL 操作 (UM web サービス)](settelephoneaccessfolderemail-operation-um-web-service.md)要求で電話でメッセージを読み取る既定の電子メールフォルダーとして指定するフォルダーの識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="4ca89-104">The **base64FolderId** element contains the identifier of the folder to specify as the default e-mail folder from which Unified Messaging reads messages over the telephone in a [SetTelephoneAccessFolderEmail operation (UM web service)](settelephoneaccessfolderemail-operation-um-web-service.md) request.</span></span> 
  
[<span data-ttu-id="4ca89-105">SetTelephoneAccessFolderEmail (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="4ca89-105">SetTelephoneAccessFolderEmail (UM web service)</span></span>](settelephoneaccessfolderemail-um-web-service.md)
  
[<span data-ttu-id="4ca89-106">base64FolderId (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="4ca89-106">base64FolderId (UM web service)</span></span>](base64folderid-um-web-service.md)
  
```xml
<base64FolderId/>
```

 <span data-ttu-id="4ca89-107">**string**</span><span class="sxs-lookup"><span data-stu-id="4ca89-107">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4ca89-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="4ca89-108">Attributes and elements</span></span>

<span data-ttu-id="4ca89-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4ca89-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4ca89-110">属性</span><span class="sxs-lookup"><span data-stu-id="4ca89-110">Attributes</span></span>

<span data-ttu-id="4ca89-111">なし</span><span class="sxs-lookup"><span data-stu-id="4ca89-111">None</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4ca89-112">子要素</span><span class="sxs-lookup"><span data-stu-id="4ca89-112">Child elements</span></span>

<span data-ttu-id="4ca89-113">なし。</span><span class="sxs-lookup"><span data-stu-id="4ca89-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4ca89-114">親要素</span><span class="sxs-lookup"><span data-stu-id="4ca89-114">Parent elements</span></span>

|<span data-ttu-id="4ca89-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="4ca89-115">**Element**</span></span>|<span data-ttu-id="4ca89-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="4ca89-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4ca89-117">SetTelephoneAccessFolderEmail (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="4ca89-117">SetTelephoneAccessFolderEmail (UM web service)</span></span>](settelephoneaccessfolderemail-um-web-service.md) <br/> |<span data-ttu-id="4ca89-118">電話アクセスの電子メールフォルダーを設定するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="4ca89-118">Defines request to set the telephone access e-mail folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4ca89-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="4ca89-119">Text value</span></span>

<span data-ttu-id="4ca89-120">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="4ca89-120">A text value is required.</span></span> <span data-ttu-id="4ca89-121">Text 値は、フォルダーの MAPI ID を表します。</span><span class="sxs-lookup"><span data-stu-id="4ca89-121">The text value represents the MAPI ID of the folder.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4ca89-122">注釈</span><span class="sxs-lookup"><span data-stu-id="4ca89-122">Remarks</span></span>

<span data-ttu-id="4ca89-123">電話アクセスの電子メールフォルダーを設定するには、 [SetTelephoneAccessFolderEmail 操作 (UM web サービス)](settelephoneaccessfolderemail-operation-um-web-service.md)を使用します。</span><span class="sxs-lookup"><span data-stu-id="4ca89-123">To set the telephone access e-mail folder, use the [SetTelephoneAccessFolderEmail operation (UM web service)](settelephoneaccessfolderemail-operation-um-web-service.md).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4ca89-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="4ca89-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4ca89-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="4ca89-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4ca89-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4ca89-126">Schema Name</span></span>  <br/> |<span data-ttu-id="4ca89-127">メッセージ</span><span class="sxs-lookup"><span data-stu-id="4ca89-127">Messages</span></span>  <br/> |
|<span data-ttu-id="4ca89-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4ca89-128">Validation File</span></span>  <br/> |<span data-ttu-id="4ca89-129">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="4ca89-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4ca89-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="4ca89-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="4ca89-131">正しくない</span><span class="sxs-lookup"><span data-stu-id="4ca89-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4ca89-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="4ca89-132">See also</span></span>



[<span data-ttu-id="4ca89-133">SetTelephoneAccessFolderEmail (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="4ca89-133">SetTelephoneAccessFolderEmail (UM web service)</span></span>](settelephoneaccessfolderemail-um-web-service.md)
  
[<span data-ttu-id="4ca89-134">SetTelephoneAccessFolderEmail 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="4ca89-134">SetTelephoneAccessFolderEmail operation (UM web service)</span></span>](settelephoneaccessfolderemail-operation-um-web-service.md)
  
[<span data-ttu-id="4ca89-135">FindFolder 操作</span><span class="sxs-lookup"><span data-stu-id="4ca89-135">FindFolder operation</span></span>](findfolder-operation.md)
  
[<span data-ttu-id="4ca89-136">FindItem 操作</span><span class="sxs-lookup"><span data-stu-id="4ca89-136">FindItem operation</span></span>](finditem-operation.md)

