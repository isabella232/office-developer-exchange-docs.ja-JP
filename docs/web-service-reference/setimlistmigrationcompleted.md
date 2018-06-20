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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833431"
---
# <a name="setimlistmigrationcompleted"></a><span data-ttu-id="da4a6-103">SetImListMigrationCompleted</span><span class="sxs-lookup"><span data-stu-id="da4a6-103">SetImListMigrationCompleted</span></span>

<span data-ttu-id="da4a6-104">**SetImListMigrationCompleted**要素は、Exchange ストアに、インスタント メッセージング クライアントによって使用されるインスタント メッセージングの項目が含まれているかどうかを示すために要求を表します。</span><span class="sxs-lookup"><span data-stu-id="da4a6-104">The **SetImListMigrationCompleted** element represents a request to indicate whether the Exchange store contains the instant messaging items used by instant messaging clients.</span></span> 
  
```XML
<SetImListMigrationCompleted>
   <ImListMigrationCompleted/>
</SetImListMigrationCompleted>
```

 <span data-ttu-id="da4a6-105">**SetImListMigrationCompletedType**</span><span class="sxs-lookup"><span data-stu-id="da4a6-105">**SetImListMigrationCompletedType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="da4a6-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="da4a6-106">Attributes and elements</span></span>

<span data-ttu-id="da4a6-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="da4a6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="da4a6-108">属性</span><span class="sxs-lookup"><span data-stu-id="da4a6-108">Attributes</span></span>

<span data-ttu-id="da4a6-109">なし。</span><span class="sxs-lookup"><span data-stu-id="da4a6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="da4a6-110">子要素</span><span class="sxs-lookup"><span data-stu-id="da4a6-110">Child elements</span></span>

[<span data-ttu-id="da4a6-111">ImListMigrationCompleted</span><span class="sxs-lookup"><span data-stu-id="da4a6-111">ImListMigrationCompleted</span></span>](imlistmigrationcompleted.md)
  
### <a name="parent-elements"></a><span data-ttu-id="da4a6-112">親要素</span><span class="sxs-lookup"><span data-stu-id="da4a6-112">Parent elements</span></span>

<span data-ttu-id="da4a6-113">なし。</span><span class="sxs-lookup"><span data-stu-id="da4a6-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="da4a6-114">備考</span><span class="sxs-lookup"><span data-stu-id="da4a6-114">Remarks</span></span>

<span data-ttu-id="da4a6-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="da4a6-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="da4a6-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="da4a6-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="da4a6-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="da4a6-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="da4a6-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="da4a6-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="da4a6-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="da4a6-119">Schema name</span></span>  <br/> |<span data-ttu-id="da4a6-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="da4a6-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="da4a6-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="da4a6-121">Validation file</span></span>  <br/> |<span data-ttu-id="da4a6-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="da4a6-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="da4a6-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="da4a6-123">Can be empty</span></span>  <br/> |<span data-ttu-id="da4a6-124">false</span><span class="sxs-lookup"><span data-stu-id="da4a6-124">false</span></span>  <br/> |
   

