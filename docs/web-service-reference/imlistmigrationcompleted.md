---
title: ImListMigrationCompleted
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 6eed9502-5d9e-4345-ba23-3582ff487147
description: ImListMigrationCompleted 要素は、Exchange ストアに、インスタントメッセージングクライアントによって使用されるインスタントメッセージングアイテムが含まれているかどうかを示します。
ms.openlocfilehash: 09f37d6e3663aab7cb98fc922f727ddd604f2acd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456025"
---
# <a name="imlistmigrationcompleted"></a><span data-ttu-id="2679c-103">ImListMigrationCompleted</span><span class="sxs-lookup"><span data-stu-id="2679c-103">ImListMigrationCompleted</span></span>

<span data-ttu-id="2679c-104">**ImListMigrationCompleted**要素は、Exchange ストアに、インスタントメッセージングクライアントによって使用されるインスタントメッセージングアイテムが含まれているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2679c-104">The **ImListMigrationCompleted** element indicates whether the Exchange store contains the instant messaging items used by instant messaging clients.</span></span> 
  
```XML
<ImListMigrationCompleted>true | false</ImListMigrationCompleted>
```

 <span data-ttu-id="2679c-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="2679c-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2679c-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="2679c-106">Attributes and elements</span></span>

<span data-ttu-id="2679c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2679c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2679c-108">属性</span><span class="sxs-lookup"><span data-stu-id="2679c-108">Attributes</span></span>

<span data-ttu-id="2679c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="2679c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2679c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="2679c-110">Child elements</span></span>

<span data-ttu-id="2679c-111">なし。</span><span class="sxs-lookup"><span data-stu-id="2679c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2679c-112">親要素</span><span class="sxs-lookup"><span data-stu-id="2679c-112">Parent elements</span></span>

[<span data-ttu-id="2679c-113">SetImListMigrationCompleted</span><span class="sxs-lookup"><span data-stu-id="2679c-113">SetImListMigrationCompleted</span></span>](setimlistmigrationcompleted.md)
  
## <a name="text-value"></a><span data-ttu-id="2679c-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="2679c-114">Text value</span></span>

<span data-ttu-id="2679c-115">**ImListMigrationCompleted**要素のテキスト値が**true**の場合は、インスタントメッセージングの連絡先ストアが Exchange ストアに移行されたことを示します。</span><span class="sxs-lookup"><span data-stu-id="2679c-115">A text value of **true** for the **ImListMigrationCompleted** element indicates that the instant messaging contacts store has been migrated to the Exchange store.</span></span> <span data-ttu-id="2679c-116">値が**false**の場合は、インスタントメッセージの連絡先ストアが移行されていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="2679c-116">A value of **false** indicates that the instant message contacts store has not been migrated.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="2679c-117">注釈</span><span class="sxs-lookup"><span data-stu-id="2679c-117">Remarks</span></span>

<span data-ttu-id="2679c-118">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="2679c-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="2679c-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="2679c-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2679c-120">要素の情報</span><span class="sxs-lookup"><span data-stu-id="2679c-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2679c-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="2679c-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2679c-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2679c-122">Schema name</span></span>  <br/> |<span data-ttu-id="2679c-123">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="2679c-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="2679c-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2679c-124">Validation file</span></span>  <br/> |<span data-ttu-id="2679c-125">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="2679c-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2679c-126">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="2679c-126">Can be empty</span></span>  <br/> ||
   

