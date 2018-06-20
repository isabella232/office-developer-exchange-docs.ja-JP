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
description: Base64FolderId 要素には、元となるユニファイド メッセージング メッセージを読み取り、SetTelephoneAccessFolderEmail の操作 (UM web サービス) の要求に電話で、既定の電子メール フォルダーとして指定するフォルダーの識別子が含まれています。
ms.openlocfilehash: 7d710542418a717c6fcad243a22682e5840ebbd2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759488"
---
# <a name="base64folderid-um-web-service"></a><span data-ttu-id="c749f-103">base64FolderId (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="c749f-103">base64FolderId (UM web service)</span></span>

<span data-ttu-id="c749f-104">**Base64FolderId**要素には、元となるユニファイド メッセージング メッセージを読み取り[(UM web サービス) の SetTelephoneAccessFolderEmail 操作](settelephoneaccessfolderemail-operation-um-web-service.md)の要求の電話で、既定の電子メール フォルダーとして指定するフォルダーの識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="c749f-104">The **base64FolderId** element contains the identifier of the folder to specify as the default e-mail folder from which Unified Messaging reads messages over the telephone in a [SetTelephoneAccessFolderEmail operation (UM web service)](settelephoneaccessfolderemail-operation-um-web-service.md) request.</span></span> 
  
[<span data-ttu-id="c749f-105">SetTelephoneAccessFolderEmail (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="c749f-105">SetTelephoneAccessFolderEmail (UM web service)</span></span>](settelephoneaccessfolderemail-um-web-service.md)
  
[<span data-ttu-id="c749f-106">base64FolderId (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="c749f-106">base64FolderId (UM web service)</span></span>](base64folderid-um-web-service.md)
  
```xml
<base64FolderId/>
```

 <span data-ttu-id="c749f-107">**string**</span><span class="sxs-lookup"><span data-stu-id="c749f-107">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c749f-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="c749f-108">Attributes and elements</span></span>

<span data-ttu-id="c749f-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c749f-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c749f-110">属性</span><span class="sxs-lookup"><span data-stu-id="c749f-110">Attributes</span></span>

<span data-ttu-id="c749f-111">なし</span><span class="sxs-lookup"><span data-stu-id="c749f-111">None</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c749f-112">子要素</span><span class="sxs-lookup"><span data-stu-id="c749f-112">Child elements</span></span>

<span data-ttu-id="c749f-113">なし。</span><span class="sxs-lookup"><span data-stu-id="c749f-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c749f-114">親要素</span><span class="sxs-lookup"><span data-stu-id="c749f-114">Parent elements</span></span>

|<span data-ttu-id="c749f-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="c749f-115">**Element**</span></span>|<span data-ttu-id="c749f-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="c749f-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c749f-117">SetTelephoneAccessFolderEmail (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="c749f-117">SetTelephoneAccessFolderEmail (UM web service)</span></span>](settelephoneaccessfolderemail-um-web-service.md) <br/> |<span data-ttu-id="c749f-118">電子メール フォルダーには、電話のアクセスを設定する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="c749f-118">Defines request to set the telephone access e-mail folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c749f-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="c749f-119">Text value</span></span>

<span data-ttu-id="c749f-120">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="c749f-120">A text value is required.</span></span> <span data-ttu-id="c749f-121">テキスト値は、フォルダーの MAPI ID を表します。</span><span class="sxs-lookup"><span data-stu-id="c749f-121">The text value represents the MAPI ID of the folder.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c749f-122">備考</span><span class="sxs-lookup"><span data-stu-id="c749f-122">Remarks</span></span>

<span data-ttu-id="c749f-123">電子メール フォルダーには、電話のアクセスを設定するには、 [SetTelephoneAccessFolderEmail 操作 (UM web サービス)](settelephoneaccessfolderemail-operation-um-web-service.md)を使用します。</span><span class="sxs-lookup"><span data-stu-id="c749f-123">To set the telephone access e-mail folder, use the [SetTelephoneAccessFolderEmail operation (UM web service)](settelephoneaccessfolderemail-operation-um-web-service.md).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c749f-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="c749f-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c749f-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="c749f-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c749f-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c749f-126">Schema Name</span></span>  <br/> |<span data-ttu-id="c749f-127">メッセージ</span><span class="sxs-lookup"><span data-stu-id="c749f-127">Messages</span></span>  <br/> |
|<span data-ttu-id="c749f-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c749f-128">Validation File</span></span>  <br/> |<span data-ttu-id="c749f-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c749f-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c749f-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="c749f-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="c749f-131">False</span><span class="sxs-lookup"><span data-stu-id="c749f-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c749f-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="c749f-132">See also</span></span>



[<span data-ttu-id="c749f-133">SetTelephoneAccessFolderEmail (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="c749f-133">SetTelephoneAccessFolderEmail (UM web service)</span></span>](settelephoneaccessfolderemail-um-web-service.md)
  
[<span data-ttu-id="c749f-134">SetTelephoneAccessFolderEmail 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="c749f-134">SetTelephoneAccessFolderEmail operation (UM web service)</span></span>](settelephoneaccessfolderemail-operation-um-web-service.md)
  
<span data-ttu-id="c749f-135">
  [FindFolder 操作](findfolder-operation.md)</span><span class="sxs-lookup"><span data-stu-id="c749f-135">[FindFolder operation](findfolder-operation.md)</span></span>
  
<span data-ttu-id="c749f-136">
  [FindItem 操作](finditem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="c749f-136">[FindItem operation](finditem-operation.md)</span></span>

