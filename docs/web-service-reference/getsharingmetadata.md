---
title: GetSharingMetadata
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetSharingMetadata
api_type:
- schema
ms.assetid: b609ee26-6d28-4559-81b6-b8e8d4759a23
description: GetSharingMetadata 要素は、共有への招待を識別する不透明な認証トークンを取得する要求を定義します。 この要素は、GetSharingMetadata 操作の基本要素です。
ms.openlocfilehash: 5283d35e11350ef10ed8cc01527e787ef54be927
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831677"
---
# <a name="getsharingmetadata"></a><span data-ttu-id="f0792-104">GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="f0792-104">GetSharingMetadata</span></span>

<span data-ttu-id="f0792-105">**GetSharingMetadata**要素は、共有への招待を識別する不透明な認証トークンを取得する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="f0792-105">The **GetSharingMetadata** element defines a request to get an opaque authentication token that identifies the sharing invitation.</span></span> <span data-ttu-id="f0792-106">この要素は、 [GetSharingMetadata 操作](getsharingmetadata-operation.md)の基本要素です。</span><span class="sxs-lookup"><span data-stu-id="f0792-106">This element is the base element for the [GetSharingMetadata operation](getsharingmetadata-operation.md).</span></span>
  
```XML
<GetSharingMetadata>
   <IdOfFolderToShare/>
   <SenderSmtpAddress/>
   <Recipients/>
</GetSharingMetadata>
```

 <span data-ttu-id="f0792-107">**GetSharingMetadataType**</span><span class="sxs-lookup"><span data-stu-id="f0792-107">**GetSharingMetadataType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f0792-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="f0792-108">Attributes and elements</span></span>

<span data-ttu-id="f0792-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f0792-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f0792-110">属性</span><span class="sxs-lookup"><span data-stu-id="f0792-110">Attributes</span></span>

<span data-ttu-id="f0792-111">なし。</span><span class="sxs-lookup"><span data-stu-id="f0792-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f0792-112">子要素</span><span class="sxs-lookup"><span data-stu-id="f0792-112">Child elements</span></span>

|<span data-ttu-id="f0792-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="f0792-113">**Element**</span></span>|<span data-ttu-id="f0792-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="f0792-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f0792-115">IdOfFolderToShare</span><span class="sxs-lookup"><span data-stu-id="f0792-115">IdOfFolderToShare</span></span>](idoffoldertoshare.md) <br/> |<span data-ttu-id="f0792-116">共有されるサーバー上のフォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="f0792-116">Represents the identifier of the folder on the server that will be shared.</span></span> <span data-ttu-id="f0792-117">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="f0792-117">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="f0792-118">SenderSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="f0792-118">SenderSmtpAddress</span></span>](sendersmtpaddress.md) <br/> |<span data-ttu-id="f0792-119">[IdOfFolderToShare](idoffoldertoshare.md)要素で指定されているフォルダーを含むメールボックスに対応する SMTP 電子メール アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="f0792-119">Represents the SMTP email address that corresponds to the mailbox that contains the folder that is identified by the [IdOfFolderToShare](idoffoldertoshare.md) element.</span></span> <span data-ttu-id="f0792-120">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="f0792-120">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="f0792-121">受信者 (ArrayOfSmtpAddressType)</span><span class="sxs-lookup"><span data-stu-id="f0792-121">Recipients (ArrayOfSmtpAddressType)</span></span>](recipients-arrayofsmtpaddresstype.md) <br/> |<span data-ttu-id="f0792-122">[IdOfFolderToShare](idoffoldertoshare.md)要素で指定されたフォルダー内のデータへのアクセスを許可する 1 つまたは複数のエンティティの SMTP 電子メール アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="f0792-122">Represents the SMTP email addresses of one or more entities that will be granted access to the data in the folder that is identified by the [IdOfFolderToShare](idoffoldertoshare.md) element.</span></span> <span data-ttu-id="f0792-123">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="f0792-123">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f0792-124">親要素</span><span class="sxs-lookup"><span data-stu-id="f0792-124">Parent elements</span></span>

<span data-ttu-id="f0792-125">なし。</span><span class="sxs-lookup"><span data-stu-id="f0792-125">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f0792-126">要素情報</span><span class="sxs-lookup"><span data-stu-id="f0792-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f0792-127">名前空間</span><span class="sxs-lookup"><span data-stu-id="f0792-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f0792-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f0792-128">Schema Name</span></span>  <br/> |<span data-ttu-id="f0792-129">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="f0792-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f0792-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f0792-130">Validation File</span></span>  <br/> |<span data-ttu-id="f0792-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f0792-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f0792-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="f0792-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="f0792-133">False</span><span class="sxs-lookup"><span data-stu-id="f0792-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f0792-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="f0792-134">See also</span></span>



[<span data-ttu-id="f0792-135">GetSharingMetadata 操作</span><span class="sxs-lookup"><span data-stu-id="f0792-135">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)


- [<span data-ttu-id="f0792-136">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="f0792-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

