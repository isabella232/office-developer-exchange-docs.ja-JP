---
title: ImListMigrationCompleted
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 6eed9502-5d9e-4345-ba23-3582ff487147
description: ImListMigrationCompleted 要素は、Exchange ストアに、インスタント メッセージング クライアントによって使用されるインスタント メッセージングの項目が含まれているかどうかを示します。
ms.openlocfilehash: 25f1b583b354a71958fbc8052c492726dc0eb7db
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831893"
---
# <a name="imlistmigrationcompleted"></a><span data-ttu-id="d6e1e-103">ImListMigrationCompleted</span><span class="sxs-lookup"><span data-stu-id="d6e1e-103">ImListMigrationCompleted</span></span>

<span data-ttu-id="d6e1e-104">**ImListMigrationCompleted**要素は、Exchange ストアに、インスタント メッセージング、インスタント メッセージング クライアントで使用されるアイテムが含まれているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d6e1e-104">The **ImListMigrationCompleted** element indicates whether the Exchange store contains the instant messaging items used by instant messaging clients.</span></span> 
  
```XML
<ImListMigrationCompleted>true | false</ImListMigrationCompleted>
```

 <span data-ttu-id="d6e1e-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="d6e1e-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d6e1e-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="d6e1e-106">Attributes and elements</span></span>

<span data-ttu-id="d6e1e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d6e1e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d6e1e-108">属性</span><span class="sxs-lookup"><span data-stu-id="d6e1e-108">Attributes</span></span>

<span data-ttu-id="d6e1e-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d6e1e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d6e1e-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d6e1e-110">Child elements</span></span>

<span data-ttu-id="d6e1e-111">なし。</span><span class="sxs-lookup"><span data-stu-id="d6e1e-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d6e1e-112">親要素</span><span class="sxs-lookup"><span data-stu-id="d6e1e-112">Parent elements</span></span>

[<span data-ttu-id="d6e1e-113">SetImListMigrationCompleted</span><span class="sxs-lookup"><span data-stu-id="d6e1e-113">SetImListMigrationCompleted</span></span>](setimlistmigrationcompleted.md)
  
## <a name="text-value"></a><span data-ttu-id="d6e1e-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="d6e1e-114">Text value</span></span>

<span data-ttu-id="d6e1e-115">の**場合は true** 、 **ImListMigrationCompleted**要素のテキスト値は、ストアが Exchange に移行済みインスタント メッセージの連絡先を格納することを示します。</span><span class="sxs-lookup"><span data-stu-id="d6e1e-115">A text value of **true** for the **ImListMigrationCompleted** element indicates that the instant messaging contacts store has been migrated to the Exchange store.</span></span> <span data-ttu-id="d6e1e-116">**False**の値は、インスタント メッセージの連絡先ストアが移行されていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="d6e1e-116">A value of **false** indicates that the instant message contacts store has not been migrated.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="d6e1e-117">備考</span><span class="sxs-lookup"><span data-stu-id="d6e1e-117">Remarks</span></span>

<span data-ttu-id="d6e1e-118">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="d6e1e-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d6e1e-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="d6e1e-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d6e1e-120">要素情報</span><span class="sxs-lookup"><span data-stu-id="d6e1e-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d6e1e-121">名前空間</span><span class="sxs-lookup"><span data-stu-id="d6e1e-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d6e1e-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d6e1e-122">Schema name</span></span>  <br/> |<span data-ttu-id="d6e1e-123">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="d6e1e-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d6e1e-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d6e1e-124">Validation file</span></span>  <br/> |<span data-ttu-id="d6e1e-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d6e1e-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d6e1e-126">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="d6e1e-126">Can be empty</span></span>  <br/> ||
   

