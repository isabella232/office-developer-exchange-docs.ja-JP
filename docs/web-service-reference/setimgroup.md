---
title: SetImGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3c107b8d-714b-4cd5-ad1b-97b7cbcb90d6
description: SetImGroup 要素は、インスタントメッセージンググループの表示名を変更する要求を表します。
ms.openlocfilehash: 96e93ef595720325448c343c193f25b846ba415e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44438069"
---
# <a name="setimgroup"></a><span data-ttu-id="483dd-103">SetImGroup</span><span class="sxs-lookup"><span data-stu-id="483dd-103">SetImGroup</span></span>

<span data-ttu-id="483dd-104">**Setimgroup**要素は、インスタントメッセージンググループの表示名を変更する要求を表します。</span><span class="sxs-lookup"><span data-stu-id="483dd-104">The **SetImGroup** element represents a request to change the display name of an instant messaging group.</span></span> 
  
```XML
<SetImGroup>
   <GroupId/>
   <NewDisplayName/>
</SetImGroup>
```

 <span data-ttu-id="483dd-105">**SetImGroupType**</span><span class="sxs-lookup"><span data-stu-id="483dd-105">**SetImGroupType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="483dd-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="483dd-106">Attributes and elements</span></span>

<span data-ttu-id="483dd-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="483dd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="483dd-108">属性</span><span class="sxs-lookup"><span data-stu-id="483dd-108">Attributes</span></span>

<span data-ttu-id="483dd-109">なし。</span><span class="sxs-lookup"><span data-stu-id="483dd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="483dd-110">子要素</span><span class="sxs-lookup"><span data-stu-id="483dd-110">Child elements</span></span>

<span data-ttu-id="483dd-111">[GroupId](groupid.md)  | [Newdisplayname](newdisplayname.md)</span><span class="sxs-lookup"><span data-stu-id="483dd-111">[GroupId](groupid.md) | [NewDisplayName](newdisplayname.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="483dd-112">親要素</span><span class="sxs-lookup"><span data-stu-id="483dd-112">Parent elements</span></span>

<span data-ttu-id="483dd-113">なし。</span><span class="sxs-lookup"><span data-stu-id="483dd-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="483dd-114">注釈</span><span class="sxs-lookup"><span data-stu-id="483dd-114">Remarks</span></span>

<span data-ttu-id="483dd-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="483dd-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="483dd-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="483dd-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="483dd-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="483dd-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="483dd-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="483dd-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="483dd-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="483dd-119">Schema name</span></span>  <br/> |<span data-ttu-id="483dd-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="483dd-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="483dd-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="483dd-121">Validation file</span></span>  <br/> |<span data-ttu-id="483dd-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="483dd-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="483dd-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="483dd-123">Can be empty</span></span>  <br/> ||
   

