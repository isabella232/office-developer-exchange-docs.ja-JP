---
title: SetImListMigrationCompleted
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4b806441-0429-44c4-90b7-1ae5c6ab9128
description: SetImListMigrationCompleted 要素は、インスタントメッセージングクライアントによって使用されるインスタントメッセージングアイテムが Exchange ストアに含まれているかどうかを示す要求を表します。
ms.openlocfilehash: e5b16044ee72a9e931a2707d3f7823931f8a642a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464827"
---
# <a name="setimlistmigrationcompleted"></a><span data-ttu-id="3df43-103">SetImListMigrationCompleted</span><span class="sxs-lookup"><span data-stu-id="3df43-103">SetImListMigrationCompleted</span></span>

<span data-ttu-id="3df43-104">**SetImListMigrationCompleted**要素は、インスタントメッセージングクライアントによって使用されるインスタントメッセージングアイテムが Exchange ストアに含まれているかどうかを示す要求を表します。</span><span class="sxs-lookup"><span data-stu-id="3df43-104">The **SetImListMigrationCompleted** element represents a request to indicate whether the Exchange store contains the instant messaging items used by instant messaging clients.</span></span> 
  
```XML
<SetImListMigrationCompleted>
   <ImListMigrationCompleted/>
</SetImListMigrationCompleted>
```

 <span data-ttu-id="3df43-105">**SetImListMigrationCompletedType**</span><span class="sxs-lookup"><span data-stu-id="3df43-105">**SetImListMigrationCompletedType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3df43-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="3df43-106">Attributes and elements</span></span>

<span data-ttu-id="3df43-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3df43-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3df43-108">属性</span><span class="sxs-lookup"><span data-stu-id="3df43-108">Attributes</span></span>

<span data-ttu-id="3df43-109">なし。</span><span class="sxs-lookup"><span data-stu-id="3df43-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3df43-110">子要素</span><span class="sxs-lookup"><span data-stu-id="3df43-110">Child elements</span></span>

[<span data-ttu-id="3df43-111">ImListMigrationCompleted</span><span class="sxs-lookup"><span data-stu-id="3df43-111">ImListMigrationCompleted</span></span>](imlistmigrationcompleted.md)
  
### <a name="parent-elements"></a><span data-ttu-id="3df43-112">親要素</span><span class="sxs-lookup"><span data-stu-id="3df43-112">Parent elements</span></span>

<span data-ttu-id="3df43-113">なし。</span><span class="sxs-lookup"><span data-stu-id="3df43-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3df43-114">注釈</span><span class="sxs-lookup"><span data-stu-id="3df43-114">Remarks</span></span>

<span data-ttu-id="3df43-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="3df43-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="3df43-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="3df43-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3df43-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="3df43-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3df43-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="3df43-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3df43-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3df43-119">Schema name</span></span>  <br/> |<span data-ttu-id="3df43-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="3df43-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3df43-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3df43-121">Validation file</span></span>  <br/> |<span data-ttu-id="3df43-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="3df43-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3df43-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="3df43-123">Can be empty</span></span>  <br/> |<span data-ttu-id="3df43-124">false</span><span class="sxs-lookup"><span data-stu-id="3df43-124">false</span></span>  <br/> |
   

