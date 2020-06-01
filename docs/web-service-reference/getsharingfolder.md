---
title: GetSharingFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetSharingFolder
api_type:
- schema
ms.assetid: ed5bb61f-89c7-4baa-83ee-30f06a49ff9b
description: GetSharingFolder 要素は、指定された共有フォルダーのローカルフォルダー識別子を取得する要求を定義します。 これは、GetSharingFolder 操作の基本要素です。
ms.openlocfilehash: cb76c534d9b30d0a9d1b267396551eb2871e638a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460506"
---
# <a name="getsharingfolder"></a><span data-ttu-id="88c72-104">GetSharingFolder</span><span class="sxs-lookup"><span data-stu-id="88c72-104">GetSharingFolder</span></span>

<span data-ttu-id="88c72-105">**Getsharingfolder**要素は、指定された共有フォルダーのローカルフォルダー識別子を取得する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="88c72-105">The **GetSharingFolder** element defines a request to get the local folder identifier of a specified shared folder.</span></span> <span data-ttu-id="88c72-106">これは、 [Getsharingfolder 操作](getsharingfolder-operation.md)の基本要素です。</span><span class="sxs-lookup"><span data-stu-id="88c72-106">It is the base element for the [GetSharingFolder operation](getsharingfolder-operation.md).</span></span>
  
```xml
<GetSharingFolder>   <SmtpAddress/>   <DataType/>   <SharedFolderId/></GetSharingFolder>
```

 <span data-ttu-id="88c72-107">**GetSharingFolderType**</span><span class="sxs-lookup"><span data-stu-id="88c72-107">**GetSharingFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="88c72-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="88c72-108">Attributes and elements</span></span>

<span data-ttu-id="88c72-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="88c72-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="88c72-110">属性</span><span class="sxs-lookup"><span data-stu-id="88c72-110">Attributes</span></span>

<span data-ttu-id="88c72-111">なし。</span><span class="sxs-lookup"><span data-stu-id="88c72-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="88c72-112">子要素</span><span class="sxs-lookup"><span data-stu-id="88c72-112">Child elements</span></span>

|<span data-ttu-id="88c72-113">**Element**</span><span class="sxs-lookup"><span data-stu-id="88c72-113">**Element**</span></span>|<span data-ttu-id="88c72-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="88c72-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="88c72-115">SmtpAddress</span><span class="sxs-lookup"><span data-stu-id="88c72-115">SmtpAddress</span></span>](smtpaddress.md) <br/> |<span data-ttu-id="88c72-116">共有関係にある相手の SMTP 電子メールアドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="88c72-116">Represents the SMTP e-mail address of the other party in the sharing relationship.</span></span> <span data-ttu-id="88c72-117">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="88c72-117">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="88c72-118">DataType</span><span class="sxs-lookup"><span data-stu-id="88c72-118">DataType</span></span>](datatype.md) <br/> |<span data-ttu-id="88c72-119">共有フォルダーによって共有されるデータの種類を表します。</span><span class="sxs-lookup"><span data-stu-id="88c72-119">Describes the type of data that is shared by a shared folder.</span></span> <span data-ttu-id="88c72-120">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="88c72-120">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="88c72-121">SharedFolderId</span><span class="sxs-lookup"><span data-stu-id="88c72-121">SharedFolderId</span></span>](sharedfolderid.md) <br/> |<span data-ttu-id="88c72-122">ローカルフォルダーの識別子を取得する必要がある共有フォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="88c72-122">Represents the identifier of the shared folder whose local folder identifier should be returned.</span></span> <span data-ttu-id="88c72-123">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="88c72-123">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="88c72-124">親要素</span><span class="sxs-lookup"><span data-stu-id="88c72-124">Parent elements</span></span>

<span data-ttu-id="88c72-125">なし。</span><span class="sxs-lookup"><span data-stu-id="88c72-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="88c72-126">注釈</span><span class="sxs-lookup"><span data-stu-id="88c72-126">Remarks</span></span>

<span data-ttu-id="88c72-127">GetSharingFolder 要素には、 [Smtpaddress](smtpaddress.md)要素を含める必要があります。</span><span class="sxs-lookup"><span data-stu-id="88c72-127">A GetSharingFolder element must contain an [SmtpAddress](smtpaddress.md) element.</span></span> <span data-ttu-id="88c72-128">GetSharingFolder 要素には、 [DataType](datatype.md)要素または[SharedFolderId](sharedfolderid.md)要素も含める必要がありますが、両方を含めることはできません。</span><span class="sxs-lookup"><span data-stu-id="88c72-128">A GetSharingFolder element must also contain either a [DataType](datatype.md) element or a [SharedFolderId](sharedfolderid.md) element, but cannot contain both.</span></span> 
  
<span data-ttu-id="88c72-129">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="88c72-129">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="88c72-130">要素の情報</span><span class="sxs-lookup"><span data-stu-id="88c72-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="88c72-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="88c72-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="88c72-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="88c72-132">Schema Name</span></span>  <br/> |<span data-ttu-id="88c72-133">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="88c72-133">Messages schema</span></span>  <br/> |
|<span data-ttu-id="88c72-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="88c72-134">Validation File</span></span>  <br/> |<span data-ttu-id="88c72-135">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="88c72-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="88c72-136">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="88c72-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="88c72-137">正しくない</span><span class="sxs-lookup"><span data-stu-id="88c72-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="88c72-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="88c72-138">See also</span></span>



[<span data-ttu-id="88c72-139">GetSharingFolder 操作</span><span class="sxs-lookup"><span data-stu-id="88c72-139">GetSharingFolder operation</span></span>](getsharingfolder-operation.md)


- [<span data-ttu-id="88c72-140">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="88c72-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

