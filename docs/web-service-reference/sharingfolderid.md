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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833485"
---
# <a name="sharingfolderid"></a><span data-ttu-id="2e817-103">SharingFolderId</span><span class="sxs-lookup"><span data-stu-id="2e817-103">SharingFolderId</span></span>

<span data-ttu-id="2e817-104">**SharingFolderId**要素は、共有の関係では、ローカル フォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="2e817-104">The **SharingFolderId** element represents the identifier of the local folder in a sharing relationship.</span></span> 
  
```xml
<SharingFolderId Id="" ChangeKey="" />
```

 <span data-ttu-id="2e817-105">**FolderIdType**</span><span class="sxs-lookup"><span data-stu-id="2e817-105">**FolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2e817-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="2e817-106">Attributes and elements</span></span>

<span data-ttu-id="2e817-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2e817-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2e817-108">属性</span><span class="sxs-lookup"><span data-stu-id="2e817-108">Attributes</span></span>

|<span data-ttu-id="2e817-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="2e817-109">**Attribute**</span></span>|<span data-ttu-id="2e817-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="2e817-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2e817-111">ID</span><span class="sxs-lookup"><span data-stu-id="2e817-111">Id</span></span>  <br/> |<span data-ttu-id="2e817-112">Exchange ストア内のフォルダーを識別する文字列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="2e817-112">Contains a string that identifies a folder in the Exchange store.</span></span> <span data-ttu-id="2e817-113">この属性は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="2e817-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="2e817-114">ChangeKey</span><span class="sxs-lookup"><span data-stu-id="2e817-114">ChangeKey</span></span>  <br/> |<span data-ttu-id="2e817-115">Id 属性によって識別されるフォルダーのバージョンを識別する文字列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="2e817-115">Contains a string that identifies a version of a folder that is identified by the Id attribute.</span></span> <span data-ttu-id="2e817-116">この属性は、省略可能です。</span><span class="sxs-lookup"><span data-stu-id="2e817-116">This attribute is optional.</span></span> <span data-ttu-id="2e817-117">フォルダーの正しいバージョンを使用するかどうかを確認するには、この属性を使用します。</span><span class="sxs-lookup"><span data-stu-id="2e817-117">Use this attribute to make sure that the correct version of a folder is used.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="2e817-118">子要素</span><span class="sxs-lookup"><span data-stu-id="2e817-118">Child elements</span></span>

<span data-ttu-id="2e817-119">なし。</span><span class="sxs-lookup"><span data-stu-id="2e817-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2e817-120">親要素</span><span class="sxs-lookup"><span data-stu-id="2e817-120">Parent elements</span></span>

|<span data-ttu-id="2e817-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="2e817-121">**Element**</span></span>|<span data-ttu-id="2e817-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="2e817-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2e817-123">RefreshSharingFolder</span><span class="sxs-lookup"><span data-stu-id="2e817-123">RefreshSharingFolder</span></span>](refreshsharingfolder.md) <br/> |<span data-ttu-id="2e817-124">指定したローカル フォルダーを更新する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="2e817-124">Defines a request to refresh the specified local folder.</span></span>  <br/> |
|[<span data-ttu-id="2e817-125">GetSharingFolderResponse</span><span class="sxs-lookup"><span data-stu-id="2e817-125">GetSharingFolderResponse</span></span>](getsharingfolderresponse.md) <br/> |<span data-ttu-id="2e817-126">[GetSharingFolder 操作](getsharingfolder-operation.md)要求に対する応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="2e817-126">Defines a response to a [GetSharingFolder operation](getsharingfolder-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="2e817-127">GetSharingFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="2e817-127">GetSharingFolderResponseMessage</span></span>](getsharingfolderresponsemessage.md) <br/> |<span data-ttu-id="2e817-128">状態および 1 つの結果が含まれています[GetSharingFolder の操作](getsharingfolder-operation.md)を要求します。</span><span class="sxs-lookup"><span data-stu-id="2e817-128">Contains the status and result of a single [GetSharingFolder operation](getsharingfolder-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2e817-129">備考</span><span class="sxs-lookup"><span data-stu-id="2e817-129">Remarks</span></span>

<span data-ttu-id="2e817-130">この要素を記述するスキーマは、Microsoft Exchange Server を実行しているコンピューターの Exchange Web サービスをホストにクライアント アクセス サーバーの役割がインストールされている IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="2e817-130">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2e817-131">要素情報</span><span class="sxs-lookup"><span data-stu-id="2e817-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2e817-132">名前空間</span><span class="sxs-lookup"><span data-stu-id="2e817-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2e817-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2e817-133">Schema Name</span></span>  <br/> |<span data-ttu-id="2e817-134">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="2e817-134">Messages schema</span></span>  <br/> |
|<span data-ttu-id="2e817-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2e817-135">Validation File</span></span>  <br/> |<span data-ttu-id="2e817-136">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="2e817-136">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2e817-137">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="2e817-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="2e817-138">False</span><span class="sxs-lookup"><span data-stu-id="2e817-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2e817-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="2e817-139">See also</span></span>



- [<span data-ttu-id="2e817-140">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="2e817-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

