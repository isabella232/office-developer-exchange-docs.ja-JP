---
title: ExpandGroupMembership
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8989e96b-8fa1-4858-93b2-2cbdb30b9ca9
description: ExpandGroupMembership 要素は、Getsearchablemailemailrequest 要求から返されるグループのメンバーシップを拡張するかどうかを示します。
ms.openlocfilehash: 8a94aa3da165ecc13282127e75c8d166f3972ead
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456907"
---
# <a name="expandgroupmembership"></a><span data-ttu-id="b8590-103">ExpandGroupMembership</span><span class="sxs-lookup"><span data-stu-id="b8590-103">ExpandGroupMembership</span></span>

<span data-ttu-id="b8590-104">**Expandgroupmembership**要素は、 **Getsearchablemailemailrequest**要求から返されるグループのメンバーシップを拡張するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b8590-104">The **ExpandGroupMembership** element indicates whether to expand the membership of the group returned from a **GetSearchableMailboxes** request.</span></span> 
  
```XML
<ExpandGroupMembership>true | false</ExpandGroupMembership>
```

 <span data-ttu-id="b8590-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="b8590-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b8590-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="b8590-106">Attributes and elements</span></span>

<span data-ttu-id="b8590-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b8590-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b8590-108">属性</span><span class="sxs-lookup"><span data-stu-id="b8590-108">Attributes</span></span>

<span data-ttu-id="b8590-109">なし。</span><span class="sxs-lookup"><span data-stu-id="b8590-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b8590-110">子要素</span><span class="sxs-lookup"><span data-stu-id="b8590-110">Child elements</span></span>

<span data-ttu-id="b8590-111">なし。</span><span class="sxs-lookup"><span data-stu-id="b8590-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b8590-112">親要素</span><span class="sxs-lookup"><span data-stu-id="b8590-112">Parent elements</span></span>

<span data-ttu-id="b8590-113">[Getdiscoverysearchconfiguration](getdiscoverysearchconfiguration.md)  | [Getsearchablemailemailボックス](getsearchablemailboxes.md)</span><span class="sxs-lookup"><span data-stu-id="b8590-113">[GetDiscoverySearchConfiguration](getdiscoverysearchconfiguration.md) | [GetSearchableMailboxes](getsearchablemailboxes.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="b8590-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="b8590-114">Text value</span></span>

<span data-ttu-id="b8590-115">**Expandgroupelement**要素のテキスト値が**true**である場合、グループメンバーシップが展開されていることを示します。</span><span class="sxs-lookup"><span data-stu-id="b8590-115">A text value of **true** for the **ExpandGroupElement** element indicates that group membership is expanded.</span></span> <span data-ttu-id="b8590-116">値が**false**の場合は、グループのメンバーシップが展開されていないことを示します。グループのメンバーが表示されます。</span><span class="sxs-lookup"><span data-stu-id="b8590-116">A value of **false** indicates that the group membership is not expanded to show the members of the group.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="b8590-117">注釈</span><span class="sxs-lookup"><span data-stu-id="b8590-117">Remarks</span></span>

<span data-ttu-id="b8590-118">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="b8590-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b8590-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="b8590-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b8590-120">要素の情報</span><span class="sxs-lookup"><span data-stu-id="b8590-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b8590-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="b8590-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b8590-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b8590-122">Schema name</span></span>  <br/> |<span data-ttu-id="b8590-123">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="b8590-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b8590-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b8590-124">Validation file</span></span>  <br/> |<span data-ttu-id="b8590-125">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="b8590-125">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b8590-126">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="b8590-126">Can be empty</span></span>  <br/> |<span data-ttu-id="b8590-127">false</span><span class="sxs-lookup"><span data-stu-id="b8590-127">false</span></span>  <br/> |
   

