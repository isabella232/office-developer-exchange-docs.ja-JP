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
description: FolderName 要素は、メールボックスに追加する単一の管理されたカスタムフォルダーを識別します。
ms.openlocfilehash: 1bb63e50c06e81337d1142a6624213fb2db12457
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461353"
---
# <a name="foldername"></a><span data-ttu-id="46559-103">FolderName</span><span class="sxs-lookup"><span data-stu-id="46559-103">FolderName</span></span>

<span data-ttu-id="46559-104">**FolderName**要素は、メールボックスに追加する単一の管理されたカスタムフォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="46559-104">The **FolderName** element identifies a single managed custom folder to add to a mailbox.</span></span> 
  
[<span data-ttu-id="46559-105">CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="46559-105">CreateManagedFolder</span></span>](createmanagedfolder.md)
  
[<span data-ttu-id="46559-106">FolderNames</span><span class="sxs-lookup"><span data-stu-id="46559-106">FolderNames</span></span>](foldernames.md)
  
[<span data-ttu-id="46559-107">FolderName</span><span class="sxs-lookup"><span data-stu-id="46559-107">FolderName</span></span>](foldername.md)
  
```xml
<FolderName>...</FolderName>
```

 <span data-ttu-id="46559-108">**string**</span><span class="sxs-lookup"><span data-stu-id="46559-108">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="46559-109">属性と要素</span><span class="sxs-lookup"><span data-stu-id="46559-109">Attributes and elements</span></span>

<span data-ttu-id="46559-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="46559-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="46559-111">属性</span><span class="sxs-lookup"><span data-stu-id="46559-111">Attributes</span></span>

<span data-ttu-id="46559-112">なし。</span><span class="sxs-lookup"><span data-stu-id="46559-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="46559-113">子要素</span><span class="sxs-lookup"><span data-stu-id="46559-113">Child elements</span></span>

<span data-ttu-id="46559-114">なし。</span><span class="sxs-lookup"><span data-stu-id="46559-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="46559-115">親要素</span><span class="sxs-lookup"><span data-stu-id="46559-115">Parent elements</span></span>

|<span data-ttu-id="46559-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="46559-116">**Element**</span></span>|<span data-ttu-id="46559-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="46559-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="46559-118">FolderNames</span><span class="sxs-lookup"><span data-stu-id="46559-118">FolderNames</span></span>](foldernames.md) <br/> |<span data-ttu-id="46559-119">メールボックスに追加する名前付きの管理されたカスタムフォルダーの配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="46559-119">Contains an array of named managed custom folders to add to a mailbox.</span></span>  <br/> <span data-ttu-id="46559-120">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="46559-120">The following is the XPath expression to this element:</span></span>  <br/>  `/CreateManagedFolder/FolderNames` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="46559-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="46559-121">Text value</span></span>

<span data-ttu-id="46559-122">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="46559-122">A text value is required.</span></span> <span data-ttu-id="46559-123">テキスト値はフォルダー名を表します。</span><span class="sxs-lookup"><span data-stu-id="46559-123">The text value represents a folder name.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="46559-124">注釈</span><span class="sxs-lookup"><span data-stu-id="46559-124">Remarks</span></span>

<span data-ttu-id="46559-125">Exchange Web サービスを使用して管理されたカスタムフォルダーをメールボックスに追加することはできますが、同じテクノロジを使用して、使用可能な管理されたカスタムフォルダーの一覧にアクセスすることはできません。</span><span class="sxs-lookup"><span data-stu-id="46559-125">Although you can use Exchange Web Services to add managed custom folders to a mailbox, you cannot use the same technology to access the list of available managed custom folders.</span></span> <span data-ttu-id="46559-126">管理されたカスタムフォルダーの一覧を取得するには、Exchange 管理シェルコマンドを使用するか、Active Directory ディレクトリサービスとのインターフェイスを使用して、API を使用します。</span><span class="sxs-lookup"><span data-stu-id="46559-126">You can obtain a list of managed custom folders by using an Exchange Management Shell command or by using an API that interfaces with the Active Directory directory service.</span></span> <span data-ttu-id="46559-127">フォルダー名は、対応する Active Directory オブジェクトの名前です。</span><span class="sxs-lookup"><span data-stu-id="46559-127">The folder name is the name of the corresponding Active Directory object.</span></span>
  
<span data-ttu-id="46559-128">[Findfolder 操作](findfolder-operation.md)を使用して、管理されたカスタムフォルダーを検索できます。</span><span class="sxs-lookup"><span data-stu-id="46559-128">You can use the [FindFolder operation](findfolder-operation.md) to find managed custom folders.</span></span> <span data-ttu-id="46559-129">管理されたカスタムフォルダーを削除するには、 [Deletefolder 操作](deletefolder-operation.md)を使用します。</span><span class="sxs-lookup"><span data-stu-id="46559-129">Use the [DeleteFolder operation](deletefolder-operation.md) to delete managed custom folders.</span></span> 
  
<span data-ttu-id="46559-130">**FolderName**は、組織内の既存の管理されたカスタムフォルダーの名前であることに注意する必要があります。</span><span class="sxs-lookup"><span data-stu-id="46559-130">It is important to note that **FolderName** is the name of an existing managed custom folder in the organization.</span></span> <span data-ttu-id="46559-131">組織内にないフォルダーを追加しようとすると、エラー応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="46559-131">An attempt to add a folder that is not in the organization will result in an error response.</span></span> 
  
<span data-ttu-id="46559-132">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="46559-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="46559-133">要素の情報</span><span class="sxs-lookup"><span data-stu-id="46559-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="46559-134">Namespace</span><span class="sxs-lookup"><span data-stu-id="46559-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="46559-135">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="46559-135">Schema Name</span></span>  <br/> |<span data-ttu-id="46559-136">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="46559-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="46559-137">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="46559-137">Validation File</span></span>  <br/> |<span data-ttu-id="46559-138">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="46559-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="46559-139">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="46559-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="46559-140">正しくない</span><span class="sxs-lookup"><span data-stu-id="46559-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="46559-141">関連項目</span><span class="sxs-lookup"><span data-stu-id="46559-141">See also</span></span>



[<span data-ttu-id="46559-142">FindFolder 操作</span><span class="sxs-lookup"><span data-stu-id="46559-142">FindFolder operation</span></span>](findfolder-operation.md)


[<span data-ttu-id="46559-143">フォルダーの検索</span><span class="sxs-lookup"><span data-stu-id="46559-143">Finding Folders</span></span>](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)
  
[<span data-ttu-id="46559-144">管理フォルダーの追加</span><span class="sxs-lookup"><span data-stu-id="46559-144">Adding Managed Folders</span></span>](https://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

