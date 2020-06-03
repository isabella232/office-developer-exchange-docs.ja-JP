---
title: SharingFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SharingFolderId
api_type:
- schema
ms.assetid: 5ad37ceb-2922-4420-9051-c29d0d57c420
description: SharingFolderId 要素は、共有関係のローカルフォルダーの識別子を表します。
ms.openlocfilehash: 02780251639ee651ca65d8eadded43260852aaf8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526579"
---
# <a name="sharingfolderid"></a><span data-ttu-id="2de29-103">SharingFolderId</span><span class="sxs-lookup"><span data-stu-id="2de29-103">SharingFolderId</span></span>

<span data-ttu-id="2de29-104">**SharingFolderId**要素は、共有関係のローカルフォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="2de29-104">The **SharingFolderId** element represents the identifier of the local folder in a sharing relationship.</span></span> 
  
```xml
<SharingFolderId Id="" ChangeKey="" />
```

 <span data-ttu-id="2de29-105">**FolderIdType**</span><span class="sxs-lookup"><span data-stu-id="2de29-105">**FolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2de29-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="2de29-106">Attributes and elements</span></span>

<span data-ttu-id="2de29-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2de29-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2de29-108">属性</span><span class="sxs-lookup"><span data-stu-id="2de29-108">Attributes</span></span>

|<span data-ttu-id="2de29-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="2de29-109">**Attribute**</span></span>|<span data-ttu-id="2de29-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="2de29-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2de29-111">ID</span><span class="sxs-lookup"><span data-stu-id="2de29-111">Id</span></span>  <br/> |<span data-ttu-id="2de29-112">Exchange ストア内のフォルダーを識別する文字列を格納します。</span><span class="sxs-lookup"><span data-stu-id="2de29-112">Contains a string that identifies a folder in the Exchange store.</span></span> <span data-ttu-id="2de29-113">この属性は必須です。</span><span class="sxs-lookup"><span data-stu-id="2de29-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="2de29-114">ChangeKey</span><span class="sxs-lookup"><span data-stu-id="2de29-114">ChangeKey</span></span>  <br/> |<span data-ttu-id="2de29-115">Id 属性によって識別されるフォルダーのバージョンを識別する文字列を格納します。</span><span class="sxs-lookup"><span data-stu-id="2de29-115">Contains a string that identifies a version of a folder that is identified by the Id attribute.</span></span> <span data-ttu-id="2de29-116">この属性は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="2de29-116">This attribute is optional.</span></span> <span data-ttu-id="2de29-117">この属性を使用して、適切なバージョンのフォルダーが使用されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="2de29-117">Use this attribute to make sure that the correct version of a folder is used.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="2de29-118">子要素</span><span class="sxs-lookup"><span data-stu-id="2de29-118">Child elements</span></span>

<span data-ttu-id="2de29-119">なし。</span><span class="sxs-lookup"><span data-stu-id="2de29-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2de29-120">親要素</span><span class="sxs-lookup"><span data-stu-id="2de29-120">Parent elements</span></span>

|<span data-ttu-id="2de29-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="2de29-121">**Element**</span></span>|<span data-ttu-id="2de29-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="2de29-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2de29-123">RefreshSharingFolder</span><span class="sxs-lookup"><span data-stu-id="2de29-123">RefreshSharingFolder</span></span>](refreshsharingfolder.md) <br/> |<span data-ttu-id="2de29-124">指定したローカルフォルダーを更新する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="2de29-124">Defines a request to refresh the specified local folder.</span></span>  <br/> |
|[<span data-ttu-id="2de29-125">GetSharingFolderResponse</span><span class="sxs-lookup"><span data-stu-id="2de29-125">GetSharingFolderResponse</span></span>](getsharingfolderresponse.md) <br/> |<span data-ttu-id="2de29-126">[Getsharingfolder 操作](getsharingfolder-operation.md)要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="2de29-126">Defines a response to a [GetSharingFolder operation](getsharingfolder-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="2de29-127">GetSharingFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="2de29-127">GetSharingFolderResponseMessage</span></span>](getsharingfolderresponsemessage.md) <br/> |<span data-ttu-id="2de29-128">1つの[Getsharingfolder 操作](getsharingfolder-operation.md)要求の状態と結果を格納します。</span><span class="sxs-lookup"><span data-stu-id="2de29-128">Contains the status and result of a single [GetSharingFolder operation](getsharingfolder-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2de29-129">注釈</span><span class="sxs-lookup"><span data-stu-id="2de29-129">Remarks</span></span>

<span data-ttu-id="2de29-130">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="2de29-130">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2de29-131">要素の情報</span><span class="sxs-lookup"><span data-stu-id="2de29-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2de29-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="2de29-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2de29-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2de29-133">Schema Name</span></span>  <br/> |<span data-ttu-id="2de29-134">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="2de29-134">Messages schema</span></span>  <br/> |
|<span data-ttu-id="2de29-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2de29-135">Validation File</span></span>  <br/> |<span data-ttu-id="2de29-136">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="2de29-136">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2de29-137">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="2de29-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="2de29-138">正しくない</span><span class="sxs-lookup"><span data-stu-id="2de29-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2de29-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="2de29-139">See also</span></span>



- [<span data-ttu-id="2de29-140">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="2de29-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

