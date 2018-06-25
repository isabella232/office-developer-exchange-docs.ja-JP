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
description: SharingFolderId 要素は、共有の関係では、ローカル フォルダーの識別子を表します。
ms.openlocfilehash: e0eb1fbd7155040508daf253f5eb4b1352d7426d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833485"
---
# <a name="sharingfolderid"></a><span data-ttu-id="5d4a0-103">SharingFolderId</span><span class="sxs-lookup"><span data-stu-id="5d4a0-103">SharingFolderId</span></span>

<span data-ttu-id="5d4a0-104">**SharingFolderId**要素は、共有の関係では、ローカル フォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="5d4a0-104">The **SharingFolderId** element represents the identifier of the local folder in a sharing relationship.</span></span> 
  
```xml
<SharingFolderId Id="" ChangeKey="" />
```

 <span data-ttu-id="5d4a0-105">**FolderIdType**</span><span class="sxs-lookup"><span data-stu-id="5d4a0-105">**FolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5d4a0-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="5d4a0-106">Attributes and elements</span></span>

<span data-ttu-id="5d4a0-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5d4a0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5d4a0-108">属性</span><span class="sxs-lookup"><span data-stu-id="5d4a0-108">Attributes</span></span>

|<span data-ttu-id="5d4a0-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="5d4a0-109">**Attribute**</span></span>|<span data-ttu-id="5d4a0-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="5d4a0-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5d4a0-111">ID</span><span class="sxs-lookup"><span data-stu-id="5d4a0-111">Id</span></span>  <br/> |<span data-ttu-id="5d4a0-112">Exchange ストア内のフォルダーを識別する文字列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5d4a0-112">Contains a string that identifies a folder in the Exchange store.</span></span> <span data-ttu-id="5d4a0-113">この属性は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="5d4a0-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="5d4a0-114">ChangeKey</span><span class="sxs-lookup"><span data-stu-id="5d4a0-114">ChangeKey</span></span>  <br/> |<span data-ttu-id="5d4a0-115">Id 属性によって識別されるフォルダーのバージョンを識別する文字列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5d4a0-115">Contains a string that identifies a version of a folder that is identified by the Id attribute.</span></span> <span data-ttu-id="5d4a0-116">この属性は、省略可能です。</span><span class="sxs-lookup"><span data-stu-id="5d4a0-116">This attribute is optional.</span></span> <span data-ttu-id="5d4a0-117">フォルダーの正しいバージョンを使用するかどうかを確認するには、この属性を使用します。</span><span class="sxs-lookup"><span data-stu-id="5d4a0-117">Use this attribute to make sure that the correct version of a folder is used.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="5d4a0-118">子要素</span><span class="sxs-lookup"><span data-stu-id="5d4a0-118">Child elements</span></span>

<span data-ttu-id="5d4a0-119">なし。</span><span class="sxs-lookup"><span data-stu-id="5d4a0-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5d4a0-120">親要素</span><span class="sxs-lookup"><span data-stu-id="5d4a0-120">Parent elements</span></span>

|<span data-ttu-id="5d4a0-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="5d4a0-121">**Element**</span></span>|<span data-ttu-id="5d4a0-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="5d4a0-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5d4a0-123">RefreshSharingFolder</span><span class="sxs-lookup"><span data-stu-id="5d4a0-123">RefreshSharingFolder</span></span>](refreshsharingfolder.md) <br/> |<span data-ttu-id="5d4a0-124">指定したローカル フォルダーを更新する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="5d4a0-124">Defines a request to refresh the specified local folder.</span></span>  <br/> |
|[<span data-ttu-id="5d4a0-125">GetSharingFolderResponse</span><span class="sxs-lookup"><span data-stu-id="5d4a0-125">GetSharingFolderResponse</span></span>](getsharingfolderresponse.md) <br/> |<span data-ttu-id="5d4a0-126">[GetSharingFolder 操作](getsharingfolder-operation.md)要求に対する応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="5d4a0-126">Defines a response to a [GetSharingFolder operation](getsharingfolder-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="5d4a0-127">GetSharingFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="5d4a0-127">GetSharingFolderResponseMessage</span></span>](getsharingfolderresponsemessage.md) <br/> |<span data-ttu-id="5d4a0-128">状態および 1 つの結果が含まれています[GetSharingFolder の操作](getsharingfolder-operation.md)を要求します。</span><span class="sxs-lookup"><span data-stu-id="5d4a0-128">Contains the status and result of a single [GetSharingFolder operation](getsharingfolder-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5d4a0-129">備考</span><span class="sxs-lookup"><span data-stu-id="5d4a0-129">Remarks</span></span>

<span data-ttu-id="5d4a0-130">この要素を記述するスキーマは、Microsoft Exchange Server を実行しているコンピューターの Exchange Web サービスをホストにクライアント アクセス サーバーの役割がインストールされている IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="5d4a0-130">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5d4a0-131">要素情報</span><span class="sxs-lookup"><span data-stu-id="5d4a0-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5d4a0-132">名前空間</span><span class="sxs-lookup"><span data-stu-id="5d4a0-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5d4a0-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5d4a0-133">Schema Name</span></span>  <br/> |<span data-ttu-id="5d4a0-134">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="5d4a0-134">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5d4a0-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5d4a0-135">Validation File</span></span>  <br/> |<span data-ttu-id="5d4a0-136">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="5d4a0-136">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5d4a0-137">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="5d4a0-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="5d4a0-138">False</span><span class="sxs-lookup"><span data-stu-id="5d4a0-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5d4a0-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="5d4a0-139">See also</span></span>



- [<span data-ttu-id="5d4a0-140">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="5d4a0-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

