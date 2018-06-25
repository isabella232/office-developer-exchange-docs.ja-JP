---
title: SetImListMigrationCompleted
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4b806441-0429-44c4-90b7-1ae5c6ab9128
description: SetImListMigrationCompleted 要素は、Exchange ストアに、インスタント メッセージング クライアントによって使用されるインスタント メッセージングの項目が含まれているかどうかを示すために要求を表します。
ms.openlocfilehash: 602583594aa171d49a1af2b70664301bf8ff1244
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833431"
---
# <a name="setimlistmigrationcompleted"></a><span data-ttu-id="bb0ff-103">SetImListMigrationCompleted</span><span class="sxs-lookup"><span data-stu-id="bb0ff-103">SetImListMigrationCompleted</span></span>

<span data-ttu-id="bb0ff-104">**SetImListMigrationCompleted**要素は、Exchange ストアに、インスタント メッセージング クライアントによって使用されるインスタント メッセージングの項目が含まれているかどうかを示すために要求を表します。</span><span class="sxs-lookup"><span data-stu-id="bb0ff-104">The **SetImListMigrationCompleted** element represents a request to indicate whether the Exchange store contains the instant messaging items used by instant messaging clients.</span></span> 
  
```XML
<SetImListMigrationCompleted>
   <ImListMigrationCompleted/>
</SetImListMigrationCompleted>
```

 <span data-ttu-id="bb0ff-105">**SetImListMigrationCompletedType**</span><span class="sxs-lookup"><span data-stu-id="bb0ff-105">**SetImListMigrationCompletedType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bb0ff-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="bb0ff-106">Attributes and elements</span></span>

<span data-ttu-id="bb0ff-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="bb0ff-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bb0ff-108">属性</span><span class="sxs-lookup"><span data-stu-id="bb0ff-108">Attributes</span></span>

<span data-ttu-id="bb0ff-109">なし。</span><span class="sxs-lookup"><span data-stu-id="bb0ff-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bb0ff-110">子要素</span><span class="sxs-lookup"><span data-stu-id="bb0ff-110">Child elements</span></span>

[<span data-ttu-id="bb0ff-111">ImListMigrationCompleted</span><span class="sxs-lookup"><span data-stu-id="bb0ff-111">ImListMigrationCompleted</span></span>](imlistmigrationcompleted.md)
  
### <a name="parent-elements"></a><span data-ttu-id="bb0ff-112">親要素</span><span class="sxs-lookup"><span data-stu-id="bb0ff-112">Parent elements</span></span>

<span data-ttu-id="bb0ff-113">なし。</span><span class="sxs-lookup"><span data-stu-id="bb0ff-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bb0ff-114">備考</span><span class="sxs-lookup"><span data-stu-id="bb0ff-114">Remarks</span></span>

<span data-ttu-id="bb0ff-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="bb0ff-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="bb0ff-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="bb0ff-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bb0ff-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="bb0ff-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bb0ff-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="bb0ff-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="bb0ff-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="bb0ff-119">Schema name</span></span>  <br/> |<span data-ttu-id="bb0ff-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="bb0ff-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="bb0ff-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="bb0ff-121">Validation file</span></span>  <br/> |<span data-ttu-id="bb0ff-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="bb0ff-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="bb0ff-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="bb0ff-123">Can be empty</span></span>  <br/> |<span data-ttu-id="bb0ff-124">false</span><span class="sxs-lookup"><span data-stu-id="bb0ff-124">false</span></span>  <br/> |
   

