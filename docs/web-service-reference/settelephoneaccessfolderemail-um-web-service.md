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
description: SetTelephoneAccessFolderEmail 要素は、ユニファイド メッセージングはの読み取り元のメッセージに電話する既定の電子メール フォルダーに設定する要求を定義します。
ms.openlocfilehash: e19f151e364411717d5129cbef8c5cc097689f89
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833461"
---
# <a name="settelephoneaccessfolderemail-um-web-service"></a><span data-ttu-id="01290-103">SetTelephoneAccessFolderEmail (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="01290-103">SetTelephoneAccessFolderEmail (UM web service)</span></span>

<span data-ttu-id="01290-104">**SetTelephoneAccessFolderEmail**要素は、ユニファイド メッセージングはの読み取り元のメッセージに電話する既定の電子メール フォルダーに設定する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="01290-104">The **SetTelephoneAccessFolderEmail** element defines a request to set the default e-mail folder from which Unified Messaging will read messages over the telephone.</span></span> 
  
[<span data-ttu-id="01290-105">SetTelephoneAccessFolderEmail (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="01290-105">SetTelephoneAccessFolderEmail (UM web service)</span></span>](settelephoneaccessfolderemail-um-web-service.md)
  
```xml
<SetTelephoneAccessFolderEmail>
  <base64FolderId>   </base64FolderId>
</SetTelephoneAccessFolderEmail>
```

 <span data-ttu-id="01290-106">**complexType**</span><span class="sxs-lookup"><span data-stu-id="01290-106">**complexType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="01290-107">属性および要素</span><span class="sxs-lookup"><span data-stu-id="01290-107">Attributes and elements</span></span>

<span data-ttu-id="01290-108">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="01290-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="01290-109">属性</span><span class="sxs-lookup"><span data-stu-id="01290-109">Attributes</span></span>

<span data-ttu-id="01290-110">なし。</span><span class="sxs-lookup"><span data-stu-id="01290-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="01290-111">子要素</span><span class="sxs-lookup"><span data-stu-id="01290-111">Child elements</span></span>

|<span data-ttu-id="01290-112">**要素**</span><span class="sxs-lookup"><span data-stu-id="01290-112">**Element**</span></span>|<span data-ttu-id="01290-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="01290-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="01290-114">base64FolderId (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="01290-114">base64FolderId (UM web service)</span></span>](base64folderid-um-web-service.md) <br/> |<span data-ttu-id="01290-115">[メール] フォルダーの識別子です。</span><span class="sxs-lookup"><span data-stu-id="01290-115">The identifier of the e-mail folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="01290-116">親要素</span><span class="sxs-lookup"><span data-stu-id="01290-116">Parent elements</span></span>

<span data-ttu-id="01290-117">なし。</span><span class="sxs-lookup"><span data-stu-id="01290-117">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="01290-118">テキスト値</span><span class="sxs-lookup"><span data-stu-id="01290-118">Text value</span></span>

<span data-ttu-id="01290-119">なし。</span><span class="sxs-lookup"><span data-stu-id="01290-119">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="01290-120">要素情報</span><span class="sxs-lookup"><span data-stu-id="01290-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="01290-121">名前空間</span><span class="sxs-lookup"><span data-stu-id="01290-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="01290-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="01290-122">Schema Name</span></span>  <br/> |<span data-ttu-id="01290-123">メッセージ</span><span class="sxs-lookup"><span data-stu-id="01290-123">Messages</span></span>  <br/> |
|<span data-ttu-id="01290-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="01290-124">Validation File</span></span>  <br/> |<span data-ttu-id="01290-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="01290-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="01290-126">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="01290-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="01290-127">False</span><span class="sxs-lookup"><span data-stu-id="01290-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="01290-128">関連項目</span><span class="sxs-lookup"><span data-stu-id="01290-128">See also</span></span>



[<span data-ttu-id="01290-129">SetTelephoneAccessFolderEmail 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="01290-129">SetTelephoneAccessFolderEmail operation (UM web service)</span></span>](settelephoneaccessfolderemail-operation-um-web-service.md)

