---
title: AddNewImContactToGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d5913619-0c13-429d-b9d2-057e8af220f1
description: AddNewImContactToGroup 要素は、インスタント メッセージング グループに新しいインスタント メッセージングの連絡先を追加する要求を定義します。
ms.openlocfilehash: 2736bac6880a11101e9bffee12033c838705700e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759290"
---
# <a name="addnewimcontacttogroup"></a><span data-ttu-id="4d178-103">AddNewImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="4d178-103">AddNewImContactToGroup</span></span>

<span data-ttu-id="4d178-104">**AddNewImContactToGroup**要素は、インスタント メッセージング グループに新しいインスタント メッセージングの連絡先を追加する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="4d178-104">The **AddNewImContactToGroup** element defines a request to add a new instant messaging contact to an instant messaging group.</span></span> 
  
```XML
<AddNewImContactToGroup>
   <ImAddress/>
   <DisplayName/>
   <GroupId/>
</AddNewImContactToGroup>
```

 <span data-ttu-id="4d178-105">**AddNewImContactToGroupType**</span><span class="sxs-lookup"><span data-stu-id="4d178-105">**AddNewImContactToGroupType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4d178-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="4d178-106">Attributes and elements</span></span>

<span data-ttu-id="4d178-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4d178-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4d178-108">属性</span><span class="sxs-lookup"><span data-stu-id="4d178-108">Attributes</span></span>

<span data-ttu-id="4d178-109">なし。</span><span class="sxs-lookup"><span data-stu-id="4d178-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4d178-110">子要素</span><span class="sxs-lookup"><span data-stu-id="4d178-110">Child elements</span></span>

<span data-ttu-id="4d178-111">[ImAddress (NonEmptyStringType)](imaddress-nonemptystringtype.md) | [(NonEmptyStringType) の表示名](displayname-nonemptystringtype.md) | [グループ Id](groupid.md)</span><span class="sxs-lookup"><span data-stu-id="4d178-111">[ImAddress (NonEmptyStringType)](imaddress-nonemptystringtype.md) | [DisplayName (NonEmptyStringType)](displayname-nonemptystringtype.md) | [GroupId](groupid.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4d178-112">親要素</span><span class="sxs-lookup"><span data-stu-id="4d178-112">Parent elements</span></span>

<span data-ttu-id="4d178-113">なし。</span><span class="sxs-lookup"><span data-stu-id="4d178-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4d178-114">備考</span><span class="sxs-lookup"><span data-stu-id="4d178-114">Remarks</span></span>

<span data-ttu-id="4d178-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="4d178-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4d178-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="4d178-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4d178-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="4d178-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4d178-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="4d178-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4d178-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4d178-119">Schema name</span></span>  <br/> |<span data-ttu-id="4d178-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="4d178-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4d178-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4d178-121">Validation file</span></span>  <br/> |<span data-ttu-id="4d178-122">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="4d178-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4d178-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="4d178-123">Can be empty</span></span>  <br/> |<span data-ttu-id="4d178-124">false</span><span class="sxs-lookup"><span data-stu-id="4d178-124">false</span></span>  <br/> |
   

