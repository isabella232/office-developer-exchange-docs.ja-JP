---
title: CreateFolderPath
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 282576cb-a921-49f7-8748-64158fd50c41
description: CreateFolderPath 要素はフォルダーのパスを作成するために使用し、親フォルダー Id とフォルダーの相対パスが含まれています。
ms.openlocfilehash: bfe31d894cfaa0f36da2d1d0045f723e0d261759
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759817"
---
# <a name="createfolderpath"></a><span data-ttu-id="b2841-103">CreateFolderPath</span><span class="sxs-lookup"><span data-stu-id="b2841-103">CreateFolderPath</span></span>

<span data-ttu-id="b2841-104">**CreateFolderPath**要素はフォルダーのパスを作成するために使用し、親フォルダー Id とフォルダーの相対パスが含まれています。</span><span class="sxs-lookup"><span data-stu-id="b2841-104">The **CreateFolderPath** element is used to create a folder path and includes a parent folder Id and a relative folder path.</span></span> 
  
```XML
<CreateFolderPath>
   <ParentFolderId/>
   <RelativeFolderPath/>
</CreateFolderPath>
```

 <span data-ttu-id="b2841-105">**CreateFolderPathType**</span><span class="sxs-lookup"><span data-stu-id="b2841-105">**CreateFolderPathType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b2841-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="b2841-106">Attributes and elements</span></span>

<span data-ttu-id="b2841-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b2841-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b2841-108">属性</span><span class="sxs-lookup"><span data-stu-id="b2841-108">Attributes</span></span>

<span data-ttu-id="b2841-109">なし。</span><span class="sxs-lookup"><span data-stu-id="b2841-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b2841-110">子要素</span><span class="sxs-lookup"><span data-stu-id="b2841-110">Child elements</span></span>

<span data-ttu-id="b2841-111">[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) | [RelativeFolderPath](relativefolderpath.md)</span><span class="sxs-lookup"><span data-stu-id="b2841-111">[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) | [RelativeFolderPath](relativefolderpath.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b2841-112">親要素</span><span class="sxs-lookup"><span data-stu-id="b2841-112">Parent elements</span></span>

<span data-ttu-id="b2841-113">なし。</span><span class="sxs-lookup"><span data-stu-id="b2841-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b2841-114">備考</span><span class="sxs-lookup"><span data-stu-id="b2841-114">Remarks</span></span>

<span data-ttu-id="b2841-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="b2841-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b2841-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="b2841-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b2841-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="b2841-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b2841-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="b2841-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b2841-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b2841-119">Schema name</span></span>  <br/> |<span data-ttu-id="b2841-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="b2841-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b2841-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b2841-121">Validation file</span></span>  <br/> |<span data-ttu-id="b2841-122">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b2841-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b2841-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="b2841-123">Can be empty</span></span>  <br/> |<span data-ttu-id="b2841-124">false</span><span class="sxs-lookup"><span data-stu-id="b2841-124">false</span></span>  <br/> |
   

