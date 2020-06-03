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
description: GetSharingMetadata 要素は、共有への招待を識別する非透過の認証トークンを取得する要求を定義します。 この要素は、GetSharingMetadata 操作の基本要素です。
ms.openlocfilehash: 406908e566d6d4249003b1a19a9ce79b8b328c4e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530847"
---
# <a name="getsharingmetadata"></a><span data-ttu-id="0c928-104">GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="0c928-104">GetSharingMetadata</span></span>

<span data-ttu-id="0c928-105">**Getsharingmetadata**要素は、共有への招待を識別する非透過の認証トークンを取得する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="0c928-105">The **GetSharingMetadata** element defines a request to get an opaque authentication token that identifies the sharing invitation.</span></span> <span data-ttu-id="0c928-106">この要素は、 [Getsharingmetadata 操作](getsharingmetadata-operation.md)の基本要素です。</span><span class="sxs-lookup"><span data-stu-id="0c928-106">This element is the base element for the [GetSharingMetadata operation](getsharingmetadata-operation.md).</span></span>
  
```XML
<GetSharingMetadata>
   <IdOfFolderToShare/>
   <SenderSmtpAddress/>
   <Recipients/>
</GetSharingMetadata>
```

 <span data-ttu-id="0c928-107">**GetSharingMetadataType**</span><span class="sxs-lookup"><span data-stu-id="0c928-107">**GetSharingMetadataType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0c928-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="0c928-108">Attributes and elements</span></span>

<span data-ttu-id="0c928-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0c928-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0c928-110">属性</span><span class="sxs-lookup"><span data-stu-id="0c928-110">Attributes</span></span>

<span data-ttu-id="0c928-111">なし。</span><span class="sxs-lookup"><span data-stu-id="0c928-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0c928-112">子要素</span><span class="sxs-lookup"><span data-stu-id="0c928-112">Child elements</span></span>

|<span data-ttu-id="0c928-113">**Element**</span><span class="sxs-lookup"><span data-stu-id="0c928-113">**Element**</span></span>|<span data-ttu-id="0c928-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="0c928-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0c928-115">IdOfFolderToShare</span><span class="sxs-lookup"><span data-stu-id="0c928-115">IdOfFolderToShare</span></span>](idoffoldertoshare.md) <br/> |<span data-ttu-id="0c928-116">共有されるサーバー上のフォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="0c928-116">Represents the identifier of the folder on the server that will be shared.</span></span> <span data-ttu-id="0c928-117">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="0c928-117">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="0c928-118">SenderSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="0c928-118">SenderSmtpAddress</span></span>](sendersmtpaddress.md) <br/> |<span data-ttu-id="0c928-119">[IdOfFolderToShare](idoffoldertoshare.md)要素によって識別されるフォルダーが含まれているメールボックスに対応する SMTP 電子メールアドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="0c928-119">Represents the SMTP email address that corresponds to the mailbox that contains the folder that is identified by the [IdOfFolderToShare](idoffoldertoshare.md) element.</span></span> <span data-ttu-id="0c928-120">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="0c928-120">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="0c928-121">受信者 (ArrayOfSmtpAddressType)</span><span class="sxs-lookup"><span data-stu-id="0c928-121">Recipients (ArrayOfSmtpAddressType)</span></span>](recipients-arrayofsmtpaddresstype.md) <br/> |<span data-ttu-id="0c928-122">[IdOfFolderToShare](idoffoldertoshare.md)要素によって識別されるフォルダー内のデータへのアクセスが許可される1つ以上のエンティティの SMTP 電子メールアドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="0c928-122">Represents the SMTP email addresses of one or more entities that will be granted access to the data in the folder that is identified by the [IdOfFolderToShare](idoffoldertoshare.md) element.</span></span> <span data-ttu-id="0c928-123">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="0c928-123">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0c928-124">親要素</span><span class="sxs-lookup"><span data-stu-id="0c928-124">Parent elements</span></span>

<span data-ttu-id="0c928-125">なし。</span><span class="sxs-lookup"><span data-stu-id="0c928-125">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0c928-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="0c928-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0c928-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="0c928-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0c928-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0c928-128">Schema Name</span></span>  <br/> |<span data-ttu-id="0c928-129">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="0c928-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0c928-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0c928-130">Validation File</span></span>  <br/> |<span data-ttu-id="0c928-131">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="0c928-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0c928-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="0c928-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="0c928-133">正しくない</span><span class="sxs-lookup"><span data-stu-id="0c928-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0c928-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="0c928-134">See also</span></span>



[<span data-ttu-id="0c928-135">GetSharingMetadata 操作</span><span class="sxs-lookup"><span data-stu-id="0c928-135">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)


- [<span data-ttu-id="0c928-136">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="0c928-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

