---
title: RelativeFolderPath
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 54e3ba52-08a6-4d48-8a44-6fd5fdbffb25
description: RelativeFolderPath 要素には、フォルダーへのパスを作成するフォルダーの相対パスを指定するフォルダーの配列が含まれています。
ms.openlocfilehash: f568d282e47a41c0aaf6d70ef383e5ef3e2b54bf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833051"
---
# <a name="relativefolderpath"></a><span data-ttu-id="674a0-103">RelativeFolderPath</span><span class="sxs-lookup"><span data-stu-id="674a0-103">RelativeFolderPath</span></span>

<span data-ttu-id="674a0-104">**RelativeFolderPath**要素には、フォルダーへのパスを作成するフォルダーの相対パスを指定するフォルダーの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="674a0-104">The **RelativeFolderPath** element contains an array of folders that indicate the relative folder path of the folder path to be created.</span></span> 
  
```XML
<RelativeFolderPath>
   <Folder/>
   <CalendarFolder/>
   <ContactsFolder/>
   <SearchFolder/>
   <TasksFolder/>
</RelativeFolderPath>
```

 <span data-ttu-id="674a0-105">**NonEmptyArrayOfFoldersType**</span><span class="sxs-lookup"><span data-stu-id="674a0-105">**NonEmptyArrayOfFoldersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="674a0-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="674a0-106">Attributes and elements</span></span>

<span data-ttu-id="674a0-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="674a0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="674a0-108">属性</span><span class="sxs-lookup"><span data-stu-id="674a0-108">Attributes</span></span>

<span data-ttu-id="674a0-109">なし。</span><span class="sxs-lookup"><span data-stu-id="674a0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="674a0-110">子要素</span><span class="sxs-lookup"><span data-stu-id="674a0-110">Child elements</span></span>

<span data-ttu-id="674a0-111">[フォルダー](folder.md) | [CalendarFolder](calendarfolder.md) | [メッセージ](contactsfolder.md) | [SearchFolder](searchfolder.md) | [TasksFolder](tasksfolder.md)</span><span class="sxs-lookup"><span data-stu-id="674a0-111">[Folder](folder.md) | [CalendarFolder](calendarfolder.md) | [ContactsFolder](contactsfolder.md) | [SearchFolder](searchfolder.md) | [TasksFolder](tasksfolder.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="674a0-112">親要素</span><span class="sxs-lookup"><span data-stu-id="674a0-112">Parent elements</span></span>

[<span data-ttu-id="674a0-113">CreateFolderPath</span><span class="sxs-lookup"><span data-stu-id="674a0-113">CreateFolderPath</span></span>](createfolderpath.md)
  
## <a name="remarks"></a><span data-ttu-id="674a0-114">備考</span><span class="sxs-lookup"><span data-stu-id="674a0-114">Remarks</span></span>

<span data-ttu-id="674a0-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="674a0-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="674a0-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="674a0-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="674a0-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="674a0-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="674a0-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="674a0-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="674a0-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="674a0-119">Schema name</span></span>  <br/> |<span data-ttu-id="674a0-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="674a0-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="674a0-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="674a0-121">Validation file</span></span>  <br/> |<span data-ttu-id="674a0-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="674a0-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="674a0-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="674a0-123">Can be empty</span></span>  <br/> ||
   

