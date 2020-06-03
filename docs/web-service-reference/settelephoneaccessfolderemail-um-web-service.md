---
title: SetTelephoneAccessFolderEmail (UM web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- SetTelephoneAccessFolderEmail
api_type:
- schema
ms.assetid: 90759da7-6dba-499e-b8c8-e44a016b3198
description: SetTelephoneAccessFolderEmail 要素は、ユニファイドメッセージングが電話でメッセージを読み取る既定の電子メールフォルダーを設定するための要求を定義します。
ms.openlocfilehash: 806bdb1f0c7930a9e89555192aa32ad997716e7e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467320"
---
# <a name="settelephoneaccessfolderemail-um-web-service"></a><span data-ttu-id="29e79-103">SetTelephoneAccessFolderEmail (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="29e79-103">SetTelephoneAccessFolderEmail (UM web service)</span></span>

<span data-ttu-id="29e79-104">**SetTelephoneAccessFolderEmail**要素は、ユニファイドメッセージングが電話でメッセージを読み取る既定の電子メールフォルダーを設定するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="29e79-104">The **SetTelephoneAccessFolderEmail** element defines a request to set the default e-mail folder from which Unified Messaging will read messages over the telephone.</span></span> 
  
[<span data-ttu-id="29e79-105">SetTelephoneAccessFolderEmail (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="29e79-105">SetTelephoneAccessFolderEmail (UM web service)</span></span>](settelephoneaccessfolderemail-um-web-service.md)
  
```xml
<SetTelephoneAccessFolderEmail>
  <base64FolderId>   </base64FolderId>
</SetTelephoneAccessFolderEmail>
```

 <span data-ttu-id="29e79-106">**complexType**</span><span class="sxs-lookup"><span data-stu-id="29e79-106">**complexType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="29e79-107">属性と要素</span><span class="sxs-lookup"><span data-stu-id="29e79-107">Attributes and elements</span></span>

<span data-ttu-id="29e79-108">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="29e79-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="29e79-109">属性</span><span class="sxs-lookup"><span data-stu-id="29e79-109">Attributes</span></span>

<span data-ttu-id="29e79-110">なし。</span><span class="sxs-lookup"><span data-stu-id="29e79-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="29e79-111">子要素</span><span class="sxs-lookup"><span data-stu-id="29e79-111">Child elements</span></span>

|<span data-ttu-id="29e79-112">**Element**</span><span class="sxs-lookup"><span data-stu-id="29e79-112">**Element**</span></span>|<span data-ttu-id="29e79-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="29e79-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="29e79-114">base64FolderId (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="29e79-114">base64FolderId (UM web service)</span></span>](base64folderid-um-web-service.md) <br/> |<span data-ttu-id="29e79-115">電子メールフォルダーの識別子。</span><span class="sxs-lookup"><span data-stu-id="29e79-115">The identifier of the e-mail folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="29e79-116">親要素</span><span class="sxs-lookup"><span data-stu-id="29e79-116">Parent elements</span></span>

<span data-ttu-id="29e79-117">なし。</span><span class="sxs-lookup"><span data-stu-id="29e79-117">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="29e79-118">テキスト値</span><span class="sxs-lookup"><span data-stu-id="29e79-118">Text value</span></span>

<span data-ttu-id="29e79-119">なし。</span><span class="sxs-lookup"><span data-stu-id="29e79-119">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="29e79-120">要素の情報</span><span class="sxs-lookup"><span data-stu-id="29e79-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="29e79-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="29e79-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="29e79-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="29e79-122">Schema Name</span></span>  <br/> |<span data-ttu-id="29e79-123">メッセージ</span><span class="sxs-lookup"><span data-stu-id="29e79-123">Messages</span></span>  <br/> |
|<span data-ttu-id="29e79-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="29e79-124">Validation File</span></span>  <br/> |<span data-ttu-id="29e79-125">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="29e79-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="29e79-126">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="29e79-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="29e79-127">正しくない</span><span class="sxs-lookup"><span data-stu-id="29e79-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="29e79-128">関連項目</span><span class="sxs-lookup"><span data-stu-id="29e79-128">See also</span></span>



[<span data-ttu-id="29e79-129">SetTelephoneAccessFolderEmail 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="29e79-129">SetTelephoneAccessFolderEmail operation (UM web service)</span></span>](settelephoneaccessfolderemail-operation-um-web-service.md)

