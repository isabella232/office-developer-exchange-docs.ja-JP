---
title: AddImContactToGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 65554e4c-c0d9-485e-9f01-ed1baa8280ab
description: AddImContactToGroup 要素は、インスタント メッセージング グループに既存のインスタント メッセージングの連絡先を追加する要求を定義します。
ms.openlocfilehash: 71c841ce6df2ed7dcbbf77597b26f3e3e742a7fb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759362"
---
# <a name="addimcontacttogroup"></a><span data-ttu-id="b740e-103">AddImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="b740e-103">AddImContactToGroup</span></span>

<span data-ttu-id="b740e-104">**AddImContactToGroup**要素は、インスタント メッセージング グループに既存のインスタント メッセージングの連絡先を追加する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="b740e-104">The **AddImContactToGroup** element defines a request to add an existing instant messaging contact to an instant messaging group.</span></span> 
  
```XML
<AddImContactToGroup>
   <ContactId/>
   <GroupId/>
</AddImContactToGroup>
```

 <span data-ttu-id="b740e-105">**AddImContactToGroupType**</span><span class="sxs-lookup"><span data-stu-id="b740e-105">**AddImContactToGroupType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b740e-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="b740e-106">Attributes and elements</span></span>

<span data-ttu-id="b740e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b740e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b740e-108">属性</span><span class="sxs-lookup"><span data-stu-id="b740e-108">Attributes</span></span>

<span data-ttu-id="b740e-109">なし。</span><span class="sxs-lookup"><span data-stu-id="b740e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b740e-110">子要素</span><span class="sxs-lookup"><span data-stu-id="b740e-110">Child elements</span></span>

<span data-ttu-id="b740e-111">[ContactId](contactid.md) | [グループ Id](groupid.md)</span><span class="sxs-lookup"><span data-stu-id="b740e-111">[ContactId](contactid.md) | [GroupId](groupid.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b740e-112">親要素</span><span class="sxs-lookup"><span data-stu-id="b740e-112">Parent elements</span></span>

<span data-ttu-id="b740e-113">なし。</span><span class="sxs-lookup"><span data-stu-id="b740e-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b740e-114">備考</span><span class="sxs-lookup"><span data-stu-id="b740e-114">Remarks</span></span>

<span data-ttu-id="b740e-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="b740e-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b740e-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="b740e-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b740e-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="b740e-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b740e-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="b740e-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b740e-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b740e-119">Schema name</span></span>  <br/> |<span data-ttu-id="b740e-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="b740e-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b740e-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b740e-121">Validation file</span></span>  <br/> |<span data-ttu-id="b740e-122">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b740e-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b740e-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="b740e-123">Can be empty</span></span>  <br/> |<span data-ttu-id="b740e-124">false</span><span class="sxs-lookup"><span data-stu-id="b740e-124">false</span></span>  <br/> |
   

