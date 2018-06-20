---
title: グループ Id
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 656d9b9a-8a65-4a75-8466-5b0d96512dab
description: GroupId 要素は、グループを一意に識別します。
ms.openlocfilehash: eaba176321c0dd872b71ef50cbaa298d1277bb79
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831750"
---
# <a name="groupid"></a><span data-ttu-id="b1b88-103">グループ Id</span><span class="sxs-lookup"><span data-stu-id="b1b88-103">GroupId</span></span>

<span data-ttu-id="b1b88-104">**GroupId**要素は、グループを一意に識別します。</span><span class="sxs-lookup"><span data-stu-id="b1b88-104">The **GroupId** element uniquely identifies a group.</span></span> 
  
```XML
<GroupId Id="" ChangeKey=""/>
```

 <span data-ttu-id="b1b88-105">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="b1b88-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b1b88-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="b1b88-106">Attributes and elements</span></span>

<span data-ttu-id="b1b88-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b1b88-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b1b88-108">属性</span><span class="sxs-lookup"><span data-stu-id="b1b88-108">Attributes</span></span>

|<span data-ttu-id="b1b88-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="b1b88-109">**Attribute**</span></span>|<span data-ttu-id="b1b88-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="b1b88-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b1b88-111">ID</span><span class="sxs-lookup"><span data-stu-id="b1b88-111">Id</span></span>  <br/> |<span data-ttu-id="b1b88-112">**Id**属性のテキスト値は、グループの識別子です。</span><span class="sxs-lookup"><span data-stu-id="b1b88-112">The text value of the **Id** attribute is the identifier of the group.</span></span>  <br/> |
|<span data-ttu-id="b1b88-113">ChangeKey</span><span class="sxs-lookup"><span data-stu-id="b1b88-113">ChangeKey</span></span>  <br/> |<span data-ttu-id="b1b88-114">**変更キー**属性のテキスト値は、グループのキーの変更です。</span><span class="sxs-lookup"><span data-stu-id="b1b88-114">The text value of the **ChangeKey** attribute is the change key of the group.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="b1b88-115">子要素</span><span class="sxs-lookup"><span data-stu-id="b1b88-115">Child elements</span></span>

<span data-ttu-id="b1b88-116">なし。</span><span class="sxs-lookup"><span data-stu-id="b1b88-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b1b88-117">親要素</span><span class="sxs-lookup"><span data-stu-id="b1b88-117">Parent elements</span></span>

<span data-ttu-id="b1b88-118">[AddNewImContactToGroup](addnewimcontacttogroup.md) | [AddNewTelUriContactToGroup](addnewteluricontacttogroup.md) | [AddImContactToGroup](addimcontacttogroup.md) | [RemoveContactFromImList](removecontactfromimlist.md) | [RemoveImContactFromGroup](removeimcontactfromgroup.md) | [RemoveImGroup](removeimgroup.md) |  [RemoveDistributionGroupFromImList](removedistributiongroupfromimlist.md) | [SetImGroup](setimgroup.md)</span><span class="sxs-lookup"><span data-stu-id="b1b88-118">[AddNewImContactToGroup](addnewimcontacttogroup.md) | [AddNewTelUriContactToGroup](addnewteluricontacttogroup.md) | [AddImContactToGroup](addimcontacttogroup.md) | [RemoveContactFromImList](removecontactfromimlist.md) | [RemoveImContactFromGroup](removeimcontactfromgroup.md) | [RemoveImGroup](removeimgroup.md) | [RemoveDistributionGroupFromImList](removedistributiongroupfromimlist.md) | [SetImGroup](setimgroup.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b1b88-119">備考</span><span class="sxs-lookup"><span data-stu-id="b1b88-119">Remarks</span></span>

<span data-ttu-id="b1b88-120">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="b1b88-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b1b88-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="b1b88-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b1b88-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="b1b88-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b1b88-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="b1b88-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b1b88-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b1b88-124">Schema name</span></span>  <br/> |<span data-ttu-id="b1b88-125">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="b1b88-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b1b88-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b1b88-126">Validation file</span></span>  <br/> |<span data-ttu-id="b1b88-127">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b1b88-127">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b1b88-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="b1b88-128">Can be empty</span></span>  <br/> ||
   

