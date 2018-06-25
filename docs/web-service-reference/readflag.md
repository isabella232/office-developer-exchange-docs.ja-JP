---
title: ReadFlag
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9d91aa89-9f9f-4877-846d-aaf48bbeec7c
description: ReadFlag 要素は、フォルダー内のアイテムに設定するのには読み取りの状態を示します。
ms.openlocfilehash: f3156a51fbdd3372dd28f2065499d26a50b3d497
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832954"
---
# <a name="readflag"></a><span data-ttu-id="ed4dd-103">ReadFlag</span><span class="sxs-lookup"><span data-stu-id="ed4dd-103">ReadFlag</span></span>

<span data-ttu-id="ed4dd-104">**ReadFlag**要素は、フォルダー内のアイテムに設定するのには読み取りの状態を示します。</span><span class="sxs-lookup"><span data-stu-id="ed4dd-104">The **ReadFlag** element indicates the read state to set on items in a folder.</span></span> 
  
```XML
<ReadFlag>true | false</ReadFlag>
```

 <span data-ttu-id="ed4dd-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="ed4dd-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ed4dd-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="ed4dd-106">Attributes and elements</span></span>

<span data-ttu-id="ed4dd-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ed4dd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ed4dd-108">属性</span><span class="sxs-lookup"><span data-stu-id="ed4dd-108">Attributes</span></span>

<span data-ttu-id="ed4dd-109">なし。</span><span class="sxs-lookup"><span data-stu-id="ed4dd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ed4dd-110">子要素</span><span class="sxs-lookup"><span data-stu-id="ed4dd-110">Child elements</span></span>

<span data-ttu-id="ed4dd-111">なし。</span><span class="sxs-lookup"><span data-stu-id="ed4dd-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ed4dd-112">親要素</span><span class="sxs-lookup"><span data-stu-id="ed4dd-112">Parent elements</span></span>

[<span data-ttu-id="ed4dd-113">MarkAllItemsAsRead</span><span class="sxs-lookup"><span data-stu-id="ed4dd-113">MarkAllItemsAsRead</span></span>](markallitemsasread.md)
  
## <a name="text-value"></a><span data-ttu-id="ed4dd-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="ed4dd-114">Text value</span></span>

<span data-ttu-id="ed4dd-115">の**場合は true** 、 **ReadFlag**要素のテキスト値は、フォルダー内のアイテムは開封としてマークされることを示します。</span><span class="sxs-lookup"><span data-stu-id="ed4dd-115">A text value of **true** for the **ReadFlag** element indicates that the items in the folder will be marked as read.</span></span> <span data-ttu-id="ed4dd-116">**False**の値は、フォルダー内のアイテムをマークすることを示します、未読です。</span><span class="sxs-lookup"><span data-stu-id="ed4dd-116">A value of **false** indicates that the items in the folder will be marked as unread.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="ed4dd-117">備考</span><span class="sxs-lookup"><span data-stu-id="ed4dd-117">Remarks</span></span>

<span data-ttu-id="ed4dd-118">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="ed4dd-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="ed4dd-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="ed4dd-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ed4dd-120">要素情報</span><span class="sxs-lookup"><span data-stu-id="ed4dd-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ed4dd-121">名前空間</span><span class="sxs-lookup"><span data-stu-id="ed4dd-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ed4dd-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ed4dd-122">Schema name</span></span>  <br/> |<span data-ttu-id="ed4dd-123">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="ed4dd-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ed4dd-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ed4dd-124">Validation file</span></span>  <br/> |<span data-ttu-id="ed4dd-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ed4dd-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ed4dd-126">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="ed4dd-126">Can be empty</span></span>  <br/> ||
   

