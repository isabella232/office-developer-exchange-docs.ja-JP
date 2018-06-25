---
title: RetentionPolicyTag
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f46679d0-9236-41e2-8624-72300079c67c
description: RetentionPolicyTag 要素は、メールボックス アイテムの保持ポリシーを指定します。
ms.openlocfilehash: 2525f6d7a0ca583342d28dd9f4857a69b3a8c05a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833226"
---
# <a name="retentionpolicytag"></a><span data-ttu-id="bd8d8-103">RetentionPolicyTag</span><span class="sxs-lookup"><span data-stu-id="bd8d8-103">RetentionPolicyTag</span></span>

<span data-ttu-id="bd8d8-104">**RetentionPolicyTag**要素は、メールボックス アイテムの保持ポリシーを指定します。</span><span class="sxs-lookup"><span data-stu-id="bd8d8-104">The **RetentionPolicyTag** element specifies the retention policy for a mailbox item.</span></span> 
  
```XML
<RetentionPolicyTag>
   <DisplayName/>
   <RetentionId/>
   <RetentionPeriod/>
   <Type/>
   <RetentionAction/>
   <Description/>
   <IsVisible/>
   <OptedInto/>
   <IsArchive/>
</RetentionPolicyTag>
```

 <span data-ttu-id="bd8d8-105">**RetentionPolicyTagType**</span><span class="sxs-lookup"><span data-stu-id="bd8d8-105">**RetentionPolicyTagType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bd8d8-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="bd8d8-106">Attributes and elements</span></span>

<span data-ttu-id="bd8d8-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="bd8d8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bd8d8-108">属性</span><span class="sxs-lookup"><span data-stu-id="bd8d8-108">Attributes</span></span>

<span data-ttu-id="bd8d8-109">なし。</span><span class="sxs-lookup"><span data-stu-id="bd8d8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bd8d8-110">子要素</span><span class="sxs-lookup"><span data-stu-id="bd8d8-110">Child elements</span></span>

<span data-ttu-id="bd8d8-111">[表示名 (文字列)](displayname-string.md) | [RetentionId](retentionid.md) | [RetentionPeriod](retentionperiod.md) | [型 (ElcFolderType)](type-elcfoldertype.md) | [RetentionAction](retentionaction.md) | [説明](description.md) | [IsVisible](isvisible.md)  |  [OptedInto](optedinto.md) | [IsArchive](isarchive.md)</span><span class="sxs-lookup"><span data-stu-id="bd8d8-111">[DisplayName (string)](displayname-string.md) | [RetentionId](retentionid.md) | [RetentionPeriod](retentionperiod.md) | [Type (ElcFolderType)](type-elcfoldertype.md) | [RetentionAction](retentionaction.md) | [Description](description.md) | [IsVisible](isvisible.md) | [OptedInto](optedinto.md) | [IsArchive](isarchive.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bd8d8-112">親要素</span><span class="sxs-lookup"><span data-stu-id="bd8d8-112">Parent elements</span></span>

[<span data-ttu-id="bd8d8-113">RetentionPolicyTags</span><span class="sxs-lookup"><span data-stu-id="bd8d8-113">RetentionPolicyTags</span></span>](retentionpolicytags.md)
  
## <a name="remarks"></a><span data-ttu-id="bd8d8-114">備考</span><span class="sxs-lookup"><span data-stu-id="bd8d8-114">Remarks</span></span>

<span data-ttu-id="bd8d8-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="bd8d8-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="bd8d8-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="bd8d8-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bd8d8-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="bd8d8-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bd8d8-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="bd8d8-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bd8d8-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="bd8d8-119">Schema name</span></span>  <br/> |<span data-ttu-id="bd8d8-120">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="bd8d8-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="bd8d8-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="bd8d8-121">Validation file</span></span>  <br/> |<span data-ttu-id="bd8d8-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="bd8d8-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bd8d8-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="bd8d8-123">Can be empty</span></span>  <br/> ||
   

