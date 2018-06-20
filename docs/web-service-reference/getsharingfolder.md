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
description: GetSharingFolder 要素は、指定した共有フォルダーのローカル フォルダーの識別子を取得する要求を定義します。 それは、GetSharingFolder 操作の基本要素です。
ms.openlocfilehash: 7c2f31aa27c1cbde6cdad2b41a341916b4bed2ce
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831669"
---
# <a name="getsharingfolder"></a><span data-ttu-id="60c59-104">GetSharingFolder</span><span class="sxs-lookup"><span data-stu-id="60c59-104">GetSharingFolder</span></span>

<span data-ttu-id="60c59-105">**GetSharingFolder**要素は、指定した共有フォルダーのローカル フォルダーの識別子を取得する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="60c59-105">The **GetSharingFolder** element defines a request to get the local folder identifier of a specified shared folder.</span></span> <span data-ttu-id="60c59-106">それは、 [GetSharingFolder 操作](getsharingfolder-operation.md)の基本要素です。</span><span class="sxs-lookup"><span data-stu-id="60c59-106">It is the base element for the [GetSharingFolder operation](getsharingfolder-operation.md).</span></span>
  
```xml
<GetSharingFolder>   <SmtpAddress/>   <DataType/>   <SharedFolderId/></GetSharingFolder>
```

 <span data-ttu-id="60c59-107">**GetSharingFolderType**</span><span class="sxs-lookup"><span data-stu-id="60c59-107">**GetSharingFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="60c59-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="60c59-108">Attributes and elements</span></span>

<span data-ttu-id="60c59-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="60c59-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="60c59-110">属性</span><span class="sxs-lookup"><span data-stu-id="60c59-110">Attributes</span></span>

<span data-ttu-id="60c59-111">なし。</span><span class="sxs-lookup"><span data-stu-id="60c59-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="60c59-112">子要素</span><span class="sxs-lookup"><span data-stu-id="60c59-112">Child elements</span></span>

|<span data-ttu-id="60c59-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="60c59-113">**Element**</span></span>|<span data-ttu-id="60c59-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="60c59-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="60c59-115">SmtpAddress</span><span class="sxs-lookup"><span data-stu-id="60c59-115">SmtpAddress</span></span>](smtpaddress.md) <br/> |<span data-ttu-id="60c59-116">共有の関係で相手の SMTP 電子メール アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="60c59-116">Represents the SMTP e-mail address of the other party in the sharing relationship.</span></span> <span data-ttu-id="60c59-117">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="60c59-117">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="60c59-118">DataType</span><span class="sxs-lookup"><span data-stu-id="60c59-118">DataType</span></span>](datatype.md) <br/> |<span data-ttu-id="60c59-119">共有フォルダーが共有されているデータの種類について説明します。</span><span class="sxs-lookup"><span data-stu-id="60c59-119">Describes the type of data that is shared by a shared folder.</span></span> <span data-ttu-id="60c59-120">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="60c59-120">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="60c59-121">SharedFolderId</span><span class="sxs-lookup"><span data-stu-id="60c59-121">SharedFolderId</span></span>](sharedfolderid.md) <br/> |<span data-ttu-id="60c59-122">返される識別子を持つローカルのフォルダーの共有フォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="60c59-122">Represents the identifier of the shared folder whose local folder identifier should be returned.</span></span> <span data-ttu-id="60c59-123">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="60c59-123">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="60c59-124">親要素</span><span class="sxs-lookup"><span data-stu-id="60c59-124">Parent elements</span></span>

<span data-ttu-id="60c59-125">なし。</span><span class="sxs-lookup"><span data-stu-id="60c59-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="60c59-126">備考</span><span class="sxs-lookup"><span data-stu-id="60c59-126">Remarks</span></span>

<span data-ttu-id="60c59-127">GetSharingFolder 要素は、 [SmtpAddress](smtpaddress.md)要素を含める必要があります。</span><span class="sxs-lookup"><span data-stu-id="60c59-127">A GetSharingFolder element must contain an [SmtpAddress](smtpaddress.md) element.</span></span> <span data-ttu-id="60c59-128">GetSharingFolder 要素は、[データ型](datatype.md)の要素または[SharedFolderId](sharedfolderid.md)要素では、いずれかも含まれている必要がありますが、両方を含めることはできません。</span><span class="sxs-lookup"><span data-stu-id="60c59-128">A GetSharingFolder element must also contain either a [DataType](datatype.md) element or a [SharedFolderId](sharedfolderid.md) element, but cannot contain both.</span></span> 
  
<span data-ttu-id="60c59-129">この要素を記述するスキーマは、Microsoft Exchange Server を実行しているコンピューターの Exchange Web サービスをホストにクライアント アクセス サーバーの役割がインストールされている IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="60c59-129">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="60c59-130">要素情報</span><span class="sxs-lookup"><span data-stu-id="60c59-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="60c59-131">名前空間</span><span class="sxs-lookup"><span data-stu-id="60c59-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="60c59-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="60c59-132">Schema Name</span></span>  <br/> |<span data-ttu-id="60c59-133">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="60c59-133">Messages schema</span></span>  <br/> |
|<span data-ttu-id="60c59-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="60c59-134">Validation File</span></span>  <br/> |<span data-ttu-id="60c59-135">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="60c59-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="60c59-136">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="60c59-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="60c59-137">False</span><span class="sxs-lookup"><span data-stu-id="60c59-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="60c59-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="60c59-138">See also</span></span>



[<span data-ttu-id="60c59-139">GetSharingFolder 操作</span><span class="sxs-lookup"><span data-stu-id="60c59-139">GetSharingFolder operation</span></span>](getsharingfolder-operation.md)


- [<span data-ttu-id="60c59-140">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="60c59-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

