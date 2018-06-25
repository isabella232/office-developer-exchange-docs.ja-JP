---
title: FolderName
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FolderName
api_type:
- schema
ms.assetid: c5a2cd55-ac47-43bf-94b5-3ab3a4c28a62
description: フォルダー名の要素は、管理されたカスタム フォルダーをメールボックスに追加するを指定します。
ms.openlocfilehash: 56a7a7d256624c5103c88a333222807519d21501
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760571"
---
# <a name="foldername"></a><span data-ttu-id="03f1c-103">FolderName</span><span class="sxs-lookup"><span data-stu-id="03f1c-103">FolderName</span></span>

<span data-ttu-id="03f1c-104">**フォルダー名**の要素は、管理されたカスタム フォルダーをメールボックスに追加するを指定します。</span><span class="sxs-lookup"><span data-stu-id="03f1c-104">The **FolderName** element identifies a single managed custom folder to add to a mailbox.</span></span> 
  
[<span data-ttu-id="03f1c-105">CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="03f1c-105">CreateManagedFolder</span></span>](createmanagedfolder.md)
  
[<span data-ttu-id="03f1c-106">表示</span><span class="sxs-lookup"><span data-stu-id="03f1c-106">FolderNames</span></span>](foldernames.md)
  
[<span data-ttu-id="03f1c-107">フォルダー名</span><span class="sxs-lookup"><span data-stu-id="03f1c-107">FolderName</span></span>](foldername.md)
  
```xml
<FolderName>...</FolderName>
```

 <span data-ttu-id="03f1c-108">**string**</span><span class="sxs-lookup"><span data-stu-id="03f1c-108">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="03f1c-109">属性および要素</span><span class="sxs-lookup"><span data-stu-id="03f1c-109">Attributes and elements</span></span>

<span data-ttu-id="03f1c-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="03f1c-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="03f1c-111">属性</span><span class="sxs-lookup"><span data-stu-id="03f1c-111">Attributes</span></span>

<span data-ttu-id="03f1c-112">なし。</span><span class="sxs-lookup"><span data-stu-id="03f1c-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="03f1c-113">子要素</span><span class="sxs-lookup"><span data-stu-id="03f1c-113">Child elements</span></span>

<span data-ttu-id="03f1c-114">なし。</span><span class="sxs-lookup"><span data-stu-id="03f1c-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="03f1c-115">親要素</span><span class="sxs-lookup"><span data-stu-id="03f1c-115">Parent elements</span></span>

|<span data-ttu-id="03f1c-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="03f1c-116">**Element**</span></span>|<span data-ttu-id="03f1c-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="03f1c-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="03f1c-118">表示</span><span class="sxs-lookup"><span data-stu-id="03f1c-118">FolderNames</span></span>](foldernames.md) <br/> |<span data-ttu-id="03f1c-119">メールボックスに追加するのには管理されたカスタム フォルダーの名前付きの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="03f1c-119">Contains an array of named managed custom folders to add to a mailbox.</span></span>  <br/> <span data-ttu-id="03f1c-120">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="03f1c-120">The following is the XPath expression to this element:</span></span>  <br/>  `/CreateManagedFolder/FolderNames` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="03f1c-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="03f1c-121">Text value</span></span>

<span data-ttu-id="03f1c-122">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="03f1c-122">A text value is required.</span></span> <span data-ttu-id="03f1c-123">テキスト値は、フォルダー名を表します。</span><span class="sxs-lookup"><span data-stu-id="03f1c-123">The text value represents a folder name.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="03f1c-124">備考</span><span class="sxs-lookup"><span data-stu-id="03f1c-124">Remarks</span></span>

<span data-ttu-id="03f1c-125">メールボックスに管理されたカスタム フォルダーを追加するのには、Exchange Web サービスを使用できますが、利用可能な管理されたカスタム フォルダーの一覧にアクセスするのと同じテクノロジーを使うことはできません。</span><span class="sxs-lookup"><span data-stu-id="03f1c-125">Although you can use Exchange Web Services to add managed custom folders to a mailbox, you cannot use the same technology to access the list of available managed custom folders.</span></span> <span data-ttu-id="03f1c-126">管理されたカスタム フォルダーの一覧を取得するには、Exchange 管理シェル コマンドを使用して、Active Directory ディレクトリ サービス インターフェイスの API を使用しています。</span><span class="sxs-lookup"><span data-stu-id="03f1c-126">You can obtain a list of managed custom folders by using an Exchange Management Shell command or by using an API that interfaces with the Active Directory directory service.</span></span> <span data-ttu-id="03f1c-127">フォルダー名は、対応する Active Directory オブジェクトの名前です。</span><span class="sxs-lookup"><span data-stu-id="03f1c-127">The folder name is the name of the corresponding Active Directory object.</span></span>
  
<span data-ttu-id="03f1c-128">[FindFolder 操作](findfolder-operation.md)を使用すると、管理されたカスタム フォルダーを検索します。</span><span class="sxs-lookup"><span data-stu-id="03f1c-128">You can use the [FindFolder operation](findfolder-operation.md) to find managed custom folders.</span></span> <span data-ttu-id="03f1c-129">管理されたカスタム フォルダーを削除するのには[DeleteFolder 操作](deletefolder-operation.md)を使用します。</span><span class="sxs-lookup"><span data-stu-id="03f1c-129">Use the [DeleteFolder operation](deletefolder-operation.md) to delete managed custom folders.</span></span> 
  
<span data-ttu-id="03f1c-130">**フォルダー名**が、組織の既存の管理されたカスタム フォルダーの名前であることを確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="03f1c-130">It is important to note that **FolderName** is the name of an existing managed custom folder in the organization.</span></span> <span data-ttu-id="03f1c-131">組織に含まれていないフォルダーを追加しようとすると、エラー応答になります。</span><span class="sxs-lookup"><span data-stu-id="03f1c-131">An attempt to add a folder that is not in the organization will result in an error response.</span></span> 
  
<span data-ttu-id="03f1c-132">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="03f1c-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="03f1c-133">要素情報</span><span class="sxs-lookup"><span data-stu-id="03f1c-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="03f1c-134">名前空間</span><span class="sxs-lookup"><span data-stu-id="03f1c-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="03f1c-135">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="03f1c-135">Schema Name</span></span>  <br/> |<span data-ttu-id="03f1c-136">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="03f1c-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="03f1c-137">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="03f1c-137">Validation File</span></span>  <br/> |<span data-ttu-id="03f1c-138">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="03f1c-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="03f1c-139">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="03f1c-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="03f1c-140">False</span><span class="sxs-lookup"><span data-stu-id="03f1c-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="03f1c-141">関連項目</span><span class="sxs-lookup"><span data-stu-id="03f1c-141">See also</span></span>



<span data-ttu-id="03f1c-142">
  [FindFolder 操作](findfolder-operation.md)</span><span class="sxs-lookup"><span data-stu-id="03f1c-142">[FindFolder operation](findfolder-operation.md)</span></span>


[<span data-ttu-id="03f1c-143">フォルダーを検索します。</span><span class="sxs-lookup"><span data-stu-id="03f1c-143">Finding Folders</span></span>](http://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)
  
[<span data-ttu-id="03f1c-144">管理フォルダーを追加します。</span><span class="sxs-lookup"><span data-stu-id="03f1c-144">Adding Managed Folders</span></span>](http://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

