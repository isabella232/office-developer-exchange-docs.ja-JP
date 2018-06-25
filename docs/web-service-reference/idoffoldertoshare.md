---
title: IdOfFolderToShare
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IdOfFolderToShare
api_type:
- schema
ms.assetid: 199d1839-f061-4070-a977-874b0c08e5be
description: IdOfFolderToShare 要素は、共有されるサーバー上のフォルダーの識別子を表します。
ms.openlocfilehash: 1e3e53819f23bbc5753ac21b9e3ea6593ac4826c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831853"
---
# <a name="idoffoldertoshare"></a><span data-ttu-id="635f7-103">IdOfFolderToShare</span><span class="sxs-lookup"><span data-stu-id="635f7-103">IdOfFolderToShare</span></span>

<span data-ttu-id="635f7-104">**IdOfFolderToShare**要素は、共有されるサーバー上のフォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="635f7-104">The **IdOfFolderToShare** element represents the identifier of the folder on the server that will be shared.</span></span> 
  
```
<IdOfFolderToShare Id="" ChangeKey="" />
```

 <span data-ttu-id="635f7-105">**FolderIdType**</span><span class="sxs-lookup"><span data-stu-id="635f7-105">**FolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="635f7-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="635f7-106">Attributes and elements</span></span>

<span data-ttu-id="635f7-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="635f7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="635f7-108">属性</span><span class="sxs-lookup"><span data-stu-id="635f7-108">Attributes</span></span>

|<span data-ttu-id="635f7-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="635f7-109">**Attribute**</span></span>|<span data-ttu-id="635f7-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="635f7-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="635f7-111">ID</span><span class="sxs-lookup"><span data-stu-id="635f7-111">Id</span></span>  <br/> |<span data-ttu-id="635f7-112">Exchange ストア内のフォルダーを識別する文字列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="635f7-112">Contains a string that identifies a folder in the Exchange store.</span></span> <span data-ttu-id="635f7-113">この属性は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="635f7-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="635f7-114">ChangeKey</span><span class="sxs-lookup"><span data-stu-id="635f7-114">ChangeKey</span></span>  <br/> |<span data-ttu-id="635f7-115">Id 属性によって識別されるフォルダーのバージョンを識別する文字列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="635f7-115">Contains a string that identifies a version of a folder that is identified by the Id attribute.</span></span> <span data-ttu-id="635f7-116">この属性は、省略可能です。</span><span class="sxs-lookup"><span data-stu-id="635f7-116">This attribute is optional.</span></span> <span data-ttu-id="635f7-117">フォルダーの正しいバージョンを使用するかどうかを確認するには、この属性を使用します。</span><span class="sxs-lookup"><span data-stu-id="635f7-117">Use this attribute to make sure that the correct version of a folder is used.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="635f7-118">子要素</span><span class="sxs-lookup"><span data-stu-id="635f7-118">Child elements</span></span>

<span data-ttu-id="635f7-119">なし。</span><span class="sxs-lookup"><span data-stu-id="635f7-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="635f7-120">親要素</span><span class="sxs-lookup"><span data-stu-id="635f7-120">Parent elements</span></span>

|<span data-ttu-id="635f7-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="635f7-121">**Element**</span></span>|<span data-ttu-id="635f7-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="635f7-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="635f7-123">GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="635f7-123">GetSharingMetadata</span></span>](getsharingmetadata.md) <br/> |<span data-ttu-id="635f7-124">共有への招待を識別する不透明な認証トークンを取得する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="635f7-124">Defines a request to get an opaque authentication token that identifies the sharing invitation.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="635f7-125">備考</span><span class="sxs-lookup"><span data-stu-id="635f7-125">Remarks</span></span>

<span data-ttu-id="635f7-126">この要素を記述するスキーマは、Microsoft Exchange Server を実行しているコンピューターの Exchange Web サービスをホストにクライアント アクセス サーバーの役割がインストールされている IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="635f7-126">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="635f7-127">要素情報</span><span class="sxs-lookup"><span data-stu-id="635f7-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="635f7-128">名前空間</span><span class="sxs-lookup"><span data-stu-id="635f7-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="635f7-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="635f7-129">Schema Name</span></span>  <br/> |<span data-ttu-id="635f7-130">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="635f7-130">Messages schema</span></span>  <br/> |
|<span data-ttu-id="635f7-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="635f7-131">Validation File</span></span>  <br/> |<span data-ttu-id="635f7-132">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="635f7-132">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="635f7-133">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="635f7-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="635f7-134">False</span><span class="sxs-lookup"><span data-stu-id="635f7-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="635f7-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="635f7-135">See also</span></span>



[<span data-ttu-id="635f7-136">GetSharingMetadata 操作</span><span class="sxs-lookup"><span data-stu-id="635f7-136">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)


- [<span data-ttu-id="635f7-137">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="635f7-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

