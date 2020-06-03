---
title: GroupId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 656d9b9a-8a65-4a75-8466-5b0d96512dab
description: GroupId 要素は、グループを一意に識別します。
ms.openlocfilehash: 3b8de4d0fef95e2caff4db0d90bb303830022d36
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530093"
---
# <a name="groupid"></a><span data-ttu-id="de532-103">GroupId</span><span class="sxs-lookup"><span data-stu-id="de532-103">GroupId</span></span>

<span data-ttu-id="de532-104">**GroupId**要素は、グループを一意に識別します。</span><span class="sxs-lookup"><span data-stu-id="de532-104">The **GroupId** element uniquely identifies a group.</span></span> 
  
```XML
<GroupId Id="" ChangeKey=""/>
```

 <span data-ttu-id="de532-105">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="de532-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="de532-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="de532-106">Attributes and elements</span></span>

<span data-ttu-id="de532-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="de532-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="de532-108">属性</span><span class="sxs-lookup"><span data-stu-id="de532-108">Attributes</span></span>

|<span data-ttu-id="de532-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="de532-109">**Attribute**</span></span>|<span data-ttu-id="de532-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="de532-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="de532-111">ID</span><span class="sxs-lookup"><span data-stu-id="de532-111">Id</span></span>  <br/> |<span data-ttu-id="de532-112">**Id**属性のテキスト値は、グループの識別子です。</span><span class="sxs-lookup"><span data-stu-id="de532-112">The text value of the **Id** attribute is the identifier of the group.</span></span>  <br/> |
|<span data-ttu-id="de532-113">ChangeKey</span><span class="sxs-lookup"><span data-stu-id="de532-113">ChangeKey</span></span>  <br/> |<span data-ttu-id="de532-114">**Changekey**属性のテキスト値は、グループの変更キーです。</span><span class="sxs-lookup"><span data-stu-id="de532-114">The text value of the **ChangeKey** attribute is the change key of the group.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="de532-115">子要素</span><span class="sxs-lookup"><span data-stu-id="de532-115">Child elements</span></span>

<span data-ttu-id="de532-116">なし。</span><span class="sxs-lookup"><span data-stu-id="de532-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="de532-117">親要素</span><span class="sxs-lookup"><span data-stu-id="de532-117">Parent elements</span></span>

<span data-ttu-id="de532-118">[AddNewImContactToGroup](addnewimcontacttogroup.md)  | [AddNewTelUriContactToGroup](addnewteluricontacttogroup.md)  | [Addimcontacttogroup](addimcontacttogroup.md)  | [RemoveContactFromImList](removecontactfromimlist.md)  | [Removeimcontactfromgroup](removeimcontactfromgroup.md)  | [Removeimgroup](removeimgroup.md)  | [RemoveDistributionGroupFromImList](removedistributiongroupfromimlist.md)  | [Setimgroup](setimgroup.md)</span><span class="sxs-lookup"><span data-stu-id="de532-118">[AddNewImContactToGroup](addnewimcontacttogroup.md) | [AddNewTelUriContactToGroup](addnewteluricontacttogroup.md) | [AddImContactToGroup](addimcontacttogroup.md) | [RemoveContactFromImList](removecontactfromimlist.md) | [RemoveImContactFromGroup](removeimcontactfromgroup.md) | [RemoveImGroup](removeimgroup.md) | [RemoveDistributionGroupFromImList](removedistributiongroupfromimlist.md) | [SetImGroup](setimgroup.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="de532-119">注釈</span><span class="sxs-lookup"><span data-stu-id="de532-119">Remarks</span></span>

<span data-ttu-id="de532-120">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="de532-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="de532-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="de532-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="de532-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="de532-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="de532-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="de532-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="de532-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="de532-124">Schema name</span></span>  <br/> |<span data-ttu-id="de532-125">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="de532-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="de532-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="de532-126">Validation file</span></span>  <br/> |<span data-ttu-id="de532-127">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="de532-127">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="de532-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="de532-128">Can be empty</span></span>  <br/> ||
   

