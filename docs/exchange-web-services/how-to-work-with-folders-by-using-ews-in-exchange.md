---
title: Exchange で EWS を使用してフォルダーを操作する
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 4b3eb746-74c4-42a0-aa2c-742c147f1871
description: Exchange で EWS マネージ API または EWS を使用して、フォルダーを作成、取得、更新、削除する方法について説明します。
ms.openlocfilehash: a9a9e5974b2751268f37a1c9faacce43a333bcdb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759091"
---
# <a name="work-with-folders-by-using-ews-in-exchange"></a><span data-ttu-id="f6e50-103">Exchange で EWS を使用してフォルダーを操作する</span><span class="sxs-lookup"><span data-stu-id="f6e50-103">How to: Work with folders by using EWS in Exchange</span></span>

<span data-ttu-id="f6e50-104">Exchange で EWS マネージ API または EWS を使用して、フォルダーを作成、取得、更新、削除する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="f6e50-104">Learn how to create, get, update, and delete folders by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="f6e50-105">Exchange の EWS は、フォルダーを使用してメールボックスの構成と整理を行います。</span><span class="sxs-lookup"><span data-stu-id="f6e50-105">EWS in Exchange uses folders to structure and organize mailboxes.</span></span> <span data-ttu-id="f6e50-106">EWS マネージ API または EWS を使用して、フォルダーを新規作成、取得、更新、削除できます。</span><span class="sxs-lookup"><span data-stu-id="f6e50-106">Learn how to create, get, update, and delete folders by using the EWS Managed API or EWS in Exchange.</span></span> <span data-ttu-id="f6e50-107">次の表にまとめられている各メソッドまたは操作は、[Folder](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx) オブジェクト、[Folder](http://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) タイプ、または[いずれかの派生 Folder クラスまたはタイプ](folders-and-items-in-ews-in-exchange.md#bk_folders)で実行されます。</span><span class="sxs-lookup"><span data-stu-id="f6e50-107">Each of the methods or operations listed in the following table is performed on a [Folder](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx) object, a [Folder](http://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) type, or [one of the derived folder classes or types](folders-and-items-in-ews-in-exchange.md#bk_folders).</span></span>
  
<span data-ttu-id="f6e50-108">**表 1. フォルダーを作成、取得、更新、削除するためのメソッドと操作**</span><span class="sxs-lookup"><span data-stu-id="f6e50-108">**Table 1.  Methods and operations for creating, getting, updating and deleting folders**</span></span>

|<span data-ttu-id="f6e50-109">**目的**</span><span class="sxs-lookup"><span data-stu-id="f6e50-109">**In order to…**</span></span>|<span data-ttu-id="f6e50-110">**EWS マネージ API メソッド**</span><span class="sxs-lookup"><span data-stu-id="f6e50-110">**EWS Managed API method**</span></span>|<span data-ttu-id="f6e50-111">**EWS 操作**</span><span class="sxs-lookup"><span data-stu-id="f6e50-111">**EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="f6e50-112">フォルダーの作成</span><span class="sxs-lookup"><span data-stu-id="f6e50-112">Create a folder</span></span>  <br/> |[<span data-ttu-id="f6e50-113">Folder.Save</span><span class="sxs-lookup"><span data-stu-id="f6e50-113">Folder.Save</span></span>](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="f6e50-114">CreateFolder</span><span class="sxs-lookup"><span data-stu-id="f6e50-114">CreateFolder</span></span>](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="f6e50-115">フォルダー階層の作成</span><span class="sxs-lookup"><span data-stu-id="f6e50-115">Create a folder hierarchy</span></span>  <br/> |<span data-ttu-id="f6e50-116">利用不可</span><span class="sxs-lookup"><span data-stu-id="f6e50-116">Not available</span></span>  <br/> |[<span data-ttu-id="f6e50-117">CreateFolderPath</span><span class="sxs-lookup"><span data-stu-id="f6e50-117">CreateFolderPath</span></span>](http://msdn.microsoft.com/library/5a10aa5e-3f25-4ec3-a0b9-284c30918a1f%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="f6e50-118">フォルダーの取得</span><span class="sxs-lookup"><span data-stu-id="f6e50-118">Get a folder</span></span>  <br/> |[<span data-ttu-id="f6e50-119">Folder.Bind</span><span class="sxs-lookup"><span data-stu-id="f6e50-119">Folder.Bind</span></span>](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="f6e50-120">GetFolder</span><span class="sxs-lookup"><span data-stu-id="f6e50-120">GetFolder</span></span>](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="f6e50-121">フォルダー階層の取得</span><span class="sxs-lookup"><span data-stu-id="f6e50-121">Get a folder hierarchy</span></span>  <br/> |[<span data-ttu-id="f6e50-122">Folder.FindFolders</span><span class="sxs-lookup"><span data-stu-id="f6e50-122">Folder.FindFolders</span></span>](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="f6e50-123">FindFolder</span><span class="sxs-lookup"><span data-stu-id="f6e50-123">FindFolder</span></span>](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="f6e50-124">フォルダーの更新</span><span class="sxs-lookup"><span data-stu-id="f6e50-124">Update a folder</span></span>  <br/> |[<span data-ttu-id="f6e50-125">Folder.Update</span><span class="sxs-lookup"><span data-stu-id="f6e50-125">Folder.Update</span></span>](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="f6e50-126">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="f6e50-126">UpdateFolder</span></span>](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="f6e50-127">フォルダーの削除</span><span class="sxs-lookup"><span data-stu-id="f6e50-127">Delete a folder</span></span>  <br/> |[<span data-ttu-id="f6e50-128">Folder.Delete</span><span class="sxs-lookup"><span data-stu-id="f6e50-128">Folder.Delete Method (Outlook)</span></span>](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="f6e50-129">DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="f6e50-129">DeleteFolder</span></span>](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |

<span data-ttu-id="f6e50-130"><a name="bk_createfolderewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="f6e50-130"></span></span>

## <a name="create-a-folder-by-using-the-ews-managed-api"></a><span data-ttu-id="f6e50-131">EWS マネージ API を使用してフォルダーを作成する</span><span class="sxs-lookup"><span data-stu-id="f6e50-131">Create a folder by using the EWS Managed API</span></span>

<span data-ttu-id="f6e50-132">次のコード例は、[Folder](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx) クラスを使用して、[DisplayName](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.displayname%28v=exchg.80%29.aspx) が「Custom Folder」で [FolderClass](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.folderclass%28v=exchg.80%29.aspx) プロパティ値が IPF.Note の汎用フォルダーを新規作成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="f6e50-132">The following code example shows how to use the [Folder](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx) class to create a new generic folder with a [DisplayName](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.displayname%28v=exchg.80%29.aspx) of "Custom Folder" and a [FolderClass](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.folderclass%28v=exchg.80%29.aspx) property value of IPF.Note.</span></span> <span data-ttu-id="f6e50-133">[Folder.Save](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) メソッドは、受信トレイ フォルダーの子フォルダーとして対象フォルダーを保存します。</span><span class="sxs-lookup"><span data-stu-id="f6e50-133">The [Folder.Save](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) method saves the folder as a child folder of the Inbox folder.</span></span> 
  
<span data-ttu-id="f6e50-134">これらの例では、**service** が有効な [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーは Exchange サーバーに既に認証されていると想定しています。</span><span class="sxs-lookup"><span data-stu-id="f6e50-134">These examples assume that **service** is a valid [ExchangeServicehttp://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice(v=exchg.80).aspx](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
// Create a custom folder.
Folder folder = new Folder(service);
folder.DisplayName = "Custom Folder";
folder.FolderClass = "IPF.Note";
// Save the folder as a child folder of the Inbox.
folder.Save(WellKnownFolderName.Inbox);
```

<span data-ttu-id="f6e50-135">[CalendarFolder](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.calendarfolder%28v=exchg.80%29.aspx)、[ContactsFolder](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.contactsfolder%28v=exchg.80%29.aspx)、[SearchFolder](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx)、[TasksFolder](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.tasksfolder%28v=exchg.80%29.aspx) など異なるタイプのフォルダーを作成するには、特定のクラスの新しいインスタンス (汎用の **Folder** クラスではなく) を作成し、**FolderClass** プロパティは設定しません。</span><span class="sxs-lookup"><span data-stu-id="f6e50-135">To create a different type of folder, such as a [CalendarFolder](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.calendarfolder%28v=exchg.80%29.aspx), [ContactsFolder](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.contactsfolder%28v=exchg.80%29.aspx), [SearchFolder](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx), or [TasksFolder](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.tasksfolder%28v=exchg.80%29.aspx), create a new instance of the specific class (instead of the generic **Folder** class) and do not set the **FolderClass** property.</span></span> <span data-ttu-id="f6e50-136">たとえば、次のコード例は、新しい [TasksFolder](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.tasksfolder%28v=exchg.80%29.aspx) を作成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="f6e50-136">For example, the following code example shows how to create a new [TasksFolder](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.tasksfolder%28v=exchg.80%29.aspx).</span></span>
  
```cs
// Create a custom Tasks folder.
TasksFolder folder = new TasksFolder(service);
folder.DisplayName = "Custom Tasks";
// Save the folder as a child folder in the Inbox folder.
// This method call results in a CreateFolder call to EWS.
folder.Save(WellKnownFolderName.Inbox);
```

<span data-ttu-id="f6e50-137">特定のクラスのインスタンスを作成し、同時に **FolderClass** プロパティも設定すると、[ErrorNoFolderClassOverride](http://msdn.microsoft.com/ja-JP/library/exchangewebservices.responsecodetype%28v=exchg.80%29.aspx) エラーがスローされます。</span><span class="sxs-lookup"><span data-stu-id="f6e50-137">If you try to create an instance of a specific class and also set the **FolderClass** property, the [ErrorNoFolderClassOverridehttp://msdn.microsoft.com/en-us/library/exchangewebservices.responsecodetype(v=exchg.80).aspx](http://msdn.microsoft.com/ja-JP/library/exchangewebservices.responsecodetype%28v=exchg.80%29.aspx) error is thrown.</span></span> 
  
<span data-ttu-id="f6e50-138">EWS マネージ API を使用して、1 回のメソッド呼び出しで複数のフォルダーの作成をバッチ操作することはできません。</span><span class="sxs-lookup"><span data-stu-id="f6e50-138">Note that you cannot batch the creation of multiple folders in a single method call by using the EWS Managed API.</span></span>
  
## <a name="create-a-folder-by-using-ews"></a><span data-ttu-id="f6e50-139">EWS を使用してフォルダーを作成する</span><span class="sxs-lookup"><span data-stu-id="f6e50-139">Create a folder by using EWS</span></span>
<span data-ttu-id="f6e50-140"><a name="bk_createfolderews"> </a></span><span class="sxs-lookup"><span data-stu-id="f6e50-140"></span></span>

<span data-ttu-id="f6e50-141">EWS を使用すると、1 つまたは複数のフォルダーを作成できます。</span><span class="sxs-lookup"><span data-stu-id="f6e50-141">You can create a single folder or multiple of folders by using EWS.</span></span>
  
<span data-ttu-id="f6e50-142">1 つのフォルダーを作成するには、[CreateFolder](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) 操作要求メッセージを送信します。</span><span class="sxs-lookup"><span data-stu-id="f6e50-142">To create a single folder, send a [CreateFolder](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) operation request message.</span></span> <span data-ttu-id="f6e50-143">この **CreateFolder** 操作要求は、親フォルダーが受信トレイで、[DisplayName](http://msdn.microsoft.com/library/e7efbbe1-6629-4d11-bed1-ed899e3f9d77%28Office.15%29.aspx) が「Custom Folder」であること、および [FolderClass](http://msdn.microsoft.com/library/0041d135-2869-4612-89a5-d1aa86aa1093%28Office.15%29.aspx) 要素の値が IPF.Note であることを示します。</span><span class="sxs-lookup"><span data-stu-id="f6e50-143">To create a single folder, send a CreateFolder operation request message. The **CreateFolder** operation request indicates that the parent folder is the Inbox, the [DisplayName](http://msdn.microsoft.com/library/e7efbbe1-6629-4d11-bed1-ed899e3f9d77%28Office.15%29.aspx) is "Custom Folder", and the [FolderClass](http://msdn.microsoft.com/library/0041d135-2869-4612-89a5-d1aa86aa1093%28Office.15%29.aspx) element value is IPF.Note.</span></span> 
  
<span data-ttu-id="f6e50-144">これは、新しいフォルダーが作成されて [Folder.Save](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) メソッドが呼び出されると、EWS マネージ API が送信する XML 要求でもあります。</span><span class="sxs-lookup"><span data-stu-id="f6e50-144">This is also the XML request that the EWS Managed API sends when you create a new folder and call the [Folder.Savehttp://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.save(v=exchg.80).aspx](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) method.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:CreateFolder>
      <m:ParentFolderId>
        <t:DistinguishedFolderId Id="inbox" />
      </m:ParentFolderId>
      <m:Folders>
        <t:Folder>
          <t:FolderClass>IPF.Note</t:FolderClass>
          <t:DisplayName>Custom Folder</t:DisplayName>
        </t:Folder>
      </m:Folders>
    </m:CreateFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="f6e50-145">サーバーは、**CreateFolder** 要求に [CreateFolderResponse](http://msdn.microsoft.com/library/158adecc-491a-47d9-af73-acc2cd3f8566%28Office.15%29.aspx) メッセージで応答します。このメッセージには、[ResponseCode](http://msdn.microsoft.com/ja-JP/library/aa580757%28v=exchg.150%29.aspx) 値 **NoError** (フォルダーが正常に作成されたことを示します)、および新しく作成されたメッセージの [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) が含まれます。</span><span class="sxs-lookup"><span data-stu-id="f6e50-145">The server responds to the **CreateFolder** request with a [CreateFolderResponse](http://msdn.microsoft.com/library/158adecc-491a-47d9-af73-acc2cd3f8566%28Office.15%29.aspx) message that includes a [ResponseCodehttp://msdn.microsoft.com/en-us/library/aa580757(v=exchg.150).aspx](http://msdn.microsoft.com/ja-JP/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the folder was created successfully, and the [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) of the newly created message.</span></span> 
  
<span data-ttu-id="f6e50-146">複数のフォルダーを作成するには、複数の [Folder](http://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) 要素を **CreateFolder** 操作要求メッセージに含めます。</span><span class="sxs-lookup"><span data-stu-id="f6e50-146">To create multiple folders, include multiple [Folder](http://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) elements in the **CreateFolder** operation request message. All the new folders must be in the same parent folder.</span></span> <span data-ttu-id="f6e50-147">すべての新しいフォルダーの親フォルダーは同じでなければなりません。</span><span class="sxs-lookup"><span data-stu-id="f6e50-147">To create multiple folders, include multiple Folder elements in the CreateFolder operation request message. All the new folders must be in the same parent folder.</span></span> 
  
## <a name="create-a-folder-hierarchy-by-using-ews"></a><span data-ttu-id="f6e50-148">EWS を使用してフォルダー階層を作成する</span><span class="sxs-lookup"><span data-stu-id="f6e50-148">Create a folder hierarchy by using EWS</span></span>
<span data-ttu-id="f6e50-149"><a name="bk_createfolderhierarchy"> </a></span><span class="sxs-lookup"><span data-stu-id="f6e50-149"></span></span>

<span data-ttu-id="f6e50-150">EWS [CreateFolderPath](http://msdn.microsoft.com/library/5a10aa5e-3f25-4ec3-a0b9-284c30918a1f%28Office.15%29.aspx) 操作を使用すると、1 回の呼び出しで 1 つのフォルダー階層を作成できます。</span><span class="sxs-lookup"><span data-stu-id="f6e50-150">You can create a folder hierarchy in a single call by using the EWS [CreateFolderPath](http://msdn.microsoft.com/library/5a10aa5e-3f25-4ec3-a0b9-284c30918a1f%28Office.15%29.aspx) operation.</span></span> <span data-ttu-id="f6e50-151">この機能は、EWS マネージ API では利用できません。</span><span class="sxs-lookup"><span data-stu-id="f6e50-151">The same functionality is not available in the EWS Managed API.</span></span> <span data-ttu-id="f6e50-152">代わりに、EWS マネージ API を使用している場合には「[EWS を使用してフォルダーを作成する](#bk_createfolderews)」に記されているようにフォルダーを 1 つずつ作成できます。</span><span class="sxs-lookup"><span data-stu-id="f6e50-152">You can create a folder hierarchy in a single call by using the EWS CreateFolderPath operation. The same functionality is not available in the EWS Managed API. Instead, if you are using the EWS Managed API, you can create folders one by one, as shown in [Create a folder by using EWS](#bk_createfolderews).</span></span>
  
> [!NOTE]
> <span data-ttu-id="f6e50-153">EWS マネージ API はこの機能を実装していません。</span><span class="sxs-lookup"><span data-stu-id="f6e50-153">The EWS Managed API does not implement this functionality.</span></span> 
  
## <a name="get-a-folder-by-using-the-ews-managed-api"></a><span data-ttu-id="f6e50-154">EWS マネージ API を使用してフォルダーを取得する</span><span class="sxs-lookup"><span data-stu-id="f6e50-154">Get a folder by using the EWS Managed API</span></span>
<span data-ttu-id="f6e50-155"><a name="bk_getfolderewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="f6e50-155"></span></span>

<span data-ttu-id="f6e50-156">次のコード例は、[Folder.Bind](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) メソッドを使用して受信トレイ フォルダーを取得する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="f6e50-156">The following code example shows how to use the [Folder.Bind](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) method to get the Inbox folder.</span></span> <span data-ttu-id="f6e50-157">ベスト プラクティスとして、アプリケーションで必要なものだけを返すようにプロパティを制限します。</span><span class="sxs-lookup"><span data-stu-id="f6e50-157">As a best practice, we recommend that you limit the properties returned to only those that are required.</span></span> <span data-ttu-id="f6e50-158">この例の場合、返されるプロパティに含まれるのは、[Id](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) プロパティだけになるよう制限しています。そのために、[PropertySet](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) オブジェクトを作成し、[IdOnly](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.basepropertyset%28v=exchg.80%29.aspx) 値を [BasePropertySet](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.propertyset.basepropertyset%28v=exchg.80%29.aspx) プロパティに適用しています。</span><span class="sxs-lookup"><span data-stu-id="f6e50-158">This example limits the return properties to only include the [Id](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) property by creating a [PropertySet](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) object and applying the [IdOnly](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.basepropertyset%28v=exchg.80%29.aspx) value to the [BasePropertySet](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.propertyset.basepropertyset%28v=exchg.80%29.aspx) property.</span></span> 
  
<span data-ttu-id="f6e50-159">この例では、**service** が有効な [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーに既に認証されていると想定しています。</span><span class="sxs-lookup"><span data-stu-id="f6e50-159">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
// As a best practice, limit the properties returned to only those that are required.
// In this scenario, you only need the FolderId.
PropertySet propSet = new PropertySet(BasePropertySet.IdOnly);
// Bind to an existing folder and get only the properties specified in the PropertySet.
// This method call results in a GetFolder call to EWS.
Folder rootfolder = Folder.Bind(service, WellKnownFolderName.Inbox, propSet);
```

<span data-ttu-id="f6e50-160">他のプロパティを返す必要がある場合、[FolderSchema](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folderschema%28v=exchg.80%29.aspx) クラスのプロパティを **PropertySet** に追加するか、すべてのファースト クラス プロパティを返すオーバーロードされた [Bind](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) メソッドを使用します。</span><span class="sxs-lookup"><span data-stu-id="f6e50-160">If you need to return additional properties, add properties from the [FolderSchemahttp://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderschema(v=exchg.80).aspx](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folderschema%28v=exchg.80%29.aspx) class to the **PropertySet**, or use one of the overloaded [Bindhttp://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind(v=exchg.80).aspx](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) methods that returns all first class properties.</span></span> 
  
<span data-ttu-id="f6e50-161">EWS マネージ API を使用して 1 度に複数のフォルダーは取得できないことに注意してください。</span><span class="sxs-lookup"><span data-stu-id="f6e50-161">Note that you cannot get multiple folders at one time by using the EWS Managed API. You have to call the Bind method on each folder separately.</span></span> <span data-ttu-id="f6e50-162">フォルダーごとに **Bind** メソッドを呼び出す必要があります。</span><span class="sxs-lookup"><span data-stu-id="f6e50-162">You have to call the **Bind** method on each folder separately.</span></span> 
  
## <a name="get-a-folder-by-using-ews"></a><span data-ttu-id="f6e50-163">EWS を使用してフォルダーを取得する</span><span class="sxs-lookup"><span data-stu-id="f6e50-163">Get a folder by using EWS</span></span>
<span data-ttu-id="f6e50-164"><a name="bk_getfolderews"> </a></span><span class="sxs-lookup"><span data-stu-id="f6e50-164"></span></span>

<span data-ttu-id="f6e50-165">EWS を使用すると、1 つまたは複数のフォルダーを取得できます。</span><span class="sxs-lookup"><span data-stu-id="f6e50-165">You can get a single folder or multiple folders by using EWS.</span></span>
  
<span data-ttu-id="f6e50-166">1 つのフォルダーを取得するには、[GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) 操作要求メッセージをサーバーに送信します。</span><span class="sxs-lookup"><span data-stu-id="f6e50-166">To get a single folder, send a [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) operation request message to the server.</span></span> <span data-ttu-id="f6e50-167">次の例では、[BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) が **IdOnly** に設定されているため、指定したフォルダーの [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) のみが返されます。</span><span class="sxs-lookup"><span data-stu-id="f6e50-167">To get a single folder, send a GetFolder operation request message to the server. In the following example, the [BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) is set to **IdOnly**, so only the [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) of the specified folder is returned. The FolderIds element indicates that the folder to retrieve is the Inbox folder.</span></span> <span data-ttu-id="f6e50-168">この [FolderIds](http://msdn.microsoft.com/library/3ff9d15a-7220-4785-ae6b-583a7eb82005%28Office.15%29.aspx) 要素は、取得するフォルダーが受信トレイ フォルダーであることを示します。</span><span class="sxs-lookup"><span data-stu-id="f6e50-168">The [FolderIds](http://msdn.microsoft.com/library/3ff9d15a-7220-4785-ae6b-583a7eb82005%28Office.15%29.aspx) element indicates that the folder to retrieve is the Inbox folder.</span></span> 
  
<span data-ttu-id="f6e50-169">これは、[Folder.Bind](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) メソッドを使用して 1 つのフォルダーにバインドされるときに、EWS マネージ API が送信する XML 要求でもあります。</span><span class="sxs-lookup"><span data-stu-id="f6e50-169">This is also the XML request that the EWS Managed API sends when you bind to a folder by using the [Folder.Bindhttp://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind(v=exchg.80).aspx](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) method.</span></span> 
  
<span data-ttu-id="f6e50-170">複数のフォルダーを取得するには、複数の [FolderIds](http://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) 要素を **GetFolder** 操作要求メッセージに含めます。</span><span class="sxs-lookup"><span data-stu-id="f6e50-170">To get multiple folders, include multiple [FolderIds](http://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) elements in the **GetFolder** operation request message.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:GetFolder>
      <m:FolderShape>
        <t:BaseShape>IdOnly</t:BaseShape>
      </m:FolderShape>
      <m:FolderIds>
        <t:DistinguishedFolderId Id="inbox" />
      </m:FolderIds>
    </m:GetFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="f6e50-171">次の XML の例は、**GetFolder** 操作要求に対する応答として、サーバーからクライアントに送信される [GetFolderResponse](http://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) メッセージを示しています。</span><span class="sxs-lookup"><span data-stu-id="f6e50-171">The following XML example shows the [GetFolderResponse](http://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) message that is sent from the server to the client in response to the **GetFolder** operation request. It only contains the FolderId value of the Inbox folder. The values of some attributes and elements have been shortened for readability.</span></span> <span data-ttu-id="f6e50-172">受信トレイ フォルダーの [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) 値のみが入っています。</span><span class="sxs-lookup"><span data-stu-id="f6e50-172">It only contains the [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) value of the Inbox folder.</span></span> <span data-ttu-id="f6e50-173">読みやすくするため、一部の属性と要素の値が短縮されています。</span><span class="sxs-lookup"><span data-stu-id="f6e50-173">The values of some attributes and elements have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="800"
                         MinorBuildNumber="16"
                         Version="V2_6"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="AAAENAAA=" ChangeKey="AQAAABYAAAAPxolXAHv3TaHUnjW8wWqXAAAEkbCr"/>
            </t:Folder>
          </m:Folders>
        </m:GetFolderResponseMessage>
      </m:ResponseMessages>
    </m:GetFolderResponse>
  </s:Body>
</s:Envelope>
```

## <a name="get-a-folder-hierarchy-by-using-the-ews-managed-api"></a><span data-ttu-id="f6e50-174">EWS マネージ API を使用してフォルダー階層を取得する</span><span class="sxs-lookup"><span data-stu-id="f6e50-174">Get a folder hierarchy by using the EWS Managed API</span></span>
<span data-ttu-id="f6e50-175"><a name="bk_getfolderhierarchyewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="f6e50-175"></span></span>

<span data-ttu-id="f6e50-176">次のコード例は、指定したルート フォルダーのサブフォルダーを取得する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="f6e50-176">The following code example shows how to retrieve the subfolders for a specified root folder.</span></span> <span data-ttu-id="f6e50-177">この例では、**MsgFolderRoot** (IPM サブツリーのルート) のサブフォルダーを取得します。IPM サブツリーにはメールボックス フォルダーとアイテムが格納されます。</span><span class="sxs-lookup"><span data-stu-id="f6e50-177">The following code example shows how to retrieve the subfolders for a specified root folder. This example retrieves the subfolders of the **MsgFolderRoot** folder, which is the root of the IPM Subtree (where your mailbox folders and items are stored).</span></span> 
  
<span data-ttu-id="f6e50-178">この例では、[FolderView](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folderview%28v=exchg.80%29.aspx) クラス オブジェクトが作成されて、[Folder.FindFolders](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) メソッドの応答結果が制限されています。</span><span class="sxs-lookup"><span data-stu-id="f6e50-178">In this example, a [FolderView](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folderview%28v=exchg.80%29.aspx) class object is created to limit the results of the [Folder.FindFolders](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) method response.</span></span> <span data-ttu-id="f6e50-179">このシナリオでは、[Id](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx)、[DisplayName](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.displayname%28v=exchg.80%29.aspx)、およびフォルダーが隠しフォルダーかどうかを示す拡張プロパティを返すよう、プロパティを制限しています。</span><span class="sxs-lookup"><span data-stu-id="f6e50-179">This scenario limits the properties to return to the following: [Id](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx), [DisplayName](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.displayname%28v=exchg.80%29.aspx), and the extended property that indicates whether the folder is a hidden folder.</span></span> <span data-ttu-id="f6e50-180">[FolderView.Traversal](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folderview.traversal%28v=EXCHG.80%29.aspx) 値を Deep に設定してサーバーがサブフォルダーを取得できるように再帰的検索を実行しています。また、ルート フォルダーを **MsgFolderRoot** に設定し、サーバーがすべてのユーザー フォルダーを返しています (サーバーは非 IPM サブツリーのシステム フォルダーは返しません)。</span><span class="sxs-lookup"><span data-stu-id="f6e50-180">Set the [FolderView.Traversal](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folderview.traversal%28v=EXCHG.80%29.aspx) value to Deep to perform a recursive search so that the server retrieves the subfolders, and set the root folder to **MsgFolderRoot**, so that the server returns all the user's folders (and the server does not return system folders in the Non-IPM Subtree).</span></span>
  
<span data-ttu-id="f6e50-181">この例では、**service** が有効な [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーに既に認証されていると想定しています。</span><span class="sxs-lookup"><span data-stu-id="f6e50-181">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```XML
// Create a new folder view, and pass in the maximum number of folders to return.
FolderView view = new FolderView(folderViewSize);
// Create an extended property definition for the PR_ATTR_HIDDEN property,
// so that your results will indicate whether the folder is a hidden folder.
ExtendedPropertyDefinition isHiddenProp = new ExtendedPropertyDefinition(0x10f4, MapiPropertyType.Boolean);
// As a best practice, limit the properties returned to only those required.
// In this case, return the folder ID, DisplayName, and the value of the isHiddenProp
// extended property.
view.PropertySet = new PropertySet(BasePropertySet.IdOnly, FolderSchema.DisplayName, isHiddenProp);
// Indicate a Traversal value of Deep, so that all subfolders are retrieved.
view.Traversal = FolderTraversal.Deep;
// Call FindFolders to retrieve the folder hierarchy, starting with the MsgFolderRoot folder.
// This method call results in a FindFolder call to EWS.
FindFoldersResults findFolderResults = service.FindFolders(WellKnownFolderName.MsgFolderRoot, view);
```

## <a name="get-a-folder-hierarchy-by-using-ews"></a><span data-ttu-id="f6e50-182">EWS を使用してフォルダー階層を取得する</span><span class="sxs-lookup"><span data-stu-id="f6e50-182">Get a folder hierarchy by using EWS</span></span>
<span data-ttu-id="f6e50-183"><a name="bk_getfolderhierarchyews"> </a></span><span class="sxs-lookup"><span data-stu-id="f6e50-183"></span></span>

<span data-ttu-id="f6e50-184">次の XML の例は、[FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) 操作を使用して EWS でフォルダー階層を取得する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="f6e50-184">The following XML examples show how to use the [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) operation to retrieve a folder hierarchy by using EWS.</span></span> <span data-ttu-id="f6e50-185">この例では、IPM サブツリーのルートである **msgfolderroot** フォルダーとそのサブフォルダーすべてが取得されます。</span><span class="sxs-lookup"><span data-stu-id="f6e50-185">This example retrieves the **msgfolderroot** folder, which is the root of the IPM Subtree, and all its subfolders.</span></span> <span data-ttu-id="f6e50-186">**Traversal** 属性が **Deep** に設定されているので、サーバーはフォルダー階層の再帰的検索を実行し、応答で指定のルート下にあるフォルダーとサブフォルダーのみを返します。</span><span class="sxs-lookup"><span data-stu-id="f6e50-186">The **Traversal** attribute is set to **Deep** so that the server performs a recursive search of the folder hierarchy and only returns folders and subfolders under the specified root in the response.</span></span> <span data-ttu-id="f6e50-187">この例では、[BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) 要素が **IdOnly** に設定されているため、サーバーは [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) 要素のみを返します。</span><span class="sxs-lookup"><span data-stu-id="f6e50-187">In this example, the [BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) element is set to **IdOnly** so that the server only returns the [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) element.</span></span> <span data-ttu-id="f6e50-188">出力を分かりやすくするために、**DisplayName** 要素を要求の [AdditionalProperties](http://msdn.microsoft.com/library/7a269aed-dcfd-4c3e-9e14-094e53828101%28Office.15%29.aspx) 要素に含めて結果にこの要素を含めています。同時に、**PR_ATTR_HIDDEN** プロパティの **ExtendedFieldURI** 値も含めて、フォルダーが隠しフォルダーかどうかがわかるようにしています。</span><span class="sxs-lookup"><span data-stu-id="f6e50-188">To make the output easier to understand, include the **DisplayName** element in your results by including it in the [AdditionalProperties](http://msdn.microsoft.com/library/7a269aed-dcfd-4c3e-9e14-094e53828101%28Office.15%29.aspx) element in the request, along with the **ExtendedFieldURI** value for the **PR_ATTR_HIDDEN** property, so that you know whether the folders are hidden folders.</span></span> 
  
<span data-ttu-id="f6e50-189">これは、[FindFolders](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx) メソッドが呼びされるときに EWS マネージ API が送信する XML 要求でもあります。</span><span class="sxs-lookup"><span data-stu-id="f6e50-189">This is also the XML request that the EWS Managed API sends when you call the [SendAndSaveCopy](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx) method.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:FindFolder Traversal="Deep">
      <m:FolderShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="folder:DisplayName" />
          <t:ExtendedFieldURI PropertyTag="4340"
                              PropertyType="Boolean" />
        </t:AdditionalProperties>
      </m:FolderShape>
      <m:IndexedPageFolderView MaxEntriesReturned="100"
                               Offset="0"
                               BasePoint="Beginning" />
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="msgfolderroot" />
      </m:ParentFolderIds>
    </m:FindFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="f6e50-190">次の XML の例は、**FindFolder** 操作要求に対する応答として、サーバーからクライアントに送信される [FindFolderResponse](http://msdn.microsoft.com/library/f5dd813c-9698-4a39-8fca-3a825df365ed%28Office.15%29.aspx) メッセージを示しています。</span><span class="sxs-lookup"><span data-stu-id="f6e50-190">The following XML example shows the [FindFolderResponse](http://msdn.microsoft.com/library/f5dd813c-9698-4a39-8fca-3a825df365ed%28Office.15%29.aspx) message that is sent from the server to the client in response to the **FindFolder** operation request.</span></span> <span data-ttu-id="f6e50-191">含まれているのは、**msgrootfolder** フォルダーのすべてのサブフォルダーに関する [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx)、[DisplayName](http://msdn.microsoft.com/library/e7efbbe1-6629-4d11-bed1-ed899e3f9d77%28Office.15%29.aspx)、および **PR_ATTR_HIDDEN** 拡張プロパティ値のみです。</span><span class="sxs-lookup"><span data-stu-id="f6e50-191">It contains only the [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx), the [DisplayName](http://msdn.microsoft.com/library/e7efbbe1-6629-4d11-bed1-ed899e3f9d77%28Office.15%29.aspx), and the value of the **PR_ATTR_HIDDEN** extended property for all the subfolders under the **msgrootfolder** folder.</span></span> <span data-ttu-id="f6e50-192">[Value](http://msdn.microsoft.com/library/9a30cadd-909e-41b1-b4e9-291643dd89c6%28Office.15%29.aspx) 要素が true に設定されていると、フォルダーはクライアント ビューで非表示になっています。</span><span class="sxs-lookup"><span data-stu-id="f6e50-192">If the [Value](http://msdn.microsoft.com/library/9a30cadd-909e-41b1-b4e9-291643dd89c6%28Office.15%29.aspx) element is set to true, the folder should be hidden in the client view.</span></span> 
  
<span data-ttu-id="f6e50-193">これは、[FindFolder](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) メソッドを使用して複数のフォルダーが取得されるときに、EWS マネージ API が送信する XML 応答でもあります。</span><span class="sxs-lookup"><span data-stu-id="f6e50-193">This is also the XML response that the EWS Managed API sends when you get multiple folders by using the [FindFolder](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) method.</span></span> <span data-ttu-id="f6e50-194">読みやすいように、いくつかの属性と要素の値に短縮されていて、簡略化するために含まれていないフォルダーもあります。</span><span class="sxs-lookup"><span data-stu-id="f6e50-194">The values of some attributes and elements have been shortened for readability, and some folders have not been included for brevity.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?><s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="815"
                         MinorBuildNumber="6"
                         Version="V2_7"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="16"
                        TotalItemsInView="16"
                        IncludesLastItemInRange="true">
            <t:Folders>
              <t:CalendarFolder>
                <t:FolderId Id="AAAEOAAA="
                            ChangeKey="AgAAABYAAAAPxolXAHv3TaHUnjW8wWqXAAAAAAA3"/>
                <t:DisplayName>Calendar</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean"/>
                  <t:Value>false</t:Value>
                </t:ExtendedProperty>
              </t:CalendarFolder>
              <t:ContactsFolder>
                <t:FolderId Id="AAAEPAAA="
                            ChangeKey="AwAAABYAAAAPxolXAHv3TaHUnjW8wWqXAAAAAAA4"/>
                <t:DisplayName>Contacts</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean"/>
                  <t:Value>false</t:Value>
                </t:ExtendedProperty>
              </t:ContactsFolder>
              <t:ContactsFolder>
                <t:FolderId Id="AAAUKAAA="
                            ChangeKey="AwAAABYAAAAPxolXAHv3TaHUnjW8wWqXAAAAAAS5"/>
                <t:DisplayName>Recipient Cache</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean"/>
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:ContactsFolder>
              <t:Folder>
                <t:FolderId Id="AAAUJAAA="
                            ChangeKey="AQAAABYAAAAPxolXAHv3TaHUnjW8wWqXAAAAAASx"/>
                <t:DisplayName>Conversation Action Settings</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean"/>
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:Folder>
…
            </t:Folders>
          </m:RootFolder>
        </m:FindFolderResponseMessage>
      </m:ResponseMessages>
    </m:FindFolderResponse>
  </s:Body>
</s:Envelope>
```

## <a name="update-a-folder-by-using-the-ews-managed-api"></a><span data-ttu-id="f6e50-195">EWS マネージ API を使用してフォルダーを更新する</span><span class="sxs-lookup"><span data-stu-id="f6e50-195">Update a folder by using the EWS Managed API</span></span>
<span data-ttu-id="f6e50-196"><a name="bk_updatefolderewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="f6e50-196"></span></span>

<span data-ttu-id="f6e50-197">次のコード例は、EWS マネージ API を使用してフォルダーの表示名を更新する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="f6e50-197">The following code example shows how to update the display name of a folder by using the EWS Managed API.</span></span>
  
<span data-ttu-id="f6e50-198">最初に、[PropertySet](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) プロパティを作成して、サーバーが [Folder.Bind](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) 応答で返すプロパティの数を限定します。</span><span class="sxs-lookup"><span data-stu-id="f6e50-198">First, create a [PropertySet](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) to limit the number of properties that the server returns in the [Folder.Bind](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) response.</span></span> <span data-ttu-id="f6e50-199">**IdOnly** の **BasePropertySet** を使用して Exchange データベースに対する呼び出しを減らすようお勧めします。</span><span class="sxs-lookup"><span data-stu-id="f6e50-199">We recommend that you use the **IdOnly** **BasePropertySet** to reduce calls to the Exchange database.</span></span> <span data-ttu-id="f6e50-200">次に、**Bind** メソッドを使用してフォルダーを更新します。</span><span class="sxs-lookup"><span data-stu-id="f6e50-200">Next, use the **Bind** method to bind to the folder to update.</span></span> <span data-ttu-id="f6e50-201">その後、[DisplayName](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.displayname%28v=exchg.80%29.aspx) プロパティを更新し、[Folder.Update](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) メソッドによって変更を保存します。</span><span class="sxs-lookup"><span data-stu-id="f6e50-201">Then, update the [DisplayName](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.displayname%28v=exchg.80%29.aspx) property, and use the [Folder.Update](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) method to save the changes.</span></span> 
  
<span data-ttu-id="f6e50-202">この例では、**service** が有効な [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトで、ユーザーは Exchange サーバーに既に認証されていると想定しています。</span><span class="sxs-lookup"><span data-stu-id="f6e50-202">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> <span data-ttu-id="f6e50-203">ローカル変数 *folderId* は、更新対象フォルダーの [Id](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) です。</span><span class="sxs-lookup"><span data-stu-id="f6e50-203">The local variable  *itemId*  is the [Id](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) of the item to update.</span></span> 
  
```cs
// As a best practice, only include the ID value in the PropertySet.
PropertySet propertySet = new PropertySet(BasePropertySet.IdOnly);
// Bind to an existing folder and get the FolderId.
// This method call results in a GetFolder call to EWS.
Folder folder = Folder.Bind(service, folderId, propertySet);
// Update the display name of the folder.
folder.DisplayName = "Updated folder name";
// Save the updates.
// This method call results in an UpdateFolder call to EWS.
folder.Update();

```

## <a name="update-a-folder-by-using-ews"></a><span data-ttu-id="f6e50-204">EWS を使用してフォルダーを更新する</span><span class="sxs-lookup"><span data-stu-id="f6e50-204">Update a folder by using EWS</span></span>
<span data-ttu-id="f6e50-205"><a name="bk_updatefolderews"> </a></span><span class="sxs-lookup"><span data-stu-id="f6e50-205"></span></span>

<span data-ttu-id="f6e50-206">次のコード例は、EWS を使用してフォルダーの表示名を更新する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="f6e50-206">The following XML examples show how to update the display name of a folder by using EWS.</span></span>
  
<span data-ttu-id="f6e50-207">最初に、「[EWS を使用してフォルダー階層を取得する](#bk_getfolderhierarchyews)」に記されているように、更新対象フォルダーを取得するために [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) 操作要求メッセージを送信します。</span><span class="sxs-lookup"><span data-stu-id="f6e50-207">First, send a [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) operation request message to get the folder to update, as shown in [Get a folder hierarchy by using EWS](#bk_getfolderhierarchyews).</span></span>
  
<span data-ttu-id="f6e50-208">次に、フォルダーを更新する [UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) 操作要求メッセージをサーバーに送信します。</span><span class="sxs-lookup"><span data-stu-id="f6e50-208">Next, send an [UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) operation request message to the server to update a folder. The UpdateFolder operation request updates the DisplayName to "Updated Custom Folder".</span></span> <span data-ttu-id="f6e50-209">この **UpdateFolder** 操作要求は、[DisplayName](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) を「Updated Custom Folder」に更新します。</span><span class="sxs-lookup"><span data-stu-id="f6e50-209">Next, send an UpdateFolder operation request message to the server to update a folder. The **UpdateFolder** operation request updates the [DisplayName](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) to "Updated Custom Folder".</span></span> 
  
<span data-ttu-id="f6e50-210">これは、[Folder.Update](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) メソッドを使用して 1 つのフォルダーが更新されるときに、EWS マネージ API が送信する XML 要求でもあります。</span><span class="sxs-lookup"><span data-stu-id="f6e50-210">This is also the XML request that the EWS Managed API sends when you update a folder by using the [Folder.Updatehttp://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.update(v=exchg.80).aspx](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) method. The values of some attributes and elements have been shortened for readability.</span></span> <span data-ttu-id="f6e50-211">読みやすくするため、一部の属性と要素の値が短縮されています。</span><span class="sxs-lookup"><span data-stu-id="f6e50-211">The values of some attributes and elements have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:UpdateFolder>
      <m:FolderChanges>
        <t:FolderChange>
          <t:FolderId Id="OrV9ZAAA=" ChangeKey="AQAAABYAAABVzRdyy/cHS4XTC9itCRdUAAAOrXWb" />
          <t:Updates>
            <t:SetFolderField>
              <t:FieldURI FieldURI="folder:DisplayName" />
              <t:Folder>
                <t:DisplayName>Updated Custom Folder</t:DisplayName>
              </t:Folder>
            </t:SetFolderField>
          </t:Updates>
        </t:FolderChange>
      </m:FolderChanges>
    </m:UpdateFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="f6e50-212">サーバーは **UpdateFolder** 要求に [UpdateFolderResponse](http://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) メッセージで応答します。このメッセージには、[ResponseCode](http://msdn.microsoft.com/ja-JP/library/aa580757%28v=exchg.150%29.aspx) 値として **NoError**、および **ChangeKey** 属性値で更新されたフォルダーの [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f6e50-212">The server responds to the **UpdateFolder** request with a [UpdateFolderResponse](http://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) message that includes the a [ResponseCodehttp://msdn.microsoft.com/en-us/library/aa580757(v=exchg.150).aspx](http://msdn.microsoft.com/ja-JP/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, and the [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) of the folder that was updated with an updated **ChangeKey** attribute value.</span></span> 
  
## <a name="delete-a-folder-by-using-the-ews-managed-api"></a><span data-ttu-id="f6e50-213">EWS マネージ API を使用してフォルダーを削除する</span><span class="sxs-lookup"><span data-stu-id="f6e50-213">Delete a folder by using the EWS Managed API</span></span>
<span data-ttu-id="f6e50-214"><a name="bk_deletefolderewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="f6e50-214"></span></span>

<span data-ttu-id="f6e50-215">この資料では、EWS マネージ API を使用してフォルダーを削除する基本的な方法の例を示します。</span><span class="sxs-lookup"><span data-stu-id="f6e50-215">This article provides a basic example that shows you how to delete a folder by using the EWS Managed API. For more details about deleting folders, see Deleting items by using EWS in Exchange.</span></span> <span data-ttu-id="f6e50-216">フォルダーの削除について詳しくは、「[Exchange の EWS を使用するアイテムの削除](deleting-items-by-using-ews-in-exchange.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="f6e50-216">For more details about deleting items, see [Deleting items by using EWS in Exchange](deleting-items-by-using-ews-in-exchange.md).</span></span>
  
<span data-ttu-id="f6e50-217">EWS マネージ API を使用してフォルダーを削除するには、最初に [Folder.Bind](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) メソッドを使用してサービス オブジェクトを、削除対象フォルダーにバインドします。</span><span class="sxs-lookup"><span data-stu-id="f6e50-217">To delete a folder by using the EWS Managed API, first, use the [Folder.Bind](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) method to bind to the service object to the folder to delete.</span></span> <span data-ttu-id="f6e50-218">次に、[Folder.Delete](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) メソッドを使用してフォルダーを削除します。そのためには、[HardDelete](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.deletemode%28v=exchg.80%29.aspx) 削除モードを使用します。</span><span class="sxs-lookup"><span data-stu-id="f6e50-218">Next, use the [Folder.Delete](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) method to delete the folder by using the [HardDelete](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.deletemode%28v=exchg.80%29.aspx) deletion mode.</span></span> 
  
<span data-ttu-id="f6e50-219">この例では、**service** が有効な [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーに既に認証されていると想定しています。</span><span class="sxs-lookup"><span data-stu-id="f6e50-219">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> <span data-ttu-id="f6e50-220">ローカル変数 *folderId* は、削除対象フォルダーの [Id](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) です。</span><span class="sxs-lookup"><span data-stu-id="f6e50-220">The local variable  *itemId*  is the [Id](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) of the item to update.</span></span> 
  
```cs
// Bind to an existing folder and get all its properties.
// This method call results in a GetFolder call to EWS.
Folder folder = Folder.Bind(service, folderId);
// HardDelete the folder.
// This method call results in a DeleteFolder call to EWS.
folder.Delete(DeleteMode.HardDelete);
```

## <a name="delete-a-folder-by-using-ews"></a><span data-ttu-id="f6e50-221">EWS を使用してフォルダーを削除する</span><span class="sxs-lookup"><span data-stu-id="f6e50-221">Delete a folder by using EWS</span></span>
<span data-ttu-id="f6e50-222"><a name="bk_deletefolderews"> </a></span><span class="sxs-lookup"><span data-stu-id="f6e50-222"></span></span>

<span data-ttu-id="f6e50-223">この資料では、EWS を使用してフォルダーを削除する基本的な方法の XML 例を示します。</span><span class="sxs-lookup"><span data-stu-id="f6e50-223">This article provides a basic XML example that shows you how to delete a folder by using EWS. For more details about deleting folders, see Deleting items by using EWS in Exchange.</span></span> <span data-ttu-id="f6e50-224">フォルダーの削除について詳しくは、「[Exchange の EWS を使用するアイテムの削除](deleting-items-by-using-ews-in-exchange.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="f6e50-224">For more details about deleting items, see [Deleting items by using EWS in Exchange](deleting-items-by-using-ews-in-exchange.md).</span></span>
  
<span data-ttu-id="f6e50-225">EWS を使用してフィルダーを削除するには、最初に、「[EWS を使用してフォルダーを取得する](#bk_getfolderews)」に記されているように、更新対象フォルダーを取得するために [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) 操作要求メッセージを送信します。 </span><span class="sxs-lookup"><span data-stu-id="f6e50-225">To delete a folder by using EWS, first, send a [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) operation request message to get the folder to update as shown in [Get a folder by using EWS](#bk_getfolderews).</span></span> 
  
<span data-ttu-id="f6e50-226">次に、フォルダーを削除する [DeleteFolder](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) 操作要求メッセージをサーバーに送信します。</span><span class="sxs-lookup"><span data-stu-id="f6e50-226">Next, send a [DeleteFolder](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) operation request message to the server to delete the folder.</span></span> <span data-ttu-id="f6e50-227">**DeleteFolder** 操作要求は **DeleteType** が **HardDelete** であることを示し、削除するフォルダーの [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f6e50-227">Next, send a DeleteFolder operation request message to the server to delete the folder. The **DeleteFolder** operation request indicates that the **DeleteType** is **HardDelete** and it includes the [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) of the folder to delete.</span></span> 
  
<span data-ttu-id="f6e50-228">また、これは [Folder.Delete](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) メソッドを使用して 1 つのフォルダーが削除されるときに、EWS マネージ API が送信する XML 要求でもあります。</span><span class="sxs-lookup"><span data-stu-id="f6e50-228">This is also the XML request that the EWS Managed API sends when you delete a folder by using the [Folder.Deletehttp://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.delete(v=exchg.80).aspx](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) method. The values of some attributes and elements have been shortened for readability.</span></span> <span data-ttu-id="f6e50-229">読みやすくするため、一部の属性と要素の値が短縮されています。</span><span class="sxs-lookup"><span data-stu-id="f6e50-229">The values of some attributes and elements have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:DeleteFolder DeleteType="HardDelete">
      <m:FolderIds>
        <t:FolderId Id="OrV9ZAAA=" ChangeKey="AQAAABYAAABVzRdyy/cHS4XTC9itCRdUAAAOrXWf" />
      </m:FolderIds>
    </m:DeleteFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="f6e50-230">サーバーは、**DeleteFolder** 要求に対して [DeleteFolderResponse](http://msdn.microsoft.com/library/27578bda-ef0a-4a33-bccc-2c1bc1735424%28Office.15%29.aspx) メッセージで応答します。このメッセージには、[ResponseCode](http://msdn.microsoft.com/ja-JP/library/aa580757%28v=exchg.150%29.aspx) 値として、フォルダーが正常に削除されたことを示す **NoError** が含まれます。</span><span class="sxs-lookup"><span data-stu-id="f6e50-230">The server responds to the **DeleteFolder** request with a [DeleteFolderResponse](http://msdn.microsoft.com/library/27578bda-ef0a-4a33-bccc-2c1bc1735424%28Office.15%29.aspx) message that includes the a [ResponseCodehttp://msdn.microsoft.com/en-us/library/aa580757(v=exchg.150).aspx](http://msdn.microsoft.com/ja-JP/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the folder deletion was successful.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="f6e50-231">次の手順</span><span class="sxs-lookup"><span data-stu-id="f6e50-231">Next steps</span></span>
<span data-ttu-id="f6e50-232"><a name="bk_nextsteps"> </a></span><span class="sxs-lookup"><span data-stu-id="f6e50-232"></span></span>

<span data-ttu-id="f6e50-233">サーバー上のフォルダーを取得するか、フォルダーに変更を加えた後、[フォルダー階層を同期する](how-to-synchronize-folders-by-using-ews-in-exchange.md)か、サーバーにおける[フォルダーの変更についての通知を購読する](notification-subscriptions-mailbox-events-and-ews-in-exchange.md)こともできます。 </span><span class="sxs-lookup"><span data-stu-id="f6e50-233">After you have retrieved the folders on the server, or made changes to folders, you might want to [synchronize your folder hierarchy](how-to-synchronize-folders-by-using-ews-in-exchange.md) or [subscribe to notifications about folder changes](notification-subscriptions-mailbox-events-and-ews-in-exchange.md) on the server.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="f6e50-234">関連項目</span><span class="sxs-lookup"><span data-stu-id="f6e50-234">See also</span></span>

- [<span data-ttu-id="f6e50-235">Exchange の EWS のフォルダーとアイテム</span><span class="sxs-lookup"><span data-stu-id="f6e50-235">Folders and items in EWS in Exchange</span></span>](folders-and-items-in-ews-in-exchange.md)   
- [<span data-ttu-id="f6e50-236">Exchange で EWS を使用して Exchange メールボックス アイテムを操作する</span><span class="sxs-lookup"><span data-stu-id="f6e50-236">How to: Work with Exchange mailbox items by using EWS in Exchange</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md)    
- [<span data-ttu-id="f6e50-237">Exchange の EWS を使用するアイテムの削除</span><span class="sxs-lookup"><span data-stu-id="f6e50-237">Deleting items by using EWS in Exchange</span></span>](deleting-items-by-using-ews-in-exchange.md)   
- [<span data-ttu-id="f6e50-238">Exchange の Web サービス クライアントを開発する</span><span class="sxs-lookup"><span data-stu-id="f6e50-238">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    

