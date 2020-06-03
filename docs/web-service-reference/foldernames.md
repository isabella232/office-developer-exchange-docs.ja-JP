---
title: FolderNames
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FolderNames
api_type:
- schema
ms.assetid: 6cbe4083-5705-4695-a54e-8dab3e472662
description: FolderNames 要素には、メールボックスに追加する名前付きの管理フォルダーの配列が含まれています。
ms.openlocfilehash: 00cb1a81f420469033ccbc745313d2719b155aff
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530987"
---
# <a name="foldernames"></a><span data-ttu-id="b3392-103">FolderNames</span><span class="sxs-lookup"><span data-stu-id="b3392-103">FolderNames</span></span>

<span data-ttu-id="b3392-104">**Foldernames**要素には、メールボックスに追加する名前付きの管理フォルダーの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b3392-104">The **FolderNames** element contains an array of named managed folders to add to a mailbox.</span></span> 
  
[<span data-ttu-id="b3392-105">CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="b3392-105">CreateManagedFolder</span></span>](createmanagedfolder.md)
  
[<span data-ttu-id="b3392-106">FolderNames</span><span class="sxs-lookup"><span data-stu-id="b3392-106">FolderNames</span></span>](foldernames.md)
  
```xml
<FolderNames>
   <FolderName/>
</FolderNames>
```

 <span data-ttu-id="b3392-107">**非 Emptyarrayoffoldernamestん**</span><span class="sxs-lookup"><span data-stu-id="b3392-107">**NonEmptyArrayOfFolderNamesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b3392-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="b3392-108">Attributes and elements</span></span>

<span data-ttu-id="b3392-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b3392-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b3392-110">属性</span><span class="sxs-lookup"><span data-stu-id="b3392-110">Attributes</span></span>

<span data-ttu-id="b3392-111">なし。</span><span class="sxs-lookup"><span data-stu-id="b3392-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b3392-112">子要素</span><span class="sxs-lookup"><span data-stu-id="b3392-112">Child elements</span></span>

|<span data-ttu-id="b3392-113">**Element**</span><span class="sxs-lookup"><span data-stu-id="b3392-113">**Element**</span></span>|<span data-ttu-id="b3392-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="b3392-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b3392-115">FolderName</span><span class="sxs-lookup"><span data-stu-id="b3392-115">FolderName</span></span>](foldername.md) <br/> |<span data-ttu-id="b3392-116">メールボックスに追加する単一の管理フォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="b3392-116">Identifies a single managed folder to add to mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b3392-117">親要素</span><span class="sxs-lookup"><span data-stu-id="b3392-117">Parent elements</span></span>

|<span data-ttu-id="b3392-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="b3392-118">**Element**</span></span>|<span data-ttu-id="b3392-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="b3392-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b3392-120">CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="b3392-120">CreateManagedFolder</span></span>](createmanagedfolder.md) <br/> |<span data-ttu-id="b3392-121">メールボックスに管理フォルダーを追加する要求のルート要素。</span><span class="sxs-lookup"><span data-stu-id="b3392-121">The root element in a request to add a managed folder to a mailbox.</span></span>  <br/> <span data-ttu-id="b3392-122">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b3392-122">The following is the XPath expression to this element:</span></span>  <br/>  `/CreateManagedFolder` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b3392-123">注釈</span><span class="sxs-lookup"><span data-stu-id="b3392-123">Remarks</span></span>

<span data-ttu-id="b3392-124">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="b3392-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b3392-125">要素の情報</span><span class="sxs-lookup"><span data-stu-id="b3392-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b3392-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="b3392-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b3392-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b3392-127">Schema Name</span></span>  <br/> |<span data-ttu-id="b3392-128">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="b3392-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b3392-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b3392-129">Validation File</span></span>  <br/> |<span data-ttu-id="b3392-130">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="b3392-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b3392-131">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="b3392-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="b3392-132">正しくない</span><span class="sxs-lookup"><span data-stu-id="b3392-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b3392-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="b3392-133">See also</span></span>



[<span data-ttu-id="b3392-134">FindFolder 操作</span><span class="sxs-lookup"><span data-stu-id="b3392-134">FindFolder operation</span></span>](findfolder-operation.md)


[<span data-ttu-id="b3392-135">フォルダーの検索</span><span class="sxs-lookup"><span data-stu-id="b3392-135">Finding Folders</span></span>](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)
  
[<span data-ttu-id="b3392-136">管理フォルダーの追加</span><span class="sxs-lookup"><span data-stu-id="b3392-136">Adding Managed Folders</span></span>](https://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

