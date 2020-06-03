---
title: CreateFolderPath
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 282576cb-a921-49f7-8748-64158fd50c41
description: CreateFolderPath 要素は、フォルダーのパスを作成するために使用され、親フォルダーの Id と相対フォルダーのパスを含みます。
ms.openlocfilehash: e6ce6c9b6e12a6a0fb6792b63368a79c87d06f07
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457537"
---
# <a name="createfolderpath"></a><span data-ttu-id="75629-103">CreateFolderPath</span><span class="sxs-lookup"><span data-stu-id="75629-103">CreateFolderPath</span></span>

<span data-ttu-id="75629-104">**Createfolderpath**要素は、フォルダーのパスを作成するために使用され、親フォルダーの Id と相対フォルダーのパスを含みます。</span><span class="sxs-lookup"><span data-stu-id="75629-104">The **CreateFolderPath** element is used to create a folder path and includes a parent folder Id and a relative folder path.</span></span> 
  
```XML
<CreateFolderPath>
   <ParentFolderId/>
   <RelativeFolderPath/>
</CreateFolderPath>
```

 <span data-ttu-id="75629-105">**CreateFolderPathType**</span><span class="sxs-lookup"><span data-stu-id="75629-105">**CreateFolderPathType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="75629-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="75629-106">Attributes and elements</span></span>

<span data-ttu-id="75629-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="75629-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="75629-108">属性</span><span class="sxs-lookup"><span data-stu-id="75629-108">Attributes</span></span>

<span data-ttu-id="75629-109">なし。</span><span class="sxs-lookup"><span data-stu-id="75629-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="75629-110">子要素</span><span class="sxs-lookup"><span data-stu-id="75629-110">Child elements</span></span>

<span data-ttu-id="75629-111">[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)  | [RelativeFolderPath](relativefolderpath.md)</span><span class="sxs-lookup"><span data-stu-id="75629-111">[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) | [RelativeFolderPath](relativefolderpath.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="75629-112">親要素</span><span class="sxs-lookup"><span data-stu-id="75629-112">Parent elements</span></span>

<span data-ttu-id="75629-113">なし。</span><span class="sxs-lookup"><span data-stu-id="75629-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="75629-114">注釈</span><span class="sxs-lookup"><span data-stu-id="75629-114">Remarks</span></span>

<span data-ttu-id="75629-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="75629-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="75629-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="75629-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="75629-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="75629-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="75629-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="75629-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="75629-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="75629-119">Schema name</span></span>  <br/> |<span data-ttu-id="75629-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="75629-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="75629-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="75629-121">Validation file</span></span>  <br/> |<span data-ttu-id="75629-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="75629-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="75629-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="75629-123">Can be empty</span></span>  <br/> |<span data-ttu-id="75629-124">false</span><span class="sxs-lookup"><span data-stu-id="75629-124">false</span></span>  <br/> |
   

