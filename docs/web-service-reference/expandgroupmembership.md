---
title: ExpandGroupMembership
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8989e96b-8fa1-4858-93b2-2cbdb30b9ca9
description: ExpandGroupMembership 要素は、GetSearchableMailboxes 要求から返されるグループのメンバーシップを展開するかどうかを示します。
ms.openlocfilehash: 11bfcf6893a147c726c94df77f7d9a9dfbaa773e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760375"
---
# <a name="expandgroupmembership"></a><span data-ttu-id="376c5-103">ExpandGroupMembership</span><span class="sxs-lookup"><span data-stu-id="376c5-103">ExpandGroupMembership</span></span>

<span data-ttu-id="376c5-104">**ExpandGroupMembership**要素は、 **GetSearchableMailboxes**要求から返されるグループのメンバーシップを展開するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="376c5-104">The **ExpandGroupMembership** element indicates whether to expand the membership of the group returned from a **GetSearchableMailboxes** request.</span></span> 
  
```XML
<ExpandGroupMembership>true | false</ExpandGroupMembership>
```

 <span data-ttu-id="376c5-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="376c5-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="376c5-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="376c5-106">Attributes and elements</span></span>

<span data-ttu-id="376c5-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="376c5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="376c5-108">属性</span><span class="sxs-lookup"><span data-stu-id="376c5-108">Attributes</span></span>

<span data-ttu-id="376c5-109">なし。</span><span class="sxs-lookup"><span data-stu-id="376c5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="376c5-110">子要素</span><span class="sxs-lookup"><span data-stu-id="376c5-110">Child elements</span></span>

<span data-ttu-id="376c5-111">なし。</span><span class="sxs-lookup"><span data-stu-id="376c5-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="376c5-112">親要素</span><span class="sxs-lookup"><span data-stu-id="376c5-112">Parent elements</span></span>

<span data-ttu-id="376c5-113">[GetDiscoverySearchConfiguration](getdiscoverysearchconfiguration.md) | [GetSearchableMailboxes](getsearchablemailboxes.md)</span><span class="sxs-lookup"><span data-stu-id="376c5-113">[GetDiscoverySearchConfiguration](getdiscoverysearchconfiguration.md) | [GetSearchableMailboxes](getsearchablemailboxes.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="376c5-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="376c5-114">Text value</span></span>

<span data-ttu-id="376c5-115">の**場合は true** 、 **ExpandGroupElement**要素のテキスト値は、グループのメンバーシップが展開されていることを示します。</span><span class="sxs-lookup"><span data-stu-id="376c5-115">A text value of **true** for the **ExpandGroupElement** element indicates that group membership is expanded.</span></span> <span data-ttu-id="376c5-116">**False**の値は、グループのメンバーシップがグループのメンバーを表示するのには展開されていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="376c5-116">A value of **false** indicates that the group membership is not expanded to show the members of the group.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="376c5-117">備考</span><span class="sxs-lookup"><span data-stu-id="376c5-117">Remarks</span></span>

<span data-ttu-id="376c5-118">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="376c5-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="376c5-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="376c5-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="376c5-120">要素情報</span><span class="sxs-lookup"><span data-stu-id="376c5-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="376c5-121">名前空間</span><span class="sxs-lookup"><span data-stu-id="376c5-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="376c5-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="376c5-122">Schema name</span></span>  <br/> |<span data-ttu-id="376c5-123">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="376c5-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="376c5-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="376c5-124">Validation file</span></span>  <br/> |<span data-ttu-id="376c5-125">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="376c5-125">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="376c5-126">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="376c5-126">Can be empty</span></span>  <br/> |<span data-ttu-id="376c5-127">false</span><span class="sxs-lookup"><span data-stu-id="376c5-127">false</span></span>  <br/> |
   

