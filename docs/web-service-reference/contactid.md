---
title: ContactId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 86f66275-1e39-48ed-bd89-ac3bffc465a7
description: ContactId 要素は、連絡先を一意に識別します。
ms.openlocfilehash: 4fd3693ed89194c85e5f1770f1db3903d835f43e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759682"
---
# <a name="contactid"></a><span data-ttu-id="08e94-103">ContactId</span><span class="sxs-lookup"><span data-stu-id="08e94-103">ContactId</span></span>

<span data-ttu-id="08e94-104">**ContactId**要素は、連絡先を一意に識別します。</span><span class="sxs-lookup"><span data-stu-id="08e94-104">The **ContactId** element uniquely identifies a contact.</span></span> 
  
```XML
<ContactId Id="" ChangeKey=""/>
```

 <span data-ttu-id="08e94-105">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="08e94-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="08e94-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="08e94-106">Attributes and elements</span></span>

<span data-ttu-id="08e94-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="08e94-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="08e94-108">属性</span><span class="sxs-lookup"><span data-stu-id="08e94-108">Attributes</span></span>

|<span data-ttu-id="08e94-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="08e94-109">**Attribute**</span></span>|<span data-ttu-id="08e94-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="08e94-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="08e94-111">ID</span><span class="sxs-lookup"><span data-stu-id="08e94-111">Id</span></span>  <br/> |<span data-ttu-id="08e94-112">**Id**属性のテキスト値は、連絡先アイテムの識別子です。</span><span class="sxs-lookup"><span data-stu-id="08e94-112">The text value of the **Id** attribute is the identifier of the contact item.</span></span>  <br/> |
|<span data-ttu-id="08e94-113">ChangeKey</span><span class="sxs-lookup"><span data-stu-id="08e94-113">ChangeKey</span></span>  <br/> |<span data-ttu-id="08e94-114">**変更キー**属性のテキスト値は、連絡先アイテムの変更キーです。</span><span class="sxs-lookup"><span data-stu-id="08e94-114">The text value of the **ChangeKey** attribute is the change key of the contact item.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="08e94-115">子要素</span><span class="sxs-lookup"><span data-stu-id="08e94-115">Child elements</span></span>

<span data-ttu-id="08e94-116">なし。</span><span class="sxs-lookup"><span data-stu-id="08e94-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="08e94-117">親要素</span><span class="sxs-lookup"><span data-stu-id="08e94-117">Parent elements</span></span>

<span data-ttu-id="08e94-118">[AddImContactToGroup](addimcontacttogroup.md) | [RemoveContactFromImList](removecontactfromimlist.md) | [RemoveImContactFromGroup](removeimcontactfromgroup.md)</span><span class="sxs-lookup"><span data-stu-id="08e94-118">[AddImContactToGroup](addimcontacttogroup.md) | [RemoveContactFromImList](removecontactfromimlist.md) | [RemoveImContactFromGroup](removeimcontactfromgroup.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="08e94-119">備考</span><span class="sxs-lookup"><span data-stu-id="08e94-119">Remarks</span></span>

<span data-ttu-id="08e94-120">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="08e94-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="08e94-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="08e94-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="08e94-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="08e94-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="08e94-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="08e94-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="08e94-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="08e94-124">Schema name</span></span>  <br/> |<span data-ttu-id="08e94-125">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="08e94-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="08e94-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="08e94-126">Validation file</span></span>  <br/> |<span data-ttu-id="08e94-127">types.xsd</span><span class="sxs-lookup"><span data-stu-id="08e94-127">types.xsd</span></span>  <br/> |
|<span data-ttu-id="08e94-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="08e94-128">Can be empty</span></span>  <br/> |<span data-ttu-id="08e94-129">false</span><span class="sxs-lookup"><span data-stu-id="08e94-129">false</span></span>  <br/> |
   

