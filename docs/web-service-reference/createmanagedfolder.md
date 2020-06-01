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
description: CreateManagedFolder 要素は、管理されたカスタムフォルダーをメールボックスに追加する要求を定義します。
ms.openlocfilehash: 01fe8b7341c38ad33089c56271434ad3f9a4e5f0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458363"
---
# <a name="createmanagedfolder"></a><span data-ttu-id="54efa-103">CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="54efa-103">CreateManagedFolder</span></span>

<span data-ttu-id="54efa-104">**CreateManagedFolder**要素は、管理されたカスタムフォルダーをメールボックスに追加する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="54efa-104">The **CreateManagedFolder** element defines a request to add managed custom folders to a mailbox.</span></span> 
  
```xml
<CreateManagedFolder>
   <FolderNames/>
   <Mailbox/>
</CreateManagedFolder>
```

 <span data-ttu-id="54efa-105">**CreateManagedFolderRequestType**</span><span class="sxs-lookup"><span data-stu-id="54efa-105">**CreateManagedFolderRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="54efa-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="54efa-106">Attributes and elements</span></span>

<span data-ttu-id="54efa-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="54efa-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="54efa-108">属性</span><span class="sxs-lookup"><span data-stu-id="54efa-108">Attributes</span></span>

<span data-ttu-id="54efa-109">なし。</span><span class="sxs-lookup"><span data-stu-id="54efa-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="54efa-110">子要素</span><span class="sxs-lookup"><span data-stu-id="54efa-110">Child elements</span></span>

|<span data-ttu-id="54efa-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="54efa-111">**Element**</span></span>|<span data-ttu-id="54efa-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="54efa-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="54efa-113">FolderNames</span><span class="sxs-lookup"><span data-stu-id="54efa-113">FolderNames</span></span>](foldernames.md) <br/> |<span data-ttu-id="54efa-114">メールボックスに追加する名前付きの管理フォルダーの配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="54efa-114">Contains an array of named managed folders to add to a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="54efa-115">メールボックス</span><span class="sxs-lookup"><span data-stu-id="54efa-115">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="54efa-116">メールが有効な Active Directory ディレクトリサービスオブジェクトを識別します。</span><span class="sxs-lookup"><span data-stu-id="54efa-116">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="54efa-117">親要素</span><span class="sxs-lookup"><span data-stu-id="54efa-117">Parent elements</span></span>

<span data-ttu-id="54efa-118">なし。</span><span class="sxs-lookup"><span data-stu-id="54efa-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="54efa-119">注釈</span><span class="sxs-lookup"><span data-stu-id="54efa-119">Remarks</span></span>

<span data-ttu-id="54efa-120">要求を行っているユーザーのアカウントは、管理フォルダーが作成されたメールボックスに対して FullAccess アクセス許可を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="54efa-120">The account of the person who is making the request must have FullAccess permissions on the mailbox where the managed folders are created.</span></span> <span data-ttu-id="54efa-121">Exchange 管理シェル**add-mailboxpermission**コマンドレットを使用して、フルアクセスのアクセス許可を割り当てることができます。</span><span class="sxs-lookup"><span data-stu-id="54efa-121">You can use the _ -AccessRights _ parameter with the Exchange Management Shell **Add-MailboxPermission** cmdlet to assign the FullAccess permission.</span></span> 
  
<span data-ttu-id="54efa-122">Exchange Web サービスを使用して管理フォルダーをメールボックスに追加することはできますが、使用可能な管理フォルダーの一覧に Exchange Web サービスを使用してアクセスすることはできません。</span><span class="sxs-lookup"><span data-stu-id="54efa-122">Although you can use Exchange Web Services to add managed folders to a mailbox, you cannot use Exchange Web Services to access the list of managed folders that are available.</span></span> <span data-ttu-id="54efa-123">利用可能な管理フォルダーの一覧を取得するには、Exchange 管理シェルコマンドレットの**取得**を使用します。</span><span class="sxs-lookup"><span data-stu-id="54efa-123">To obtain a list of available managed folders, use the **get-managedfolder** Exchange Management Shell cmdlet.</span></span> <span data-ttu-id="54efa-124">**Managedfolder コマンドレット**によって返されるリストには、管理されたカスタムフォルダーと管理された既定のフォルダーの両方が含まれます。</span><span class="sxs-lookup"><span data-stu-id="54efa-124">The list that is returned by the **get-managedfolder cmdlet** will contain both managed custom folders and managed default folders.</span></span> <span data-ttu-id="54efa-125">CreateManagedFolder 操作を使用して、 **managedcustomfolder**型のフォルダーのみをメールボックスに追加できます。</span><span class="sxs-lookup"><span data-stu-id="54efa-125">You can only add folders of type **managedcustomfolder** to the mailbox by using the CreateManagedFolder operation.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="54efa-126">また、Microsoft .NET Framework の System.directoryservices API を使用して、管理フォルダーの一覧を取得することもできます。</span><span class="sxs-lookup"><span data-stu-id="54efa-126">You can also get a list of managed folders by using the DirectoryServices API of the Microsoft .NET Framework.</span></span> 
  
<span data-ttu-id="54efa-127">[Findfolder 操作](findfolder-operation.md)を使用して、メールボックス内の管理されたフォルダーを検索できます。</span><span class="sxs-lookup"><span data-stu-id="54efa-127">You can use the [FindFolder operation](findfolder-operation.md) to find managed folders in a mailbox.</span></span> <span data-ttu-id="54efa-128">管理フォルダーは、 [Baseshape](baseshape.md)要素を要求の allproperties に設定することで区別できます。</span><span class="sxs-lookup"><span data-stu-id="54efa-128">Managed folders can be distinguished by setting the [BaseShape](baseshape.md) element to AllProperties in the request.</span></span> <span data-ttu-id="54efa-129">応答には、管理フォルダーを Exchange ストアフォルダーから区別する[Managedfolderinformation](managedfolderinformation.md)要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="54efa-129">The response will contain a [ManagedFolderInformation](managedfolderinformation.md) element to distinguish the managed folders from the Exchange store folders.</span></span> <span data-ttu-id="54efa-130">他のフォルダーの種類を削除するのと同じ方法で、管理フォルダーを削除することができます。</span><span class="sxs-lookup"><span data-stu-id="54efa-130">You can delete managed folders in the same manner that you delete other folder types.</span></span> 
  
<span data-ttu-id="54efa-131">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="54efa-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="54efa-132">要素の情報</span><span class="sxs-lookup"><span data-stu-id="54efa-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="54efa-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="54efa-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="54efa-134">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="54efa-134">Schema Name</span></span>  <br/> |<span data-ttu-id="54efa-135">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="54efa-135">Messages schema</span></span>  <br/> |
|<span data-ttu-id="54efa-136">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="54efa-136">Validation File</span></span>  <br/> |<span data-ttu-id="54efa-137">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="54efa-137">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="54efa-138">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="54efa-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="54efa-139">正しくない</span><span class="sxs-lookup"><span data-stu-id="54efa-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="54efa-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="54efa-140">See also</span></span>



[<span data-ttu-id="54efa-141">CreateManagedFolder 操作</span><span class="sxs-lookup"><span data-stu-id="54efa-141">CreateManagedFolder operation</span></span>](createmanagedfolder-operation.md)
  
<span data-ttu-id="54efa-142">
  [FindFolder 操作](findfolder-operation.md)</span><span class="sxs-lookup"><span data-stu-id="54efa-142">[FindFolder operation](findfolder-operation.md)</span></span>


[<span data-ttu-id="54efa-143">フォルダーの検索</span><span class="sxs-lookup"><span data-stu-id="54efa-143">Finding Folders</span></span>](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)
  
[<span data-ttu-id="54efa-144">管理フォルダーの追加</span><span class="sxs-lookup"><span data-stu-id="54efa-144">Adding Managed Folders</span></span>](https://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

