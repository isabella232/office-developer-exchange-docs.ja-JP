---
title: MarkAllItemsAsRead
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 22244afb-99ec-41b4-8f73-3fbccd56d1ab
description: MarkAllItemsAsRead 要素には、フォルダー内のすべてのアイテムへの要求が含まれています。
ms.openlocfilehash: 9d7eb8eb7194cb5d77e909dc08abfb70e2385d56
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832346"
---
# <a name="markallitemsasread"></a><span data-ttu-id="a3c66-103">MarkAllItemsAsRead</span><span class="sxs-lookup"><span data-stu-id="a3c66-103">MarkAllItemsAsRead</span></span>

<span data-ttu-id="a3c66-104">**MarkAllItemsAsRead**要素には、フォルダー内のすべてのアイテムへの要求が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a3c66-104">The **MarkAllItemsAsRead** element contains the request to mark all the items in a folder as read.</span></span> 
  
```XML
<MarkAllItemsAsRead>
   <ReadFlag/>
   <SuppressReadReceipts/>
   <FolderIds/>
</MarkAllItemsAsRead>
```

 <span data-ttu-id="a3c66-105">**MarkAllItemsAsReadType**</span><span class="sxs-lookup"><span data-stu-id="a3c66-105">**MarkAllItemsAsReadType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a3c66-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="a3c66-106">Attributes and elements</span></span>

<span data-ttu-id="a3c66-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a3c66-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a3c66-108">属性</span><span class="sxs-lookup"><span data-stu-id="a3c66-108">Attributes</span></span>

<span data-ttu-id="a3c66-109">なし。</span><span class="sxs-lookup"><span data-stu-id="a3c66-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a3c66-110">子要素</span><span class="sxs-lookup"><span data-stu-id="a3c66-110">Child elements</span></span>

<span data-ttu-id="a3c66-111">[ReadFlag](readflag.md) | [SuppressReadReceipts](suppressreadreceipts.md) | [FolderIds](folderids.md)</span><span class="sxs-lookup"><span data-stu-id="a3c66-111">[ReadFlag](readflag.md) | [SuppressReadReceipts](suppressreadreceipts.md) | [FolderIds](folderids.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a3c66-112">親要素</span><span class="sxs-lookup"><span data-stu-id="a3c66-112">Parent elements</span></span>

<span data-ttu-id="a3c66-113">なし。</span><span class="sxs-lookup"><span data-stu-id="a3c66-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a3c66-114">備考</span><span class="sxs-lookup"><span data-stu-id="a3c66-114">Remarks</span></span>

<span data-ttu-id="a3c66-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="a3c66-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="a3c66-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="a3c66-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a3c66-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="a3c66-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a3c66-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="a3c66-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a3c66-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a3c66-119">Schema name</span></span>  <br/> |<span data-ttu-id="a3c66-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="a3c66-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a3c66-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a3c66-121">Validation file</span></span>  <br/> |<span data-ttu-id="a3c66-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="a3c66-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a3c66-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="a3c66-123">Can be empty</span></span>  <br/> ||
   

