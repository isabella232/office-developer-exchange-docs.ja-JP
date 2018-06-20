---
title: 表示
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
description: 表示要素には、メールボックスに追加するのには管理対象のフォルダーを名前付きの配列が含まれています。
ms.openlocfilehash: 819b3c2df1cfcae3a5d4a48539e369a00b1f7229
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760568"
---
# <a name="foldernames"></a><span data-ttu-id="4678f-103">表示</span><span class="sxs-lookup"><span data-stu-id="4678f-103">FolderNames</span></span>

<span data-ttu-id="4678f-104">**表示**要素には、メールボックスに追加するのには管理対象のフォルダーを名前付きの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="4678f-104">The **FolderNames** element contains an array of named managed folders to add to a mailbox.</span></span> 
  
[<span data-ttu-id="4678f-105">CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="4678f-105">CreateManagedFolder</span></span>](createmanagedfolder.md)
  
[<span data-ttu-id="4678f-106">表示</span><span class="sxs-lookup"><span data-stu-id="4678f-106">FolderNames</span></span>](foldernames.md)
  
```xml
<FolderNames>
   <FolderName/>
</FolderNames>
```

 <span data-ttu-id="4678f-107">**NonEmptyArrayOfFolderNamesType**</span><span class="sxs-lookup"><span data-stu-id="4678f-107">**NonEmptyArrayOfFolderNamesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4678f-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="4678f-108">Attributes and elements</span></span>

<span data-ttu-id="4678f-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4678f-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4678f-110">属性</span><span class="sxs-lookup"><span data-stu-id="4678f-110">Attributes</span></span>

<span data-ttu-id="4678f-111">なし。</span><span class="sxs-lookup"><span data-stu-id="4678f-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4678f-112">子要素</span><span class="sxs-lookup"><span data-stu-id="4678f-112">Child elements</span></span>

|<span data-ttu-id="4678f-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="4678f-113">**Element**</span></span>|<span data-ttu-id="4678f-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="4678f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4678f-115">フォルダー名</span><span class="sxs-lookup"><span data-stu-id="4678f-115">FolderName</span></span>](foldername.md) <br/> |<span data-ttu-id="4678f-116">メールボックスに追加するのには 1 つの管理フォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="4678f-116">Identifies a single managed folder to add to mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4678f-117">親要素</span><span class="sxs-lookup"><span data-stu-id="4678f-117">Parent elements</span></span>

|<span data-ttu-id="4678f-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="4678f-118">**Element**</span></span>|<span data-ttu-id="4678f-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="4678f-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4678f-120">CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="4678f-120">CreateManagedFolder</span></span>](createmanagedfolder.md) <br/> |<span data-ttu-id="4678f-121">メールボックスに管理フォルダーを追加する要求のルート要素です。</span><span class="sxs-lookup"><span data-stu-id="4678f-121">The root element in a request to add a managed folder to a mailbox.</span></span>  <br/> <span data-ttu-id="4678f-122">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="4678f-122">The following is the XPath expression to this element:</span></span>  <br/>  `/CreateManagedFolder` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4678f-123">備考</span><span class="sxs-lookup"><span data-stu-id="4678f-123">Remarks</span></span>

<span data-ttu-id="4678f-124">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="4678f-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4678f-125">要素情報</span><span class="sxs-lookup"><span data-stu-id="4678f-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4678f-126">名前空間</span><span class="sxs-lookup"><span data-stu-id="4678f-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4678f-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4678f-127">Schema Name</span></span>  <br/> |<span data-ttu-id="4678f-128">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="4678f-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4678f-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4678f-129">Validation File</span></span>  <br/> |<span data-ttu-id="4678f-130">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="4678f-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4678f-131">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="4678f-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="4678f-132">False</span><span class="sxs-lookup"><span data-stu-id="4678f-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4678f-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="4678f-133">See also</span></span>



<span data-ttu-id="4678f-134">
  [FindFolder 操作](findfolder-operation.md)</span><span class="sxs-lookup"><span data-stu-id="4678f-134">[FindFolder operation](findfolder-operation.md)</span></span>


[<span data-ttu-id="4678f-135">フォルダーを検索します。</span><span class="sxs-lookup"><span data-stu-id="4678f-135">Finding Folders</span></span>](http://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)
  
[<span data-ttu-id="4678f-136">管理フォルダーを追加します。</span><span class="sxs-lookup"><span data-stu-id="4678f-136">Adding Managed Folders</span></span>](http://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

