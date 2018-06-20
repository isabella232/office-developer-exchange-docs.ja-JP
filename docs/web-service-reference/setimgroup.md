---
title: SetImGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3c107b8d-714b-4cd5-ad1b-97b7cbcb90d6
description: SetImGroup 要素は、インスタント メッセージング グループの表示名を変更する要求を表します。
ms.openlocfilehash: 67fd8188e3436d5042a2867fe54e673348cba807
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833422"
---
# <a name="setimgroup"></a><span data-ttu-id="ac180-103">SetImGroup</span><span class="sxs-lookup"><span data-stu-id="ac180-103">SetImGroup</span></span>

<span data-ttu-id="ac180-104">**SetImGroup**要素は、インスタント メッセージング グループの表示名を変更する要求を表します。</span><span class="sxs-lookup"><span data-stu-id="ac180-104">The **SetImGroup** element represents a request to change the display name of an instant messaging group.</span></span> 
  
```XML
<SetImGroup>
   <GroupId/>
   <NewDisplayName/>
</SetImGroup>
```

 <span data-ttu-id="ac180-105">**SetImGroupType**</span><span class="sxs-lookup"><span data-stu-id="ac180-105">**SetImGroupType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ac180-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="ac180-106">Attributes and elements</span></span>

<span data-ttu-id="ac180-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ac180-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ac180-108">属性</span><span class="sxs-lookup"><span data-stu-id="ac180-108">Attributes</span></span>

<span data-ttu-id="ac180-109">なし。</span><span class="sxs-lookup"><span data-stu-id="ac180-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ac180-110">子要素</span><span class="sxs-lookup"><span data-stu-id="ac180-110">Child elements</span></span>

<span data-ttu-id="ac180-111">[GroupId](groupid.md) | [NewDisplayName](newdisplayname.md)</span><span class="sxs-lookup"><span data-stu-id="ac180-111">[GroupId](groupid.md) | [NewDisplayName](newdisplayname.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ac180-112">親要素</span><span class="sxs-lookup"><span data-stu-id="ac180-112">Parent elements</span></span>

<span data-ttu-id="ac180-113">なし。</span><span class="sxs-lookup"><span data-stu-id="ac180-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ac180-114">備考</span><span class="sxs-lookup"><span data-stu-id="ac180-114">Remarks</span></span>

<span data-ttu-id="ac180-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="ac180-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="ac180-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="ac180-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ac180-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="ac180-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ac180-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="ac180-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ac180-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ac180-119">Schema name</span></span>  <br/> |<span data-ttu-id="ac180-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="ac180-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ac180-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ac180-121">Validation file</span></span>  <br/> |<span data-ttu-id="ac180-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ac180-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ac180-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="ac180-123">Can be empty</span></span>  <br/> ||
   

