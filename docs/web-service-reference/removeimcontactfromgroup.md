---
title: RemoveImContactFromGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a62b0640-9800-45a6-a297-2105ff36881e
description: RemoveImContactFromGroup 要素は、インスタント メッセージ、インスタント メッセージング グループから連絡先を削除する要求を定義します。
ms.openlocfilehash: 402cbd6929428d410ce5701b0c1afa901703bc29
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833094"
---
# <a name="removeimcontactfromgroup"></a><span data-ttu-id="db914-103">RemoveImContactFromGroup</span><span class="sxs-lookup"><span data-stu-id="db914-103">RemoveImContactFromGroup</span></span>

<span data-ttu-id="db914-104">**RemoveImContactFromGroup**要素は、インスタント メッセージ、インスタント メッセージング グループから連絡先を削除する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="db914-104">The **RemoveImContactFromGroup** element defines a request to remove an instant messaging contact from an instant messaging group.</span></span> 
  
```XML
<RemoveImContactFromGroup>
   <ContactId/>
   <GroupId/>
</RemoveImContactFromGroup>
```

 <span data-ttu-id="db914-105">**RemoveImContactFromGroupType**</span><span class="sxs-lookup"><span data-stu-id="db914-105">**RemoveImContactFromGroupType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="db914-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="db914-106">Attributes and elements</span></span>

<span data-ttu-id="db914-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="db914-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="db914-108">属性</span><span class="sxs-lookup"><span data-stu-id="db914-108">Attributes</span></span>

<span data-ttu-id="db914-109">なし。</span><span class="sxs-lookup"><span data-stu-id="db914-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="db914-110">子要素</span><span class="sxs-lookup"><span data-stu-id="db914-110">Child elements</span></span>

<span data-ttu-id="db914-111">[ContactId](contactid.md) | [グループ Id](groupid.md)</span><span class="sxs-lookup"><span data-stu-id="db914-111">[ContactId](contactid.md) | [GroupId](groupid.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="db914-112">親要素</span><span class="sxs-lookup"><span data-stu-id="db914-112">Parent elements</span></span>

<span data-ttu-id="db914-113">なし。</span><span class="sxs-lookup"><span data-stu-id="db914-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="db914-114">備考</span><span class="sxs-lookup"><span data-stu-id="db914-114">Remarks</span></span>

<span data-ttu-id="db914-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="db914-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="db914-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="db914-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="db914-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="db914-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="db914-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="db914-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="db914-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="db914-119">Schema name</span></span>  <br/> |<span data-ttu-id="db914-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="db914-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="db914-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="db914-121">Validation file</span></span>  <br/> |<span data-ttu-id="db914-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="db914-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="db914-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="db914-123">Can be empty</span></span>  <br/> ||
   

