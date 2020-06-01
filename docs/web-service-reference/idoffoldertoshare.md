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
ms.openlocfilehash: 93a4740d9adefbb35aae071f0a6bfcb4b2021b4d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457628"
---
# <a name="idoffoldertoshare"></a><span data-ttu-id="efbfe-103">IdOfFolderToShare</span><span class="sxs-lookup"><span data-stu-id="efbfe-103">IdOfFolderToShare</span></span>

<span data-ttu-id="efbfe-104">**IdOfFolderToShare**要素は、共有されるサーバー上のフォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="efbfe-104">The **IdOfFolderToShare** element represents the identifier of the folder on the server that will be shared.</span></span> 
  
```
<IdOfFolderToShare Id="" ChangeKey="" />
```

 <span data-ttu-id="efbfe-105">**FolderIdType**</span><span class="sxs-lookup"><span data-stu-id="efbfe-105">**FolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="efbfe-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="efbfe-106">Attributes and elements</span></span>

<span data-ttu-id="efbfe-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="efbfe-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="efbfe-108">属性</span><span class="sxs-lookup"><span data-stu-id="efbfe-108">Attributes</span></span>

|<span data-ttu-id="efbfe-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="efbfe-109">**Attribute**</span></span>|<span data-ttu-id="efbfe-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="efbfe-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="efbfe-111">ID</span><span class="sxs-lookup"><span data-stu-id="efbfe-111">Id</span></span>  <br/> |<span data-ttu-id="efbfe-112">Exchange ストア内のフォルダーを識別する文字列を格納します。</span><span class="sxs-lookup"><span data-stu-id="efbfe-112">Contains a string that identifies a folder in the Exchange store.</span></span> <span data-ttu-id="efbfe-113">この属性は必須です。</span><span class="sxs-lookup"><span data-stu-id="efbfe-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="efbfe-114">ChangeKey</span><span class="sxs-lookup"><span data-stu-id="efbfe-114">ChangeKey</span></span>  <br/> |<span data-ttu-id="efbfe-115">Id 属性によって識別されるフォルダーのバージョンを識別する文字列を格納します。</span><span class="sxs-lookup"><span data-stu-id="efbfe-115">Contains a string that identifies a version of a folder that is identified by the Id attribute.</span></span> <span data-ttu-id="efbfe-116">この属性は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="efbfe-116">This attribute is optional.</span></span> <span data-ttu-id="efbfe-117">この属性を使用して、適切なバージョンのフォルダーが使用されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="efbfe-117">Use this attribute to make sure that the correct version of a folder is used.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="efbfe-118">子要素</span><span class="sxs-lookup"><span data-stu-id="efbfe-118">Child elements</span></span>

<span data-ttu-id="efbfe-119">なし。</span><span class="sxs-lookup"><span data-stu-id="efbfe-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="efbfe-120">親要素</span><span class="sxs-lookup"><span data-stu-id="efbfe-120">Parent elements</span></span>

|<span data-ttu-id="efbfe-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="efbfe-121">**Element**</span></span>|<span data-ttu-id="efbfe-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="efbfe-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="efbfe-123">GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="efbfe-123">GetSharingMetadata</span></span>](getsharingmetadata.md) <br/> |<span data-ttu-id="efbfe-124">共有への招待を識別する非透過の認証トークンを取得する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="efbfe-124">Defines a request to get an opaque authentication token that identifies the sharing invitation.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="efbfe-125">注釈</span><span class="sxs-lookup"><span data-stu-id="efbfe-125">Remarks</span></span>

<span data-ttu-id="efbfe-126">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="efbfe-126">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="efbfe-127">要素の情報</span><span class="sxs-lookup"><span data-stu-id="efbfe-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="efbfe-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="efbfe-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="efbfe-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="efbfe-129">Schema Name</span></span>  <br/> |<span data-ttu-id="efbfe-130">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="efbfe-130">Messages schema</span></span>  <br/> |
|<span data-ttu-id="efbfe-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="efbfe-131">Validation File</span></span>  <br/> |<span data-ttu-id="efbfe-132">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="efbfe-132">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="efbfe-133">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="efbfe-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="efbfe-134">正しくない</span><span class="sxs-lookup"><span data-stu-id="efbfe-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="efbfe-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="efbfe-135">See also</span></span>



[<span data-ttu-id="efbfe-136">GetSharingMetadata 操作</span><span class="sxs-lookup"><span data-stu-id="efbfe-136">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)


- [<span data-ttu-id="efbfe-137">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="efbfe-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

