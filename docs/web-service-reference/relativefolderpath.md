---
title: RelativeFolderPath
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 54e3ba52-08a6-4d48-8a44-6fd5fdbffb25
description: RelativeFolderPath 要素には、作成するフォルダーパスの相対フォルダパスを示すフォルダーの配列が含まれています。
ms.openlocfilehash: 8a0fc0020943afdbe6cd4c79d51d61337f8dd329
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457159"
---
# <a name="relativefolderpath"></a><span data-ttu-id="1c3ec-103">RelativeFolderPath</span><span class="sxs-lookup"><span data-stu-id="1c3ec-103">RelativeFolderPath</span></span>

<span data-ttu-id="1c3ec-104">**RelativeFolderPath**要素には、作成するフォルダーパスの相対フォルダパスを示すフォルダーの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1c3ec-104">The **RelativeFolderPath** element contains an array of folders that indicate the relative folder path of the folder path to be created.</span></span> 
  
```XML
<RelativeFolderPath>
   <Folder/>
   <CalendarFolder/>
   <ContactsFolder/>
   <SearchFolder/>
   <TasksFolder/>
</RelativeFolderPath>
```

 <span data-ttu-id="1c3ec-105">**非 Emptyarrayoffolderstype**</span><span class="sxs-lookup"><span data-stu-id="1c3ec-105">**NonEmptyArrayOfFoldersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1c3ec-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="1c3ec-106">Attributes and elements</span></span>

<span data-ttu-id="1c3ec-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1c3ec-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1c3ec-108">属性</span><span class="sxs-lookup"><span data-stu-id="1c3ec-108">Attributes</span></span>

<span data-ttu-id="1c3ec-109">なし。</span><span class="sxs-lookup"><span data-stu-id="1c3ec-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1c3ec-110">子要素</span><span class="sxs-lookup"><span data-stu-id="1c3ec-110">Child elements</span></span>

<span data-ttu-id="1c3ec-111">[フォルダー](folder.md)  | [Calendarfolder](calendarfolder.md)  | [ContactsFolder](contactsfolder.md)  | [Searchfolder](searchfolder.md)  | [タスクフォルダー](tasksfolder.md)</span><span class="sxs-lookup"><span data-stu-id="1c3ec-111">[Folder](folder.md) | [CalendarFolder](calendarfolder.md) | [ContactsFolder](contactsfolder.md) | [SearchFolder](searchfolder.md) | [TasksFolder](tasksfolder.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1c3ec-112">親要素</span><span class="sxs-lookup"><span data-stu-id="1c3ec-112">Parent elements</span></span>

[<span data-ttu-id="1c3ec-113">CreateFolderPath</span><span class="sxs-lookup"><span data-stu-id="1c3ec-113">CreateFolderPath</span></span>](createfolderpath.md)
  
## <a name="remarks"></a><span data-ttu-id="1c3ec-114">注釈</span><span class="sxs-lookup"><span data-stu-id="1c3ec-114">Remarks</span></span>

<span data-ttu-id="1c3ec-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="1c3ec-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="1c3ec-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="1c3ec-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1c3ec-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="1c3ec-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1c3ec-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="1c3ec-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1c3ec-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1c3ec-119">Schema name</span></span>  <br/> |<span data-ttu-id="1c3ec-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="1c3ec-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1c3ec-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1c3ec-121">Validation file</span></span>  <br/> |<span data-ttu-id="1c3ec-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="1c3ec-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1c3ec-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="1c3ec-123">Can be empty</span></span>  <br/> ||
   

