---
title: AddNewImContactToGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d5913619-0c13-429d-b9d2-057e8af220f1
description: AddNewImContactToGroup 要素は、インスタントメッセージンググループに新しいインスタントメッセージングの連絡先を追加する要求を定義します。
ms.openlocfilehash: c493ba81b23832a462acd425eb60297801f8768f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463651"
---
# <a name="addnewimcontacttogroup"></a><span data-ttu-id="849a6-103">AddNewImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="849a6-103">AddNewImContactToGroup</span></span>

<span data-ttu-id="849a6-104">**AddNewImContactToGroup**要素は、インスタントメッセージンググループに新しいインスタントメッセージングの連絡先を追加する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="849a6-104">The **AddNewImContactToGroup** element defines a request to add a new instant messaging contact to an instant messaging group.</span></span> 
  
```XML
<AddNewImContactToGroup>
   <ImAddress/>
   <DisplayName/>
   <GroupId/>
</AddNewImContactToGroup>
```

 <span data-ttu-id="849a6-105">**AddNewImContactToGroupType**</span><span class="sxs-lookup"><span data-stu-id="849a6-105">**AddNewImContactToGroupType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="849a6-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="849a6-106">Attributes and elements</span></span>

<span data-ttu-id="849a6-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="849a6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="849a6-108">属性</span><span class="sxs-lookup"><span data-stu-id="849a6-108">Attributes</span></span>

<span data-ttu-id="849a6-109">なし。</span><span class="sxs-lookup"><span data-stu-id="849a6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="849a6-110">子要素</span><span class="sxs-lookup"><span data-stu-id="849a6-110">Child elements</span></span>

<span data-ttu-id="849a6-111">[Imaddress (非 Emptystringtype)](imaddress-nonemptystringtype.md)  | [DisplayName (非 Emptystringtype)](displayname-nonemptystringtype.md)  | [GroupId](groupid.md)</span><span class="sxs-lookup"><span data-stu-id="849a6-111">[ImAddress (NonEmptyStringType)](imaddress-nonemptystringtype.md) | [DisplayName (NonEmptyStringType)](displayname-nonemptystringtype.md) | [GroupId](groupid.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="849a6-112">親要素</span><span class="sxs-lookup"><span data-stu-id="849a6-112">Parent elements</span></span>

<span data-ttu-id="849a6-113">なし。</span><span class="sxs-lookup"><span data-stu-id="849a6-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="849a6-114">注釈</span><span class="sxs-lookup"><span data-stu-id="849a6-114">Remarks</span></span>

<span data-ttu-id="849a6-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="849a6-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="849a6-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="849a6-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="849a6-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="849a6-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="849a6-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="849a6-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="849a6-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="849a6-119">Schema name</span></span>  <br/> |<span data-ttu-id="849a6-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="849a6-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="849a6-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="849a6-121">Validation file</span></span>  <br/> |<span data-ttu-id="849a6-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="849a6-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="849a6-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="849a6-123">Can be empty</span></span>  <br/> |<span data-ttu-id="849a6-124">false</span><span class="sxs-lookup"><span data-stu-id="849a6-124">false</span></span>  <br/> |
   

