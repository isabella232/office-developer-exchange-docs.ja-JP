---
title: CreateManagedFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateManagedFolder
api_type:
- schema
ms.assetid: cfdf01a9-0191-47c7-a7ad-5254d8bdee4a
description: CreateManagedFolder 要素は、メールボックスに管理されたカスタム フォルダーを追加する要求を定義します。
ms.openlocfilehash: 4acc931de2a8665db092c3b309d914f0a3c67558
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759850"
---
# <a name="createmanagedfolder"></a><span data-ttu-id="72876-103">CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="72876-103">CreateManagedFolder</span></span>

<span data-ttu-id="72876-104">**CreateManagedFolder**要素は、メールボックスに管理されたカスタム フォルダーを追加する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="72876-104">The **CreateManagedFolder** element defines a request to add managed custom folders to a mailbox.</span></span> 
  
```xml
<CreateManagedFolder>
   <FolderNames/>
   <Mailbox/>
</CreateManagedFolder>
```

 <span data-ttu-id="72876-105">**CreateManagedFolderRequestType**</span><span class="sxs-lookup"><span data-stu-id="72876-105">**CreateManagedFolderRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="72876-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="72876-106">Attributes and elements</span></span>

<span data-ttu-id="72876-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="72876-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="72876-108">属性</span><span class="sxs-lookup"><span data-stu-id="72876-108">Attributes</span></span>

<span data-ttu-id="72876-109">なし。</span><span class="sxs-lookup"><span data-stu-id="72876-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="72876-110">子要素</span><span class="sxs-lookup"><span data-stu-id="72876-110">Child elements</span></span>

|<span data-ttu-id="72876-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="72876-111">**Element**</span></span>|<span data-ttu-id="72876-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="72876-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="72876-113">表示</span><span class="sxs-lookup"><span data-stu-id="72876-113">FolderNames</span></span>](foldernames.md) <br/> |<span data-ttu-id="72876-114">メールボックスに追加するのには管理対象のフォルダーを名前付きの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="72876-114">Contains an array of named managed folders to add to a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="72876-115">メールボックス</span><span class="sxs-lookup"><span data-stu-id="72876-115">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="72876-116">メールが有効な Active Directory ディレクトリ サービス オブジェクトを識別します。</span><span class="sxs-lookup"><span data-stu-id="72876-116">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="72876-117">親要素</span><span class="sxs-lookup"><span data-stu-id="72876-117">Parent elements</span></span>

<span data-ttu-id="72876-118">なし。</span><span class="sxs-lookup"><span data-stu-id="72876-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="72876-119">備考</span><span class="sxs-lookup"><span data-stu-id="72876-119">Remarks</span></span>

<span data-ttu-id="72876-120">要求を行っているユーザーのアカウントによっては、メールボックスの管理フォルダーが作成される場所に FullAccess アクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="72876-120">The account of the person who is making the request must have FullAccess permissions on the mailbox where the managed folders are created.</span></span> <span data-ttu-id="72876-121">**追加 MailboxPermission**の Exchange 管理シェル コマンドレットで・ ・ アクセス権の _ _ パラメーターを使用するには FullAccess アクセス許可を割り当てるには。</span><span class="sxs-lookup"><span data-stu-id="72876-121">You can use the _ -AccessRights _ parameter with the Exchange Management Shell **Add-MailboxPermission** cmdlet to assign the FullAccess permission.</span></span> 
  
<span data-ttu-id="72876-122">メールボックスに管理フォルダーを追加するのには、Exchange Web サービスを使用できますが、使用可能な管理対象フォルダーの一覧にアクセスするのには Exchange Web サービスを使うことはできません。</span><span class="sxs-lookup"><span data-stu-id="72876-122">Although you can use Exchange Web Services to add managed folders to a mailbox, you cannot use Exchange Web Services to access the list of managed folders that are available.</span></span> <span data-ttu-id="72876-123">使用可能な管理対象フォルダーの一覧を取得するには、 **get managedfolder**の Exchange 管理シェル コマンドレットを使用します。</span><span class="sxs-lookup"><span data-stu-id="72876-123">To obtain a list of available managed folders, use the **get-managedfolder** Exchange Management Shell cmdlet.</span></span> <span data-ttu-id="72876-124">**Get managedfolder コマンドレット**によって返されるリストは、管理されたカスタム フォルダーおよび管理された既定フォルダーの両方に含まれます。</span><span class="sxs-lookup"><span data-stu-id="72876-124">The list that is returned by the **get-managedfolder cmdlet** will contain both managed custom folders and managed default folders.</span></span> <span data-ttu-id="72876-125">CreateManagedFolder オペレーションを使用してメールボックスにのみ型の**managedcustomfolder**のフォルダーを追加できます。</span><span class="sxs-lookup"><span data-stu-id="72876-125">You can only add folders of type **managedcustomfolder** to the mailbox by using the CreateManagedFolder operation.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="72876-126">管理対象フォルダーの一覧は、Microsoft.NET Framework のつ API を使用しても取得できます。</span><span class="sxs-lookup"><span data-stu-id="72876-126">You can also get a list of managed folders by using the DirectoryServices API of the Microsoft .NET Framework.</span></span> 
  
<span data-ttu-id="72876-127">[FindFolder 操作](findfolder-operation.md)を使用すると、メールボックス内の管理フォルダーを検索します。</span><span class="sxs-lookup"><span data-stu-id="72876-127">You can use the [FindFolder operation](findfolder-operation.md) to find managed folders in a mailbox.</span></span> <span data-ttu-id="72876-128">管理フォルダーは、要求に[BaseShape](baseshape.md)の要素を AllProperties に設定することで区別できます。</span><span class="sxs-lookup"><span data-stu-id="72876-128">Managed folders can be distinguished by setting the [BaseShape](baseshape.md) element to AllProperties in the request.</span></span> <span data-ttu-id="72876-129">応答は、Exchange ストアのフォルダーから管理対象のフォルダーを識別するために[ManagedFolderInformation](managedfolderinformation.md)の要素に含まれます。</span><span class="sxs-lookup"><span data-stu-id="72876-129">The response will contain a [ManagedFolderInformation](managedfolderinformation.md) element to distinguish the managed folders from the Exchange store folders.</span></span> <span data-ttu-id="72876-130">その他の種類のフォルダーを削除することと同じ方法で管理対象のフォルダーを削除できます。</span><span class="sxs-lookup"><span data-stu-id="72876-130">You can delete managed folders in the same manner that you delete other folder types.</span></span> 
  
<span data-ttu-id="72876-131">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="72876-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="72876-132">要素情報</span><span class="sxs-lookup"><span data-stu-id="72876-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="72876-133">名前空間</span><span class="sxs-lookup"><span data-stu-id="72876-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="72876-134">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="72876-134">Schema Name</span></span>  <br/> |<span data-ttu-id="72876-135">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="72876-135">Messages schema</span></span>  <br/> |
|<span data-ttu-id="72876-136">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="72876-136">Validation File</span></span>  <br/> |<span data-ttu-id="72876-137">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="72876-137">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="72876-138">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="72876-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="72876-139">False</span><span class="sxs-lookup"><span data-stu-id="72876-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="72876-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="72876-140">See also</span></span>



[<span data-ttu-id="72876-141">CreateManagedFolder 操作</span><span class="sxs-lookup"><span data-stu-id="72876-141">CreateManagedFolder operation</span></span>](createmanagedfolder-operation.md)
  
<span data-ttu-id="72876-142">
  [FindFolder 操作](findfolder-operation.md)</span><span class="sxs-lookup"><span data-stu-id="72876-142">[FindFolder operation](findfolder-operation.md)</span></span>


[<span data-ttu-id="72876-143">フォルダーを検索します。</span><span class="sxs-lookup"><span data-stu-id="72876-143">Finding Folders</span></span>](http://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)
  
[<span data-ttu-id="72876-144">管理フォルダーを追加します。</span><span class="sxs-lookup"><span data-stu-id="72876-144">Adding Managed Folders</span></span>](http://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

