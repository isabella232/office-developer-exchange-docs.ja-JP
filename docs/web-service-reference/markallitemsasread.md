---
title: MarkAllItemsAsRead
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 22244afb-99ec-41b4-8f73-3fbccd56d1ab
description: MarkAllItemsAsRead 要素には、フォルダー内のすべてのアイテムを開封済みとしてマークする要求が含まれています。
ms.openlocfilehash: 0338b2a1eed503b7e8fb0ec8b4a8ebcf12b6dbd6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530889"
---
# <a name="markallitemsasread"></a><span data-ttu-id="9847b-103">MarkAllItemsAsRead</span><span class="sxs-lookup"><span data-stu-id="9847b-103">MarkAllItemsAsRead</span></span>

<span data-ttu-id="9847b-104">**Markallitemsasread**要素には、フォルダー内のすべてのアイテムを開封済みとしてマークする要求が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9847b-104">The **MarkAllItemsAsRead** element contains the request to mark all the items in a folder as read.</span></span> 
  
```XML
<MarkAllItemsAsRead>
   <ReadFlag/>
   <SuppressReadReceipts/>
   <FolderIds/>
</MarkAllItemsAsRead>
```

 <span data-ttu-id="9847b-105">**MarkAllItemsAsReadType**</span><span class="sxs-lookup"><span data-stu-id="9847b-105">**MarkAllItemsAsReadType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9847b-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="9847b-106">Attributes and elements</span></span>

<span data-ttu-id="9847b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9847b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9847b-108">属性</span><span class="sxs-lookup"><span data-stu-id="9847b-108">Attributes</span></span>

<span data-ttu-id="9847b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9847b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9847b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9847b-110">Child elements</span></span>

<span data-ttu-id="9847b-111">[Readflag](readflag.md)  | [SuppressReadReceipts](suppressreadreceipts.md)  | [FolderIds](folderids.md)</span><span class="sxs-lookup"><span data-stu-id="9847b-111">[ReadFlag](readflag.md) | [SuppressReadReceipts](suppressreadreceipts.md) | [FolderIds](folderids.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9847b-112">親要素</span><span class="sxs-lookup"><span data-stu-id="9847b-112">Parent elements</span></span>

<span data-ttu-id="9847b-113">なし。</span><span class="sxs-lookup"><span data-stu-id="9847b-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9847b-114">注釈</span><span class="sxs-lookup"><span data-stu-id="9847b-114">Remarks</span></span>

<span data-ttu-id="9847b-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="9847b-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="9847b-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="9847b-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9847b-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="9847b-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9847b-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="9847b-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9847b-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9847b-119">Schema name</span></span>  <br/> |<span data-ttu-id="9847b-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="9847b-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9847b-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9847b-121">Validation file</span></span>  <br/> |<span data-ttu-id="9847b-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="9847b-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9847b-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="9847b-123">Can be empty</span></span>  <br/> ||
   

